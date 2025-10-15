---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 타임시트 승인
description: 타임시트 승인 프로세스를 통해 관리자는 직접 보고서의 작업 시간을 볼 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 충분한 시간이 기록되었는지 확인할 수 있습니다.
author: Lisa
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 69cd5fb1d089b81b7a1673609b92537137b6b68e
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# 타임시트 승인

<!--Audited: 8/2024-->

타임시트 승인 프로세스를 통해 관리자는 직접 보고서의 작업 시간을 볼 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 충분한 시간이 기록되었는지 확인할 수 있습니다.

Adobe Workfront은 이 영역에서 지원할 타임시트 승인을 구성하는 기능을 제공합니다.

타임시트 제출에 대한 자세한 내용은 [승인을 위해 타임시트 제출](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td><p>타임시트 및 시간에 대한 관리 액세스</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 타임시트 승인자 지정

일반적으로 타임시트는 기능 관리자나 인사 담당자가 승인합니다. 타임시트는 일반적으로 프로젝트 관리자가 승인하지 않습니다. 프로젝트 관리자는 프로젝트에 로그온한 시간을 승인할 수 있지만 팀 또는 인적 자원 관리자는 타임시트를 승인해야 합니다.

타임시트 승인자는 타임시트 프로필을 만들 때 정의됩니다. 승인자로 지정되려면 플랜 라이선스가 있어야 합니다.

타임시트 승인자 지정에 대한 자세한 내용은 문서 [타임시트 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create)의 [타임시트 프로필 만들기 또는 편집](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) 섹션을 참조하십시오.

## 타임시트 승인

승인자로 지정된 위치에 제출된 모든 타임시트를 승인할 수 있습니다. 승인을 위해 타임시트가 제출되면 해당 타임시트는 **홈** 영역의 **내 승인** 위젯에 나열됩니다. 자세한 내용은 [작업 승인](../../review-and-approve-work/manage-approvals/approving-work.md)을 참조하세요.

다음 알림 설정이 있는 경우 승인을 위해 타임시트를 제출하는 사용자는 타임시트가 승인된 후 이메일을 수신합니다.

* Workfront 관리자가 사용자에 대한 타임시트 승인 및 사용자 이벤트 핸들러에 대한 타임시트 거부를 활성화했습니다. 이벤트 알림 활성화에 대한 자세한 내용은 [이벤트 알림 유형](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)을 참조하세요.
* 내 타임시트 승인됨 개인 알림은 사용자의 프로필 페이지에서 활성화됩니다. 자세한 내용은 [전자 메일 알림 수정](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

### 타임시트 영역에서 타임시트 승인

{{step1-to-timesheets}}

**타임시트** 영역이 열립니다.

1. (조건부) 마지막으로 액세스한 시간이 열리면 화면 왼쪽 상단의 **타임시트로 돌아가기**&#x200B;를 클릭합니다.

1. 승인한 타임시트만 보려면 페이지의 오른쪽 상단에서 **내 타임시트 승인**&#x200B;을 선택하십시오.

   또는

   타임시트 목록 맨 위에서 **내 타임시트 승인** 필터를 선택합니다.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 템플릿에서 내 타임시트 승인 필터를 제거한 경우 내 타임시트 승인 옵션이 타임시트 목록 맨 위나 필터 목록에 표시되지 않습니다.
   >
   >자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.
   >   
   >

1. (선택 사항) 타임시트 목록 맨 위에 있는 **검색** 아이콘 ![](assets/search-icon.png)을(를) 클릭하고 키워드를 입력하여 특정 타임시트를 찾습니다. 일정, 소유자 또는 승인자의 이름을 검색할 수 있습니다.
1. 승인할 타임시트의 시간대를 클릭합니다. 타임시트가 열립니다.

   >[!TIP]
   >
   >승인 대기 중인 타임시트의 상태는 [!UICONTROL 제출됨]입니다.


1. **승인** 클릭

   또는

   타임시트를 거부하려면 타임시트의 왼쪽 아래에서 **거부**&#x200B;를 클릭합니다.

   승인되면 타임시트 상태가 **닫힘**(으)로 변경됩니다.

   거부되면 타임시트 상태가 **거부됨**(으)로 변경됩니다.

### 홈 영역에서 타임시트 승인

{{step1-to-home}}

홈 영역이 열립니다.

1. 홈 영역에 **내 승인** 위젯이 추가되었는지 확인하십시오. 자세한 내용은 [새 홈에서 위젯 추가, 편집 또는 제거](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)를 참조하세요.
1. 내 승인 위젯에서 타임시트 승인을 찾습니다.
1. (선택 사항) 승인 또는 거부 단추 오른쪽에 있는 드롭다운 메뉴를 확장하여 결정에 대한 댓글을 추가한 다음 **추가**&#x200B;를 클릭합니다.
1. 다음 버튼 중 하나를 클릭하여 승인 결정을 내립니다.

   * 승인
   * 거부

   **내 승인** 위젯에서 승인이 제거되었습니다.


