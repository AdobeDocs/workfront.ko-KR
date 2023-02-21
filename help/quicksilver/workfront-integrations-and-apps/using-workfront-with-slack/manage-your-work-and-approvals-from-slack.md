---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Slack에서 작업 및 승인 관리
description: 홈 작업 목록에 액세스하여 작업 및 문제에 대해 검토하고 동의하고 Slack에서 직접 승인을 검토하거나 결정할 수 있습니다.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 1%

---

# 다음 위치에서 작업 및 승인 관리 [!DNL Slack]

설치한 후 [!DNL Adobe Workfront for Slack]로 지정하는 경우 다음을 수행할 수 있습니다.

* 사용자 목록 액세스 [!UICONTROL 홈] 항목 [!DNL Slack]
* 작업 및 문제 해결 [!DNL Slack]
* 승인을 검토하고 결정하려면 [!DNL Slack]

구성에 대한 자세한 정보 [!DNL Workfront] with [!DNL Slack]를 참조하십시오. [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 플랜</a>*</td> 
   <td> <p>[!UICONTROL Pro] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

작업 및 승인을 관리하려면 먼저 [!DNL Slack]:

* Configure [!DNL Workfront for Slack]\
   구성에 대한 지침 [!DNL Workfront for Slack]를 참조하십시오. [구성 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 다음 위치에서 작업 관리 [!DNL Slack]

1. 에 로그인합니다. [!DNL Slack] 인스턴스 및 로그인 [!DNL Workfront] 변환 전: [!DNL Slack].\
   로그인하는 방법에 대한 자세한 정보 [!DNL Workfront] 변환 전: [!DNL Slack]에 로그인하는 것은 [!DNL Workfront] 변환 전: [!DNL Slack]&quot; 섹션 [액세스 [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 채널에서 메시지 필드에 다음 명령을 입력합니다.

   `/workfront home`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* 명령을 `/wf` 대신 `/workfront`.


   작업, 문제 및 승인 목록에 액세스할 수 있는 단추가 표시됩니다. 버튼 중 하나를 클릭하면 각 목록에 있는 처음 20개 항목이 표시됩니다. [!DNL Slack].

1. (선택 사항) **[!UICONTROL 작업]** 모든 작업을 표시합니다.

   의 작업 관리에 대한 자세한 내용은 [!DNL Slack]를 참조하십시오. [작업 관리 [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (선택 사항) **[!UICONTROL 문제]** 모든 문제를 표시합니다.

   의 문제 관리에 대한 자세한 정보 [!DNL Slack]를 참조하십시오. [문제 관리 [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (선택 사항) **[!UICONTROL 승인]** 결정을 기다리는 모든 승인을 표시합니다.\
   에서 승인 관리에 대한 자세한 정보 [!DNL Slack]를 참조하십시오. [다음 위치에서 승인 관리 [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## 다음 위치에서 작업 관리 [!DNL Slack] {#manage-your-tasks-from-slack}

1. 에 로그인합니다. [!DNL Slack] 인스턴스 및 로그인 [!DNL Workfront] 변환 전: [!DNL Slack].\
   로그인하는 방법에 대한 자세한 내용 [!DNL Workfront] 변환 전: [!DNL Slack]에 로그인하는 것은 [!DNL Workfront] 변환 전: [!DNL Slack]&quot; 섹션 [액세스 [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력합니다.

   `/workfront home`를 클릭한 다음 **[!UICONTROL 작업]**

   또는

   `/workfront tasks`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* 명령을 `/wf` 대신 `/workfront`.


   목록에 있는 처음 20개의 작업이 표시됩니다.

1. 클릭 **[!UICONTROL +`<remaining number>` 자세히]** 추가 작업을 표시합니다.
1. 작업 항목에 대한 다음 정보를 검토하십시오.

   * **[!UICONTROL 이름]**
   * **[!UICONTROL 프로젝트 이름]** 또는 **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** 작업 항목.
   * **[!DNL Assigned By Name]**: 작업을 자신에게 할당한 사용자의 이름입니다.
   * **[!UICONTROL 상태]**

1. (선택 사항) 항목의 이름을 클릭하여 별도의 브라우저 탭에서 Workfront에서 엽니다.
1. (선택 사항)에서 **[!UICONTROL 상태]** 필드에서 새 상태를 선택합니다.
1. (선택 사항) **[!UICONTROL 로그 시간]**&#x200B;를 선택한 다음 을 선택합니다 **[!UICONTROL 시간 유형]** 및 한 시간은 항목에 대한 로그 시간입니다.

   >[!NOTE]
   >
   >* 최대 12시간 30분 동안 전체 또는 30분 단위로 시간만 로그인할 수 있습니다.
   >* 로그하는 시간(오늘 시작 날짜)이 있습니다. 다음부터는 과거 또는 미래 날짜에 대한 시간을 기록할 수 없습니다 [!DNL Slack].


   시간이 기록되었다는 확인 메시지가 나타납니다.

1. (선택 사항) **[!UICONTROL 작업]** 일을 맡도록 수락하다. 다음 [!UICONTROL 작업] 단추가 사라집니다.

## 다음에서 문제 관리 [!DNL Slack] {#manage-your-issues-from-slack}

1. 에 로그인합니다. [!DNL Slack] 인스턴스 및 로그인 [!DNL Workfront] 변환 전: [!DNL Slack].\
   로그인하는 방법에 대한 자세한 정보 [!DNL Workfront] 변환 전: [!DNL Slack]를 참조하고 [에 로그인 [!DNL Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력합니다.

   `/workfront home`를 클릭한 다음 **[!UICONTROL 문제]**

   또는

   `/workfront issues`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* 명령을 `/wf` 대신 `/workfront`.


   목록의 처음 20개의 문제가 표시됩니다.

1. 클릭 **[!UICONTROL + 남음 `<number>` 자세히]** 추가 항목을 표시하려면 다음을 수행하십시오.
1. 작업 항목에 대한 다음 정보를 검토하십시오.

   * **[!UICONTROL 이름]**
   * **[!UICONTROL 프로젝트]** 이름 또는 상위 개체 이름
   * **[!UICONTROL 기한]** 날짜: 작업 항목의 계획 완료 일자입니다.
   * **[!DNL Requested by]** 이름: 기본 연락처(문제) 또는 할당을 수행한 사용자(작업)

1. (선택 사항) 문제 이름을 클릭하여 별도의 브라우저 탭에서 Workfront에서 엽니다.
1. (선택 사항) **[!DNL Work on it]** 아직 수락하지 않은 문제에 대해 작업을 시작하기 위해

   다음 [!UICONTROL 작업] 단추가 사라집니다.

## 다음 위치에서 승인 관리 [!DNL Slack] {#manage-your-approvals-from-slack}

1. 에 로그인합니다. [!DNL Slack] 인스턴스 및 로그인 [!DNL Workfront] 변환 전: [!DNL Slack].\
   로그인하는 방법에 대한 자세한 정보 [!DNL Workfront] 변환 전: [!DNL Slack]에 로그인하는 것은 [!DNL Workfront] 변환 전: [!DNL Slack]&quot; 섹션 [액세스 [!DNL Adobe Workfront] 변환 전: [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 채널에서 메시지 필드에 다음 명령 중 하나를 입력합니다.

   `/workfront home`를 클릭한 다음 **[!UICONTROL 승인]**

   또는

   `/workfront approvals`

   >[!NOTE]
   >
   >* 명령은 대/소문자를 구분합니다.
   >* 명령을 `/wf` 대신 `/workfront`.


   처음 20개 항목이 **[!UICONTROL 승인]** 목록 표시. 항목을 요청한 사용자 이름 또는 항목이 속한 프로젝트의 이름과 같은 항목에 대한 추가 정보도 표시됩니다.

1. 클릭 **[!UICONTROL + 남음 `<number>` 자세히]** 추가 항목을 표시하려면 다음을 수행하십시오.

1. 다음 객체에 대한 승인 관리를 고려해 보십시오.

   * **프로젝트**

      클릭 **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]** 프로젝트의 상태 변경을 수락하거나 거부하려면

   * **작업**

      클릭 **[!UICONTROL 승인]** 또는 **[!UICONTROL 거부]** 작업의 상태 변경을 수락하거나 거부합니다.

   * **문제**

      클릭 **[!UICONTROL 승인]** 또는 **[!DNL Reject]** 문제 상태 변경을 수락하거나 거부합니다.

   * **문서**

      클릭 **[!UICONTROL 승인]** 문서를 승인하려면 **[!UICONTROL 거부]** 거부하거나 **[!UICONTROL 변경 사항]** 승인하지만 문서에 추가 변경 사항이 필요함을 나타냅니다.\
      (선택 사항) 문서 축소판 위로 마우스를 가져가면 돋보기를 클릭하고 문서를 미리 볼 수 있습니다.

   * **증명**&#x200B;증명 &#x200B; 이름을 클릭하여 엽니다. [!DNL Workfront] 별도의 탭에서 승인을 관리합니다.
   * **액세스 권한 요청**

      클릭 **[!UICONTROL 액세스 권한 부여]** 요청된 개체에 향상된 권한을 부여하거나 **[!UICONTROL 무시]** 추가 액세스 요청을 무시합니다.

1. (선택 사항) 승인을 위해 제출된 객체의 이름을 클릭하여 엽니다. [!DNL Workfront] 새 브라우저 탭에서 을 클릭합니다.
