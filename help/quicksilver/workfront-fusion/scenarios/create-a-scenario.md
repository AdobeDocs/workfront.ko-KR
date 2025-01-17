---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion에서 시나리오 만들기
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 시나리오 만들기

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [시나리오를 만들기 위한 워크플로](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

다음 작업에서는 [!DNL Adobe Workfront Fusion] 시나리오를 만드는 방법을 설명합니다.

자동화 시나리오를 만드는 과정을 안내하는 연습 연습을 보려면 [연습 자동화 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)를 참조하십시오.

제공하는 데이터를 사용하여 통합 시나리오를 만드는 과정을 안내하는 연습 연습을 보려면 [Adobe Workfront Fusion에서 연습 통합 시나리오 만들기](../../workfront-fusion/get-started/create-a-practice-scenario.md)를 참조하십시오.

>[!NOTE]
>
>템플릿에서 시나리오를 만들려면 [템플릿을 사용하여 시나리오 만들기 [!DNL Adobe Workfront Fusion] 템플릿](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront 플랜</td>  
      <td>임의</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront 라이선스</td>  
      <td>
        새로운 기능: 표준<br>
        또는<br>
        현재: 작업 시간 이상
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion 라이선스</td>  
      <td> 
        현재: Workfront Fusion 라이센스 요구 사항이 없습니다.<br>
        또는<br>
        레거시: 모두
      </td>  
    </tr>  
    <tr>  
      <td>제품</td>  
      <td> 
        새로운 기능: Select 또는 Prime Workfront 플랜: 조직에서 Adobe Workfront Fusion을 구매해야 합니다.<br>
        Ultimate Workfront 플랜: Workfront Fusion이 포함됩니다.<br>
        또는<br>
        현재: 조직은 Adobe Workfront Fusion을 구매해야 합니다.
      </td>  
    </tr> 
  </tbody>  
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

+++

## 시나리오 만들기 시작

1. 왼쪽 패널에서 **[!UICONTROL 시나리오]** ![](assets/scenarios-icon.png)을(를) 클릭합니다.

1. 페이지의 오른쪽 상단에 있는 **[!UICONTROL 새 시나리오 만들기]**&#x200B;를 클릭합니다.
1. 표시되는 화면(시나리오 편집기)에서 새 시나리오를 만드는 경우 왼쪽 상단의 **[!UICONTROL 새 시나리오]**&#x200B;를 클릭하고 시나리오 이름을 입력하십시오.
1. [시나리오에 모듈 추가](#add-a-module-in-a-scenario)를 계속합니다.

## 시나리오에 모듈 추가

1. 시나리오에 첫 번째 모듈을 추가하려면 물음표 아이콘을 클릭합니다. ![](assets/question-mark-icon.gif)

   또는

   시나리오에 모듈을 추가하려면 따르려는 모듈의 오른쪽에 있는 핸들을 클릭합니다.

1. 표시되는 상자에서 시작하려는 앱 또는 서비스를 찾아 클릭합니다.

   이전에 선택한 모든 앱은 쉽게 액세스할 수 있도록 상자에 표시되고 화면 하단의 **[!UICONTROL 즐겨찾기]** 섹션에 표시됩니다.

   **[!UICONTROL 다른 모듈 추가]**&#x200B;를 클릭하면 표시되는 모듈은 모듈을 추가하는 시나리오의 위치에 따라 다릅니다. 일부 모듈은 다른 모듈 사이에만 배치할 수 있고 다른 모듈은 시나리오의 시작 위치에만 배치할 수 있습니다.

   >[!TIP]
   >
   >두 가지 가장 일반적인 모듈 유형은 작업과 트리거입니다. 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md)을 참조하세요.

1. 표시되는 모듈 목록에서 시나리오에 추가할 첫 번째 모듈을 클릭합니다.

   표시되는 모듈은 시나리오에서 모듈을 추가할 위치에 따라 다릅니다. 일부 모듈은 다른 모듈 사이에만 배치할 수 있고 다른 모듈은 시나리오의 시작 위치에만 배치할 수 있습니다.

   두 가지 가장 일반적인 모듈 유형은 작업과 트리거입니다. 자세한 내용은 [모듈 유형](../../workfront-fusion/modules/module-types.md)을 참조하세요.

1. 계속해서 [모듈의 앱 또는 웹 서비스를  [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion)에 연결합니다.

## 모듈의 앱 또는 웹 서비스를 [!DNL Workfront Fusion]에 연결 {#connect-the-modules-app-or-web-service-to-workfront-fusion}

앱에 연결하는 Workfront Fusion 모듈(예: [!DNL Workfront], [!DNL Salesforce] 또는 [!DNL Jira)])에는 [!UICONTROL 연결] 필드가 있습니다. 여기에서 이 모듈에서 앱에 연결하는 데 사용할 연결을 지정할 수 있습니다. 드롭다운에서 기존 연결을 선택하거나 새 연결을 만들 수 있습니다.

시나리오에서 앱에 대한 연결을 선택하거나 만들 때 이후 모듈을 설정할 때 다른 연결을 선택하지 않는 한 해당 앱에 대한 다른 모듈이 자동으로 동일한 연결을 사용합니다.

자세한 내용은 [연결 개요](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)를 참조하십시오.

![](assets/connection-field-350x169.png)

[!DNL Workfront Fusion] 모듈 내에서 연결을 만들려면:

1. **[!UICONTROL 추가]**&#x200B;를 클릭하여 **[!UICONTROL 연결 만들기]** 상자를 엽니다.
1. (선택 사항) 기본 **[!UICONTROL 연결 이름]**&#x200B;을 변경합니다.
1. (조건부) 앱에 ID, 키 또는 [!UICONTROL 암호]와 같은 고급 연결 설정이 필요한 경우 해당 정보를 입력하십시오.

   이러한 정보를 입력할 수 있는 필드를 표시하려면 **[!UICONTROL 고급 설정 표시]**&#x200B;를 클릭해야 할 수 있습니다.

1. **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
1. 아직 로그인하지 않은 경우 표시되는 로그인 창에서 자격 증명을 입력하여 앱에 로그인합니다.
1. (조건부) **[!UICONTROL 허용]** 단추가 표시되면 커넥터가 수행할 수 있는 작업을 검사한 다음 단추를 클릭하여 앱을 [!DNL Workfront Fusion]에 연결합니다.
1. [모듈을 구성](#configure-the-module)합니다.


## 모듈 구성

1. 연결 필드 아래의 필드에서 모듈에 대한 설정을 구성한 다음 **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

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

1. [시나리오에 모듈 추가](#add-a-module-in-a-scenario) 및 [모듈을 구성](#configure-the-module) 섹션의 단계를 반복하여 시나리오에 다른 모듈을 추가합니다.

1. (선택 사항) 모듈 또는 모듈 그룹을 복사하여 붙여넣습니다.

   자세한 내용은 [Adobe Workfront Fusion의 모듈 또는 시나리오 복사](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)를 참조하십시오.

1. [시나리오 구성 및 작업을 계속합니다](#configure-and-work-with-your-scenario).

## 시나리오 구성 및 작업

1. 시나리오를 구성하려면 다음 중 하나를 수행하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">시나리오가 실행되는 시기와 빈도를 지정합니다.</td> 
      <td> <p>시계 아이콘을 클릭합니다. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>자세한 내용은 <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>에서 시나리오 예약을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경로 설정</td> 
      <td> <p>두 모듈 사이에 있는 렌치 아이콘 <img src="assets/wrench-icon.gif">을(를) 클릭하고 다음 옵션 중 하나를 사용합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>의 시나리오에 필터 추가 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">를 참조하십시오.</p> 
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
      <td>[!UICONTROL 시나리오 설정] 아이콘을 클릭합니다. <img src="assets/gear-icon-settings.png"> 이러한 설정은 주로 고급 사용자를 위한 것입니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>의 시나리오 설정 패널 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">을(를) 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">흐름 제어 설정 구성</td> 
      <td> <p>[!UICONTROL 흐름 제어] 아이콘을 클릭합니다. <img src="assets/flow-control-icon.gif"> 작업을 설정하여 지정된 횟수만큼 반복하고 배열을 일련의 번들로 변환하며 여러 번들을 하나의 번들로 병합할 수 있습니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>의 <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">흐름 컨트롤을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">고급 도구를 사용하여 시나리오 개선</td> 
      <td>[!DNL Tools] 아이콘을 클릭합니다. <img src="assets/tools-icon.gif"> 트리거, 작업, 집계 및 변환기를 만들 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">도구</a>를 참조하세요.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 텍스트 구문 분석 도구</td> 
      <td>[!DNL Text parser] 아이콘 <img src="assets/text-parser-icon.gif">을(를) 클릭합니다. HTML 코드에서 요소를 검색하고, 검색 패턴과 일치하는 문자열 요소를 찾아 추출하고, 텍스트를 검색하여 바꾸고, 웹 사이트에서 데이터를 "스크랩"할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">도구</a>를 참조하세요.</td> 
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
      <td> <p>시나리오 편집기에서 [!UICONTROL 편집 종료] 화살표 <img src="assets/exit-editing-arrow.png">을(를) 클릭하여 시나리오 세부 정보 페이지를 봅니다. 로그는 창 아래쪽이나 오른쪽 아래 모서리에 표시됩니다. 여기에는 각 단계에 대한 정보와 시나리오를 실행하는 동안 발생한 모든 오류가 포함되어 있습니다.</p> <p>[!DNL scenario editor]에서 시나리오 작업으로 돌아가려면 시나리오 세부 정보 페이지의 아무 곳이나 클릭하십시오.</p> <p>시나리오 세부 정보 페이지에 대한 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>의 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">시나리오 세부 정보를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">가장 일반적으로 사용되는 앱 및 서비스에 액세스</td> 
      <td> 화면 하단의 <strong>[!UICONTROL 즐겨찾기]</strong> 섹션에서 아이콘을 클릭합니다. 앱과 서비스를 시나리오에 추가할 때 아이콘이 이 섹션에 자동으로 표시됩니다. [!UICONTROL 추가] 아이콘 <img src="assets/add-icon.gif">을(를) 클릭하여 이 영역에 앱과 서비스를 수동으로 추가할 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시나리오의 데이터 흐름 방식을 보여 주는 애니메이션 보기</td> 
      <td>[!UICONTROL 흐름 설명] 아이콘 <img src="assets/explain-flow-airplane-icon.gif">을(를) 클릭합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">모듈 레이아웃 자동 정렬 </td> 
      <td>[!UICONTROL Auto-align] 아이콘 <img src="assets/auto-align-icon.gif">을(를) 클릭합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시나리오에 대한 참고 사항 입력 또는 보기</td> 
      <td>[!UICONTROL Notes] 아이콘 <img src="assets/notes-icon.gif">을(를) 클릭합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">모듈 제거</td> 
      <td>모듈을 마우스 오른쪽 단추로 클릭한 다음 <strong>[!UICONTROL Delete module]</strong>을(를) 클릭합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 시나리오를 테스트 실행하려면 **[!UICONTROL 한 번 실행]**&#x200B;을 클릭하세요.

   활성화하기 전에 시나리오가 예상대로 실행되는지 확인하는 것이 중요합니다. 활성화되면 시나리오는 일정에 따라 실행됩니다. 모든 항목이 예상대로 실행되지 않으면 [오류 처리 위치 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md)를 참조하세요.

1. 시나리오 편집을 마치면(또는 편집하는 동안) ![](assets/save-icon.gif) 창 아래쪽에 있는 [!UICONTROL 저장] 아이콘을 클릭합니다.

시나리오 활성화에 대한 자세한 내용은 [다음 위치에서 시나리오 활성화 또는 비활성화 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)를 참조하십시오.

## Workfront Fusion 시나리오 키보드 단축키

시나리오를 만들거나 편집할 때 다음 키보드 단축키를 사용할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>액션</p> </th> 
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
