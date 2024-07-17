---
product-area: projects;user-management
navigation-topic: manage-projects
title: 프로젝트에서 사용자 제거
description: 사용자가 프로젝트에서 작업을 완료하는 데 더 이상 참여하지 않을 때 프로젝트에서 사용자를 제거할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# 프로젝트에서 사용자 제거

사용자가 프로젝트에서 작업을 완료하는 데 더 이상 참여하지 않을 때 프로젝트에서 사용자를 제거할 수 있습니다. 프로젝트에서 사용자를 제거하면 프로젝트 역할뿐만 아니라 작업 및 문제 할당에도 영향을 줍니다. 제거된 사용자가 프로젝트 팀에 대한 알림 수신을 중지합니다. 프로젝트 팀에 대한 알림에 대한 자세한 내용은 [이벤트 알림 유형](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)을 참조하세요.

프로젝트와 연결된 사용자는 프로젝트의 사람 영역에 나열됩니다. 이들은 프로젝트 팀을 나타냅니다. 프로젝트 팀에 대한 자세한 내용은 [프로젝트 팀 개요](../../../manage-work/projects/planning-a-project/project-team-overview.md)를 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 사용자 제거가 기존 작업, 문제 및 프로젝트에 미치는 영향

사용자가 프로젝트에서 제거되면 해당 사용자가 제거되었을 때 작업 또는 문제가 완료되었는지 여부에 따라 할당된 작업 또는 문제가 영향을 받을 수 있습니다.

* **사용자가 제거되었을 때 항목이 완료되지 않은 경우:** 작업 역할이 이미 할당되었거나 사용자가 해당 항목에 대해 수행하는 작업 역할에 할당된 경우 항목이 작업 역할에 다시 할당됩니다. 항목 또는 사용자에게 작업 역할이 할당되지 않은 경우 항목을 수동으로 다시 할당해야 합니다.
* **사용자가 제거될 때 항목이 완료된 경우:** 제거된 사용자의 이름은 항목에 남아 있습니다.
* **제거된 사용자가 프로젝트 제작자인 경우:** 프로젝트 영역의 **내가 진행 중인 프로젝트** 목록에서 프로젝트가 제거되지 않습니다. 입력한 사람 필드로 해당 프로젝트를 필터링하는 다른 모든 사용자의 목록에서 프로젝트가 제거됩니다.
* **사용자가 프로젝트 소유자 또는 스폰서인 경우:** 사용자는 스폰서 또는 프로젝트 소유자로서 자신의 역할에 남아 있습니다.

## 프로젝트 및 프로젝트 팀에서 사용자 제거

프로젝트 팀에서 사용자를 제거하여 프로젝트에서 사용자를 제거할 수 있습니다.

사용자가 프로젝트에서 역할을 수행하면 프로젝트 팀에 포함됩니다.

프로젝트에서 사용자를 역할에서 제거하면 해당 사용자는 프로젝트 팀의 일부로 유지됩니다.

프로젝트에서 사용자 역할에 대한 자세한 내용은 [프로젝트 팀 관리](../planning-a-project/manage-project-team.md)를 참조하십시오.

프로젝트 팀에서 사용자를 제거하려면 다음 작업을 수행하십시오.

1. 사용자를 제거할 프로젝트로 이동합니다.

1. 왼쪽 패널에서 **직원**&#x200B;을 클릭한 다음 제거할 사용자를 선택합니다. **자세히 표시**&#x200B;를 클릭한 다음 **사람**&#x200B;을 클릭해야 할 수 있습니다.

1. 사용자 목록 맨 위에 있는 **제거** 아이콘 ![항목 제거](assets/remove-icon---x-in-circle.png)를 클릭합니다.

1. **예, 선택한 사용자 제거**&#x200B;를 클릭하여 제거를 확인합니다.

   사용자는 프로젝트 팀 및 할당되었을 수 있는 미완료 작업 또는 문제에서 제거됩니다. 더 이상 프로젝트 팀에 대한 알림이 수신되지 않습니다.
