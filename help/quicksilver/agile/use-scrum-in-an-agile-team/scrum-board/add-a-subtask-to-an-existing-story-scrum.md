---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드의 기존 스토리에 하위 작업 추가
description: 기존 스토리에 대한 하위 작업을 만들 때는 스토리가 업데이트되는 방식에 영향을 주므로 프로젝트에 대한 완료 모드 설정을 기억하십시오.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# 의 기존 스토리에 하위 작업 추가 [!UICONTROL 스크럼] 보드

기존 스토리에 대한 하위 작업을 만들 때는 다음 사항에 유의하십시오.

**이 [!UICONTROL 완료 모드] 프로젝트에 대한 설정이 [!UICONTROL 수동]:**

* 하위 작업이 있는 상위 스토리를 [!UICONTROL 완료] 상위 스토리를 100%로 업데이트하고 [!UICONTROL 상태] to [!UICONTROL 완료]. 하위 작업은 업데이트되지 않습니다.
* 를 업데이트하려면 [!UICONTROL 완료율] 기사를 위해서, 당신은 그것을 [!UICONTROL 스토리] 탭 또는 [!UICONTROL 세부 사항] 개체의 페이지입니다.

**이 [!UICONTROL 완료 모드] 프로젝트에 대한 설정이 [!UICONTROL 자동]**:

* 하위 작업이 있는 상위 스토리를 [!UICONTROL 완료] 상위 스토리를 100%로 업데이트하고 [!UICONTROL 상태] to [!UICONTROL 완료]. 하위 작업도 100%로 업데이트되고 [!UICONTROL 상태] 업데이트됨: [!UICONTROL 완료].
* 를 업데이트하려면 [!UICONTROL 완료율] 기사를 위해서, [!UICONTROL 완료율] 모든 하위 작업에 사용할 수 있습니다. 다음 [!UICONTROL 완료율] 의 경우 스토리는 [!UICONTROL 완료율] 모든 하위 작업 중

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
   <td> <p>하위 작업이 있는 작업에 대한 [!UICONTROL Contribute] 또는 [!UICONTROL Manage] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 스크럼 보드의 기존 스토리에 하위 작업 추가

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 하위 작업을 추가할 스토리가 포함된 민첩한 반복 또는 프로젝트로 이동합니다. 반복으로 이동하는 방법에 대한 자세한 내용은 [반복 보기](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. 하위 작업을 추가할 스토리 보드의 스토리 타일로 이동합니다.
1. 클릭 **[!UICONTROL 하위 작업 추가]** 주 이야기 카드에서 이야기 하위 작업을 만듭니다.

   ![하위 작업 추가](assets/agile-story-addsubtask-NWE.png)

   또는

   클릭 **[!UICONTROL 하위 작업 추가]** 하위 작업 타일에서 하위 작업에 하위 작업을 만들 수 있습니다.

   [!DNL Workfront] 에서는 하위 작업의 무한 수준을 지원하지만, 애자일 스토리 보드에 두 수준(하위 작업의 하위 작업)만 표시됩니다.

   ![하위 작업 추가](assets/agile-story-addsubtask2-NWE.png)

   현재 수영선이 없는 이야기에 하위 작업을 추가하면 상위 작업이 [!UICONTROL 상위 스토리] 기둥과 부제가 수영선 안에서 움직입니다.

1. 다음 정보를 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask Name]</strong></td>
      <td> 하위 작업의 이름을 지정합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>하위 작업에 대한 설명을 지정합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]</strong></td>
      <td>하위 작업의 예상 값을 지정합니다.<br><p>예측을 생성할 때는 다음 사항을 기억하십시오.</p>
       <ul>
        <li>애자일 팀이 스토리를 포인트로 추정하도록 구성된 경우 기본적으로 1포인트는 8시간입니다. 추정은 스토리에 [!UICONTROL 계획된 시간]으로 추가됩니다.</li>
        <li>모든 하위 작업에 대한 총 예상 수는 상위 스토리의 추정치를 결정합니다. 자세한 내용은 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">스크럼 보드의 스토리 및 하위 작업 상태 업데이트</a>.</li>
        <li>새 하위 작업을 만들 때 [!UICONTROL 예상] 필드가 이미 설정되어 있습니다. 하위 작업에서 견적을 재설정하면 상위 스토리에 대한 예상 값을 재설정합니다(상위 스토리가 모든 하위 작업의 합계이므로).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 계획된 시간]</strong></td>
      <td> (프로젝트에서만 사용 가능) 작업에 대해 계획된 시간 수를 지정합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignment]</strong></td>
      <td>하위 작업을 할당할 팀의 이름을 입력하고 드롭다운 목록에 나타나면 클릭합니다.</td>
     </tr>
    </tbody>
   </table>

1. Click **[!UICONTROL Create]**.
