---
product-area: enterprise-scenario-planner-product-area
keywords: 계획,권한,공유,이니셔티브,시나리오,시나리오
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 시나리오 계획자에서 계획 공유
description: Adobe Workfront 시나리오 플래너에서 만든 계획을 다른 사용자와 공유할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# 에서 플랜 공유 [!DNL Scenario Planner]

에서 플랜을 공유할 수 있습니다 [!DNL Adobe Workfront Scenario Planner] 다른 사용자와 협업할 수 있습니다.

>[!TIP]
>
>계획에 대한 링크를 다른 사용자에게 보내는 경우 계획을 공유할 수 있도록 해당 계획을 다른 사용자와 공유해야 합니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 플랜*</b> </p> </td> 
   <td>[!UICONTROL Business] 이상</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 라이센스*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td><b>제품</b> </td> 
   <td> <p>에 대한 추가 라이센스를 구입해야 합니다. [!DNL Adobe Workfront Scenario Planner] 을 눌러 이 문서에 설명된 기능에 액세스합니다.</p> <p>를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>[!UICONTROL Edit]에 액세스하면 [!DNL Scenario Planner]</p> <p>여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p> 계획에 대한 [!UICONTROL Manage] 권한
     <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL Request] 의 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

* 계획에 대한 권한이 부여된 사용자는 [!DNL Scenario Planner] 사용자가 부여한 액세스 수준의 영역 [!DNL Workfront] 관리자 를 사용하여 계획에 대한 권한을 받습니다.

   예, [!UICONTROL 요청자] 계획을 조회, 생성 또는 편집할 수 없습니다. 요청자 라이센스가 있는 사용자와 계획을 공유할 때는 이를 염두에 두어야 합니다.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

액세스 권한에 대한 자세한 정보 [!DNL Scenario Planner] 다양한 라이선스 유형에 대해서는 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## 계획 공유에 대한 고려 사항

* 단일 계획을 공유하거나 여러 계획을 일괄적으로 공유할 수 있습니다.
* 생성하지 않았거나 사용자와 공유되지 않은 계획은 조회할 수 없습니다.
* 플랜은 다른 사용자와만 공유할 수 있습니다. 그룹, 팀 또는 회사와 계획을 공유할 수 없습니다.
* 계획을 공유하려면 먼저 계획을 저장해야 합니다.
* 계획에 URL을 다른 사용자와 공유할 수 있습니다. 사용자에게 적어도 계획을 볼 수 있는 권한이 없는 경우 URL을 받을 때 다른 사용자의 계획에 대한 액세스를 요청할 수 있습니다. 계획에 대한 액세스 요청에 대한 자세한 내용은 [에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* 이미 다른 사용자와 공유된 여러 계획을 공유할 때 공유하는 사용자는 대체되지 않지만 선택한 각 계획에서 기존 사용자에게 추가됩니다.

## 플랜 공유

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 시나리오]**.
1. 계획 이름을 눌러 엽니다

   또는

   여러 계획을 선택하여 일괄적으로 공유할 수 있습니다.

   >[!TIP]
   >
   >계획 헤더의 오른쪽 위 모서리에서 계획을 공유한 사용자의 아바타를 눌러 계획을 공유할 수 있습니다.

1. (조건부) 계획을 연 경우 **[!UICONTROL 자세히]** 아이콘 ![](assets/more-icon.png) 오른쪽 [!UICONTROL 계획] name을 클릭한 다음 **[!UICONTROL 공유]**

   또는

   여러 계획을 일괄 공유하도록 선택한 경우 **[!UICONTROL 공유]** 아이콘 ![](assets/share-icon-26x26.png) 그 계획을 열 계획 목록의 맨 위에서 [!UICONTROL 계획] 액세스 상자

   >[!TIP]
   >
   >* 선택한 모든 계획에 대한 권한이 있는 사용자가 [!UICONTROL 계획] 액세스 상자
   >* 선택한 모든 계획에서 추가 사용자가에 추가되며 기존 사용자를 대체하지 않습니다.


1. 에서 **[!UICONTROL 계획 액세스 권한 부여]** 필드에서 계획을 공유할 사용자의 이름을 입력하고 목록에 표시될 때 선택합니다.
1. 사용자 이름의 오른쪽에 있는 권한 드롭다운 메뉴에서 계획에 부여할 권한 수준을 선택합니다.
1. 다음 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>계획을 공유하는 사용자는 계획을 볼 수 있는 권한이 있습니다. 계획, 이니셔티브, 시나리오 또는 게시 시나리오에 대한 정보는 편집할 수 없습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Manage]</td> 
      <td> <p>계획을 공유하는 사용자는 편집 정보, 이니셔티브 추가, 시나리오 및 계획 게시가 포함된 계획을 관리할 권한이 있습니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >계획을 생성한 경우에만 계획을 삭제할 수 있습니다. 공유된 계획은 삭제할 수 없습니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 지정한 사용자와 계획이 공유됩니다.

   계획 목록 또는 계획 헤더의 오른쪽 위 모서리에 있는 나와 공유 열의 계획에 대한 권한이 있는 사용자를 볼 수 있습니다.

   >[!TIP]
   >
   >다음을 적용하여 사용자와 공유된 계획을 볼 수 있습니다 [!UICONTROL 나와 공유] 계획 목록으로 필터링합니다.

## 계획 권한 옵션

다음 표에는 계획을 공유할 때 부여할 수 있는 권한이 나와 있습니다. 라이센스를 기반으로 하는 액세스 사용자에 대한 자세한 내용은 [액세스 권한 부여 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>액션</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>계획 보기 </p> </td> 
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

*계획에 대한 관리 권한이 있더라도 계획에 대한 재무 정보를 보거나 관리하려면 재무 데이터에 액세스할 수 있어야 합니다. 재무 데이터 액세스에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**시나리오를 게시할 수 있도록 프로젝트를 관리하려면 만들기 및 사용 권한에 대한 액세스 권한이 있어야 합니다.

프로젝트 액세스 수준에 대한 자세한 내용은 [프로젝트에 대한 액세스 권한 부여](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

프로젝트 권한에 대한 자세한 내용은 [에서 프로젝트 공유 [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
