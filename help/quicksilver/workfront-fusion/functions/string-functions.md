---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 문자열 함수
description: Adobe Workfront Fusion 매핑 패널에서 다음 문자열 함수를 사용할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# 의 문자열 함수 [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii(텍스트) [분음 부호 제거])]

텍스트 문자열에서 모든 비ascii 문자를 제거합니다.

>[!INFO]
>
>**예:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
   >
   >   반환: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
   >
   >   반환: [!UICONTROL escrz]


## [!UICONTROL base64 (텍스트)]

텍스트를 base64로 변환합니다.

>[!INFO]
>
>**예:**
>
>`base64( workfront )`
>
>반환: d29ya2Zyb250==

## [!UICONTROL 대문자(텍스트)]

텍스트 문자열의 첫 번째 문자를 대문자로 변환합니다.

>[!INFO]
>
>**예:**
>
>`capitalize( workfront )`
>
>반환: [!DNL Workfront]

## 포함(텍스트) search string)

텍스트에 검색 문자열이 포함되어 있는지 확인합니다.

>[!INFO]
>
>**예:**
>
>* `contains( Hello World ; Hello )`
   >
   >   반환: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
   >
   >   반환: [!UICONTROL false]


## [!UICONTROL decodeURL(텍스트)]

URL의 특수 문자를 텍스트로 디코딩합니다.

>[!INFO]
>
>**예:**
>`decodeURL( Automate%20your%20workflow )`
>
>반환: [!UICONTROL 워크플로우 자동화]

## [!UICONTROL encodeURL(텍스트)]

일부 텍스트의 특수 문자를 유효한 URL 주소로 인코딩합니다.

## [!UICONTROL escapeHTML(텍스트)]

텍스트의 모든 HTML 태그를 이스케이프 처리합니다.

>[!INFO]
>
>**예:**
>
>`escapeHTML( <b>Hello</b> )`
>
> 반환: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(텍스트)]

텍스트의 모든 Markdown 태그를 이스케이프 처리합니다.

>[!INFO]
>
>**예:**
>
>`escapeMarkdown( # Header )`
>
>반환: `&#35; Header`

## [!DNL indexOf (string; value; [start])]

문자열에서 지정된 값의 첫 번째 발생 위치를 반환합니다. 이 메서드는 검색된 값이 없으면 &#39;-1&#39;을 반환합니다. 시작 값은 문자열에서 검색이 시작되는 위치를 나타냅니다.

>[!INFO]
>
>**예:**
>
>* `indexOf( Workfront ; o )`
   >
   >   반환: 1
>
>* `indexOf( Workfront ; x )`
   >
   >   반환: -1
>
>* `indexOf( Workfront ; o ; 3 )`
   >
   >   반환: 6


## [!UICONTROL length(텍스트 또는 버퍼)]

텍스트 문자열의 길이(문자 수) 또는 이진 버퍼(바이트 크기)를 반환합니다.

>[!INFO]
>
>**예:**
>
>`length( hello )`
>
>반환: 5개

## [!UICONTROL lower(텍스트)]

텍스트 문자열의 모든 알파벳 문자를 소문자로 변환합니다.

>[!INFO]
>
>**예:**
>
>`lower( Hello )`
>
>반환: hello

## [!UICONTROL md5(텍스트)]

문자열의 md5 해시를 계산합니다.

>[!INFO]
>
>**예:**
>
>`md5( Workfront )`
>
>반환: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL 바꾸기(텍스트;검색 문자열) 대체 문자열)]

검색 문자열을 새 문자열로 바꿉니다.

>[!INFO]
>
>**예:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>반환: [!UICONTROL Hi World]

정규 표현식(묶음 `/.../`)은 플래그(예: `g`, `i`, `m`) 추가됨:

>[!INFO]
>
>**예:**
>
>![](assets/replace---1-350x31.png)
>
>이러한 모든 숫자 X X X X는 X로 대체됩니다

교체 문자열에는 다음과 같은 특수 대체 패턴이 포함될 수 있습니다.

* `$&` 일치하는 하위 문자열을 삽입합니다.
* `$n` 여기서 n은 100보다 작은 양의 정수입니다. 에서는 괄호로 묶인 n번째 하위 일치 문자열을 삽입합니다. 1색인입니다.

>[!INFO]
>
>**예:**
>
>![](assets/variable-value-350x63.png)
>
>반환: 전화 번호 `+420777111222`
>>![](assets/variable-value---2-350x55.png)
>반환: 전화 번호: `+420777111222`

>[!CAUTION]
다음과 같은 명명된 캡처 그룹을 사용하지 마십시오 `/ is (?<number>\d+)/` 를 반환합니다. 이렇게 하면 오류가 발생합니다.

정규 표현식에 대한 자세한 내용은 [텍스트 파서](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1(text; [인코딩]; [key])]

문자열의 sha1 해시를 계산합니다. 키 인수를 지정하면 sha1 HMAC 해시가 대신 반환됩니다. 지원되는 인코딩: &quot;hex&quot;(기본값), &quot;base64&quot; 또는 &quot;latin1&quot;

>[!INFO]
**예:**
`sha1( workfront )`
반환: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256(텍스트; [인코딩]; [key])]

문자열의 sha256 해시 계산. 키 인수를 지정하면 sha256 HMAC 해시가 대신 반환됩니다. 지원되는 인코딩: &quot;hex&quot;(기본값), &quot;base64&quot; 또는 &quot;latin1&quot;>

>[!INFO]
**예:**
`sha256( workfront )`
반환: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512(텍스트; [출력 인코딩]; [key]; [키 인코딩])]

문자열의 sha512 해시 계산. 키 인수를 지정하면 sha512 HMAC 해시가 대신 반환됩니다.

지원되는 인코딩:

* &quot;[!UICONTROL 육각]&quot; (기본값)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

지원되는 키 인코딩:

* &quot;[!UICONTROL 텍스트]&quot; (기본값)
* &quot;[!UICONTROL 육각]&quot;
* &quot;[!UICONTROL base64]&quot; 또는 &quot;[!UICONTROL 이진]&quot;

사용 시 &quot;[!UICONTROL 이진]&quot; 키 인코딩을 수행하려면 키가 문자열이 아닌 버퍼여야 합니다.

>[!INFO]
**예:**
`sha512(workfront)`
반환: 789ae41b9456357e4f27c6a09956a767abb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd4316390345aadf2cf7ec26e9f7fb19

## [!UICONTROL 분할(텍스트) 구분 기호)]

문자열을 부분 문자열로 구분하여 문자열을 문자열 배열로 분할합니다.

>[!INFO]
**예:**
`split( John, George, Paul ; , )`

## [!UICONTROL startcase(텍스트)]

모든 단어의 첫 번째 문자를 대문자로 지정하고 다른 모든 문자는 소문자로 바꿉니다.

>[!INFO]
**예:**
`startcase( hello WORLD )`
반환: [!UICONTROL Hello World]

## [!UICONTROL stripHTML(텍스트)]

텍스트에서 모든 HTML 태그를 제거합니다.

>[!INFO]
**예:**
`stripHTML( <b>Hello</b> )`
반환: Hello

## [!UICONTROL substring (text; start;end)]

시작 위치와 끝 위치 사이의 텍스트 문자열 일부를 반환합니다.

>[!INFO]
**예:**
* `substring( Hello ; 0 ; 3)`

   반환: 도움말
* `substring( Hello ; 1 ; 3 )`

   반환: el


## [!UICONTROL toBinary(값)]

모든 값을 이진 데이터로 변환합니다.

인코딩을 두 번째 인수로 지정하여 16진수 또는 base64에서 이진 데이터에 이진 변환을 적용할 수도 있습니다.

>[!INFO]
**예:**
* `toBinary( Workfront )`

   반환: 57 6f 72 6b 66 72 6f6e 74
* `toBinary( V29ya2Zyb250 ; base64 )`

   반환: 57 6f 72 6b 66 72 6f6e 74


## [!UICONTROL toString(값)]

모든 값을 문자열로 변환합니다.

## [!UICONTROL trim(텍스트)]

텍스트 시작 또는 끝에서 공백 문자를 제거합니다.

## [!UICONTROL 위쪽(텍스트)]

텍스트 문자열의 모든 알파벳 문자를 대문자로 변환합니다.

>[!INFO]
**예:**
`upper( Hello )`
반환: [!UICONTROL HELLO]
