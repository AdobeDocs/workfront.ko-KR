---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: 진단 기능을 사용하여 자동화된 프로세스를 트리거합니다
description: 진단 유틸리티를 사용하여 시간 기반 스크립트, 재계산 또는 이메일 알림과 같은 자동화된 프로세스를 수동으로 트리거할 수 있습니다.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 6%

---

# 진단 기능을 사용하여 자동화된 프로세스를 트리거합니다

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

진단 유틸리티를 사용하여 시간 기반 스크립트, 재계산 또는 이메일 알림과 같은 자동화된 프로세스를 수동으로 트리거할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront 플랜</a> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront 라이선스 개요</a> </td> 
   <td> <p>플랜 </p>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</td> 
  </tr> 
 </tbody> 
</table>

## 진단 기능을 사용하여 자동화된 프로세스 트리거

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 확장 **시스템**&#x200B;를 클릭한 다음 **진단**.
1. 다음 옵션 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">지연 알림 보내기</td> 
      <td> <p>지연된 작업 및 문제에 대한 자동 미리 알림 메시지를 수동으로 보냅니다. </p> <p>자동 미리 알림 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">자동 미리 알림 설정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사전 알림 보내기</td> 
      <td> <p>만기 날짜가 가까워지는 작업 및 문제에 대한 자동 미리 알림 메시지를 수동으로 보냅니다.</p> <p>자동 미리 알림 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">자동 미리 알림 설정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림 보내기</td> 
      <td> <p>미리 알림 알림을 수동으로 보냅니다. </p> <p>미리 알림 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">미리 알림 설정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">POP 계정 모두 확인</td> 
      <td> <p>Workfront에 연결된 POP 계정으로 전송된 새 이메일을 확인합니다. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임라인 다시 계산</td> 
      <td> <p>현재 상태에 있는 Workfront의 모든 프로젝트에 대한 타임라인을 다시 계산합니다. </p> <p>프로젝트의 타임라인을 자동으로 또는 수동으로 계산하는 방법에 대한 자세한 내용은 한 번에 하나의 프로젝트를 참조하십시오. <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">프로젝트 타임라인 다시 계산</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 고객 보고서 복원</td> 
      <td>원래 Workfront과 함께 제공된 기본 보고서를 <strong>보고서</strong> 섹션을 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트 생성</td> 
      <td>되풀이하는 작업표 프로필에 따라 사용자의 작업표를 생성합니다. 작업표 프로필이 사용자에게 할당된 후, 현재 작업표와 이후 작업표가 삭제된 후에만 이 옵션을 실행해야 합니다.</td> 
     </tr> 
    </tbody> 
   </table>
