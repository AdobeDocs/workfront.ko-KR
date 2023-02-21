---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 관리 [!DNL Adobe Workfront] 알림 [!DNL Microsoft] 팀
description: 에서 알림을 받을 수 있습니다 [!DNL Adobe Workfront] 승인해야 하는 항목에 대한 정보, 지정한 할당 또는 연결된 항목에 대한 설명 및 변경 사항
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 473a1fe3cb7e247749d9b540e3e5556cbe17a1dd
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 0%

---

# 관리 [!DNL Adobe Workfront] 알림 [!DNL Microsoft Teams]

에서 알림을 받을 수 있습니다 [!DNL Adobe Workfront] 승인해야 하는 항목에 대한 정보, 지정한 할당 또는 연결된 항목에 대한 설명 및 변경 사항

이러한 알림은 다음을 포함합니다 [!DNL Workfront] 가능한 작업 [!DNL Microsoft Teams] 이동 없이 [!DNL Microsoft Teams] 이를 실현하기 위해

>[!NOTE]
>
>[!DNL Microsoft Teams] 더 이상 지원되지 않음 [!DNL Internet Explorer]. 를 사용하려면 [!DNL Adobe Workfront for Microsoft Teams integration]를 채울 때는 다음 이외의 웹 브라우저를 사용해야 합니다 [!DNL Internet Explorer].


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 수신 사전 요구 사항 [!DNL Workfront] 의 알림 [!DNL Microsoft Teams]

받을 수 있습니다 [!DNL Workfront] 알림 [!DNL Microsoft Teams] 다음 조건이 충족되는 경우:

* 팀 소유자가 설치 및 구성되었습니다 [!DNL Workfront for Microsoft Teams] 팀용.
* 로그인되어 있습니다. [!DNL Workfront] 변환 전: [!DNL Microsoft Teams].
* 에서 인스턴트 알림을 활성화했습니다 [!DNL Workfront]. 인스턴트 알림 활성화에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

설치에 대한 자세한 정보 [!DNL Workfront for Microsoft Teams] 및에 로그인하십시오. [!DNL Workfront from Microsoft Teams]를 참조하십시오. [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## 관리 [!DNL Workfront] 의 알림 [!DNL Microsoft Teams]

이 [!DNL Workfront for Microsoft Teams] 앱이 설치되어 있고, [!DNL Workfront] 채팅 채널은 [!DNL Microsoft Teams] 해당 팀의 모든 구성원에게 에서 특정 작업이 수행되는 경우 [!DNL Workfront]에 대한 설정을 구성할 수 있습니다. [!DNL Workfront for Microsoft Teams] 에서 해당 작업에 대한 알림을 수신하려면 [!DNL Workfront] 채팅 채널 [!DNL Microsoft Teams].

작업 시 다음 사항을 고려하십시오 [!DNL Workfront] 알림 [!DNL Microsoft Teams]:

* 모두 받을 수는 없지만 선택한 개수만 받을 수 있습니다 [!DNL Workfront] 알림 [!DNL Microsoft Teams].
* 받는 모든 알림 [!DNL Workfront] 에 나타납니다. [!DNL Workfront] 보트 채팅 채널.

   설치에 대한 자세한 내용은 [!DNL Workfront] 보트 채널입니다. 자세한 내용은 [에 로그인 [!DNL Workfront] 변환 전: [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) 섹션 [설치 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) 문서.

* 에서 업데이트가 수행된 시간 사이에 최대 5분 지연이 있을 수 있습니다 [!DNL Workfront] 그리고 다음에 대한 알림을 받으면 [!DNL Microsoft Teams].
* 각 [!DNL Microsoft Teams] 알림 또한 이메일 알림을 받습니다.

를 관리하려면 [!DNL Workfront] 수신할 수 있는 알림 [!DNL Microsoft Teams]:

1. 을(를) 클릭합니다. **[!UICONTROL 추가 추가됨]** (3점) 앱 아이콘 [!DNL Microsoft Teams].

1. 클릭 [!DNL Workfront] 표시됩니다.
1. 을(를) 선택합니다 **[!UICONTROL 설정]** 탭.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. 수신하지 않을 알림을 비활성화합니다. 정보 또는 승인 알림과 같은 알림 그룹을 활성화하거나 비활성화하거나 개별적으로 알림을 관리할 수 있습니다.

   모든 알림은 기본적으로 활성화되어 있습니다.

   에 대한 알림 설정 [!DNL Workfront for Microsoft] 팀이 자동으로 저장됩니다.

   >[!NOTE]
   >
   >기본적으로 사용할 수 있는 알림은 더 추가할 수 없습니다.

## 에 응답 [!DNL Workfront] 의 알림 및 승인 요청 [!DNL Microsoft Teams]

1. 에 로그인합니다. [!DNL Workfront] 변환 전: [!DNL Microsoft Teams].\
   로그인하는 방법에 대한 자세한 내용 [!DNL Workfront]를 참조하십시오. [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. 로 이동합니다. **[!UICONTROL 채팅]** 영역을 클릭하고 **[!DNL Workfront]** 보트 채널.\
   이 채널은 [!DNL Workfront] 보트. 모두 [!DNL Workfront] 여기에 알림이 표시됩니다.
1. 받은 알림 유형에 따라 관련 섹션을 진행합니다.

   * [승인 알림](#approval-notifications-approval-notifications)
   * [할당 알림](#assignment-notifications-assignment-notifications)
   * [댓글 알림](#comment-notifications-comment-notifications)
   * [알림 업데이트](#update-notifications-update-notifications)
   * [날짜 변경 알림](#date-change-notifications-date-change-notifications)

### 승인 알림 {#approval-notifications}

작업, 작업표 또는 증명과 같은 개체의 승인을 요청받으면 승인 알림을 받습니다. 통지에 대해서는 여전히 주석을 달 수 있습니다.승인 알림에서 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 승인]**: 을(를) 클릭하여 항목을 승인합니다.
* **[!UICONTROL 변경]**: 변경 사항이 있는 항목을 승인하려면 를 클릭합니다.
* **[!UICONTROL 거부]**: 항목을 거부하려면 을(를) 클릭합니다.
* **[!UICONTROL 댓글]**: 을(를) 클릭하여 주석을 답니다. 댓글은 [!DNL Workfront] 알림의 대상이 되는 객체에 대한 업데이트입니다.
* **[!UICONTROL 증명으로 이동]**: 증명을 열려면 를 클릭합니다. 그런 다음 증명한 내용을 직접 결정할 수 있습니다. 자세한 내용은 [교정 뷰어의 증명 결정](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>승인 결정을 한 후에는 알림에서 변경할 수 없습니다.

#### 특정 승인 알림에 사용할 수 있는 작업:

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
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL 증명으로 이동] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">프로젝트를 승인해야 합니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업을 승인해야 합니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">문제를 승인해야 합니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">문서를 승인해야 합니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">객체에 대한 액세스를 승인해야 합니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업표를 승인해야 합니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">누군가 이 증명을 승인하기를 원합니다</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업표가 거부됨</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업표가 다시 열립니다</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">요청한 문서 승인 요청이 승인됩니다</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">요청한 문서 승인 요청이 변경 내용으로 승인됩니다</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">요청한 문서 승인 요청이 거부됩니다</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업표가 승인되었습니다.</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 할당 알림 {#assignment-notifications}

사용자나 현재 있는 팀이 Workfront에서 작업이나 문제에 할당되면 할당 알림을 받습니다. 발령 통지에서는 다음 조치를 수행할 수 있습니다.

* **[!UICONTROL 작업]**: 항목을 사용하여 작업하려면 을(를) 선택합니다. 새 항목이 작업 목록에 추가되었음을 확인하는 알림이 잠깐 표시됩니다.
* **[!UICONTROL 에서 보기[!DNL Workfront]]**: Workfront에서 지정된 문제 또는 작업을 보려면 이 옵션을 선택하면 새 탭이 열립니다.
* **[!UICONTROL 시작]**: 항목에 대한 작업을 시작하려면 을(를) 클릭합니다. 새 항목이 작업 목록에 추가되었음을 확인하는 알림이 잠깐 표시됩니다.
* **[!UICONTROL 댓글]**: 을(를) 클릭하여 항목에 주석을 추가합니다. Workfront의 항목 업데이트 스트림에도 주석이 표시됩니다.
* **[!UICONTROL 상태]**: 을(를) 클릭한 다음 드롭다운 메뉴에서 작업 항목의 새 상태를 선택합니다.

#### 특정 지정 알림에 사용할 수 있는 작업:

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
   <td role="rowheader">문제에 할당되었습니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">할당된 팀이 작업에 대한 작업 요청을 받습니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">할당된 팀이 문제에 대한 작업 요청을 받습니다</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 댓글 알림 {#comment-notifications}

사용자가 연결된 항목에 대한 댓글 또는 업데이트에 사용자를 포함하면 통신 알림을 받게 됩니다. 통신 알림에서 다음 작업을 수행할 수 있습니다.

* **Reply**: 댓글에 답글을 달려면 을(를) 클릭하거나 [!UICONTROL 업데이트]. 답변은 Workfront에 주석이 표시되는 업데이트 스트림에도 나타납니다.
* **[!UICONTROL Workfront에서 보기]**: 을(를) 선택하여 새 탭에서 열리는 Workfront의 주석 및 항목을 확인합니다.
* **[!UICONTROL 상태]**: 을(를) 클릭한 다음, 주석 또는 업데이트가 관련된 작업 항목의 새 상태를 선택합니다.

#### 특정 통신 알림에 사용할 수 있는 작업:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL 상태]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">귀하의 요청에 댓글이 게시됩니다</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">회신은 작업 요청에 게시됩니다</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">현재 사용 중인 스레드에 대한 의견</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업 항목 중 하나에 대한 댓글이 있습니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자가 승인하는 작업표에 대한 의견</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">사용자 프로필 페이지에 댓글을 추가하거나 여러 사용자를 벌크 편집하여 주석을 추가합니다</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">업데이트 중 하나에 댓글이 추가됩니다</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업표에 주석이 추가됩니다</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 알림 업데이트 {#update-notifications}

연관된 항목에 대한 업데이트가 있으면 정보 알림을 받게 되지만 항목에 대해 조치를 취할 필요는 없습니다. 정보 알림에서 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 회신]**: 을(를) 클릭하여 [!UICONTROL 업데이트]. 답변이 Workfront의 항목 업데이트 스트림에도 표시됩니다.
* **Workfront에서 보기**: 을(를) 선택하여 새 탭에서 열리는 Workfront의 주석 및 항목을 확인합니다.
* **[!UICONTROL 상태]**: 을(를) 클릭한 다음 드롭다운 메뉴에서 항목의 새 상태를 선택합니다.

#### 특정 정보 알림에 사용할 수 있는 작업:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL 상태]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">구독한 작업, 문제 또는 프로젝트에 대한 업데이트가 수행됩니다</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">누가 당신을 소개시켜</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 지정 업데이트]에 팀이 포함되어 있습니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 날짜 변경 알림 {#date-change-notifications}

지정한 작업 항목에 대한 날짜가 변경되면 날짜 변경 통지를 받게 됩니다. 날짜 변경 알림에서 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 댓글]**: 을(를) 클릭하여 항목에 주석을 추가합니다. Workfront의 항목 업데이트 스트림에도 주석이 표시됩니다.
* **[!UICONTROL 상태]**: 을(를) 클릭한 다음 드롭다운 메뉴에서 작업 항목의 새 상태를 선택합니다.

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
   <td role="rowheader">지정한 작업의 기한 변경</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
