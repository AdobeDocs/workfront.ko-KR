---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Devtool을 사용하여 시나리오 디버그
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1861'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] Devtool을 사용하여 시나리오 디버그

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [시나리오 디버그](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/debug-a-scenario.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Fusion] Devtool을 사용하면 시나리오를 이해하고 문제를 해결할 수 있습니다. Devtool이 [!DNL Chrome Developer Tools]에 추가 패널을 추가합니다. 이 디버거 패널을 사용하면 시나리오의 모든 수동 실행을 확인하고, 수행된 모든 작업을 검토하고, 수행된 모든 API 호출에 대한 세부 정보를 볼 수 있습니다. 오류를 일으킨 모듈, 작업 또는 단일 응답을 확인하고 해당 지식을 사용하여 시나리오를 구체화할 수 있습니다.

>[!NOTE]
>
>비밀 시나리오, 자동 실행 및 성공적인 작업에 대해 디버거 패널의 로깅이 제한되거나 사용할 수 없습니다.

비디오 소개 및 Fusion Devtool에 대한 설명은

* [Fusion 개발 도구](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Devtool 연습](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html)

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
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
   </td>    </tr> 
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

## Workfront Fusion Devtool 액세스

Devtool 액세스는 [!DNL Adobe Unified Experience]에서 Fusion을 사용하는지 여부에 따라 다릅니다.

* [ [!DNL Adobe Unified Experience]에서 Devtool에 액세스](#access-the-devtool-in-the-adobe-unified-experience)
* [클래식 [!DNL Fusion] 경험에서 Devtool에 액세스](#access-the-devtool-in-the-classic-fusion-experience)

### [!DNL Adobe Unified Experience] 또는 새 Fusion 경험에서 Devtool에 액세스

Adobe 통합 쉘에서 Fusion을 사용하거나 새 Fusion 경험으로 업데이트한 경우 시나리오 편집기에서 개발 도구에 액세스할 수 있습니다.

1. 화면 하단 근처에 있는 **도우미 도구** ![도우미 도구](assets/debugger-icon.png) 아이콘을 클릭합니다.

또는:

1. 디버그하려는 시나리오의 시나리오 편집기로 이동합니다.

   시나리오 편집기를 찾으려면 [시나리오 편집기](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md)를 참조하십시오.

1. 모듈이 아닌 페이지의 빈 영역을 마우스 오른쪽 버튼으로 클릭합니다.
1. **Devtool 열기**&#x200B;를 선택합니다.

### 클래식 [!DNL Fusion] 경험에서 Devtool에 액세스

클래식 [!DNL Fusion] 환경에서 Devtool을 사용하려면 [!DNL Chrome] 확장을 설치해야 합니다. 그런 다음 [!DNL Chrome] 개발자 도구에서 이 확장을 사용할 수 있습니다.

* [ [!DNL Chrome] Devtool 확장 설치](#install-the-chrome-devtool-extension)
* [ [!DNL Workfront Fusion] Devtool 찾기](#locate-the-workfront-fusion-devtool)

#### [!DNL Chrome] Devtool 확장 설치

[!UICONTROL [!DNL Chrome] 웹 스토어]를 통해 [!DNL Workfront Fusion] Devtool을 [!DNL Chrome]에 추가할 수 있습니다.

1. [이 링크](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn)를 클릭하여 [!UICONTROL [!DNL Chrome] 웹 스토어의 [!DNL Workfront Fusion] Devtool](으)로 이동합니다.
1. **[!UICONTROL [!DNL Chrome]]**&#x200B;에 추가를 클릭합니다.
1. 열려 있는 창에서 권한을 검사합니다. 사용 권한에 동의하면 **[!UICONTROL 확장 추가]**&#x200B;를 클릭하세요.

[!DNL Workfront Fusion] Devtool 확장이 [!DNL Chrome] 확장에 추가됩니다.


#### [!DNL Workfront Fusion] Devtool 찾기

[!DNL Workfront Fusion] Devtool을 사용하려면 [Chrome Devtool 확장 설치](#install-the-chrome-Devtool-extension)에 설명된 대로 [!DNL Workfront Fusion] Devtool 확장을 [!DNL Chrome] 브라우저에 추가해야 합니다.

1. [!DNL Workfront Fusion] 시나리오를 엽니다.
1. [!DNL Chrome Developer Tools] 열기:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Command + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Ctrl + Shift + I</p> <p> 또는 </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >모듈을 더 잘 보려면 맨 아래에 [!DNL Chrome Developer Console]을(를) 연결하는 것이 좋습니다.

1. [!DNL Chrome Dev Tools]에서 **[!DNL Workfront Fusion]** 탭을 클릭합니다.

## [!DNL Workfront Fusion] Devtool 사용

Workfront Fusion Devtool은 3개의 기본 섹션으로 나뉩니다. Devtool 창의 왼쪽 패널에서 찾을 수 있습니다.

* [라이브 스트림](#live-stream)
* [시나리오 디버거](#scenario-debugger)
* [도구](#tools)

### 라이브 스트림

시나리오에서 한 번 실행 을 클릭하면 백그라운드에서 발생하는 상황이 라이브 스트림에 표시됩니다.

1. **[!UICONTROL 라이브 스트림]** 아이콘 ![](assets/live-stream-icon.png)을(를) 클릭하여 라이브 스트림 섹션을 엽니다.
1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>액션</th> 
      <th>지침</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">요청 정보 보기</td> 
      <td> <p>시나리오의 각 모듈에 대한 다음 정보를 볼 수 있습니다</p> 
       <ul> 
        <li> <p>요청 헤더(API 끝점 URL, http 메서드, 요청이 호출된 시간 및 날짜, 요청 헤더 및 쿼리 문자열)</p> </li> 
        <li> <p>요청 본문</p> </li> 
        <li> <p>응답 헤더</p> </li> 
        <li> <p>응답 본문</p> </li> 
       </ul> <p>이 정보를 보려면 [!DNL Workfront Fusion] Devtool의 오른쪽 패널에서 해당 탭을 클릭합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>요청 및 응답 검색</p> </td> 
      <td> <p>[!DNL Workfront Fusion] Devtool의 왼쪽 패널에 있는 검색 필드에 검색어를 입력하여 검색어가 포함된 요청만 표시합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>요청 목록 제거 </p> </td> 
      <td> <p>Devtool의 왼쪽 패널 오른쪽 위 모서리에 있는 휴지통 아이콘을 클릭하여 [!DNL Workfront Fusion] Devtool에서 기록한 요청 목록을 지웁니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>콘솔 로깅 활성화</p> </td> 
      <td> <p>Devtool의 왼쪽 패널의 오른쪽 위 모서리에 있는 컴퓨터 아이콘 <img src="assets/console-computer-icon.png">을(를) 클릭합니다.</p> <p>컴퓨터 아이콘이 녹색이면 콘솔에 로그인할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>원시 JSON 형식 또는 cURL로 요청 검색</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>원시 JSON</strong> </p> <p>Devtool 오른쪽 창의 오른쪽 위 모서리에 있는 <strong>[!UICONTROL Copy RAW]</strong>을(를) 클릭합니다.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Devtool 오른쪽 창의 오른쪽 위 모서리에서 <strong>[!UICONTROL Copy cURL]</strong>을(를) 클릭합니다.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 시나리오 디버거

시나리오 디버거는 보다 복잡한 시나리오에 유용합니다. 시나리오 실행 기록이 표시되며, 이를 사용하여 모듈 이름이나 ID로 모듈을 검색할 수 있습니다.

1. **[!UICONTROL 시나리오 디버거]** 아이콘 ![](assets/scenario-debugger-icon.png)을(를) 클릭하여 시나리오 디버거를 엽니다.
1. (선택 사항) [!UICONTROL Scenario Debugger] 섹션의 [!DNL Workfront Fusion] Devtool 왼쪽 창에 있는 검색 필드에 검색어(이름 또는 모듈 ID)를 입력합니다.
1. 모듈 이름을 두 번 클릭하여 시나리오 편집기에서 설정을 엽니다.
1. 원하는 작업을 클릭하여 요청 세부 정보를 봅니다.

### 도구

[!DNL Workfront Fusion] Devtool에는 시나리오를 더 쉽게 설정할 수 있는 도구가 있습니다.

1. **[!UICONTROL 도구]** 아이콘 ![](assets/console-tools-icon.png)을 클릭하여 도구를 엽니다.
1. 사용할 도구를 선택합니다
1. 아래에 자세히 설명된 대로 필드를 구성합니다.
1. **[!UICONTROL 실행]**&#x200B;을 클릭합니다.

도구 및 해당 필드:

* [모듈에 포커스](#focus-a-module)
* [매핑으로 모듈 찾기](#find-modules-by-mapping)
* [앱 메타데이터 가져오기](#get-app-metadata)
* [매핑 복사](#copy-mapping)
* [필터 복사](#copy-filter)
* [연결 교체](#swap-connection)
* [변수 교체](#swap-variable)
* [앱 교체](#swap-app)
* [기본 64](#base-64)
* [모듈 이름 복사](#copy-module-name)
* [Source 다시 매핑](#remap-source)
* [앱 강조 표시](#highlight-app)
* [GS 마이그레이션](#migrate-gs)

#### [!UICONTROL 모듈에 포커스]

지정된 모듈의 설정을 ID로 엽니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 모듈 ID]</td>
        <td>설정을 열 모듈의 ID를 입력합니다.</td>
    </tr>
</table>

#### [!UICONTROL 매핑으로 모듈 찾기]

지정된 용어에 대한 모듈 값을 검색할 수 있습니다. 출력에는 검색한 용어가 포함된 모듈의 ID가 포함됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 키워드]</td> 
   <td> <p> 검색할 용어를 입력합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 값만 사용]</p> </td> 
   <td> <p>모듈 필드의 값만 검색하려면 이 옵션을 활성화하십시오.</p> <p>모듈 필드 이름에서도 검색하려면 이 옵션을 비활성화하십시오.</p> <p>이름 및 레이블 매개 변수를 통해 검색이 수행됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 앱 메타데이터 가져오기]

앱의 모듈 이름 또는 ID로 앱의 메타데이터를 검색합니다. 이 기능은 예를 들어 시나리오에 사용된 앱의 버전을 알고 있어야 할 때 유용합니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>메타데이터를 검색할 모듈을 선택합니다.</td>
    </tr>
</table>

#### [!UICONTROL 매핑 복사]

소스 모듈에서 대상 모듈로 값을 복사합니다.

>[!CAUTION]
>
>올바른 소스 및 대상 모듈을 설정했는지 확인하십시오. 다른 유형의 모듈을 선택하면 대상 모듈의 값이 삭제됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> 모듈을 선택하거나 필드 값을 복사할 대상 모듈의 ID를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>모듈을 선택하거나 소스 모듈 값을 삽입할 모듈의 ID를 입력합니다.</p> <p>중요: 대상 모듈의 값을 덮어씁니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 필터 복사]

소스 모듈에서 대상 모듈로 필터 설정을 복사합니다.

>[!NOTE]
>
>선택한 모듈의 왼쪽에 배치된 필터에서 복사 작업이 수행됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> 모듈을 선택하거나 필터 값을 복사할 원본 모듈의 ID를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>모듈을 선택하거나 소스 모듈의 필터 값을 삽입할 모듈의 ID를 입력합니다.</p> <p>중요: 대상 모듈의 값을 덮어씁니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 대체 경로 설정 유지]</p> </td> 
   <td> <p>원본 필터는 대체 경로로 설정됩니다. 대상 필터가 대체 경로로 설정되도록 설정하려면 이 옵션을 활성화하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 연결 교체]

소스 모듈에서 동일한 앱의 시나리오에 있는 모든 모듈로 연결을 복제합니다.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>모듈을 선택하거나 연결을 복제할 모듈의 ID를 입력합니다.</td>
    </tr>
</table>

#### [!UICONTROL 변수 교체]

시나리오에서 지정된 변수를 검색하고 새 변수로 바꿉니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable to Find]</td> 
   <td> <p> 시나리오의 모듈에서 바꿀 변수 알약을 찾아 이 ([!UICONTROL Variable to Find]) 필드에 복사합니다. 필드에는 이중 중괄호가 표시됩니다. 예: <code>&#123;&#123;5.value&#125;&#125;</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 다음으로 바꾸기]</p> </td> 
   <td> <p>시나리오의 모듈에서 변수를 로 바꿀 변수 알약을 찾아 이 ([!UICONTROL Variable to Find]) 필드에 복사합니다. 필드에는 이중 중괄호가 표시됩니다. 예: <code>&#123;&#123;5.value&#125;&#125;</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module]</p> </td> 
   <td> <p>변수를 바꿀 모듈을 선택합니다. 모듈을 선택하지 않으면 전체 시나리오에서 변수가 대체됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 앱 교체]

시나리오에서 선택한 앱 버전을 다른 앱 버전으로 바꿉니다.

예를 들어 Gmail 및 이메일 앱의 모듈을 최신 버전으로 업그레이드하는 데 사용할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">바꿀 [!UICONTROL 앱]</td> 
   <td> <p> 바꿀 앱을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 다음으로 바꾸기]</p> </td> 
   <td> <p>바꿀 앱을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 기본 64]

입력한 데이터를 Base64로 인코딩하거나 Base64를 디코딩할 수 있습니다. 일부 요청은 Base64로 인코딩됩니다. 이 도구는 인코딩된 요청에서 특정 데이터를 검색하려는 경우 유용할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업] </td> 
   <td> <p>[!UICONTROL 원시 데이터] 필드에서 Base64로 데이터를 인코딩할지 또는 Base64에서 원시 데이터로 Base64를 디코딩할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 원시 데이터]</p> </td> 
   <td> <p> 위의 [!UICONTROL Operation] 필드에서 선택한 옵션에 따라 원시 데이터로 디코딩하려는 경우 Base64 또는 Base64로 인코딩할 데이터를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 모듈 이름 복사]

선택한 모듈의 이름을 클립보드에 복사합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Module] </td> 
   <td> <p>이름을 복사할 모듈을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Source 다시 매핑]

한 모듈에서 다른 모듈로 매핑 소스를 변경할 수 있습니다.

먼저 소스 모듈로 사용할 모듈을 시나리오의 경로에 추가해야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> 시나리오의 다른 모듈에 대한 매핑 소스로 바꿀 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>새 매핑 소스로 사용할 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Module to Edit]</p> </td> 
   <td> <p>전체 시나리오에서 매핑을 변경하지 않으려면 매핑을 변경할 모듈을 선택합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 앱 강조 표시]

시나리오에서 지정된 앱의 모듈을 강조 표시합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App to be Highlight] </td> 
   <td> <p> 시나리오에서 강조 표시할 앱을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 버전] </p> </td> 
   <td> <p>강조 표시할 앱의 버전을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 강조 표시 색상]</p> </td> 
   <td> <p> 강조 표시 모듈에 사용할 색상 16진수를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL GS 마이그레이션]

이 도구는 특히 [!DNL Google Sheets](기존) 모듈을 최신 [!DNL Google Sheets] 버전으로 업그레이드하기 위해 만들어졌습니다. 시나리오 경로에서 모듈의 기존 버전 바로 뒤에 새 버전의 모듈을 추가합니다.

이 모듈에서는 매개 변수를 설정할 필요가 없습니다.
