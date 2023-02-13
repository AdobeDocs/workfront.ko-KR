---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 반복에서 애자일 스토리 만들기
description: 이 문서에서는 이미 반복 작업을 수행할 때 새로운 애자일 스토리를 만드는 방법을 설명합니다.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 반복에서 애자일 스토리 만들기

이 문서에서는 이미 반복 작업을 수행할 때 새로운 애자일 스토리를 만드는 방법을 설명합니다. 작업, 문제 또는 다른 영역에서 애자일 스토리를 만드는 방법에 대한 정보 [!DNL Adobe Workfront]를 참조하십시오. [기존 반복에 스토리 추가](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>스토리가 있는 프로젝트에 대한 [!UICONTROL Manage] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 반복에서 애자일 스토리 만들기

1. 스토리를 만들 민첩한 반복으로 이동합니다.

   1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 팀]**.

   1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

   1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]**.
   1. 스토리를 작성할 특정 이터레이션의 이름을 클릭합니다.
   1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 스토리]**.

1.  클릭 **[!UICONTROL 새 스토리].**
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
      <td>스토리에 대한 예상 을 지정합니다. 애자일 팀이 스토리를 포인트로 추정하도록 구성된 경우 기본적으로 1포인트는 8시간입니다. 추정은 스토리에 [!UICONTROL 계획된 시간]으로 추가됩니다.<br>예를 들어 스토리를 3점으로 추정하면 기본 동작은 스토리에 24개의 계획된 시간을 추가하는 것입니다.<br>스토리에 하위 작업이 포함되어 있으면 모든 하위 작업에 대한 결합된 추정치가 상위 스토리의 추정치를 결정합니다. 자세한 내용은 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">[!UICONTROL Screum] 보드의 기존 스토리에 하위 작업 추가</a>.</td>
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
