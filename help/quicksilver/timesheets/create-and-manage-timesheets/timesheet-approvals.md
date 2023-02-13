---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 작업표 승인
description: 작업표 승인 프로세스를 통해 관리자는 직접 보고서의 작업 시간을 파악할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 대해 충분한 시간이 기록되었는지 확인할 수 있습니다.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# 작업표 승인

작업표 승인 프로세스를 통해 관리자는 직접 보고서의 작업 시간을 파악할 수 있습니다. 승인자는 기록된 모든 시간이 올바른 영역에 할당되었고 해당 기간에 대해 충분한 시간이 기록되었는지 확인할 수 있습니다.

Adobe Workfront은 이 영역에서 지원할 작업표 승인을 구성하는 기능을 제공합니다.

작업표 제출에 대한 자세한 내용은 [승인을 위한 작업표 제출](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업표 승인자 지정

일반적으로 작업표는 기능적 관리자나 인력 직원이 승인합니다. (작업표는 프로젝트 관리자가 일반적으로 승인하지 않습니다.)

작업표 프로필을 만들 때 작업표 승인자가 정의됩니다. 승인자로 지정하려면 계획 라이센스가 있어야 합니다.

작업표 승인자 지정에 대한 자세한 내용은 섹션을 참조하십시오 [작업표 프로필 만들기 또는 편집](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) 기사 [작업표 프로필 만들기, 편집 및 할당](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## 작업표 승인

승인자로 지정된 작업표를 제출한 모든 작업표를 승인할 수 있습니다. 승인을 위해 작업표를 제출하면 작업표가 **승인** 영역 **홈**  페이지. 자세한 내용은 [작업 승인](../../review-and-approve-work/manage-approvals/approving-work.md).

Workfront 관리자가 사용자에게 작업표 승인 및 사용자 이벤트 처리기에 대한 작업표 거부 기능을 활성화한 경우 작업표가 승인되거나 거부되면 사용자에게 통지됩니다. 이벤트 알림 활성화에 대한 자세한 내용은 [Adobe Workfront에서 사용할 수 있는 이벤트 알림](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

작업표를 승인하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서
1. 클릭 **작업표**.
1. 을(를) 선택합니다 **내 작업표 승인** 페이지의 오른쪽 위 모서리에서 사용자가 승인한 작업표만 볼 수 있습니다.

   또는

   을(를) 선택합니다 **내 작업표 승인** 작업표 목록의 맨 위에서 필터링합니다.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 설정 영역의 목록 컨트롤 또는 레이아웃 서식 파일에서 내 작업표 승인 필터를 제거한 경우 작업표 목록의 맨 위에 또는 필터 목록에 내 작업표 승인 옵션이 표시되지 않습니다. 자세한 내용은 다음 문서를 참조하십시오.
   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (선택 사항) **검색** 아이콘 ![](assets/search-icon.png) 작업표 목록 맨 위에 특정 작업표를 찾을 키워드를 입력합니다. 기간, 소유자 또는 승인자 이름을 검색할 수 있습니다.
1. 승인할 작업표의 기간을 클릭합니다. 작업표가 열립니다.

   >[!TIP]
   승인을 기다리는 작업표의 상태는 다음과 같습니다. [!UICONTROL 제출됨].


1. 클릭 **승인**

   또는

   작업표를 거부하려면 **거부** 작업표의 왼쪽 아래 모서리에 있습니다.

   승인되면 작업표 상태가 **닫힘**.

   거부된 경우 작업표 상태가 **거부됨**.
