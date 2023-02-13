---
navigation-topic: notifications
title: Adobe Workfront의 항목 구독
description: Adobe Workfront에서는 사용자가 할당했거나 소유하고 있는 항목에 대한 알림을 보냅니다. 사용자에게 지정되지 않지만 작업에 영향을 줄 수 있는 항목에 대한 커뮤니케이션을 따르려면 해당 항목에 가입할 수 있습니다.
author: Lisa
feature: Get Started with Workfront
exl-id: 5eee62b8-d72e-4263-a0c5-749047bc6812
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 0%

---

# 의 항목에 가입 [!DNL Adobe Workfront]

[!UICONTROL Adobe Workfront] 사용자가 할당했거나 소유하고 있는 항목에 대한 알림을 보냅니다. 사용자에게 지정되지 않지만 작업에 영향을 줄 수 있는 항목에 대한 커뮤니케이션을 따르려면 해당 항목에 가입할 수 있습니다.

또한 사용자가 소유한 항목의 업데이트 상태에 구독하여 관리자 및 피어가 작업 중에 업데이트되도록 할 수도 있습니다 [!UICONTROL 관리] 및 [!UICONTROL 공유] 사용 권한.

현재 다음 항목에 가입할 수 있습니다.

* 문제
* 작업
* 프로젝트

문제, 작업 또는 프로젝트에 가입하면 다른 사람이 해당 문제에 주석을 게시하면 인앱 알림을 받게 됩니다. 활성화한 기능에 따라 구독한 항목에 대한 이메일 및 모바일 앱 푸시 알림을 받을 수도 있습니다.

>[!NOTE]
>
>구독하는 항목에 발생하는 다른 이벤트에 대한 알림을 받지 않습니다. 누군가 항목에 댓글을 달 때만 알림을 받게 됩니다.

구독 작업에 대한 자세한 내용은 [구독 작업 정보](#about-working-with-subscriptions).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Adobe Workfront] 계획*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>만약 [!DNL Workfront] 관리자가 활성화됨 <strong>[!UICONTROL View는 대화에 포함된 업데이트만 표시합니다.]</strong> 액세스 수준에서 [!DNL Workfront].</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!UICONTROL Workfront] 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. [!UICONTROL Workfront] 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>[!UICONTROL View]에서 프로젝트, 작업 또는 문제에 액세스하거나 그 이상에 가입합니다.</p> <p>[!UICONTROL Manage] 액세스 및 [!UICONTROL Share] 프로젝트, 작업 또는 문제(다른 사용자 구독)에 대한 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 항목 구독

항목을 구독하는 프로세스는 모든 항목에 대해 동일합니다.

예를 들어 문제에 가입하려면 다음을 수행하십시오.

1. 구독할 문제로 이동합니다.

   >[!TIP]
   >
   >프로젝트에 가입하려면 다음 중 하나를 수행할 수 있습니다.
   >
   >* 구독할 프로젝트로 이동하여 **[!UICONTROL 자세히]** 아이콘 ![](assets/qs-more-menu.png) 프로젝트 이름의 오른쪽에 있는 **[!UICONTROL 구독]**.
   >* 프로젝트 목록 또는 보고서로 이동하고 프로젝트를 선택한 다음 **[!UICONTROL 자세히]** 아이콘 ![](assets/qs-more-menu.png) 목록의 맨 위에서 을 클릭합니다. **[!UICONTROL 구독]**. 프로젝트 목록에서만 사용할 수 있습니다.


1. 클릭 **[!UICONTROL 자세히]** ![](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL 구독]**.

   ![](assets/subscribe-to-a-work-item-350x258.png)

   벨 위에 확인 표시가 나타나고 그 옆에 있는 번호가 업데이트되어 구독한 사용자 수에 사용자를 추가합니다.

   이제 해당 문제를 구독했습니다. 문제를 구독한 문제 레코드에 대한 업데이트 상태 입니다.

   누군가 이 문제에 대해 댓글을 달 때마다 인앱 알림을 받게 됩니다. 활성화한 기능에 따라 이메일 알림 및 모바일 앱 푸시 알림을 받을 수도 있습니다.

   구독 이메일에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 항목에서 가입 해지

의 항목에서 간편하게 구독을 취소할 수 있습니다 [!DNL Workfront]. 의 항목에서 가입 해지 프로세스 [!DNL Workfront] 은 모든 항목에 대해 동일합니다.

예를 들어 문제 시 구독을 취소하려면,

1. 가입을 해지할 문제로 이동합니다.

   >[!TIP]
   >
   >프로젝트 구독을 취소하려면 다음 중 하나를 수행할 수 있습니다.
   >
   >* 구독을 취소할 프로젝트로 이동하여 **[!UICONTROL 자세히]** 아이콘 ![](assets/qs-more-menu.png) 프로젝트 이름의 오른쪽에 있는 **[!UICONTROL 구독 취소]**.
   >* 프로젝트 목록 또는 보고서로 이동하고 프로젝트를 선택한 다음 **[!UICONTROL 자세히]** 아이콘 ![](assets/qs-more-menu.png) 목록의 맨 위에서 을 클릭합니다. **[!UICONTROL 구독 취소]**. 프로젝트 목록에서만 사용할 수 있습니다.


1. 클릭 **[!UICONTROL 자세히]** ![](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL 구독 취소]**.

   ![](assets/unsubscribe-to-a-work-item-350x258.png)

1. 을 클릭하여 구독한 항목에서 구독을 취소할 수도 있습니다 [!UICONTROL 구독 취소] 링크를 클릭합니다.

   항목의 구독을 취소하면 해당 문제에 대해 다른 사람이 주석을 달 때 더 이상 알림을 받지 않습니다.

   문제의 구독을 취소한 항목 레코드의 업데이트 상태 입니다.

## 구독자 관리

관리 및 공유 권한이 있는 프로젝트, 작업 및 문제에 가입한 사용자를 관리할 수 있습니다.

* [다른 사용자를 항목에 가입](#subscribe-another-user-to-an-item)
* [항목에서 다른 사람 가입 해지](#unsubscribe-another-person-from-an-item)

모든 구독자가 제공됩니다 [!UICONTROL 보기] 구독 항목에 대한 권한. 새 구독자에게 이미 항목에 대한 권한이 있는 경우 해당 권한이 그대로 유지됩니다.

### 다른 사용자를 항목에 가입

1. 다른 사용자를 구독할 항목으로 이동합니다.

   >[!TIP]
   >
   >프로젝트에 다른 사용자를 구독하려면 다음 중 하나를 수행할 수 있습니다.
   >
   >* 다른 사용자를 구독할 프로젝트로 이동하거나
   >   
   >* 프로젝트 목록 또는 보고서로 이동하고 프로젝트를 선택합니다.


1. 클릭 **[!UICONTROL 자세히]** ![](assets/more-icon.png).
1. 다음 옆에 있는 숫자 버블을 클릭합니다. **[!UICONTROL 구독]** 링크를 클릭합니다.
1. 표시되는 상자에서 사용자 이름을 **[!UICONTROL 다른 사용자 구독]** 상자를 선택한 다음 표시되는 옵션에서 사용자를 선택합니다.

1. (선택 사항) 구독자를 더 추가하려면 4단계를 반복합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

구독자에게 구독 알림이 전송되지 않지만 구독에 대한 항목이 해당 항목의 시스템 업데이트에 추가됩니다.

누군가 다음에 주석을 추가할 때 [!UICONTROL 업데이트] 항목의 탭에서 구독자는 인앱 알림을 받습니다. Workfront 관리자가 활성화한 기능에 따라 구독자가 해당 항목에 대한 전자 메일 및 모바일 알림을 받을 수도 있습니다.

### 항목에서 다른 사람 가입 해지

1. 다른 사용자의 구독을 취소할 항목으로 이동합니다.

   >[!TIP]
   >
   >다른 사용자의 프로젝트 가입을 해지하려면 다음 중 하나를 수행할 수 있습니다.
   >
   >* 다른 사용자의 가입을 해지할 프로젝트로 이동하거나
   >   
   >* 프로젝트 목록 또는 보고서로 이동하고 프로젝트를 선택합니다.


1. 클릭 **[!UICONTROL 자세히]** ![](assets/more-icon.png).
1. 다음 옆에 있는 숫자 버블을 클릭합니다. **[!UICONTROL 구독]** 또는 **[!UICONTROL 구독 취소]** 링크를 클릭합니다.
1. 설정 **[!UICONTROL 구독자]** 페이지가 표시되면 가입을 해지할 사용자 이름 옆에 있는 &quot;X&quot;를 클릭합니다.

   또는

   에 사용자 이름을 입력합니다. **[!UICONTROL 목록에서 사람 검색]** 상자를 클릭한 다음 사용자 이름 오른쪽에 있는 &quot;X&quot;를 클릭합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   사용자는 해당 항목의 가입 해지 알림을 받지 않지만 해당 항목의 시스템 업데이트에 가입에 대한 항목이 추가됩니다.

## 인앱 알림 받기

사용자가 가입한 항목에 대한 댓글을 게시하면 바로 인앱 알림을 받게 됩니다.

![](assets/in-app-not---cmmnt-sbscibd-to-350x164.png)

자세한 내용은 [인앱 알림 보기 및 관리](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## 구독 이메일 받기

사용자의 기능에 따라 [!UICONTROL Workfront] 관리자가 활성화하면 구독하는 항목에 대한 댓글이 있을 때마다 인앱 알림 외에도 구독 이메일을 받을 수 있습니다.

이메일 설정 또는 비활성화에 대한 자세한 내용은 [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

>[!NOTE]
>
>구독 이메일을 끄더라도 구독한 항목에 대한 댓글이 있을 때마다 인앱 알림을 계속 받게 됩니다.

## 항목을 구독한 사용자 나열

항목을 구독하는 사용자를 확인하려면:

1. 구독자를 볼 항목으로 이동합니다.

   항목의 구독자가 있으면 벨 옆에 구독자 수가 표시됩니다. 해당 수를 마우스로 가리키면 해당 항목에 가입한 사용자 목록을 표시할 수 있습니다. 처음 25명의 구독자는 알파벳 순서로 표시됩니다.

   ![구독자 보기](assets/bell-hover-for-list-qs-350x90.png)

   또한 [!UICONTROL 가입자] 필드를 가입 항목에 대한 보고서 또는 뷰의 열로 지정합니다. 자세한 내용은 [용어 설명 [!DNL Adobe Workfront] 용어](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## 구독 작업 정보

구독을 사용할 때 다음 사항을 고려하십시오.

* 다음 [!DNL Workfront] 관리자는 사용자가 가입하거나 구독할 수 없는 항목을 제어할 수 없습니다.

   이 [!UICONTROL 보기] 또는 작업, 문제 또는 프로젝트에 대한 더 높은 권한이 해당 작업에 가입할 수 있습니다.

* 일별 다이제스트 전자 메일에 대해 구독을 구성할 수 없습니다.
* 작업, 문제 또는 프로젝트에 가입하고 사용자가 할당자, 기본 연락처 또는 프로젝트 소유자인 경우 사용자가 구독하는 항목에 대한 의견을 표시할 때만 구독 이메일을 받게 됩니다.

   항목 중 하나에 대한 설명이 수행될 때 트리거되는 전자 메일 알림에 대한 자세한 내용은 [Adobe Workfront 알림](../../workfront-basics/using-notifications/wf-notifications.md).

* 항목을 구독하고 댓글을 달면 댓글에 이름을 포함하지 않는 한 해당 댓글에 대한 구독 이메일을 받지 못합니다.
* 항목에 대해 댓글을 다는 사용자가 설명을 잠그어 비공개로 댓글을 작성하고 사용자가 해당 사용자와 동일한 회사의 구성원이 아닌 경우 해당 댓글에 대한 알림을 받지 않습니다. 회사에 대한 비공개 설명을 만드는 방법에 대한 자세한 내용은 [작업 항목에 업데이트 추가](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) 섹션 [작업 업데이트](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* 구독에 대한 보고서를 작성할 수 없습니다. 감사가 항목을 구독하거나 가입 해지할 때 모든 항목의 업데이트 상태에 기록됩니다.
* 자식 개체에 대한 주석은 상위 개체에 대한 구독 알림을 트리거하지 않습니다. 프로젝트에 가입하면 해당 프로젝트에 대한 댓글 알림만 수신됩니다. 각 하위 항목에 가입하지 않으면 프로젝트와 관련된 하위 항목(즉, 작업 또는 문제)에 대한 댓글 알림을 받지 않습니다. 개체 관계에 대한 자세한 내용은 [개체의 상호 종속성 및 계층](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 섹션 [의 개체 이해 [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
