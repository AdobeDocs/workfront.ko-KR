---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시
description: 프로젝트 및 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 일치시킬 수 있습니다. 이를 통해 초과 할당 또는 저사용을 방지할 수 있습니다.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시

>[!IMPORTANT]
>
>조직은 Adobe Analytics 세트에 대해 추가 라이센스를 구입해야 합니다 [!DNL Adobe Workfront Scenario Planner] 프로젝트에 대한 이니셔티브 정보를 볼 수 있습니다. 를 가져오는 방법에 대한 자세한 내용은 [!DNL Workfront Scenario Planner]를 참조하십시오. [을 사용하는 데 필요한 액세스 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

프로젝트 및 이니셔티브를 연결한 후 리소스 할당을 나란히 관리하여 일치시킬 수 있습니다. 이를 통해 초과 할당 또는 저사용을 방지할 수 있습니다.

이 문서에서는 [!UICONTROL 역할 할당] 프로젝트의 작업 목록에 있는 패널입니다.

사전 요구 사항을 포함하여 프로젝트 및 이니셔티브 간 리소스 조정에 대한 일반적인 내용은 [프로젝트 및 이니셔티브 간 리소스 할당 조정 개요](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## 액세스 요구 사항

다음을 수행해야 합니다.

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
   <td> <p>프로젝트에 대한 [!UICONTROL 보기] 이상 액세스 </p> <p>참고: 여전히 액세스 권한이 없는 경우 [!UICONTROL Workfront] 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. [!UICONTROL Workfront] 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 보기] 이상의 권한</p> <p>계획에 대한 추가 액세스 요청에 대한 내용은 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">에서 계획에 대한 액세스 요청 [!DNL Scenario Planner]</a>.</p> <p>프로젝트에 대한 추가 액세스 요청에 대한 내용은 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시

회사가 [!DNL Workfront Scenario Planner] 라이센스에서 이니셔티브와 이 이니셔티브에 연결된 프로젝트 간의 자원 할당을 [!UICONTROL 작업] 섹션에 나열된 상태로 남아 있습니다.

1. (조건부) 에 설명된 방법 중 하나를 사용하여 프로젝트를 이니셔티브로 연결합니다 [작업 목록에 프로젝트 및 이니셔티브에 대한 역할 할당 표시](#Connect) 이 문서의

   >[!IMPORTANT]
   >
   >이니셔티브에서 리소스를 변경할 경우, 이니셔티브가 속한 시나리오를 다시 게시하여 프로젝트에 대한 최신 리소스 정보를 업데이트해야 합니다.

1. 프로젝트에 대한 작업 역할 할당 및 관련 이니셔티브를 검토할 프로젝트로 이동합니다.
1. 클릭 **[!UICONTROL 작업]** 왼쪽 패널에 표시됩니다.
1. 을(를) 클릭합니다. **[!UICONTROL 역할 할당 표시]** 아이콘 ![](assets/show-role-allocation-icon.png) 를 클릭합니다.

   다음 [!UICONTROL 역할 할당] 패널이 표시됩니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 에서 다음 정보를 검토하십시오 **[!UICONTROL 프로젝트 합계]** 의 영역 [!UICONTROL 역할 할당] 패널:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 작업 역할]</td> 
      <td> <p>다음 중 하나와 연관된 작업 역할의 이름:</p> 
       <ul> 
        <li> <p>프로젝트의 작업</p> </li> 
        <li> <p>프로젝트의 문제</p> </li> 
        <li> <p>프로젝트에 연결된 이니셔티브</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>이니셔티브 총 기간 동안 이니셔티브의 각 작업 역할과 연관된 필요한 시간 수입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 계획된 시간]</td> 
      <td>프로젝트의 총 기간 동안 프로젝트의 작업 또는 문제에 관련된 각 작업 역할과 연관된 계획된 시간 수입니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>이니셔티브에 필요한 시간과 프로젝트 작업과 관련된 계획 시간의 차이입니다. [!DNL Workfront] 다음 공식을 사용하여 [!UICONTROL Variance]를 계산합니다.</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>이니셔티브에 필요한 시간보다 더 많은 시간 동안 리소스를 계획하면 [!UICONTROL Variance]는 음수이며 빨간색으로 표시됩니다. 즉, 리소스가 너무 많이 할당되었습니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >프로젝트의 계획된 시간은 다음 시나리오에 표시되지 않습니다.
   >
   >   
   >   
   >   * 작업 또는 문제가 작업 역할에 할당되지 않거나 작업 역할이 연결된 사용자가 할당된 경우
   >   * 작업 또는 문제에 기간이 0인 경우




1. (선택 사항) [!UICONTROL 분산] 열에는 리소스가 오버할당되었음을 나타내며 다음 중 하나를 조정합니다.

   * 초과 할당 또는 작업에 더 많은 자원을 추가하고 새 자원에 더 많은 계획 시간을 분배하는 하나의 작업 역할에 대한 계획 시간 수를 줄입니다. 작업 또는 문제를 편집할 때 발령이나 계획 시간 수를 갱신할 수 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

      * [작업 편집](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [문제 편집](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >작업 및 문제를 편집하려면 추가 액세스 및 권한이 있어야 합니다.

   * 이니셔티브 상의 초과 할당을 보여주는 역할에 필요한 시간 수를 늘립니다. 자세한 내용은 [에서 이니셔티브 만들기 및 편집 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >계획을 편집하려면 추가 액세스 권한과 사용 권한이 있어야 합니다.



