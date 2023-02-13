---
title: SOAP API FAQ
description: SOAP API FAQ
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# SOAP API FAQ

## 첫 번째 파일 증명을 만들려면 어떻게 해야 합니까?

3단계로 구성됩니다.

**1단계**: 게시물 요청을 통해에 전송하여 Workfront Proof에 파일을 업로드합니다.  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). 파일 해시를 반환하겠습니다. 매우 중요합니다! 이 단계에서는 사용자 계정에 아무 것도 표시되지 않으며, 지금까지 수행한 작업은 파일을 Adobe에 보내지만 어떻게 해야 하는지 알려주지 않은 것입니다.

**2단계**: 세션 ID가 아직 없는 경우 doLogin() 또는 getSessionID() 메서드를 사용하여 세션을 얻습니다. 사용자의 이메일 주소와 암호를 사용하여 &#39;로그인&#39;하거나 사용자의 이메일 주소와 인증 토큰이 있는 경우 뒤의 메서드를 사용합니다.

**3단계:** 이제 여러분의 증거를 만들 때입니다. createProof() 메서드를 사용하여 필요한 필드(현재 5개만 있음)를 하나 이상 보내 주십시오. 증명을 만들 때 사용할 파일을 결정할 수 있도록 해시 매개 변수를 &quot;1단계&quot; 동안 반환되는 파일 해시로 설정해야 합니다.

이제 계정에 로그인하면 증명서가 표시됩니다.

## 첫 번째 웹 스냅샷 증명을 만들려면 어떻게 해야 합니까?

간단한 2단계를 수행합니다.

**1단계**: 세션 ID가 아직 없는 경우 doLogin() 또는 getSessionID() 메서드를 사용하여 가져옵니다. 사용자의 이메일 주소와 암호를 사용하여 &#39;로그인&#39;하거나 사용자의 이메일 주소와 인증 토큰이 있는 경우 뒤의 메서드를 사용합니다.

**2단계:**이제 증명을 만들 차례입니다. createProof() 메서드를 사용하여 필요한 필드(현재 5개만 있음)를 하나 이상 보내 주십시오. 해시 매개 변수를 &quot;web&quot;으로 설정하고 SourceName 매개 변수를 캡처할 웹 페이지의 URL로 설정해야 합니다.

이제 계정에 로그인하면 증명서가 표시됩니다.

## 증명과 버전 간의 차이점은 무엇입니까?

Workfront 증명 버전에는 단일 증명으로 표시됩니다. 웹 UI에서 특정 버전을 클릭하면 해당 버전의 세부 사항이 표시됩니다. 실제로 각 버전은 별도의 증거이며 웹 UI에서 함께 표시됩니다.

API의 관점에서 볼 때, 각 버전은 별도의 증명이며, 증명을 해당 ID로 함께 연결합니다.

**createProof()** 은 항상 **버전 1** 증거입니다. 이 증명 &quot;100&quot;에 대해 반환된 ID의 예를 가정해 보겠습니다.

사용 시 **createProofVersion()** 항상 이전 버전의 ID로 보내십시오. 다음과 같은 코드를 **버전 2** &quot;100&quot; 증거에서 **parentFileID에 대해 &quot;100&quot;에 전달** 매개 변수. 이는 시스템에 이 증명이 세트 버전 2여야 함을 알려줍니다. 메서드는 고유한 증명 ID를 반환합니다. 예를 들어 이 경우 &quot;101&quot;입니다.

세 번째 버전인 경우 **버전 3** 는 필수 사항이며 **createProofVersion()** 이번에는 **parentFileID에 대해 &quot;101&quot;에 전달** 연결된 버전 목록이 제대로 작성되도록 합니다.

## 모든 호출 전에 새 세션 ID를 가져와야 합니까?

모든 세션 ID는 기본적으로 작업을 수행하는 사용자임을 지적하는 것이 중요합니다. 

API를 매번 호출하기 전에 새 세션 ID를 가져올 필요가 없으며 24시간 동안 유효합니다. 만료 시간은 API를 호출할 때마다 재설정됩니다.

## 증명/개인 URL이란 무엇입니까?

**팀/공용**: 증명 버전마다 고유한 팀(공개) URL이 있습니다. 활성화된 경우 읽기 전용 모드로 증명을 엽니다. 를 사용하여 팀 URL을 가져올 수 있습니다 [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) 메서드를 사용합니다.

**개인**: 개인 URL은 모든 검토자와 증명 버전에 대해 고유합니다. 증명 세트에 3개의 버전이 포함되어 있고 검토자가 모든 버전에 있는 경우 검토자는 3개의 고유한 개인 URL을 보유하게 됩니다. 개인 URL은 검토자가 이미 식별된 증명 버전을 열므로 안전하게 보관되고 공유되지 않아야 합니다. 개인 URL은 [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) 메서드 및 각  [SOAPRecpientObject](http://api.proofhq.com/home/objects/soaprecipientobject) 매개 변수 &quot;proof_url&quot;을 가져옵니다.

## >축소판을 열 때 사용자 지정 매개 변수를 포함하는 방법

축소판을 사용하면 교정 도구를 페이지에 포함할 수 있습니다. 사용자가 축소 증명에서 닫기 단추를 클릭할 때 리디렉션 URL을 제공하기 위해 &quot;referer&quot; 매개 변수를 축소 정의의 일부로 포함할 수 있습니다. 이스케이프 처리된 &#39;&amp;&#39; 문자를 사용하여 원하는 개수의 사용자 지정 매개 변수를 이 리디렉션 URL의 일부로 포함할 수 있습니다(예: ). %26.

예를 들어, 축소 가능한 URL입니다
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` 는 로 인코딩해야 합니다. 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` 를 전달하는 것이 좋습니다.

## Java Web Service 클라이언트를 만드는 방법

[이 비디오](http://screencast.com/t/xsSNrqs5b) eclipse 및 Workfront 증명 WSDL 정의를 사용하여 Java Web Service 클라이언트를 만드는 방법을 보여 줍니다.
