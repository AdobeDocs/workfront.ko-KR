---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: 이벤트 구독 메시지 필터링
description: 이벤트 구독 메시지 필터링
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1767'
ht-degree: 0%

---

# 이벤트 구독 메시지 필터링

비즈니스에 필요한 이벤트 구독 메시지만 필터링하고 처리하는 데 도움이 되는 중간 처리 구성 요소를 빌드할 수 있습니다.

이벤트 구독에 대한 자세한 내용은 [이벤트 구독 API](../../wf-api/general/event-subs-api.md)를 참조하세요.

## 이벤트 메시지 필터링

이 섹션에는 이벤트 구독 메시지 로드를 줄이기 위해 구현할 수 있는 필터링의 코드 조각이 포함되어 있습니다.  다양한 언어의 구문에서 차이점을 표시하는 데 도움이 되도록 이 코드 조각은 다음 언어로 작성된 동일한 필터 세트를 보여 줍니다.

[https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples)에서 필터링의 예를 볼 수 있습니다. 여기에서 각 언어의 구문과 AWS SDK와의 상호 작용 수단에 대한 차이점을 확인할 수 있습니다. 이러한 예제는 중간 필터링 및 처리 구성 요소를 사용하는 일반적인 방법인 AWS Lambda로 작성됩니다.

다음 코드 조각은 배포 준비가 거의 완료되었으며 보다 복잡한 고유한 필터 및 처리 구성 요소를 작성하는 데 도움이 되는 시작점으로 사용할 수 있습니다.

### Java

Java의 다음 예제에서는 [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)에서 수행한 대로 프로젝트의 그룹 ID를 기반으로 프로젝트 페이로드를 필터링하는 방법을 보여 줍니다

1. 찾고 있는 그룹 ID를 설정하고 정적 상수로 만듭니다.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   이 예제에서 AWS Lambda 표준 메서드 이름인 handleRequest 메서드는 Map 형식을 첫 번째 매개 변수로 사용합니다. 이 매개 변수는 이벤트 구독 메시지 콘텐츠입니다.\
   두 번째 매개 변수는 현재 Lambda 프록시 요청의 컨텍스트입니다.\
   Context 개체는 CloudWatchLogs에 메시지를 쓰는 데 사용되는 Lambda 로거를 얻는 데 사용됩니다.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. handleRequest 메서드를 호출하면 리소스의 업데이트된 상태를 나타내는 이벤트 구독 메시지의 &quot;newState&quot; 속성을 가져옵니다.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   newState 형식에 대한 자세한 내용은 [이벤트 구독에 대한 아웃바운드 메시지 형식](../../wf-api/api/message-format-event-subs.md)을 참조하세요.

3. 메시지에서 &quot;newState&quot; 맵을 구문 분석한 후, 개체의 그룹 ID가 1단계에서 식별한 그룹 ID와 일치하는지 확인합니다.

4. (조건부) ID **이(가) 일치하지 않으면** 빈 응답이 반환되도록 메시지를 삭제합니다.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >빈 성공적인 응답을 반환하는 것은 중요합니다. 200 수준 응답을 제외한 모든 응답은 게재 실패로 간주됩니다.

5. 메시지를 처리합니다.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   AWS SDK는 필터링된 메시지를 원하는 끝점에 전달하는 다른 Lambda를 호출하는 데 사용됩니다.

   메시지를 다른 Lambda에 전달할 책임을 전달하는 목적은 이벤트 구독 서비스에서 오는 배달 요청의 시간 제한을 방지하기 위한 것입니다. 현재, 게재에 허용 가능한 시간 초과가 5초로 설정되어 있습니다. 필터가 설정에 허용된 시간보다 오래 걸리는 경우 요청을 처리할 수 있지만 이벤트 구독 서비스는 시간 초과 기간 내에 200 수준의 응답을 받을 때까지 시간 초과되어 재시도 루프에 속하게 됩니다.

   메시지 게재 관리에 대한 자세한 내용은 [시간 초과를 수용하는 동안 메시지 게재 개선](#improving-message-delivery-while-accommodating-timeouts)을 참조하세요.

### Python

Java 예제와 Python 예제의 주요 차이점은 Java 예제의 경우 이벤트 구독 메시지가 첫 번째 매개 변수로 수신되며, Python 예제의 경우 첫 번째 매개 변수가 AWS Lambda 프록시 요청에 대한 정보와 함께 이벤트 구독 메시지를 포함하는 Lambda 프록시 &quot;event&quot;라는 것입니다.

Python의 다음 예제는 [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)에서 수행한 대로 프로젝트의 그룹 ID를 기반으로 프로젝트 페이로드를 필터링하는 방법을 보여 줍니다

1. 찾고 있는 그룹 ID를 설정하고 정적 상수로 만듭니다.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   첫 번째 매개 변수는 이벤트 구독 메시지와 구문 분석해야 하는 일부 추가 정보를 포함하는 Lambda 프록시 &quot;event&quot;입니다.\
   두 번째 매개 변수는 현재 Lambda 프록시 요청의 컨텍스트입니다.\
   이 예제에서는 Context 개체를 사용하여 CloudWatchLogs에 메시지를 작성하는 데 사용되는 Lambda 로거를 가져옵니다.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. 이벤트에서 메시지를 구문 분석합니다.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. 이벤트 구독 메시지의 &quot;newState&quot; 속성을 가져옵니다.\
   newState 속성은 리소스의 업데이트된 상태를 나타냅니다.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   newState 형식에 대한 자세한 내용은 [이벤트 구독에 대한 아웃바운드 메시지 형식](../../wf-api/api/message-format-event-subs.md)을 참조하세요.

1. 메시지에서 &quot;newState&quot; 맵을 구문 분석한 후, 개체의 그룹 ID가 1단계에서 식별한 그룹 ID와 일치하는지 확인합니다.

1. (조건부) ID가 일치하지 않으면 빈 응답이 반환되도록 메시지를 삭제합니다.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >빈 성공적인 응답을 반환하는 것은 중요합니다. 200 수준 응답을 제외한 모든 응답은 게재 실패로 간주됩니다.

1. 메시지를 처리합니다.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   AWS SDK는 필터링된 메시지를 원하는 끝점에 전달하는 다른 Lambda를 호출하는 데 사용됩니다.

   메시지를 다른 Lambda에 전달할 책임을 전달하는 목적은 이벤트 구독 서비스에서 오는 배달 요청의 시간 제한을 방지하기 위한 것입니다. 현재, 게재에 대한 시간 제한은 5초로 설정되어 있습니다. 필터가 설정에 허용된 시간보다 오래 걸리는 경우 요청을 처리할 수 있지만 이벤트 구독 서비스는 시간 초과 기간 내에 200 수준의 응답을 받을 때까지 시간 초과되어 재시도 루프에 속하게 됩니다.


### Node.js

프로젝트 그룹 ID 필터링의 Node.js 예는 Java 및 Python 예와 유사합니다. Python 예제와 마찬가지로 첫 번째 매개 변수는 Lambda 프록시 이벤트이고 두 번째 매개 변수는 Lambda 컨텍스트입니다.

Node.js의 다음 예제는 [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)에서 수행한 대로 프로젝트의 그룹 ID를 기반으로 프로젝트 페이로드를 필터링하는 방법을 보여 줍니다.

1. 찾고 있는 그룹 ID를 설정하고 정적 상수로 만듭니다.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   첫 번째 매개 변수는 이벤트 구독 메시지와 구문 분석해야 하는 일부 추가 정보를 포함하는 Lambda 프록시 &quot;event&quot;입니다.\
   두 번째 매개 변수는 현재 Lambda 프록시 요청의 컨텍스트입니다.\
   이 예제에서는 Context 개체를 사용하여 CloudWatchLogs에 메시지를 작성하는 데 사용되는 Lambda 로거를 가져옵니다.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. 이벤트에서 메시지를 구문 분석합니다.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. 이벤트 구독 메시지의 &quot;newState&quot; 속성에서 projectGroupID를 가져온 다음, 1단계에서 식별한 그룹의 그룹 ID와 비교합니다.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   newState 형식에 대한 자세한 내용은 [이벤트 구독에 대한 아웃바운드 메시지 형식](../../wf-api/api/message-format-event-subs.md)을 참조하세요.

4. (조건부) ID가 일치하지 않으면 빈 응답이 반환되도록 메시지를 삭제합니다.\
   다음 예에서는 일치하는 그룹 ID를 보여 줍니다.

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >빈 성공적인 응답을 반환하는 것은 중요합니다. 200 수준 응답을 제외한 모든 응답은 게재 실패로 간주됩니다.

5. 메시지를 처리합니다.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   AWS SDK는 필터링된 메시지를 원하는 끝점에 전달하는 다른 Lambda를 호출하는 데 사용됩니다.\
   메시지를 다른 Lambda에 전달할 책임을 전달하는 목적은 이벤트 구독 서비스에서 오는 배달 요청의 시간 제한을 방지하기 위한 것입니다. 현재, 게재에 대한 시간 제한은 5초로 설정되어 있습니다. 필터가 설정에 허용된 시간보다 오래 걸리는 경우 요청을 처리할 수 있지만 이벤트 구독 서비스는 시간 초과 기간 내에 200 수준의 응답을 받을 때까지 시간 초과되어 재시도 루프에 속하게 됩니다.\
   메시지 배달 관리에 대한 자세한 내용은 [시간 초과를 수용하는 동안 메시지 배달 개선](#improving-message-delivery-while-accommodating-timeouts)을 참조하세요.

## 시간 초과를 수용하는 동안 메시지 전달 개선

Event Subscription 서비스의 모든 게재 요청에 대해 **5초**&#x200B;의 엄격한 시간 제한이 있습니다. 메시지 게재가 허용된 시간을 초과하는 경우 이벤트 구독 서비스는 해당 메시지에 대한 다시 시도 주기를 시작합니다.

예를 들어 [이벤트 메시지 필터링](#filtering-event-messages)에 있는 예제 중 하나와 유사한 프로젝트 그룹 ID 필터를 빌드하고 데이터베이스 조회를 포함하여 메시지가 필요한지 여부를 확인합니다. 데이터베이스 조회에 필요한 처리 시간 및 Lambda가 콜드 스타트에 도달하는 데 필요한 시간이 5초 이상 소요될 수 있으므로 이벤트 구독 서비스가 메시지 배달을 다시 시도할 수 있습니다.

메시지가 처리 및 게재할 논리인지 여부를 결정하는 논리와 프로세스에서 시간이 많이 소요되는 부분을 분리하여 재시도를 방지할 수 있습니다. 이렇게 하면 메시지를 수락하고 이벤트 구독 서비스에 대한 200단계 응답을 다시 보내는 동시에 백그라운드에서 메시지를 비동기적으로 계속 처리하거나 필터링할 수 있습니다(예를 들어 [Java](#java)의 5단계 참조).


처리 또는 필터링이 5초 시간 제한을 초과하지 않더라도 클라이언트측의 다른 처리 또는 게재 단계와 메시지 필터링 또는 처리의 첫 번째 터치 포인트를 분리하는 것이 여전히 유리합니다. 이러한 방식으로 이벤트 구독 서비스에서 대상으로의 메시지 핸드오프는 양 당사자에게 최소한의 시간 및 성능에 영향을 줍니다.

다시 시도 메커니즘에 대한 자세한 내용은 [이벤트 구독 다시 시도](../../wf-api/api/event-sub-retries.md)를 참조하세요.

## 클라우드없는 아키텍처에서 호스팅된 필터 구현

이벤트 구독 필터링에 클라우드 아키텍처를 활용할 수 없는 경우에도 [이벤트 메시지 필터링](#filtering-event-messages)의 예제를 자체 호스트된 필터 또는 처리 구성 요소를 구현하는 방법에 대한 로드맵으로 사용할 수 있습니다.

### 독립형 서비스에 대한 필터링 예제 조정

클라우드가 없는 환경에서 필터링 예를 사용하기 전에 다음을 수행하십시오.

* Context 매개 변수와 같은 예제의 Lambda 관련 부분을 생략합니다.

* 예제에서 다른 Lambda의 호출을 다른 필터 또는 호스팅하는 처리 구성 요소에 대한 추가 비동기 HTTP 요청으로 변경합니다.

* Python 및 Node.js 예를 참조하는 경우 첫 번째 이벤트 매개 변수를 Java 예제에 표시된 첫 번째 페이로드 매개 변수로 대체하십시오. [Java](#java)의 1단계를 참조하세요.

* 웹 기반 API를 사용하여 필터 또는 프로세서를 배포합니다.

### 누락된 이벤트 구독 메시지 방지

때때로 클라우드가 없는 아키텍처에서 이벤트 구독 메시지 수신을 담당하는 서비스에 연결할 수 없습니다. 이러한 경우 메시지 내의 정보를 검색할 방법 없이 메시지가 다시 시도 제한을 초과하여 손실될 수 있습니다.

서비스를 시작하는 동안 누락된 메시지에 포함되었을 수 있는 모든 리소스의 최신 상태를 묻는 쿼리를 구현하는 것이 좋습니다. 다음 예제와 같이 필터 기준을 사용하여 해당 기준과 일치하는 리소스를 쿼리한 다음 현재 상태를 처리할 수 있습니다.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

리소스를 쿼리하면 통합 시스템에 최신 버전의 리소스가 있는지 확인할 수 있습니다.

### 메시지 전달에서 비동기 처리 구현

[이벤트 메시지 필터링](#filtering-event-messages) 섹션의 모든 예제는 필터링된 메시지를 다른 AWS Lambda에 전달할 권한을 전달합니다. 이 작업은 요청을 발행하는 이벤트 구독 서비스에 의해 적용되는 게재 요청에서 5초 시간 제한을 초과하지 않도록 하기 위해 수행됩니다.

클라우드가 없는 아키텍처에서는 AWS SDK를 사용하여 다른 AWS Lambda에 대한 비동기 호출을 허용하는 방법과 유사한 비동기 처리 메커니즘을 구현해야 할 수 있습니다. 대부분의 최신 프로그래밍 언어에는 비동기 처리를 처리하는 서드파티 또는 코어 라이브러리가 있으므로 예제에서 구현된 비동기 스타일의 처리를 활용할 수 있습니다.
