---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Adobe Workfront Fusion 시나리오 예: 이메일, 텍스트 파서 및 Google Sheets 연결'
description: 이 시나리오는 모든 이메일 메시지의 로그를 만들고 스프레드시트에서 추가 작업을 위해 태그를 지정하는 데 도움이 됩니다. 검색 패턴으로 정규 표현식(Regex)을 사용하여 스프레드시트의 두 개의 별도 테이블에 이메일 본문을 캡처합니다. 상기 제1 패턴은 어구를 검색하고, 상기 제2 패턴은 동일한 어구 및 이메일 주소를 검색합니다.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 시나리오 예: 전자 메일 연결, [!UICONTROL 텍스트 구문 분석기] 및 [!DNL Google Sheets]

이 시나리오는 모든 이메일 메시지의 로그를 만들고 스프레드시트에서 추가 작업을 위해 태그를 지정하는 데 도움이 됩니다. 검색 패턴으로 정규 표현식(Regex)을 사용하여 스프레드시트의 두 개의 별도 테이블에 이메일 본문을 캡처합니다. 상기 제1 패턴은 어구를 검색하고, 상기 제2 패턴은 동일한 어구 및 이메일 주소를 검색합니다.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
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

## 전제 조건

이 자습서에서는 정규 표현식에 대한 기본 지식이 필요합니다. Regex에 대해 알아보려면 [https://regexone.com](https://regexone.com/)을(를) 방문하세요.

첫 번째 모듈을 추가하고 구성합니다.

1. 이메일을 검색하고 트리거로 **[!UICONTROL 이메일 보기]**&#x200B;를 선택합니다.

   >[!NOTE]
   >
   >E메일 모듈을 사용하여 [!DNL Google] 계정에 연결할 수 있지만 [!DNL Gmail] 모듈도 사용할 수 있습니다.

1. [!DNL Google] 계정 또는 다른 IMAP 기반 전자 메일 클라이언트(예: [!DNL Outlook])에 연결합니다.
1. 연결된 후에는 [!UICONTROL 받은 편지함]과 같이 수신 전자 메일을 감시할 폴더를 선택하십시오.
1. [!UICONTROL 기준]에서 **[!UICONTROL 모든 전자 메일]**&#x200B;을(를) 선택합니다(또는 읽거나 읽지 않은 전자 메일로 좁히기).

   가져온 이메일을 읽음 또는 읽지 않음으로 표시하도록 선택할 수도 있습니다.

1. [!UICONTROL 최대 결과 수]을(를) 1로 설정합니다.

   ![](assets/save-max-as-1-350x304.png)

   받은 메시지의 양에 따라 변경할 수 있습니다. 하지만 낮은 값을 설정하고 시나리오를 더 자주 실행하는 것이 좋습니다.

1. 맨 아래에 있는 **[!UICONTROL 고급 설정 표시]**&#x200B;를 클릭합니다.

   ![](assets/show-adv-settings-350x332.png)

1. [!UICONTROL 보낸 사람 주소], [!UICONTROL 제목] 및 [!UICONTROL 구문]을 기준으로 이메일을 필터링합니다.

   관련 이메일만 볼 수 있습니다. 이 예제에서는 제목 필터만 추가하고 나머지 2개는 비워 둡니다.

   >[!NOTE]
   >
   >[!UICONTROL 일치 패턴] 반복기와 정규식(Regex)을 검색 패턴으로 사용하여 전자 메일에서 구를 찾는 라우터를 추가합니다. 이를 통해 다중 유틸리티 시나리오를 구축할 수도 있습니다.

1. 구성이 완료되고 전자 메일 보기를 시작할 위치를 지정하라는 메시지가 표시되면 **[!DNL From now on]**&#x200B;을(를) 클릭합니다.

   ![](assets/from-now-on-350x236.png)

1. [계속 [!UICONTROL 흐름 제어 검색]을 계속하고 [!UICONTROL 라우터]](#search-for-flow-control-and-add-a-router)를 추가하십시오.

## [!UICONTROL 흐름 제어]를 검색하고 [!UICONTROL 라우터] 추가

1. 데이터를 다음 모듈로 보내기 전에 데이터를 분할하거나 복제하려면 모듈 뒤에 라우터를 추가하십시오.

   여기서는 [!UICONTROL Router]을(를) 사용하여 전자 메일 본문 텍스트를 [!DNL Google Sheet]의 두 개의 개별 테이블로 보냈습니다.

   ![](assets/search-for-flow-control-350x220.png)

## [!UICONTROL 텍스트 구문 분석기] 모듈 사용

1. [!UICONTROL 일치 패턴] 변환기를 추가하여 전자 메일에서 구를 검색합니다.

   모든 수신 이메일에서 &quot;[!UICONTROL 텍스트 구문 분석기 모듈]&quot; 구문을 검색하여 해당 구문과 일치하는 구문의 본문과 발신자 이름을 캡처합니다.

   1. 패턴을 정규 표현식으로 작성합니다.

      text\sparser\smodule

   1. (선택 사항) 다른 패턴 옵션을 사용합니다.

      ![](assets/pattern-350x318.png)

      다중 행은 텍스트에 여러 행이 포함되어 있고 각 행에서 패턴을 검색해야 하는 경우에 유용합니다. 이 자습서에서는 전체 이메일 본문 텍스트에서 패턴을 검색해야 하므로 선택하지 않고 둡니다.

   1. [!UICONTROL 텍스트] 필드의 목록에서 **텍스트 콘텐츠** 특성을 클릭합니다.

      ![](assets/text-content-350x264.png)

      패턴을 검색할 이메일 본문의 텍스트를 저장하는 속성입니다.

1. 같은 구문과 전자 메일 주소를 검색하는 다른 [!UICONTROL 일치 패턴]을(를) 추가합니다.

   이 기능은 여러 명의 사용자가 있는 고객 계정이 있는 경우 특히 유용합니다. 시간을 절약하기 위해 방금 만든 [!UICONTROL Text Parser] 모듈을 복제하고 라우터에 연결할 수 있습니다.

   ![](assets/clone.png)

1. 다음과 같이 패턴을 편집합니다.

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   이 패턴은 &quot;[!UICONTROL 텍스트 구문 분석기 모듈]&quot; 구문과 john.doe@gmail.com과 같은 전자 메일 주소를 검색하고 전자 메일 주소만 반환합니다.

   >[!NOTE]
   >
   >수락하는 이메일 주소의 사양에 따라 정규 표현식을 작성하는 것이 중요하지만 위의 정규 표현식은 대부분의 표준 이메일 주소를 처리합니다.

   * 이메일 주소만 검색하려면 아래 정규 표현식을 사용하십시오.

     ([\w.-]+@[\w.-]+)

   * 아래 정규 표현식을 사용하여 전화 번호만 검색할 수도 있습니다.

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
위의 패턴은 전화 번호가 기록되는 가장 일반적인 형식을 다룹니다.

   패턴을 테스트하려면 [!DNL javascript]과(와) 함께 [[!DNL https://regex101.com]](https://regex101.com/)을(를) 사용하는 것이 좋습니다.

   나머지 구성은 이전 구성과 동일하게 유지됩니다.

## [!DNL Google Sheets] 모듈 추가

[!DNL Sheets]의 경우 먼저 필수 헤더가 있는 스프레드시트를 만들어야 합니다.

1. 사용자 데이터를 캡처할 열이 있는 스프레드시트를 만듭니다. 기존 파일도 자유롭게 사용할 수 있습니다.

   예를 들어, 발신자 이름, 발신자 이메일 및 이메일 콘텐츠를 열로 하는 &quot;이메일 데이터: 지원 티켓&quot;이라는 것을 만듭니다. 워크시트 이름을 &quot;contains: 텍스트 파서 모듈&quot;로 지정합니다.

1. 작업으로 **[!UICONTROL 행 추가]**&#x200B;와 함께 [!UICONTROL Google 시트] 모듈을 추가합니다.

   ![](assets/add-a-row-350x174.png)

1. [!DNL Google] 계정을 연결합니다(아직 연결하지 않은 경우). 앞에서 만든 파일을 선택한 다음 데이터를 캡처할 워크시트를 선택합니다.

   설정은 다음과 같아야 합니다.

   ![](assets/connect-google-acct-350x279.png)

1. 관련 필드(열)의 속성을 매핑하여 모듈 설정을 완료합니다.

   ![](assets/map-attributes-350x282.png)

1. 방금 만든 모듈을 복제하고 두 번째 [!UICONTROL Text Parser] 모듈에 연결합니다.

   1. 스프레드시트로 이동하여 이전에 만든 워크시트를 복제하고 이름을 지정합니다.

      예를 들어 이름을 &quot;contains: 텍스트 파서 모듈 및 이메일&quot;로 지정합니다.

   1. 다른 열을 추가하여 이메일 본문에 포함된 이메일 주소를 저장합니다.

      예를 들어 이름을 &quot;이메일 주소 공유됨&quot;으로 지정합니다.

   1. 복제된 [!DNL Google Sheets] 모듈을 클릭하여 설정을 구성합니다.
   1. 워크시트를 방금 만든 새 워크시트로 변경합니다.
   1. [!UICONTROL 일치 패턴] 모듈($1)의 출력을 전자 메일 주소(전자 메일 주소 공유)를 저장할 열에 매핑합니다.

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. **[!UICONTROL 확인]**&#x200B;을 클릭하고 시나리오를 저장한 다음 테스트 실행에 사용합니다.

      다음과 같이 연결된 이메일 주소로 두 개의 이메일을 각각 보내야 합니다.

      * &quot;[!UICONTROL 텍스트 구문 분석기 모듈]&quot; 구문을 포함(전자 메일 주소 없음)

        ![](assets/text-parser-module-350x103.png)

      * 위의 구 및 이메일 주소 포함

        ![](assets/above-phrase-and-email-350x106.png)

        설정에 오류가 없으면 첫 번째 워크시트가 &quot;[!UICONTROL 텍스트 구문 분석기 모듈]&quot; 구문을 포함하는 모든 전자 메일을 캡처하는 반면 두 번째 워크시트는 &quot;[!UICONTROL 텍스트 구문 분석기 모듈]&quot; 구문과 전자 메일 주소를 포함하는 전자 메일만 캡처합니다. 아래 스크린샷을 참조하십시오.

        워크시트 1:

        ![](assets/worksheet-1-350x57.png)

        워크시트 2:

        ![](assets/worksheet-2-350x41.png)

## 리소스

* 정규식에 대해 알아보려면 [무료 연습](https://regexone.com/)
* [전화 번호 일치에 대해 알아보기](https://regexone.com/problem/matching_phone_numbers) Regex 사용
* Regex를 사용하여 [전자 메일 일치에 대해 알아보기](https://regexone.com/problem/matching_emails)
* [정규 표현식 테스트](https://regex101.com/)
