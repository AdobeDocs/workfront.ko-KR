---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: 텍스트 파서
description: 텍스트 파서 도구를 사용하여 다른 곳에서 사용할 텍스트를 구문 분석할 수 있습니다 [!DNL Adobe Workfront Fusion] 시나리오 모듈입니다. 텍스트 파서에는 연결이 필요하지 않습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL 텍스트 파서]

를 사용할 수 있습니다 [!UICONTROL 텍스트 파서 도구] 다른 용도로 사용할 텍스트를 구문 분석합니다. [!DNL Adobe Workfront Fusion] 시나리오 모듈입니다. 다음 [!UICONTROL 텍스트 파서] 에는 연결이 필요하지 않습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
  <td> <p>[!UICONTROL Pro] 이상</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 텍스트 파서] 모듈 및 해당 필드

구성 시 [!UICONTROL 텍스트 파서] 모듈, [!DNL Adobe Workfront Fusion] 아래 나열된 필드를 표시합니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 트랜스포머

* [[!UICONTROL HTML에서 요소 가져오기]](#get-elements-from-html)
* [[!UICONTROL 텍스트에서 요소 가져오기]](#get-elements-from-text)
* [[!UICONTROL 텍스트로 HTML]](#html-to-text)
* [[!UICONTROL 일치 패턴]](#match-pattern)
* [[!UICONTROL 바꾸기]](#replace)

#### [!UICONTROL HTML에서 요소 가져오기]

HTML 코드에서 원하는 요소를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 모듈이 일치하는 항목을 찾지 못하는 경우에도 경로 실행을 계속합니다.]</td> 
   <td> <p>결과가 반환되지 않는 경우 모듈이 시나리오를 중단하지 않도록 하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 요소 유형]</td> 
   <td> <p> HTML 코드에서 검색할 요소 유형을 선택합니다. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame 요소]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>지정된 요소 유형을 검색할 HTML 코드를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 텍스트에서 요소 가져오기]

지정된 패턴을 기반으로 텍스트에서 요소를 구문 분석합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 입력 텍스트]</td> 
   <td> <p>구문 분석할 텍스트를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>텍스트에서 구문 분석할 요소를 반영하는 패턴을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 중복 발생 무시]</td> 
   <td> <p>텍스트 요소의 중복 발생을 무시하려면 이 상자를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 텍스트로 HTML]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>일반 텍스트로 변환할 HTML 코드를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Line Break] </td> 
   <td> <p>줄바꿈 유형(라인 브레이크)을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 대문자 머리글]</p> </td> 
   <td> <p>제목 태그(예: &lt;h2&gt; &lt;/h2&gt;)을 대문자로 바꿉니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 일치 패턴]

다음 [!UICONTROL 일치 패턴] 모듈 을 사용하면 주어진 텍스트에서 검색 패턴과 일치하는 문자열 요소를 찾아 추출할 수 있습니다. 이 모듈은 정규 표현식(regex 또는 regexp라고도 함)을 사용합니다.

정규 표현식은 각 문자가 메타문자이거나, 특별한 의미를 가지거나, 리터럴 의미가 있는 정규 문자인 일련의 문자입니다. 이러한 문자 및 메타문자는 텍스트를 검색하는 데 사용할 수 있는 패턴을 식별합니다. 예를 들어 이름을 검색하려는 경우 대문자로 시작하는 두 개의 연속된 단어로 구성된 패턴을 검색하도록 정규 표현식을 설정할 수 있습니다. 정규 표현식은 텍스트를 검색하고 조작하는 강력한 도구입니다.

정규 표현식의 논의는 이 기사의 범위를 벗어난다. 다음 리소스를 권장합니다.

* 메타문자 전체 목록은 다음을 참조하십시오. [정규 표현식](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) mdn 웹 문서
* 정규 표현식을 만드는 방법에 대한 자습서는 다음과 같습니다 [RegexOne](https://regexone.com/).
* 정규 표현식을 테스트하려면 [정규 표현식 101](https://regex101.com/) 웹 사이트입니다. 왼쪽 패널에서 ECMAScript(JavaScript) FLAVOR를 선택합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>정규 표현식 패턴을 입력합니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> 제공된 텍스트에 있는 모든 숫자를 추출합니다.</p> <p>참고:  <p>패턴에는 괄호 안에 캡처 그룹이 하나 이상 있어야 합니다 <code>()</code>. 패턴에 캡처 그룹이 없으면 출력 번들이 비어 있습니다.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 전역 일치]</td> 
   <td> <p>텍스트에서 모든 일치 항목을 검색하려면 이 옵션을 활성화하십시오. 각 일치 항목은 별도의 번들로 출력됩니다. 이 옵션을 비활성화하면 모듈은 첫 번째 항목만 검색합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대/소문자 구분]</td> 
   <td> <p> 이 모듈에서 텍스트를 대/소문자를 구분하도록 처리하려면 이 옵션을 활성화하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>시작 및 종료 메타문자(<code>^</code> 및 <code>$</code>)은 전체 입력 문자열의 맨 시작 또는 끝뿐만 아니라 각 줄의 시작 또는 끝과 일치합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>기간(.)을 확인하려면 이 옵션을 활성화합니다 줄바꿈 문자(<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 모듈이 결과를 반환하지 않더라도 경로 실행을 계속합니다.]</td> 
   <td> <p>결과가 반환되지 않는 경우 모듈이 시나리오를 중단하지 않도록 하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>패턴과 일치시킬 텍스트를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 바꾸기]

입력한 텍스트에서 지정된 값 또는 정규 표현식을 검색하고 결과를 새 값으로 바꿉니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>검색어를 입력합니다. 정규 표현식을 사용할 수도 있습니다. 정규 표현식에 대한 자세한 내용은 <a href="#match-pattern" class="MCXref xref">[!UICONTROL 일치 패턴]</a> 모듈.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 값]</td> 
   <td> <p> 검색어를 대체하는 값을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 전역 일치]</td> 
   <td> <p>텍스트에서 모든 일치 항목을 검색하려면 이 옵션을 활성화하십시오. 각 일치 항목은 별도의 번들로 출력됩니다. 이 옵션을 비활성화하면 모듈은 첫 번째 항목만 검색합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대/소문자 구분]</td> 
   <td> <p> 이 모듈에서 텍스트를 대/소문자를 구분하도록 처리하려면 이 옵션을 활성화하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>시작 및 종료 메타문자(<code>^</code> 및 <code>$</code>)은 전체 입력 문자열의 맨 시작 또는 끝뿐만 아니라 각 줄의 시작 또는 끝과 일치합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>기간(.)을 확인하려면 이 옵션을 활성화합니다 줄바꿈 문자(<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>검색할 텍스트를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 데이터 스크랩

웹 스크랩, 데이터 추출 또는 웹 하베딩이라고도 하는 데이터 스크랩은 웹 사이트에서 데이터를 수집하여 로컬 데이터베이스 또는 스프레드시트에 저장하는 프로세스입니다. 웹 사이트에서 데이터를 스크랩하고 정규 표현식에 익숙하지 않은 경우 데이터 스크랩 도구를 사용할 수 있습니다.

* [Apify](https://apify.com/)
* [2019년 최고의 데이터 스크랩 도구](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

데이터 스크랩 도구가 REST API를 제공하는 경우 범용 를 통해 연결할 수 있습니다 [[!UICONTROL HTTP] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) 및 [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) 모듈.
