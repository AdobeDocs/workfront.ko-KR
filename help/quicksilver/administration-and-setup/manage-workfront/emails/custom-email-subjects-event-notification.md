---
navigation-topic: notifications
title: 이벤트 알림에 대한 이메일 주체 사용자 정의
description: 이벤트 알림으로 트리거되는 전자 메일의 제목 줄을 사용자 지정할 수 있습니다.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 4%

---

# 이벤트 알림에 대한 이메일 주체 사용자 정의

이벤트 알림으로 트리거되는 전자 메일의 제목 줄을 사용자 지정할 수 있습니다.

제목란 변경은 수신자의 액세스 수준에 관계없이 시스템의 모든 사용자에게 영향을 줍니다. 사용자는 전자 메일 제목에 포함된 모든 개체 및 필드를 봅니다.

일부 이벤트 알림에는 여러 제목 줄이 있으며, 이는 해당 이벤트 알림에 해당 기능에 따라 여러 이메일 주제가 있을 수 있음을 의미합니다.

>[!IMPORTANT]
>
>제목 줄이 여러 객체를 참조하는 경우 기본 필드를 삭제할 때 주의하십시오. 다음은 이러한 제목 줄을 포함하는 이벤트 알림 목록입니다.
>
>* 누군가가 지시된 업데이트에 나를 포함시킵니다.
>* 누군가가 지시된 업데이트에 내 팀을 포함시킵니다.
>* 스레드 참가자에 대한 작업 항목 주석
>* 작업 항목 피할당자에 대한 작업 항목 주석
>


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
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>미리 알림 알림에 대한 관리자 액세스 권한이 있는 계획자 이상</p> <p>계획 사용자 관리 액세스 권한을 제공하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 이벤트 알림에 대한 이메일 제목 줄 사용자 지정 {#customize-email-subject-lines-for-event-notifications}

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **이메일** > **알림 을 참조하십시오**.

1. 을(를) 클릭합니다. **이벤트 알림** 탭.
1. 사용자 지정할 이벤트 알림의 이름을 클릭하여 **이벤트 알림** 상자.
1. 에서 **이메일 제목 줄** 상자에서 전자 메일 제목에서 사용자 지정 필드를 포함한 텍스트 및 필드를 변경합니다.

   추가된 필드의 이름은 데이터베이스 구조의 카멜 사례 구문과 일치해야 합니다. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. 클릭 **업데이트** 이메일에 대한 새 제목 줄을 저장하려면 을 클릭합니다.

## 다중 개체 이메일에 대한 이메일 제목 줄 사용자 지정

일부 이벤트 알림에는 트리거되는 객체에 따라 여러 제목 줄이 있습니다.

예를 들어 &quot;Someone includes me on a directed update&quot;에는 두 개의 서로 다른 주체 라인이 있습니다. 먼저 작업, 문제, 템플릿 작업 및 문서(&quot;referenceObject&quot;라고도 함)를 위한 것이며, 두 번째 것은 사용자가 포트폴리오, 프로그램 등과 같은 주석을 달 수 있는 객체(&quot;topReferenceObject&quot;라고도 함)를 위한 것입니다.

![](assets/Ev-not-mult-subj-lines.png)

사용자가 작업, 문제, 템플릿 작업 또는 문서의 대화에 포함된 경우 첫 번째 제목 줄로 전자 메일이 생성됩니다. 제목 줄에는 &quot;referenceObject:name&quot;이 포함되어 있으며, 시스템에서는 개체를 정의하고 제목 필드에 적절한 이름을 표시합니다. 이메일 제목란은 다음과 유사합니다. &quot;프로젝트 ABC의 작업 123에 대한 설명&quot;

프로젝트 대화에 추가하면 두 번째 주제가 포함된 이메일이 생성됩니다. 제목 줄에는 &quot;topReferenceObject:name&quot;이 포함되어 있으며, Workfront에서도 참조한 개체를 식별하여 제목에서 &quot;topReferenceObject:name&quot; 대신 해당 개체 이름을 반환합니다. 이메일 제목란은 다음과 유사합니다. &quot;프로젝트 ABC에 댓글&quot;

전자 메일 제목 줄을 편집하고 제목 줄에 필드를 추가하려면 다음을 참조하십시오 [이벤트 알림에 대한 이메일 제목 줄 사용자 지정](#customize-email-subject-lines-for-event-notifications) 참조하십시오.

## 여러 작업 이메일에 대한 이메일 제목 줄 사용자 지정

일부 이벤트 알림에는 개체에 대해 수행되는 다양한 작업의 개요를 설명하는 여러 이메일 주제도 있습니다.

예를 들어 문제에 문서를 추가하도록 요청하는 것은 두 개의 다른 이메일을 트리거할 수 있는 이벤트입니다. 문서가 추가될 때, 문서가 편집될 때 각각 하나씩,

![](assets/ev-not-mult-subj-lines-diff-actions.png)

전자 메일 제목 줄을 편집하고 제목 줄에 필드를 추가하려면 다음을 참조하십시오 [이벤트 알림에 대한 이메일 제목 줄 사용자 지정](#customize-email-subject-lines-for-event-notifications) 참조하십시오.
