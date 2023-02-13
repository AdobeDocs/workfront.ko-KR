---
product-area: projects;user-management
navigation-topic: manage-projects
title: 프로젝트에서 사용자 제거
description: 사용자가 더 이상 프로젝트에서 작업을 완료하지 않으면 프로젝트에서 사용자를 제거할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 301c86152340a184345bd39cec77fdcf28258196
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 프로젝트에서 사용자 제거

사용자가 더 이상 프로젝트에서 작업을 완료하지 않으면 프로젝트에서 사용자를 제거할 수 있습니다. 프로젝트에서 사용자를 제거하면 프로젝트 역할 뿐만 아니라 작업 및 문제 할당에도 영향을 줍니다. 프로젝트 팀에 대한 알림 수신을 중지한 사용자가 제거되었습니다. 프로젝트 팀의 알림에 대한 자세한 내용은 [Adobe Workfront에서 사용할 수 있는 이벤트 알림](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

프로젝트와 연결된 사용자는 프로젝트의 사람 영역에 나열됩니다. 프로젝트 팀을 나타냅니다. 프로젝트 팀에 대한 자세한 내용은 [프로젝트 팀 개요](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자를 제거하면 기존 작업, 문제 및 프로젝트에 미치는 영향

사용자가 프로젝트에서 제거되면 사용자가 제거될 때 작업이 완료되었는지 아니면 문제가 완료되었는지에 따라 사용자에게 할당된 모든 작업 또는 문제가 영향을 받을 수 있습니다.

* **사용자가 제거될 때 항목이 완료되지 않으면:** 작업 역할이 이미 할당된 경우 또는 사용자가 해당 항목에 대해 충족한 작업 역할에 항목이 할당된 경우 해당 항목이 작업 역할에 다시 할당됩니다. 항목이나 사용자에게 작업 역할이 할당되지 않은 경우 수동으로 항목을 다시 할당해야 합니다.
* **사용자가 제거될 때 항목이 완료된 경우:** 제거된 사용자의 이름이 항목에 남아 있습니다.
* **사용자가 제거된 경우 프로젝트의 작성자도 다음과 같습니다.** 프로젝트가 제거되지는 않습니다 **프로젝트 설정** 프로젝트 영역에 나열된 상태로 표시됩니다. 입력한 사람 필드로 해당 프로젝트를 필터링하는 다른 모든 사용자의 목록에서 프로젝트가 제거됩니다.
* **사용자가 프로젝트 소유자 또는 스폰서인 경우:** 사용자는 프로젝트 스폰서 또는 소유자로서 자신의 역할에 남습니다.

## 프로젝트 및 프로젝트 팀에서 사용자 제거

프로젝트 팀에서 사용자를 제거하여 프로젝트에서 사용자를 제거할 수 있습니다.

사용자가 프로젝트에서 역할을 이행하면 프로젝트 팀의 일부가 됩니다.

사용자가 프로젝트에서 해당 역할에서 제거되면 해당 사용자는 프로젝트 팀의 일부로 남습니다.

프로젝트에서 사용자의 역할에 대한 자세한 내용은 [프로젝트 팀 관리](../planning-a-project/manage-project-team.md).

프로젝트 팀에서 사용자를 제거하려면

1. 사용자를 제거할 프로젝트로 이동합니다.

1. 클릭 **사람** 왼쪽 패널에서 제거할 사용자를 선택합니다. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **사람**.

1. 을(를) 클릭합니다. **제거** 아이콘  ![항목 제거](assets/remove-icon---x-in-circle.png) 를 클릭합니다.

1. 클릭 **예, 선택한 사용자 제거** 제거 를 확인합니다.

   사용자는 프로젝트 팀으로부터 제거되고 사용자가 할당될 수 있는 불완전한 작업이나 문제로부터 제거됩니다. 더 이상 프로젝트 팀에 대한 알림을 받지 않습니다.
