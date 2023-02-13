---
content-type: reference
navigation-topic: notifications
title: '''알림: 목표'
description: '''알림: 목표'
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 6%

---

# 알림: 목표

에서 발생하는 이벤트에 대해 이메일 알림을 활성화할 수 있습니다 [!DNL Adobe Workfront Goals] 참조하십시오. 사용자가 [!UICONTROL 계획] 라이센스는 다른 사용자에 대해 이러한 사용자를 활성화할 수도 있습니다. 자세한 내용은 [[!DNL Adobe Workfront] 알림](../../workfront-basics/using-notifications/wf-notifications.md).

## 액세스 요구 사항

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>제품</strong></td> 
   <td>[!DNL Workfront Goals] <p>에 대한 자세한 정보 [!DNL Workfront Goals]를 참조하십시오. <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL View] 액세스 권한 [!DNL Goals] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

사용자의 [!DNL Goals] 알림은 다음 조건을 충족해야 합니다.

* 다음을 포함하는 레이아웃 템플릿 [!DNL Goals] 의 영역 [!UICONTROL 기본 메뉴].
* 새 항목에 액세스 [!DNL Adobe Workfront] 경험으로 제어됩니다.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!DNL Goals] 의 알림 [!UICONTROL 사용자 프로필] 영역

다음 표에 나열된 알림에서는 [!DNL Workfront Goals]목표, 결과 또는 활동을 할당하거나 사용자가 소유한 목표, 결과 또는 활동을 업데이트하기 위한 작성자 등 수신한 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>에 대한 즉각적인 알림 [!DNL Goals] 기본적으로 비활성화되어 있습니다. 일별 알림을 활성화하거나 비활성화할 수 없으며 이 카테고리의 이벤트에 대한 일별 다이제스트 이메일을 받지 않습니다. 에 대해 개별 인스턴트 알림을 활성화하거나 비활성화할 수 있습니다 [!DNL Goals] 카테고리.

참조 - [이벤트 알림](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>알림</strong></td> 
   <td> <p><strong>포함된 필드</strong> </p> <p><strong>*인스턴트 알림만</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>누군가가 나에게 결과/활동을 할당함</strong></td> 
   <td> <p>결과 또는 활동을 자신에게 할당한 사람의 이름입니다</p> <p>결과 또는 활동에 대한 목표 기간</p> <p>결과 또는 활동의 이름</p> <p>다음 <strong>[!UICONTROL 웹 앱에서 열기]</strong> [!UICONTROL 목표 세부 사항] 패널을 여는 단추</p> <p>다음 <strong>[!UICONTROL Change Notifications Settings]</strong> 버튼을 클릭하여 알림을 관리할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>누군가 나를 위해 새로운 개인 목표를 만들었습니다.</strong> </td> 
   <td> <p>목표를 할당한 사람의 이름입니다</p> <p>목표 기간</p> <p>목표의 이름</p> <p>다음 <strong>[!UICONTROL 웹 앱에서 열기]</strong> [!UICONTROL 목표 세부 사항] 패널을 여는 단추</p> <p>다음 <strong>[!UICONTROL Change Notifications Settings]</strong> 버튼을 클릭하여 알림을 관리할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>누군가 내 목표에 댓글을 남겼습니다.</strong></td> 
   <td> <p>댓글을 남긴 사람의 이름입니다</p> <p>목표 기간 </p> <p>목표의 이름</p> <p>주석의 텍스트</p> <p>다음 <strong>[!UICONTROL 웹 앱에서 열기]</strong> [!UICONTROL 목표 세부 사항] 패널을 여는 단추</p> <p>다음 <strong>[!UICONTROL Change Notifications Settings]</strong> 버튼을 클릭하여 알림을 관리할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>누군가 목표의 내 댓글에 좋아요를 눌렀습니다.</strong></td> 
   <td> <p>설명을 좋아하는 사람의 이름입니다</p> <p>목표 기간 </p> <p>목표의 이름</p> <p>주석의 텍스트 </p> <p>다음 <strong>[!UICONTROL 웹 앱에서 열기]</strong> [!UICONTROL 목표 세부 사항] 패널을 여는 단추</p> <p>다음 <strong>[!UICONTROL Change Notifications Settings]</strong> 버튼을 클릭하여 알림을 관리할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>누군가 내 목표의 업데이트에 좋아요를 눌렀습니다.</strong></td> 
   <td> <p>누군가 목표에 대한 댓글을 좋아하거나 목표의 결과나 활동의 진행 상황을 업데이트하면 이메일이 전송됩니다. </p> <p>업데이트를 좋아하는 사람의 이름</p> <p>목표 기간 </p> <p>목표의 이름</p> <p>다음 <strong>[!UICONTROL 웹 앱에서 열기]</strong> [!UICONTROL 목표 세부 사항] 패널을 여는 단추</p> <p>다음 <strong>[!UICONTROL Change Notifications Settings]</strong> 버튼을 클릭하여 알림을 관리할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
