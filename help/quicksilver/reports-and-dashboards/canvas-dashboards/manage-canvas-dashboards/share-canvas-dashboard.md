---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: 캔버스 대시보드 공유
description: 다른 Adobe Workfront 사용자가 보거나 편집할 수 있도록 캔버스 대시보드를 공유할 수 있습니다.
author: Courtney
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 3%

---

# 캔버스 대시보드 공유

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 이 단계에서 기능 일부가 완전하지 않거나 의도한 대로 작동하지 않을 수 있습니다. Canvas Dashboards Beta 개요 문서의 [피드백 제공](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) 섹션에 있는 지침에 따라 경험에 대한 피드백을 제출하십시오.<br>
>가능한 버그 또는 기술 문제에 대한 피드백이 있는 경우 Workfront 지원에 티켓을 제출하십시오. 자세한 내용은 [고객 지원 센터에 문의](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)<br>를 참조하세요.
>다음 클라우드 공급자에서는 이 Beta를 사용할 수 없습니다.
>
>* Amazon Web Services에 대한 자체 키 가져오기
>* Azure
>* Google Cloud 플랫폼

You can share a Canvas dashboard with other Adobe Workfront users so they can view or edit it.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>Any </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td> 
<p>표준 </p> 
<p>플랜</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td><p>View access to Reports, Dashboards, and Calendars</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td><p>View permissions for the dashboard to share the dashboard</p>
   <p>대시보드 권한을 할당하려면 대시보드에 대한 권한을 관리하십시오.</p>
  </td> 
  </tr>
</tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 대시보드 공유에 대한 고려 사항

* 대시보드는 사용자, 팀, 그룹, 작업 역할 또는 회사 리소스와 공유할 수 있습니다.

* By default, the creator of a dashboard has Manage permissions for the dashboard.

* System administrators and users with Manage permission can grant View or Manage access to a dashboard.

* Users with View permission to a dashboard can grant View access to a dashboard.

* When sharing a dashboard, the resources it&#39;s shared with will inherit permissions to the reports displayed on the dashboard.

* When a dashboard is distributed through a layout template, an automatic View permission for the dashboard (and its reports) is granted to all resources assigned to the layout template.


## 캔버스 대시보드 공유


{{step1-to-dashboards}}

1. 왼쪽 패널에서 **캔버스 대시보드**&#x200B;를 클릭합니다.

1. **캔버스 대시보드** 페이지에서 공유할 대시보드를 선택합니다.

1. 페이지의 오른쪽 상단 모서리에서 **공유** 단추를 클릭합니다. **대시보드 공유** 대화 상자가 나타납니다.

   ![공유 단추](assets/share-button.png)

1. **액세스 권한 부여** 필드에서 캔버스 대시보드를 공유할 특정 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 선택합니다.

1. (Optional) To edit a resource&#39;s access to the dashboard, click **View** next to their name, then select **Manage** in the drop-down list that appears.

   >[!NOTE]
   >
   > When users do not have the Edit permissions to a dashboard assigned through their access level, they cannot be assigned Manage permissions to a dashboard.

1. Repeat steps 5-6 for each resource you want to share the dashboard with.

1. Click the **Share** button. The recipients receive an email notification informing them that the dashboard has been shared with them, which they can now access at **Dashboards** > **Canvas Dashboards** > **Shared Dashboards**.

   >[!NOTE]
   >
   > Individual user preferences and system exclusions for email notifications may apply. <br>
   > Notifications are only sent when shared directly with a user. 그룹, 역할, 회사 및 팀에 공유해도 전자 메일 알림이 생성되지 않습니다.<br>
   > 레이아웃 템플릿에서 상속된 권한은 대시보드 액세스에 대한 이메일 알림을 생성하지 않습니다.
