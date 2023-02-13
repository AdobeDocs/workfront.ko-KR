---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: 애자일 스토리 만들기
description: 다양한 방법으로 반복에 대해 애자일 스토리를 만들 수 있습니다. 애자일 스토리를 만든 후 하위 작업을 스토리에 추가할 수 있습니다.
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 애자일 스토리 만들기

다양한 방법으로 반복에 대해 애자일 스토리를 만들 수 있습니다. 애자일 스토리를 만든 후 하위 작업을 스토리에 추가할 수 있습니다.

반복에서 스토리나 하위 작업을 추가하면 기간 유형이 로 설정됩니다 [!UICONTROL 단순] 작업 제약 조건(Task Constraint)이 고정 날짜(Fixed Date)로 설정되어 있고 이터레이션 내에서 날짜가 잠겨 있습니다. 반복에서 기간 유형 또는 작업 제약 조건을 수정할 수 없습니다. 또한 작업 기간은 0분을 초과해야 합니다.

이터레이션에 추가된 스토리를 관리하는 방법에 대한 자세한 내용은 [반복](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>스토리가 있는 프로젝트에 대한 [!UICONTROL Manage] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 반복에서 애자일 스토리 만들기

1. 스토리를 만들 민첩한 반복으로 이동합니다.

   1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

   1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

   1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]** 특정 이터레이션을 선택하려면 **[!UICONTROL 현재 반복]**.
   1. 스토리를 작성할 특정 이터레이션의 이름을 클릭합니다.

   ![반복에 새 스토리 추가](assets/iteration-add-story.png)

1. 클릭 **[!UICONTROL 새 스토리].**
1. 다음 정보를 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>스토리의 이름을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>스토리에 대한 설명을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>스토리를 반복에 추가할 준비가 되면 이 옵션을 선택합니다. 이 옵션을 선택하면 백로그의 스토리를 반복에 추가할 준비가 된 사용자에게 표시됩니다.<br>스토리가 표시되는지 여부에 관계없이 반복에 추가할 수 있습니다 <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate](포인트)</strong></td>
      <td>스토리에 대한 예상 을 지정합니다. 애자일 팀이 스토리를 포인트로 추정하도록 구성된 경우 기본적으로 1포인트는 8시간입니다. 추정은 스토리에 [!UICONTROL 계획된 시간]으로 추가됩니다.<br>예를 들어 스토리를 3점으로 추정하면 기본 동작은 스토리에 24개의 [!UICONTROL Planning Hours]를 추가하는 것입니다.<br>스토리에 하위 작업이 포함되어 있으면 모든 하위 작업에 대한 결합된 추정치가 상위 스토리의 추정치를 결정합니다. 자세한 내용은 <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">기존 반복에 스토리 추가</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상위 프로젝트]</strong></td>
      <td>이 스토리와 연결할 프로젝트의 이름을 입력합니다.<br>기본적으로 스토리 색상은 이 프로젝트의 다른 스토리와 동일한 색상으로 표시됩니다.<br>프로젝트의 상태를 [!UICONTROL Current]로 설정해야 합니다. 프로젝트의 상태가 [!UICONTROL Current]를 제외한 경우에는 드롭다운 메뉴에 표시되지 않습니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상위 작업]</strong></td>
      <td>상위 프로젝트를 선택하면 상위 작업을 선택할 수 있는 옵션이 제공됩니다. 상위 작업을 선택하면 스토리가 선택한 프로젝트에서 상위 작업의 하위 작업으로 만들어집니다.<br>스토리에 대한 상위 작업 이름을 입력하고 드롭다운 목록에 나타나면 클릭합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>스토리에 추가할 사용자 지정 양식을 선택합니다.</td>
     </tr>
    </tbody>
   </table>

1. 클릭 **[!UICONTROL 스토리 저장]**.

## 백로그에서 애자일 스토리 만들기

섹션에 설명된 대로 애자일 백로그에서 애자일 스토리를 생성할 수 있습니다 [백로그에 새 스토리 만들기](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) 기사 [[!UICONTROL 관리] 빠른 백로그](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## 민첩한 스토리로 작업 또는 문제 추가

기존 작업이나 문제를 반복에 스토리로 추가할 수 있습니다. 자세한 내용은 [기존 반복에 스토리 추가](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) 또는 [에서 스토리 및 문제 추가 [!UICONTROL 스크럼] 보드](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## 애자일 스토리에 하위 작업 만들기

다음 방법 중 하나를 사용하여 애자일 스토리에 하위 작업을 만들 수 있습니다.

* 를 사용하여 **[!UICONTROL 하위 작업]** 탭에 설명된 대로 [하위 작업 만들기](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) in [하위 작업 만들기](../../manage-work/tasks/create-tasks/create-subtasks.md).

* 에 설명된 대로 스토리 보드에서 직접 [반복 만들기](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
