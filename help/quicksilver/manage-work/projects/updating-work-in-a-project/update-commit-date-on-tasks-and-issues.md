---
product-area: projects
navigation-topic: update-work-in-a-project
title: 작업 및 문제에 대한 커밋 일자 업데이트
description: 할당된 작업 또는 문제의 커밋 일자를 수동으로 업데이트할 수 있습니다. Adobe Workfront의 커밋 일자에 대한 자세한 내용은 커밋 일자 개요 를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---


# 작업 및 문제에 대한 커밋 일자 업데이트

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리보기 환경 또는 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서만 사용할 수 있습니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 활성화 또는 비활성화](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">현재 릴리스에 대한 자세한 내용은 [2024년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

할당된 작업 또는 문제의 커밋 일자를 수동으로 업데이트할 수 있습니다. Adobe Workfront의 커밋 일자에 대한 자세한 내용은 다음을 참조하십시오. [커밋 일자 개요](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 액세스 요구 사항

<!--Audited: 01/2024-->

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
   새 라이센스의 경우:
   <ul>
   <li><p>작업 표준</p> </li>
   <li><p>문제에 대한 기여자 이상</p></li>
   </ul>
   현재 라이센스의 경우:
<ul>
   <li><p>작업 이상</p></li> 
   <li><p>문제에 대한 요청 이상</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 문제에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 또는 문제에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 전제 조건

작업 또는 문제의 커밋 일자를 편집하려면 먼저 해당 커밋 일자를 업데이트해야 하는 작업 또는 문제에 할당해야 합니다.

## 작업 및 문제에 대한 커밋 일자 업데이트


Workfront의 다음 영역에서 작업 또는 문제의 커밋 일자를 업데이트할 수 있습니다.

* 작업 또는 문제의 세부 정보 섹션
* <span class="preview">작업 또는 문제 헤더</span>

  <span class="preview">Workfront 또는 그룹 관리자가 작업 또는 문제 페이지에서 보려면 레이아웃 템플릿의 작업 또는 문제 헤더에 커밋 일자를 추가해야 합니다.
자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

커밋 일자 업데이트는 작업 및 문제와 동일합니다.

>[!NOTE]
>
>Workfront의 다양한 영역에서 보다 쉽게 업데이트할 수 있도록 시스템 또는 그룹 관리자에게 요약 패널에 커밋 일자 필드를 추가하도록 요청할 수 있습니다.
>
>자세한 내용은 다음 문서를 참조하십시오.
>
>* [요약 개요](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [레이아웃 템플릿을 사용하여 홈 및 요약 맞춤화](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. (으)로 할당된 작업 또는 문제로 이동 **소유자**.

   문제 또는 작업에 대한 작업 소유자 확인에 대한 자세한 내용은 섹션을 참조하십시오 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 이 문서에서 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. <span class="preview">(조건부 및 선택 사항) Workfront 또는 그룹 관리자가 커밋 일자를 작업 또는 문제 헤더에 추가한 경우 **커밋 일자** 머리글에서 필드를 선택한 다음 달력에서 날짜를 선택합니다. 커밋 일자 가 헤더에 없으면 다음 단계를 진행하십시오. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

1. 클릭 **작업 세부 정보** 또는 **문제 세부 정보** 왼쪽 패널에서
1. 클릭 **개요** 확장하기 위해
1. 업데이트 **커밋 일자** 필드.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   이 변경 작업을 수행한 후 다음 작업이 수행됩니다.

   * 작업 또는 문제의 커밋 일자와 계획된 완료 일자가 더 이상 동일하지 않습니다.

     대신 작업 또는 문제의 커밋 일자와 예상 완료 일자가 같아집니다.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * 작업 또는 문제에 대한 새 커밋 날짜를 제안했다는 알림이 Workfront 인앱 알림을 통해 프로젝트 소유자에게 표시됩니다.
   * 업데이트 섹션에서 프로젝트 소유자에게 새 커밋 일자를 제안했다는 알림이 표시되며 사용자는 이때 제안한 커밋 일자와 일치하도록 작업 또는 문제의 계획된 완료 일자를 업데이트할 수 있습니다.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     이 변경으로 인해 트리거되는 알림 및 업데이트에 대한 자세한 내용은 문서의 &quot;커밋 일자 변경으로 인해 트리거되는 알림 및 업데이트&quot; 섹션을 참조하십시오 [커밋 일자 개요](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->