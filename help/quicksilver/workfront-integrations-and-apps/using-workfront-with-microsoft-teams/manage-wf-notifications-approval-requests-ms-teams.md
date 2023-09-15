---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 관리 [!DNL Adobe Workfront] 의 알림 [!DNL Microsoft] 팀
description: 다음 위치에서 알림을 받을 수 있습니다. [!DNL Adobe Workfront] 승인해야 하는 항목, 주어진 할당 또는 연결된 항목에 대한 댓글 및 변경 사항 정보.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 0%

---

# 관리 [!DNL Adobe Workfront] 의 알림 [!DNL Microsoft Teams]

다음 위치에서 알림을 받을 수 있습니다. [!DNL Adobe Workfront] 승인해야 하는 항목, 주어진 할당 또는 연결된 항목에 대한 댓글 및 변경 사항 정보.

이러한 알림에는 다음이 포함됩니다. [!DNL Workfront] 내에서 수행할 수 있는 작업 [!DNL Microsoft Teams] 에서 멀리 떠나지 않고 [!DNL Microsoft Teams] 이를 실현하기 위해

>[!NOTE]
>
>[!DNL Microsoft Teams] 더 이상 을 지원하지 않음 [!DNL Internet Explorer]. 을(를) 사용하려면 [!DNL Adobe Workfront for Microsoft Teams integration], 이외의 웹 브라우저를 사용해야 합니다. [!DNL Internet Explorer].


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 수신 사전 요구 사항 [!DNL Workfront] 의 알림 [!DNL Microsoft Teams]

다음을 받을 수 있습니다. [!DNL Workfront] 의 알림 [!DNL Microsoft Teams] 다음 조건이 충족되는 경우:

* 팀 소유자가 설치 및 구성했습니다. [!DNL Workfront for Microsoft Teams] 팀용입니다.
* 에 로그인되었습니다. [!DNL Workfront] 출처: [!DNL Microsoft Teams].
* 에서 인스턴트 알림을 활성화했습니다. [!DNL Workfront]. 즉시 알림 활성화에 대한 자세한 내용은 [이메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

설치에 대한 자세한 내용 [!DNL Workfront for Microsoft Teams] 및에 로그인합니다. [!DNL Workfront from Microsoft Teams], 참조 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## 관리 [!DNL Workfront] 의 알림 [!DNL Microsoft Teams]

다음의 경우 [!DNL Workfront for Microsoft Teams] 앱이 설치되었습니다. [!DNL Workfront] 채팅 채널 생성일: [!DNL Microsoft Teams] 모든 팀원을 위해. 특정 작업이 다음 위치에서 수행되는 경우 [!DNL Workfront], 다음에 대한 설정을 구성할 수 있습니다. [!DNL Workfront for Microsoft Teams] 에서 해당 작업에 대한 알림을 받으려면 [!DNL Workfront] 의 채팅 채널 [!DNL Microsoft Teams].

를 사용하여 작업할 때 다음 사항을 고려하십시오 [!DNL Workfront] 다음에서 알림: [!DNL Microsoft Teams]:

* 다음을 모두 받을 수 없지만, 선택한 숫자만 받습니다. [!DNL Workfront] 의 알림 [!DNL Microsoft Teams].
* 받는 모든 알림 [!DNL Workfront] 다음에 표시: [!DNL Workfront] 봇 채팅 채널.

  설치에 대한 자세한 내용 [!DNL Workfront] 보트 채널, 참조: [에 로그인하는 중 [!DNL Workfront] 출처: [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) 의 섹션 [설치 중 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) 기사.

* 업데이트가 이루어지는 시간 사이에 최대 5분의 지연이 있을 수 있습니다 [!DNL Workfront] 및에서 이에 대한 알림을 받을 때 [!DNL Microsoft Teams].
* 각 [!DNL Microsoft Teams] 알림은 이메일 알림도 받습니다.

을 관리하려면 [!DNL Workfront] 에서 수신할 수 있는 알림 [!DNL Microsoft Teams]:

1. 다음을 클릭합니다. **[!UICONTROL 추가 추가됨]** 의 왼쪽 탐색 막대에 있는 (점 3개) 앱 아이콘 [!DNL Microsoft Teams].

1. 클릭 [!DNL Workfront] 표시되는 목록에서 을 클릭합니다.
1. 다음 항목 선택 **[!UICONTROL 설정]** 탭.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. 수신하지 않을 알림을 비활성화합니다. 정보 또는 승인 알림과 같은 알림 그룹을 활성화 또는 비활성화하거나 개별적으로 알림을 관리할 수 있습니다.

   모든 알림은 기본적으로 활성화되어 있습니다.

   에 대한 알림 설정 [!DNL Workfront for Microsoft] 팀은 자동으로 저장됩니다.

   >[!NOTE]
   >
   >기본적으로 사용할 수 있는 알림에는 알림을 더 추가할 수 없습니다.

## 다음에 응답 [!DNL Workfront] 의 알림 및 승인 요청 [!DNL Microsoft Teams]

1. 에 로그인 [!DNL Workfront] 출처: [!DNL Microsoft Teams].\
   에 로그인하는 방법에 대한 자세한 내용 [!DNL Workfront], 참조 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. 로 이동 **[!UICONTROL 채팅]** 영역을 클릭하고 **[!DNL Workfront]** 보트 채널.\
   이 채널은 사용자와의 개인 채팅을 위한 것입니다. [!DNL Workfront] 보트. 모두 [!DNL Workfront] 알림이 여기에 표시됩니다.
1. 수신하는 알림 유형에 따라 관련 섹션으로 진행하십시오.

   * [승인 알림](#approval-notifications-approval-notifications)
   * [할당 알림](#assignment-notifications-assignment-notifications)
   * [댓글 알림](#comment-notifications-comment-notifications)
   * [알림 업데이트](#update-notifications-update-notifications)
   * [날짜 변경 알림](#date-change-notifications-date-change-notifications)

### 승인 알림 {#approval-notifications}

작업, 타임시트 또는 증명과 같은 개체를 승인하라는 메시지가 표시되면 승인 알림을 받습니다. 알림에 주석을 달 수 있지만 승인 알림에서 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 승인]**: 항목을 승인하려면 클릭하십시오.
* **[!UICONTROL 변경]**: 변경 사항이 있는 항목을 승인하려면 클릭하십시오.
* **[!UICONTROL 거부]**: 항목을 거부하려면 클릭합니다.
* **[!UICONTROL 댓글]**: 댓글을 달려면 클릭하십시오. 주석은에 표시됩니다. [!DNL Workfront] 알림이 포함된 객체에 대한 업데이트입니다.
* **[!UICONTROL 증명으로 이동]**: 증명을 열려면 를 클릭합니다. 그런 다음 증명에서 직접 결정을 내릴 수 있습니다. 자세한 내용은 [증명 뷰어에서 증명 결정](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>승인 결정을 한 후에는 알림에서 변경할 수 없습니다.

#### 특정 승인 알림에서 사용할 수 있는 작업:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL 거부]</th> 
   <th> <p>[!UICONTROL 변경]</p> </th> 
   <th> <p>[!UICONTROL 증명으로 이동] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">프로젝트를 승인해야 합니다.</td> 
   <td>✓ 덧신</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업을 승인해야 합니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">문제를 승인해야 합니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">문서를 승인해야 합니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">오브젝트에 대한 액세스를 승인해야 합니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">타임시트를 승인해야 합니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">누군가가 이 증명의 승인을 요청했습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">내 타임시트가 거부되었습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">타임시트가 다시 열렸습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">요청한 문서 승인 요청이 승인되었습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">요청한 문서 승인 요청이 변경 사항과 함께 승인되었습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">요청한 문서 승인 요청이 거부되었습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">타임시트가 승인되었습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 할당 알림 {#assignment-notifications}

귀하 또는 귀하가 속한 팀이 Workfront의 작업 또는 문제에 할당되었을 때 할당 알림을 받습니다. 발령 통지에서 다음 조치를 수행할 수 있습니다.

* **[!UICONTROL 처리 중]**: 항목에 대한 작업을 커밋하려면 선택합니다. 작업 목록에 새 항목이 추가되었음을 확인하는 알림이 잠시 표시됩니다.
* **[!UICONTROL 다음에서 보기[!DNL Workfront]]**: Workfront에서 할당된 문제 또는 작업을 보려면 을 선택합니다. 그러면 새 탭이 열립니다.
* **[!UICONTROL 시작]**: 항목 작업을 시작하려면 클릭하십시오. 작업 목록에 새 항목이 추가되었음을 확인하는 알림이 잠시 표시됩니다.
* **[!UICONTROL 댓글]**: 항목에 대한 댓글을 달려면 클릭합니다. 댓글은 Workfront에서 항목의 업데이트 스트림에도 표시됩니다.
* **[!UICONTROL 상태]**: 를 클릭한 다음, 드롭다운 메뉴에서 작업 항목에 대한 새 상태를 선택합니다.

#### 특정 할당 알림에서 사용할 수 있는 작업:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>[!UICONTROL 시작]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL 상태]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">작업에 할당되었습니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">문제에 할당되었습니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">할당된 팀에게 작업에 대한 작업 요청이 수신됨</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자에게 할당된 팀이 문제에 대한 작업 요청을 받습니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 댓글 알림 {#comment-notifications}

누군가 나와 관련된 항목에 댓글을 달거나 귀하를 업데이트에 포함시키면 커뮤니케이션 알림을 받게 됩니다. 통신 통지에서 다음 작업을 수행할 수 있습니다.

* **Reply**: 댓글에 답글을 달거나 [!UICONTROL 업데이트]. 답변이 Workfront에서 댓글이 표시되는 업데이트 스트림에도 표시됩니다.
* **[!UICONTROL Workfront에서 보기]**: 새 탭에서 열리는 Workfront의 주석 및 항목을 보려면 을 선택합니다.
* **[!UICONTROL 상태]**: 을(를) 클릭한 다음, 댓글 또는 업데이트와 관련된 작업 항목에 대한 새 상태를 선택합니다.

#### 특정 통신 알림에서 사용할 수 있는 작업:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>[!UICONTROL 회신]</th> 
   <th> <p>[!UICONTROL 상태]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">귀하의 요청에 댓글이 게시되었습니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">귀하의 작업 요청에 답글이 게시되었습니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">누군가가 내가 속한 스레드에 댓글을 남겼습니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">누군가 내 작업 항목 중 하나에 주석을 남김</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">누군가가 내가 승인한 타임시트에 댓글을 남겼습니다.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">주석이 사용자 프로필 페이지에 추가되거나 여러 사용자를 일괄 편집하여 추가됩니다</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">업데이트 중 하나에 댓글이 추가되었습니다.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">타임시트에 댓글이 추가되었습니다.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 알림 업데이트 {#update-notifications}

연관된 항목에 대한 업데이트가 있을 때 정보 알림을 수신하지만, 해당 항목에 대해 어떤 조치도 취할 필요가 없습니다. 정보 통지에서 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 답변]**: 회신하려면 클릭 [!UICONTROL 업데이트]. 답변은 Workfront에서 항목의 업데이트 스트림에도 표시됩니다.
* **Workfront에서 보기**: 새 탭에서 열리는 Workfront의 주석 및 항목을 보려면 을 선택합니다.
* **[!UICONTROL 상태]**: 를 클릭한 다음, 드롭다운 메뉴에서 항목에 대한 새 상태를 선택합니다.

#### 특정 정보 알림에서 사용할 수 있는 작업:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>[!UICONTROL 회신]</th> 
   <th> <p>[!UICONTROL 상태]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">구독 중인 작업, 문제 또는 프로젝트에 업데이트가 이루어짐</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">누군가가 지시된 업데이트에 귀하를 포함시킵니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">누군가가 [!UICONTROL 지정 업데이트에 귀하의 팀을 포함시킵니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 날짜 변경 알림 {#date-change-notifications}

할당된 작업 항목에 대한 날짜가 변경되면 날짜 변경 알림을 받습니다. 일자 변경 통지부터 다음 조치를 수행할 수 있습니다.

* **[!UICONTROL 댓글]**: 항목에 대한 댓글을 달려면 클릭합니다. 댓글은 Workfront에서 항목의 업데이트 스트림에도 표시됩니다.
* **[!UICONTROL 상태]**: 를 클릭한 다음, 드롭다운 메뉴에서 작업 항목에 대한 새 상태를 선택합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL 상태]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">할당된 작업의 기한 변경</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
