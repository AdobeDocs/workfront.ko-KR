---
title: SOAP API FAQ
description: SOAP API FAQ
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: a033216655b6ab89d178291e6d019691cb175f83
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# SOAP API FAQ

## 첫 번째 파일 증명을 만들려면 어떻게 해야 합니까?

3가지 간단한 단계를 수행합니다.

**1단계**: Post 요청을 통해 파일을 Workfront 증명으로 업로드합니다.  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). 파일 해시를 반환합니다. 이는 매우 중요합니다! 이 단계에서 귀하의 계정에서 아무것도 볼 수 없습니다, 당신이 지금까지 수행 한 모든 파일을 보내지만 우리에게 그것을 어떻게 해야하는지 알려주지 않습니다.

**2단계**: 아직 세션 ID가 없는 경우 doLogin() 또는 getSessionID() 메서드를 사용하여 세션 ID를 얻습니다. 사용자의 이메일 주소와 인증 토큰이 있는 경우 전자를 사용하여 사용자의 이메일 주소와 암호를 사용하여 &#39;로그인&#39;하거나 후자의 방법을 사용합니다.

**3단계:** 이제 증명을 만들 차례입니다. createProof() 메서드를 사용하고 최소 필수 필드를 보내십시오(현재 5개 필드만 있음). 증명을 만들 때 사용할 파일을 결정할 수 있으므로 Hash 매개 변수를 &quot;1단계&quot; 중에 반환되는 파일 해시로 설정해야 합니다.

지금 계정에 로그인하면 증명이 표시됩니다.

## 첫 번째 웹 스냅숏 증명을 만드는 방법

2가지 간단한 단계를 수행합니다.

**1단계**: 아직 세션 ID가 없는 경우 doLogin() 또는 getSessionID() 메서드를 사용하여 세션 ID를 얻습니다. 사용자의 이메일 주소와 인증 토큰이 있는 경우 전자를 사용하여 사용자의 이메일 주소와 암호를 사용하여 &#39;로그인&#39;하거나 후자의 방법을 사용합니다.

**2단계:**이제 증명을 만들 차례입니다. createProof() 메서드를 사용하고 최소 필수 필드를 보내십시오(현재 5개 필드만 있음). Hash 매개 변수를 &quot;web&quot;으로 설정하고 SourceName 매개 변수를 캡처할 웹 페이지의 URL로 설정해야 합니다.

지금 계정에 로그인하면 증명이 표시됩니다.

## 증명과 버전의 차이점은 무엇입니까?

Workfront Proof에서는 버전이 단일 증명으로 표시됩니다. 웹 UI에서 특정 버전을 클릭하면 해당 버전의 세부 정보가 표시됩니다. 실제로 각 버전은 별도의 증명이며 웹 UI가 함께 표시합니다.

API의 관점에서 각 버전은 별도의 증명이며 증명은 해당 ID로 함께 연결됩니다.

**createProof()** 은(는) 항상 **버전 1** 을 참조하십시오. 이 증명에 대해 반환된 ID가 &quot;100&quot;이라고 가정해 보겠습니다.

사용 시 **createProofVersion()** 항상 이전 버전의 ID를 보냅니다. 다음을 생성하려는 경우 **버전 2** 증명 &quot;100&quot;에서 **parentFileID에 대해 &quot;100&quot;을 전달합니다.** 매개 변수. 이는 이 증명이 집합의 버전 2여야 함을 시스템에 알려줍니다. 이 메서드는 고유한 증명 ID를 반환합니다. 예를 들어 이 예제를 &quot;101&quot;이라고 가정합니다.

세 번째 버전인 경우 **버전 3** 은(는) 필수입니다. 을 호출합니다. **createProofVersion()** 이번에도 **parentFileID에 대해 &quot;101&quot;을 전달합니다.** 이렇게 하면 연결된 버전 목록이 제대로 생성됩니다.

## 모든 호출을 수행하기 전에 새 세션 ID를 받아야 합니까?

모든 세션 ID는 기본적으로 작업을 수행하는 사용자라는 점을 참고하십시오. 

API를 호출할 때마다 새 세션 ID를 가져올 필요가 없으며 24시간 동안 유효합니다. API를 호출할 때마다 만료 시간이 재설정됩니다.

## 증명/개인 URL이란 무엇입니까?

**팀/공용**: 각 증명 버전에는 고유한 팀(공개) URL이 있습니다. 활성화되면 증명이 읽기 전용 모드로 열립니다. 다음을 사용하여 팀 URL을 가져올 수 있습니다 [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) 메서드를 사용합니다.

**개인**: 개인 URL은 모든 검토자 및 증명 버전에 대해 고유합니다. 증명 세트에 3개의 버전이 포함되어 있고 검토자가 모든 버전에 있는 경우 검토자는 3개의 고유한 개인 URL을 갖게 됩니다. 개인 URL은 검토자가 이미 식별한 증명 버전을 엽니다. 따라서 안전하고 공유되지 않아야 합니다. 개인 URL은 [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) 메서드, 각 요소에 대해 반복  [SOAPRecepentObject](http://api.proofhq.com/home/objects/soaprecipientobject) 및 매개 변수 &quot;proof_url&quot;을 가져오는 중.

## >축소판을 열 때 사용자 지정 매개 변수를 포함하는 방법

축소판을 사용하면 증명 도구를 자신의 페이지에 포함할 수 있습니다. &quot;referer&quot; 매개 변수는 사용자가 miniproof에서 닫기 단추를 클릭할 때 리디렉션 URL을 제공하기 위해 miniproof의 일부로 포함될 수 있습니다. 이스케이프 처리된 &#39;&amp;&#39; 문자를 사용하여 사용자 지정 매개 변수를 추가하여 이 리디렉션 URL의 일부로 포함할 수 있습니다(예: %26).

예: miniproof URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` 은(는) (으)로 인코딩해야 합니다. 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` 사용자 지정 매개 변수를 전달하려면

## Java Web Service 클라이언트를 만드는 방법

[이 비디오](http://screencast.com/t/xsSNrqs5b) eclipse 및 Workfront Proof WSDL 정의를 사용하여 Java 웹 서비스 클라이언트를 만드는 방법을 보여 줍니다.

