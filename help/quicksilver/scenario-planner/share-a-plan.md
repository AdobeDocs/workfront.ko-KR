---
product-area: enterprise-scenario-planner-product-area
keywords: 계획,권한,공유,이니셔티브,시나리오,시나리오
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 플래너에서 계획 공유
description: Adobe Workfront 시나리오 플래너에서 만든 플랜을 다른 사용자와 공유할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# [!DNL Scenario Planner]에서 플랜 공유

<!--Audited: 07/2024-->

[!DNL Adobe Workfront Scenario Planner]의 플랜을 다른 사용자와 공유할 수 있으므로 사용자가 수행하는 동일한 작업에 대해 공동 작업을 수행할 수 있습니다.

>[!TIP]
>
>플랜에 대한 링크를 다른 사용자에게 전송하는 경우 플랜을 볼 수 있도록 플랜을 다른 사용자와 공유해야 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 패키지</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>메모</b></p>
<p>다른 Workfront 패키지가 있는 경우 Workfront 담당자에게 문의하십시오.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스</p> </td> 
   <td> <p>[!UICONTROL Light] 이상</p> 
   <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
    <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>다음에 대한 [!UICONTROL 편집] 액세스 권한: [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>개체 권한 </p> </td> 
   <td> <p>플랜에 대한 [!UICONTROL 관리] 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

시나리오 플래너에 액세스하는 방법에 대한 자세한 내용은 [을(를) 사용하는 데 필요한 액세스 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)를 참조하십시오.

Workfront 액세스 요구 사항에 대한 자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 전제 조건

* 플랜에 대한 권한을 부여받은 사용자는 [!DNL Scenario Planner] 관리자가 부여한 대로 자신의 액세스 수준에서 [!DNL Workfront] 영역에 액세스할 수 있어야 플랜에 대한 권한을 받을 수 있습니다.

  예를 들어 [!UICONTROL 요청자]은(는) 계획을 보거나 만들거나 편집할 수 없습니다. 요청자 라이선스를 가진 사용자와 플랜을 공유할 때는 이 점을 염두에 두어야 합니다.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

다양한 라이선스 유형에 대한 [!DNL Scenario Planner] 액세스에 대한 자세한 내용은 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)를 참조하십시오.

## 플랜 공유에 대한 고려 사항

* 시스템 관리자를 포함한 모든 사용자는 자신이 생성한 플랜에만 액세스할 수 있습니다.
* 단일 계획을 공유하거나 여러 계획을 일괄적으로 공유할 수 있습니다.
* 본인이 만들지 않았거나 본인과 공유하지 않은 플랜은 볼 수 없습니다.
* 플랜은 다른 사용자와만 공유할 수 있습니다. 그룹, 팀 또는 회사와 플랜을 공유할 수 없습니다.
* 플랜을 공유하려면 먼저 저장해야 합니다.
* 플랜에 대한 URL을 다른 사용자와 공유할 수 있습니다. 사용자에게 플랜을 볼 수 있는 권한이 없는 경우 URL을 수신할 때 다른 사용자에게 플랜에 대한 액세스를 요청할 수 있습니다. 플랜에 대한 액세스 요청에 대한 자세한 내용은 [의 플랜에 대한 액세스 요청 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)을 참조하십시오.
* 다른 사용자와 이미 공유된 여러 플랜을 공유할 때 공유하는 사용자는 바꾸지 않고 선택한 각 플랜의 기존 사용자에 추가됩니다.

## 플랜 권한 옵션

다음 표에는 계획을 공유할 때 부여할 수 있는 권한이 나열되어 있습니다. 사용자가 라이선스를 기반으로 하는 액세스 권한에 대한 자세한 내용은 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)를 참조하십시오.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL 관리]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL 보기]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>플랜 보기 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>이니셔티브 보기 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>시나리오 보기</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>작업 역할 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>비용 및 예산 정보 보기*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>비용 및 예산 정보 관리*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>이니셔티브 만들기</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>시나리오 만들기</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>이니셔티브 또는 시나리오 삭제</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>시나리오 복사</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>시나리오 게시**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*플랜에 대한 관리 권한이 있더라도 플랜에 대한 재무 정보를 보거나 관리하려면 재무 데이터에 대한 액세스 권한이 있어야 합니다. 재무 데이터에 대한 액세스 정보는 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

**시나리오를 게시할 수 있도록 프로젝트를 만들고 관리할 수 있는 액세스 권한이 있어야 합니다.

프로젝트 액세스 수준에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)를 참조하십시오.

프로젝트 권한에 대한 자세한 내용은 [프로젝트 공유 [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)를 참조하십시오.

## 플랜 공유

{{step1-to-scenario-planner}}

1. 계획명을 눌러 계획 열기

   또는

   여러 플랜을 선택하여 일괄적으로 공유할 수 있습니다.

   >[!TIP]
   >
   >플랜 헤더의 오른쪽 상단 모서리에서 플랜을 공유하는 사용자의 아바타를 클릭하여 플랜을 공유할 수 있습니다.

1. (조건부) 플랜을 연 경우 **[!UICONTROL 플랜]** 이름 오른쪽에 있는 ![자세히](assets/more-icon.png) 아이콘 [!UICONTROL 자세히 아이콘]을 클릭한 다음 **[!UICONTROL 공유]**&#x200B;를 클릭합니다

   또는

   여러 개의 플랜을 일괄적으로 공유하도록 선택한 경우 플랜 목록 상단의 **[!UICONTROL 공유]** 아이콘 ![](assets/share-icon-26x26.png)을(를) 클릭하여 [!UICONTROL 플랜] 액세스 상자를 엽니다.

   >[!TIP]
   >
   >* 선택한 모든 계획에 대한 권한이 있는 사용자가 [!UICONTROL 계획] 액세스 상자에 표시됩니다.
   >* 추가 사용자가 추가되며 선택한 모든 플랜의 기존 사용자를 대체하지 않습니다.

1. **[!UICONTROL 플랜 액세스 권한 부여]** 필드에서 플랜을 공유할 사용자의 이름을 입력한 다음 목록에 표시될 때 선택합니다.
1. 사용자 이름의 오른쪽에 있는 권한 드롭다운 메뉴에서 플랜에 부여할 권한 수준을 선택합니다.
1. 다음 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 보기]</td> 
      <td>플랜을 공유하는 사용자는 플랜을 볼 수 있는 권한이 있습니다. 계획에 대한 정보를 편집하거나, 이니셔티브, 시나리오를 추가하거나, 시나리오를 게시할 수 없습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 관리]</td> 
      <td> <p>플랜을 공유하는 사용자는 정보 편집, 이니셔티브 추가, 시나리오 추가 및 플랜 게시를 포함하여 플랜을 관리할 수 있는 권한이 있습니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >계획을 생성한 경우에만 계획을 삭제할 수 있습니다. 공유된 플랜은 삭제할 수 없습니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 플랜이 지정한 사용자와 공유됩니다.

   플랜 목록 또는 플랜 헤더의 오른쪽 상단 모서리의 나와 공유 열에서 플랜에 대한 권한이 있는 사용자를 볼 수 있습니다.

   >[!TIP]
   >
   >플랜 목록에서 [!UICONTROL 나와 공유] 필터를 적용하여 사용자와 공유된 플랜을 볼 수 있습니다.


