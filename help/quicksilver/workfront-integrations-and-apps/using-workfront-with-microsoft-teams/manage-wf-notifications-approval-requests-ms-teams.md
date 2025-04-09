---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 'Teams에서 [!DNL Microsoft] 알림 관리 [!DNL Adobe Workfront] '
description: 승인해야 하는 항목, 받은 과제 또는 연결된 항목의 댓글 및 변경 사항에 대한 알림을 [!DNL Adobe Workfront] 받을 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 41d898e82bc5b06498966ba938b68ed10e742d3b
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 0%

---

# 알림 관리 [!DNL Adobe Workfront] 위치 [!DNL Microsoft Teams]

>[!NOTE]
>
>2025년 7월 1일부터 Microsoft는 클래식 Teams 데스크탑 앱에 대한 지원을 제거합니다. 따라서 클래식 Teams 데스크탑 앱을 더 이상 사용할 수 없게 된 후에는 Microsoft Teams와의 Workfront 통합이 지원되지 않습니다.

[!DNL Adobe Workfront]에서 승인해야 하는 항목, 받은 할당 또는 연결된 항목에 대한 댓글 및 변경 사항에 대한 알림을 받을 수 있습니다.

이러한 알림에는 다른 [!DNL Microsoft Teams] 곳으로 이동하지 않고 내부 [!DNL Microsoft Teams] 에서 수행할 수 있는 작업이 포함되어 [!DNL Workfront] 있습니다.

>[!NOTE]
>
>[!DNL Microsoft Teams] 더 이상 를 지원하지 [!DNL Internet Explorer]않습니다. 을 [!DNL Adobe Workfront for Microsoft Teams integration]&#x200B;(를) 사용하려면 가 아닌 [!DNL Internet Explorer]다른 웹 브라우저()를 사용해야 합니다.


## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## [!DNL Microsoft Teams]에서 [!DNL Workfront] 알림을 받기 위한 필수 구성 요소

다음 조건이 충족되는 경우 알림을 받을 [!DNL Workfront] 수 있습니다.[!DNL Microsoft Teams]

* 팀 팀 소유자가 설치 및 구성 [!DNL Workfront for Microsoft Teams] 되었습니다.
* 에서 [!DNL Microsoft Teams]로그인 [!DNL Workfront] 했습니다.
* [!DNL Workfront]에서 인스턴트 알림을 사용하도록 설정했습니다. 인스턴트 알림을 사용하는 방법에 대한 자세한 내용은 [전자 메일 알림 수정](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)을 참조하세요.

[!DNL Workfront for Microsoft Teams]을(를) 설치하고 [!DNL Workfront from Microsoft Teams]에 로그인하는 방법에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)를 참조하십시오.

## [!DNL Microsoft Teams]에서 [!DNL Workfront]개의 알림 관리

[!DNL Workfront for Microsoft Teams] 앱이 설치되면 해당 팀의 모든 구성원에 대해 [!DNL Microsoft Teams]에 [!DNL Workfront] 채팅 채널이 만들어집니다. [!DNL Workfront]에서 특정 작업이 수행되면 [!DNL Microsoft Teams]의 [!DNL Workfront] 채팅 채널에서 해당 작업에 대한 알림을 받도록 [!DNL Workfront for Microsoft Teams]에 대한 설정을 구성할 수 있습니다.

[!DNL Microsoft Teams]의 [!DNL Workfront] 알림을 사용하여 작업할 때 다음 사항을 고려하십시오.

* 모두 받을 수 없지만 [!DNL Microsoft Teams]에서 선택한 개수의 [!DNL Workfront]개의 알림만 받습니다.
* [!DNL Workfront]에서 받은 모든 알림이 [!DNL Workfront] 봇 채팅 채널에 표시됩니다.

  [!DNL Workfront] 보트 채널 설치에 대한 자세한 내용은 [설치 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) 문서의 [로그인 대상 [!DNL Workfront] 부터 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) 섹션을 참조하십시오.

* [!DNL Workfront]에서 업데이트를 수행한 시간과 [!DNL Microsoft Teams]에서 해당 알림이 전송되는 시간 사이에 최대 5분이 지연될 수 있습니다.
* 각 [!DNL Microsoft Teams] 알림에 대해 전자 메일 알림도 받습니다.

[!DNL Microsoft Teams]에서 받을 수 있는 [!DNL Workfront] 알림을 관리하려면:

1. [!DNL Microsoft Teams]의 왼쪽 탐색 막대에 있는 **[!UICONTROL 추가 추가]**(점 3개) 앱 아이콘을 클릭합니다.

1. 표시되는 목록에서 [!DNL Workfront]을(를) 클릭합니다.
1. **[!UICONTROL 설정]** 탭을 선택합니다.

   ![MS 팀 설정 탭](assets/ms-teams-settings-tab-350x552.png)

1. 수신하지 않을 알림을 비활성화합니다. 정보 또는 승인 알림과 같은 알림 그룹을 활성화 또는 비활성화하거나 개별적으로 알림을 관리할 수 있습니다.

   모든 알림은 기본적으로 활성화되어 있습니다.

   [!DNL Workfront for Microsoft] 팀에 대한 알림 설정이 자동으로 저장됩니다.

   >[!NOTE]
   >
   >기본적으로 사용할 수 있는 알림에는 알림을 더 추가할 수 없습니다.

## [!DNL Microsoft Teams]에서 [!DNL Workfront]개의 알림 및 승인 요청에 응답 중

1. [!DNL Microsoft Teams]에서 [!DNL Workfront]에 로그인합니다.\
   [!DNL Workfront]에 로그인하는 방법에 대한 자세한 내용은 [설치 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)를 참조하십시오.

1. **[!UICONTROL 채팅]** 영역으로 이동하여 **[!DNL Workfront]** 봇 채널을 클릭합니다.\
   이 채널은 보트 간의 개인 채팅을 [!DNL Workfront] 위한 것입니다. 모든 [!DNL Workfront] 알림이 여기에 표시됩니다.
1. 수신한 알림 유형에 따라 관련 섹션으로 진행하십시오.

   * [승인 알림](#approval-notifications-approval-notifications)
   * [할당 통지](#assignment-notifications-assignment-notifications)
   * [댓글 알림](#comment-notifications-comment-notifications)
   * [알림 업데이트](#update-notifications-update-notifications)
   * [날짜 변경 알림](#date-change-notifications-date-change-notifications)

### 승인 알림 {#approval-notifications}

승인 알림은 작업, 작업표 또는 증명과 같은 개체를 승인하라는 요청을 받을 때 받을 수 있습니다. 그러나 알림 내용에는 계속 댓글을 달 수 있습니다. 승인 알림 화면에서 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 승인]**: 항목을 승인하려면 클릭합니다.
* **[!UICONTROL 변경]**: 변경 내용이 있는 항목을 승인하려면 클릭하세요.
* **[!UICONTROL 거부]**: 항목을 거부하려면 클릭하십시오.
* **[!UICONTROL 댓글]**: 댓글을 달려면 클릭하세요. 주석은 알림 관련 개체에 대한 업데이트로도 [!DNL Workfront] 표시됩니다.
* **[!UICONTROL 증명으로]** 이동: 증명을 열려면 클릭합니다. 그런 다음 증명에서 직접 결정을 내릴 수 있습니다. 자세한 내용은 교정 뷰어](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)에서 증명에 대한 결정을 참조하십시오[.

>[!NOTE]
>
>승인 결정을 내린 후에는 알림 에서 변경할 수 없습니다.

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
   <th>[! UICONTROL 승인]</th> 
   <th>[! UICONTROL 거부]</th> 
   <th> <p>[!UICONTROL 변경]</p> </th> 
   <th> <p>[! UICONTROL 증명으로 이동] </p> </th> 
   <th>[! UICONTROL 댓글]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">프로젝트를 승인해야 합니다.</td> 
   <td>✓</td> 
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
   <td role="rowheader">작업표가 거부되었습니다.</td> 
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
   <td role="rowheader">요청한 문서 결재 요청 승인</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">요청한 문서 결재 요청 변경 내용이 승인됩니다</td> 
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

* **[!UICONTROL 작업]**: 항목에 대해 작업하도록 커밋하려면 선택하십시오. 작업 목록에 새 항목이 추가되었음을 확인하는 알림이 잠시 표시됩니다.
* **[!UICONTROL [!DNL Workfront]]**&#x200B;에서 보기: Workfront에서 할당된 문제 또는 작업을 보려면 선택하십시오. 그러면 새 탭이 열립니다.
* **[!UICONTROL 시작]**: 항목에 대한 작업을 시작하려면 클릭하세요. 작업 목록에 새 항목이 추가되었음을 확인하는 알림이 잠시 표시됩니다.
* **[!UICONTROL 댓글]**: 항목에 댓글을 달려면 클릭하세요. 댓글은 Workfront에서 항목의 업데이트 스트림에도 표시됩니다.
* **[!UICONTROL 상태]**: 을(를) 클릭한 다음 드롭다운 메뉴에서 작업 항목에 대한 새 상태를 선택합니다.

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
   <td role="rowheader">사용자에게 배정된 팀 문제에 대한 작업 요청</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 댓글 알림 {#comment-notifications}

누군가 나와 관련된 항목에 댓글을 달거나 귀하를 업데이트에 포함시키면 커뮤니케이션 알림을 받게 됩니다. 통신 통지에서 다음 작업을 수행할 수 있습니다.

* **Rep ly**: 댓글에 답글을 달거나 [!UICONTROL 업데이트]하려면 클릭합니다. 답장은 Workfront에서 댓글이 표시되는 업데이트 스트림에도 표시됩니다.
* **[!UICONTROL Workfront]**&#x200B;에서 보기: 새 탭에 열려 있는 Workfront에서 댓글 및 항목을 보려면 선택합니다.
* **[!UICONTROL 상태]**: 을 클릭한 다음, 주석 또는 업데이트와 관련된 작업 항목의 새 상태를 선택합니다.

#### 특정 통신 알림에서 사용할 수 있는 작업:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th>[! UICONTROL 회신]</th> 
   <th> <p>[! UICONTROL 상태]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">요청 시 댓글이 게시됩니다.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업 요청 시 회신이 게시됩니다.</td> 
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
   <td role="rowheader">승인한 작업표에 다른 사람의 댓글</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">주석이 사용자 프로필 페이지에 추가되거나 여러 사용자를 벌크 편집하여 추가된 경우</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">업데이트 중 하나에 주석이 추가됩니다.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">작업표에 메모가 추가됩니다.</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 알림 업데이트 {#update-notifications}

연관된 항목에 대한 업데이트가 있을 때 정보 알림을 수신하지만, 해당 항목에 대해 어떤 조치도 취할 필요가 없습니다. 정보 통지에서 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 회신]**: [!UICONTROL 업데이트]에 회신하려면 클릭하세요. 답변은 Workfront에서 항목의 업데이트 스트림에도 표시됩니다.
* **Workfront**&#x200B;에서 보기: 새 탭에 열려 있는 Workfront에서 댓글 및 항목을 보려면 선택합니다.
* **[!UICONTROL 상태]**: 클릭하여 드롭다운 메뉴에서 항목에 대한 새 상태를 선택합니다.

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

지정된 작업 항목의 날짜가 변경되면 날짜 변경 알림 알림을 받게 됩니다. 날짜 변경 알림 후 다음 작업을 수행할 수 있습니다.

* **[!UICONTROL 댓글]**: 항목에 댓글을 남기려면 클릭합니다. 주석은 Workfront의 항목 업데이트 스트림에도 표시됩니다.
* **[!UICONTROL 상태]**: 을 클릭한 다음, 드롭다운 메뉴에서 작업 항목의 새 상태를 선택합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>알림</th> 
   <th> <p>[! UICONTROL 댓글]</p> </th> 
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
