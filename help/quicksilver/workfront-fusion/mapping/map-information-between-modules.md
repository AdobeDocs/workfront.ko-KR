---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]
description: 매핑은 항목으로 구성된 모듈의 출력을 다른 모듈의 입력 필드에 할당하는 프로세스입니다.
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# 의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]

매핑은 항목으로 구성된 모듈의 출력을 다른 모듈의 입력 필드에 할당하는 프로세스입니다.

시나리오에서 이전 모듈에서 출력된 값을 삽입할 필드를 클릭하면 매핑 패널이 표시됩니다. 모듈 내에서 매핑에 사용할 수 있는 모든 필드에서 매핑 패널에서 사용자가 입력하는 정적 텍스트와 함께 함수와 매핑된 항목의 조합을 사용하여 수식을 만들 수 있습니다. 이러한 요소는 서로 내부에 중첩될 수 있습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 번들 및 항목

모듈의 작업으로 0, 1 이상의 번들이 출력으로 생성됩니다. 번들은 하나 이상의 항목으로 구성됩니다.

모듈의 출력을 탐색하려면

1. 클릭 **[!UICONTROL 한 번 실행]** 를 눌러 모듈을 실행합니다.
1. 모듈 위에 있는 버블을 클릭합니다.

   모듈의 모든 단계가 포함된 로그가 표시됩니다. 모듈의 작업 단계에서 출력되는 번들 또는 번들은 **[!UICONTROL 출력]** 제목. 각 번들에는 해당 항목과 각 항목의 값이 포함되어 있습니다.

>[!INFO]
>
>**예:** 이 예는 모듈을 보여 줍니다 [!UICONTROL 이메일] > [!UICONTROL 이메일 보기]. 다음과 같은 다양한 항목이 포함된 단일 번들을 생성하는 1개의 작업을 수행했음을 알 수 있습니다 `Date`, `Email ID (UID)`, `size`등
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>모듈 사이에 래핑된 출력입니다 [!UICONTROL 반복기] 및 [!UICONTROL 누적] 그 이후에 액세스할 수 없음 [!UICONTROL 누적] 모듈.

## 항목 매핑

두 개 이상의 모듈을 연결하여 모듈 시퀀스를 생성한 후 각 모듈은 앞에 오는 모듈에 의해 출력되는 항목의 값을 처리할 수 있습니다.

모듈의 입력 필드에 항목을 할당하려면

1. 이전 모듈이나 모듈의 출력을 처리할 모듈을 클릭합니다.
1. 표시되는 모듈 설정 패널에서 이전 모듈에서 출력한 항목의 값을 사용할 필드를 클릭합니다.

   매핑 패널이 열립니다.

1. 매핑 패널에서 항목을 클릭하여 필드에 삽입합니다.
1. (선택 사항) 매핑 패널에서 특정 필드를 검색하려면 매핑 패널 검색 막대를 클릭하고 검색할 용어를 입력합니다. 목록에 해당 필드가 나타나면 필드를 클릭합니다.

   검색 결과에 검색어가 포함되며 대/소문자를 구분하지 않습니다.

자세한 내용은 [에서 모듈 설정 구성 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## 공식

여러 항목을 필드에 매핑하고 리터럴(고정 값)과 결합하고 연산자 및 함수를 사용하여 복잡한 공식을 만들 수 있습니다.

![](assets/operators-and-functions-350x187.png)

매핑 패널의 탭 중 하나에서 함수와 연산자를 찾을 수 있습니다.

![](assets/functions-toolbar-350x189.png)

첫 번째 탭 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (패널을 열 때 표시됨)에는 다른 모듈에서 매핑할 수 있는 항목이 표시됩니다.

다른 탭에는 다음과 같은 유형의 함수가 포함되어 있습니다.

* **일반 함수** ![](assets/toolbar-icon-general-function.png) - 다음을 참조하십시오. [의 일반 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 추가 정보.

* **수학 함수** ![](assets/toolbar-icon-math-functions.png) - 다음을 참조하십시오. [의 수학 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 추가 정보.

* **텍스트 및 이진 함수** ![](assets/toolbar-icon-text&binary-functions.png) - 다음을 참조하십시오. [의 문자열 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 추가 정보.

* **날짜 및 시간** ![](assets/toolbar-icon-date&time-functions.png) - 다음을 참조하십시오. [의 날짜 및 시간 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 자세한 내용은 아래 문서를 참조하십시오.

   * [의 날짜 및 시간 형식에 대한 토큰 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Adobe Workfront Fusion의 날짜 및 시간 구문 분석에 대한 토큰](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **어레이 작업 기능** ![](assets/toolbar-icon-functions-for-arrays.png) - 다음을 참조하십시오. [의 배열 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 추가 정보.

>[!TIP]
>
>다른 필드에서 다시 사용하려는 복잡한 수식을 만들 때, 조합이 들어 있는 필드를 클릭하고 Command-A 또는 Ctrl-A를 사용하여 선택한 다음 복사하여 다른 필드에 붙여넣을 수 있습니다.

함수를 사용하여 항목 매핑에 대한 자세한 내용은 [에서 함수를 사용하여 항목 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## 컬렉션

일부 항목은 여러 유형의 여러 값을 포함할 수 있습니다. 컬렉션 유형 항목입니다.

를 식별할 수 있습니다 [!UICONTROL 컬렉션] 항목의 레이블 오른쪽에 표시되는 작은 검은색 사각형과 자동으로 확장된 하위 항목 목록을 사용하여 항목을 입력합니다.

![](assets/collection.png)

>[!NOTE]
>
>대부분의 경우 전체 컬렉션을 나타내는 항목이 아니라 컬렉션의 하위 항목을 매핑합니다.

컬렉션에 대한 자세한 내용은 [의 항목 데이터 유형 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

## 어레이

일부 항목은 같은 유형의 여러 요소를 포함할 수 있습니다. 배열 유형 항목입니다.

항목 레이블 끝에 있는 대괄호로 배열 유형 항목을 식별할 수 있습니다. 항목 레이블 오른쪽에 있는 작은 검은색 사각형을 클릭하여 요소의 항목을 표시합니다.

![](assets/array.png)

배열에 대한 자세한 내용은 [의 항목 데이터 유형 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### 배열의 첫 번째 요소 매핑

배열의 `Recipient name` 항목, 다음과 같은 필드에 표시됩니다.

![](assets/map-array-1st-element.png)

대괄호 안의 숫자는 사용할 배열의 요소를 결정하는 인덱스입니다. 기본적으로 1로 설정되어 있습니다.

### 배열의 n번째 요소 매핑

다른 요소에 액세스하려면 대괄호를 클릭하고 인덱스 값을 편집합니다.

![](assets/access-another-element.png)

### 배열의 요소를 지정된 키에 매핑

일부 배열에는 키 및 값 항목이 있는 컬렉션이 여러 개 있습니다. 일반적으로 다양한 메타데이터, 속성 등입니다.

다음 예는 의 결과를 보여 줍니다 [!DNL Jira] 앱.

![](assets/output-of-jira-app-350x100.png)

이 예에서는 ID가 10108인 특정 첨부 파일의 첨부 파일 배열에서 파일 이름을 가져옵니다.

출력 위치 [!DNL Jira] 의 모습은 다음과 같습니다.

![](assets/output-from-jira-350x261.png)

일반적인 요구 사항은 주어진 키 값으로 요소를 검색하고 값 항목에서 해당 값을 가져오는 것입니다. 이 방법은 `map()` 및 `get()` 함수 위에 있어야 합니다.

다음은 수식의 세부 분류입니다.

1. 의 첫 번째 매개 변수 `map()` 함수는 전체 배열 항목입니다.
1. 두 번째 매개 변수는 값 항목의 원시 이름입니다. 원시 이름을 얻으려면 [!UICONTROL 매핑] 패널:

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >모든 매개 변수는 대/소문자를 구분합니다. 이 특정 예제에서 항목의 레이블은 원래 이름과 대문자로만 다르지만 레이블 Value와 대조적으로 모두 소문자인 원시 이름을 사용해야 합니다.

1. 세 번째 매개 변수는 키 항목의 원시 이름입니다.

   ![](assets/3rd-parameter-350x166.png)

1. 네 번째 매개 변수는 주어진 키 값입니다.

왜냐하면 `map()` 함수는 배열을 반환합니다(지정된 키 값이 있는 요소가 더 있을 수 있으므로). `get()` 첫 번째 요소를 가져오는 함수:

* 의 첫 번째 매개 변수 `get()` 함수는 `map()` 함수 위에 있어야 합니다.

* 두 번째 매개 변수는 요소의 색인(하나)입니다.

에 대한 자세한 정보 `map()` 함수 위에 있어야 합니다. [의 배열 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

에 대한 자세한 정보 `get()` 함수 위에 있어야 합니다. [의 일반 함수 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## 요소를 일련의 번들로 변환

어레이는 [!UICONTROL 반복기] 모듈. 자세한 내용은 [[!UICONTROL 반복기] 모듈 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## 문제 해결

### 매핑 패널에서 항목이 누락됨

각 모듈에 대해 매핑 패널에는 모듈 작성자가 나열한 모든 출력 항목이 표시됩니다. 경우에 따라 이 목록이 불완전할 수 있으며 일부 항목이 누락될 수 있습니다. [!DNL Workfront Fusion] 시나리오 편집기에서 모듈을 실행할 때 누락된 출력 항목을 자동으로 검색할 수 있습니다. 정확한 절차는 모듈 유형에 따라 약간 다릅니다.

#### 즉시 트리거

1. 모듈을 마우스 오른쪽 단추로 클릭한 다음 **[!UICONTROL 이 모듈만 실행]** 를 클릭합니다.

   대기 중인 웹 후크가 없는 경우 모듈은 새 웹 후크가 처리될 때까지 기다립니다.

1. 웹 후크를 생성합니다.

   예를 들어 웹 후크 모듈입니다 **[!DNL Slack]>[!UICONTROL 새 이벤트 수신]** (채널에서 새 채널 메시지를 감시하는)는 채널로 메시지를 보냅니다.

1. 모듈 실행이 완료되면 모듈 위의 버블을 클릭하여 전체 출력을 탐색합니다.

   매핑 패널에는 모듈의 출력에서 검색된 모든 항목이 포함됩니다.

#### 폴링 트리거

1. 모듈을 마우스 오른쪽 단추로 클릭한 다음 **[!UICONTROL 이 모듈만 실행]** 를 클릭합니다.
1. 출력이 없으면 를 클릭합니다 **[!UICONTROL 시작할 위치 선택]** 설정을 조정합니다.
1. 처리할 이벤트가 없으면 이벤트를 만들고 2단계로 돌아갑니다.

   예를 들어 웹 후크 모듈입니다 **[!UICONTROL Gmail] >[!UICONTROL 이메일 보기]** 모듈이 보고 있는 폴더로 이메일을 보냅니다.

1. 모듈 실행이 완료되면 모듈 위의 버블을 클릭하여 전체 출력을 탐색합니다.

   이제 매핑 패널에 모듈의 출력에서 검색된 모든 항목이 포함됩니다.

#### 기타 모듈

다음을 실행하도록 선택할 수 있습니다.

* 전체 시나리오(또는 모듈이 포함된 부품)

   시나리오가 트리거로 시작하는 경우 [즉시 트리거](#instant-trigger) 또는 [폴링 트리거](#polling-trigger) 섹션에 있는 마지막 항목이 될 필요가 없습니다.

* 단일 모듈만

단일 모듈만 실행되도록 선택하는 경우:

1. 모듈을 마우스 오른쪽 단추로 클릭한 다음 **[!UICONTROL 이 모듈만 실행]** 표시되는 메뉴에서..
1. 입력 항목에 대한 샘플 값을 제공한 다음 **[!UICONTROL 확인]** .
1. 모듈 실행이 완료되면 모듈 위의 버블을 클릭하여 전체 출력을 탐색합니다.

   이제 매핑 패널에 모듈의 출력에서 검색된 모든 항목이 포함됩니다.
