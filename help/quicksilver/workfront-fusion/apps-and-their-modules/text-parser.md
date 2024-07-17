---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: 텍스트 구문 분석기
description: Text 파서 도구를 사용하여 다른 [!DNL Adobe Workfront Fusion] 시나리오 모듈에서 사용할 텍스트를 구문 분석할 수 있습니다. 텍스트 파서는 연결할 필요가 없습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 0%

---

# [!UICONTROL 텍스트 구문 분석기]

[!UICONTROL 텍스트 파서 도구]를 사용하여 다른 [!DNL Adobe Workfront Fusion] 시나리오 모듈에서 사용할 텍스트를 구문 분석할 수 있습니다. [!UICONTROL 텍스트 구문 분석기]에는 연결이 필요하지 않습니다.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## [!UICONTROL 텍스트 구문 분석기] 모듈과 해당 필드

[!UICONTROL 텍스트 파서] 모듈을 구성할 때 [!DNL Adobe Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

### 트랜스포머

* [[!UICONTROL HTML에서 요소 가져오기]](#get-elements-from-html)
* [[!UICONTROL 텍스트에서 요소 가져오기]](#get-elements-from-text)
* [[!UICONTROL 텍스트 HTML]](#html-to-text)
* [[!UICONTROL 패턴 일치]](#match-pattern)
* [[!UICONTROL 바꾸기]](#replace)

#### [!UICONTROL HTML에서 요소 가져오기]

HTML 코드에서 원하는 요소를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 모듈이 일치 항목을 찾지 못하더라도 라우트 실행을 계속합니다.]</td> 
   <td> <p>이 옵션을 활성화하면 모듈이 결과를 반환하지 않는 경우 시나리오를 중지하지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 요소 유형]</td> 
   <td> <p> HTML 코드에서 검색할 요소의 유형을 선택합니다. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame 요소]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>지정된 요소 유형을 가져올 HTML 코드를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 텍스트에서 요소 가져오기]

제공된 패턴을 기반으로 텍스트에서 요소를 구문 분석합니다.

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

#### [!UICONTROL 텍스트 HTML]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>일반 텍스트로 변환할 HTML 코드를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 줄 바꿈] </td> 
   <td> <p>줄바꿈(줄 바꿈) 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 대문자]</p> </td> 
   <td> <p>제목 태그로 둘러싸인 텍스트(&lt;h2&gt; &lt;/h2&gt; 등)를 대문자로 변환하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 패턴 일치]

[!UICONTROL 패턴 일치] 모듈을 사용하면 지정된 텍스트에서 검색 패턴과 일치하는 문자열 요소를 찾아 추출할 수 있습니다. 이 모듈에서는 정규 표현식(regex 또는 regexp라고도 함)을 사용합니다.

정규 표현식은 각 문자가 특별한 의미를 갖는 메타문자 또는 리터럴 의미를 갖는 정규 문자인 문자의 시퀀스입니다. 이러한 문자 및 메타문자는 텍스트 검색에 사용할 수 있는 패턴을 식별합니다. 예를 들어 이름을 검색하려면 정규 표현식을 설정하여 대문자로 시작하는 연속된 두 단어로 구성된 패턴을 검색할 수 있습니다. 정규 표현식은 텍스트를 검색하고 조작할 수 있는 강력한 도구입니다.

정규 표현식에 대한 논의는 이 글의 범위를 벗어난다. 다음 리소스를 권장합니다.

* 전체 메타문자 목록은 MDN 웹 문서에서 [정규 표현식](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)을(를) 참조하십시오.
* 정규식을 만드는 방법에 대한 자습서를 보려면 [RegexOne](https://regexone.com/)을 사용하는 것이 좋습니다.
* 정규식으로 실험하려면 [정규식 101](https://regex101.com/) 웹 사이트를 사용하는 것이 좋습니다. 왼쪽 패널에서 ECMAScript(JavaScript) 버전 을 선택합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>정규 표현식 패턴을 입력합니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code>은(는) 제공된 텍스트에서 모든 숫자를 추출합니다.</p> <p>참고:  <p>패턴은 괄호 <code>()</code>에 캡처 그룹을 하나 이상 포함해야 합니다. 패턴에 캡처 그룹이 없으면 출력 번들은 비어 있습니다.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 전역 일치]</td> 
   <td> <p>텍스트에서 모든 일치 항목을 검색하려면 이 옵션을 활성화합니다. 각 일치 항목은 별도의 번들로 출력됩니다. 이 옵션이 비활성화되면 모듈은 첫 번째 항목만 검색합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대/소문자 구분]</td> 
   <td> <p> 이 모듈에서 텍스트를 대소문자를 구분하도록 하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>시작 및 끝 메타문자(<code>^</code> 및 <code>$</code>)가 전체 입력 문자열의 시작 또는 끝뿐만 아니라 각 줄의 시작 또는 끝과 일치하도록 하려면 이 옵션을 활성화하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>이 옵션을 활성화하여 마침표(.)가 줄 바꿈 문자(<code>\n</code>)와 일치합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 모듈이 결과를 반환하지 않더라도 라우트 실행을 계속합니다.]</td> 
   <td> <p>이 옵션을 활성화하면 모듈이 결과를 반환하지 않는 경우 시나리오를 중지하지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>패턴과 일치시킬 텍스트를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 바꾸기]

입력한 텍스트에서 지정된 값이나 정규 표현식을 검색하고 결과를 새 값으로 바꿉니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>검색어를 입력합니다. 정규 표현식을 사용할 수도 있습니다. 정규 표현식에 대한 자세한 내용은 <a href="#match-pattern" class="MCXref xref">[!UICONTROL 일치 패턴]</a> 모듈을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 값]</td> 
   <td> <p> 검색어를 대체할 값을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 전역 일치]</td> 
   <td> <p>텍스트에서 모든 일치 항목을 검색하려면 이 옵션을 활성화합니다. 각 일치 항목은 별도의 번들로 출력됩니다. 이 옵션이 비활성화되면 모듈은 첫 번째 항목만 검색합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 대/소문자 구분]</td> 
   <td> <p> 이 모듈에서 텍스트를 대소문자를 구분하도록 하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>시작 및 끝 메타문자(<code>^</code> 및 <code>$</code>)가 전체 입력 문자열의 시작 또는 끝뿐만 아니라 각 줄의 시작 또는 끝과 일치하도록 하려면 이 옵션을 활성화하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>이 옵션을 활성화하여 마침표(.)가 줄 바꿈 문자(<code>\n</code>)와 일치합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>검색할 텍스트를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 데이터 스크래핑

웹 스크래핑, 데이터 추출 또는 웹 수확 이라고도 하는 데이터 스크래핑은 웹 사이트에서 데이터를 수집하여 로컬 데이터베이스나 스프레드시트에 저장하는 프로세스입니다. 웹 사이트에서 데이터를 스크랩하려는 경우 정규 표현식에 익숙하지 않은 경우 데이터 스크랩 도구를 사용할 수 있습니다.

데이터 스크래핑 도구가 REST API를 제공하는 경우 범용 [[!UICONTROL HTTP] 모듈](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) 및 [웹후크](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) 모듈을 통해 연결할 수 있습니다.
