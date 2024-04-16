---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion에서 시나리오 만들기
description: 다음 작업에서는 를 만드는 방법을 설명합니다. [!DNL Adobe Workfront Fusion] 시나리오.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 0%

---

# 에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]

다음 작업에서는 를 만드는 방법을 설명합니다. [!DNL Adobe Workfront Fusion] 시나리오.

자동화 시나리오를 만드는 과정을 안내하는 연습은 를 참조하십시오. [에서 연습 자동화 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

제공하는 데이터를 사용하여 통합 시나리오를 만드는 과정을 안내하는 연습 문제는 다음을 참조하십시오. [Adobe Workfront Fusion에서 연습 통합 시나리오 만들기](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>템플릿에서 시나리오를 만들려면 다음을 참조하십시오. [다음을 사용하여 시나리오 만들기 [!DNL Adobe Workfront Fusion] 템플릿](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 시나리오 만들기 시작

1. 클릭 **[!UICONTROL 시나리오]** ![](assets/scenarios-icon.png) 왼쪽 패널에서

1. 클릭 **[!UICONTROL 새 시나리오 만들기]** 페이지의 오른쪽 상단 모서리에서 을 참조하십시오.
1. 표시되는 화면(시나리오 편집기)에서 새 시나리오를 만드는 경우 **[!UICONTROL 새 시나리오]** 왼쪽 위 모서리에 시나리오의 이름을 입력합니다.
1. 계속 진행 [시나리오에 모듈 추가](#add-a-module-in-a-scenario).

## 시나리오에 모듈 추가

1. 시나리오에 첫 번째 모듈을 추가하려면 물음표 아이콘을 클릭합니다. ![](assets/question-mark-icon.gif)

   또는

   시나리오에 모듈을 추가하려면 따르려는 모듈의 오른쪽에 있는 핸들을 클릭합니다.

1. 표시되는 상자에서 시작하려는 앱 또는 서비스를 찾아 클릭합니다.

   이전에 선택한 모든 앱은 쉽게 액세스할 수 있도록 상자에 표시되고 **[!UICONTROL 즐겨찾기]** 섹션 을 참조하십시오.

   다음을 클릭: **[!UICONTROL 다른 모듈 추가]**&#x200B;를 검색하는 경우, 표시되는 모듈은 모듈을 추가하는 시나리오의 위치에 따라 다릅니다. 일부 모듈은 다른 모듈 사이에만 배치할 수 있고 다른 모듈은 시나리오의 시작 위치에만 배치할 수 있습니다.

   >[!TIP]
   >
   >두 가지 가장 일반적인 모듈 유형은 작업과 트리거입니다. 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md).

1. 표시되는 모듈 목록에서 시나리오에 추가할 첫 번째 모듈을 클릭합니다.

   표시되는 모듈은 시나리오에서 모듈을 추가할 위치에 따라 다릅니다. 일부 모듈은 다른 모듈 사이에만 배치할 수 있고 다른 모듈은 시나리오의 시작 위치에만 배치할 수 있습니다.

   두 가지 가장 일반적인 모듈 유형은 작업과 트리거입니다. 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md).

1. 계속 진행 [모듈의 앱 또는 웹 서비스 연결 [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## 모듈의 앱 또는 웹 서비스 연결 [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

앱에 연결하는 Workfront Fusion 모듈(예: [!DNL Workfront], [!DNL Salesforce], 또는 [!DNL Jira)] 기능: [!UICONTROL 연결] 필드. 여기에서 이 모듈에서 앱에 연결하는 데 사용할 연결을 지정할 수 있습니다. 드롭다운에서 기존 연결을 선택하거나 새 연결을 만들 수 있습니다.

시나리오에서 앱에 대한 연결을 선택하거나 만들 때 이후 모듈을 설정할 때 다른 연결을 선택하지 않는 한 해당 앱에 대한 다른 모듈이 자동으로 동일한 연결을 사용합니다.

자세한 내용은 [연결 개요](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

내부 연결을 만들려면 [!DNL Workfront Fusion] 모듈:

1. 클릭 **[!UICONTROL 추가]** 을(를) 열려면 **[!UICONTROL 연결 만들기]** 상자.
1. (선택 사항) 기본값 변경 **[!UICONTROL 연결 이름]**.
1. (조건부) 앱에 ID, 키 또는 [!UICONTROL 비밀]를 누르고 해당 정보를 입력합니다.

   다음을 클릭해야 할 수 있습니다. **[!UICONTROL 고급 설정 표시]** 이러한 정보를 입력할 수 있는 필드를 표시합니다.

1. 클릭 **[!UICONTROL 계속]**.
1. 아직 로그인하지 않은 경우 표시되는 로그인 창에서 자격 증명을 입력하여 앱에 로그인합니다.
1. (조건부) **[!UICONTROL 허용]** 버튼을 표시하고 커넥터가 수행할 수 있는 작업을 검사한 다음 버튼을 클릭하여 앱을 연결합니다. [!DNL Workfront Fusion].
1. 계속 진행 [모듈 구성](#configure-the-module).


## 모듈 구성

1. 연결 필드 아래의 필드에서 모듈에 대한 설정을 구성한 다음 를 클릭합니다 **[!UICONTROL 확인]**.

   ![](assets/conf-settigs-mod-350x547.png)

   이러한 설정은 모든 모듈에 대해 다릅니다. 굵은 제목은 필수 설정을 나타냅니다.

   >[!TIP]
   >
   >시나리오에 대한 작업을 수행할 때 언제든지 모듈을 클릭하여 이 설정 상자를 표시할 수 있습니다.
   >
   >
   >모듈에 검정색 원이 표시되면 설정 구성이 완료되지 않은 것입니다. 모듈을 클릭하여 열고 구성을 계속합니다.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. 시나리오의 첫 번째 모듈을 추가하는 경우 실행할 때마다 시나리오가 시작될 위치를 나타내는 옵션을 선택합니다.

   ![](assets/choose-where-start-350x194.png)

1. 섹션의 단계를 반복합니다 [시나리오에 모듈 추가](#add-a-module-in-a-scenario) 및 [모듈 구성](#configure-the-module) 다른 모듈을 시나리오에 추가합니다.

1. (선택 사항) 모듈 또는 모듈 그룹을 복사하여 붙여넣습니다.

   자세한 내용은 [Adobe Workfront Fusion의 모듈 또는 시나리오 복사](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. 계속 진행 [시나리오 구성 및 작업](#configure-and-work-with-your-scenario).

## 시나리오 구성 및 작업

1. 시나리오를 구성하려면 다음 중 하나를 수행하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">시나리오가 실행되는 시기와 빈도를 지정합니다.</td> 
      <td> <p>시계 아이콘을 클릭합니다. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>자세한 내용은 <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">시나리오 예약 위치 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경로 설정</td> 
      <td> <p>렌치 아이콘 클릭 <img src="assets/wrench-icon.gif"> 두 모듈 사이에서 다음 옵션 중 하나를 사용합니다. 자세한 내용은 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">의 시나리오에 필터 추가 [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL 필터 설정]</strong>: 시나리오의 특정 지점에서 사용되는 번들을 제어합니다.</li> 
        <li><strong>[!UICONTROL 연결 해제]</strong>: 경로를 제거합니다.</li> 
        <li><strong>[!UICONTROL 라우터 추가]</strong>: 모듈 사이에 라우터를 추가합니다. </li> 
        <li><strong>[!UICONTROL 모듈 추가]</strong>: 모듈 사이에 새 모듈을 추가합니다.</li> 
        <li><strong>[!UICONTROL 메모 추가]</strong>: 경로에 메모를 추가합니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">시나리오 설정 구성</td> 
      <td>[!UICONTROL 시나리오 설정] 아이콘을 클릭합니다. <img src="assets/gear-icon-settings.png"> 이러한 설정은 주로 고급 사용자를 위한 것입니다. 자세한 내용은 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">의 시나리오 설정 패널 [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">흐름 제어 설정 구성</td> 
      <td> <p>[!UICONTROL 흐름 제어] 아이콘을 클릭합니다. <img src="assets/flow-control-icon.gif"> 주어진 횟수만큼 반복하도록 작업을 설정하고, 배열을 일련의 번들로 변환하고, 여러 번들을 하나의 번들로 병합할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">의 흐름 제어 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">고급 도구를 사용하여 시나리오 개선</td> 
      <td>다음을 클릭합니다. [!DNL Tools] 아이콘. <img src="assets/tools-icon.gif"> 트리거, 작업, 집계 및 변환기를 만들 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">도구</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 텍스트 구문 분석 도구</td> 
      <td>다음을 클릭합니다. [!DNL Text parser] 아이콘 <img src="assets/text-parser-icon.gif">. HTML 코드에서 요소를 검색하고, 검색 패턴과 일치하는 문자열 요소를 찾아 추출하고, 텍스트를 검색하여 바꾸고, 웹 사이트에서 데이터를 "스크랩"할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">도구</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 시나리오 작업을 수행하려면 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">시나리오가 실행될 때 발생하는 이벤트 로그 보기</td> 
      <td> <p>[!UICONTROL 편집 종료] 화살표를 클릭합니다 <img src="assets/exit-editing-arrow.png"> 시나리오 편집기에서 시나리오 세부 사항 페이지를 볼 수 있습니다. 로그는 창 아래쪽이나 오른쪽 아래 모서리에 표시됩니다. 여기에는 각 단계에 대한 정보와 시나리오를 실행하는 동안 발생한 모든 오류가 포함되어 있습니다.</p> <p>로 돌아가서 의 시나리오를 사용하여 작업 [!DNL scenario editor]시나리오 세부 사항 페이지의 아무 곳이나 클릭합니다.</p> <p>시나리오 세부 사항 페이지에 대한 자세한 내용은 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">의 시나리오 세부 정보 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">가장 일반적으로 사용되는 앱 및 서비스에 액세스</td> 
      <td> 에서 아이콘을 클릭합니다. <strong>[!UICONTROL 즐겨찾기]</strong> 섹션 을 참조하십시오. 앱과 서비스를 시나리오에 추가할 때 아이콘이 이 섹션에 자동으로 표시됩니다. [!UICONTROL Add] 아이콘을 클릭할 수도 있습니다 <img src="assets/add-icon.gif"> 이 영역에 앱 및 서비스를 수동으로 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시나리오의 데이터 흐름 방식을 보여 주는 애니메이션 보기</td> 
      <td>[!UICONTROL 흐름 설명] 아이콘을 클릭합니다 <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">모듈 레이아웃 자동 정렬 </td> 
      <td>[!UICONTROL Auto-align] 아이콘을 클릭합니다 <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시나리오에 대한 참고 사항 입력 또는 보기</td> 
      <td>[!UICONTROL Notes] 아이콘을 클릭합니다. <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">모듈 제거</td> 
      <td>모듈을 마우스 오른쪽 단추로 클릭한 다음 <strong>[!UICONTROL Delete module]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 시나리오를 테스트 실행하려면 **[!UICONTROL 한 번 실행]**.

   활성화하기 전에 시나리오가 예상대로 실행되는지 확인하는 것이 중요합니다. 활성화되면 시나리오는 일정에 따라 실행됩니다. 모든 것이 예상대로 실행되지 않으면 다음을 참조하십시오. [에서 오류 처리 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. 시나리오 편집이 끝나면(또는 편집하는 동안) [!UICONTROL 저장] 창 하단에 있는 아이콘 ![](assets/save-icon.gif).

시나리오 활성화에 대한 내용은 다음을 참조하십시오. [에서 시나리오 활성화 또는 비활성화 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Workfront Fusion 시나리오 키보드 단축키

시나리오를 만들거나 편집할 때 다음 키보드 단축키를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>개 액션</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 저장] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 한 번 실행]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
