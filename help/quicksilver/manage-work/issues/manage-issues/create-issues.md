---
product-area: projects
navigation-topic: manage-issues
title: 문제 만들기
description: 프로젝트에서 작업하는 동안 예기치 않은 이벤트가 발생할 수 있습니다. 이러한 예기치 않은 이벤트를 특정 프로젝트 또는 작업의 문제로 기록할 수 있습니다. 적절한 액세스 권한이 있는 사용자는 프로젝트 또는 작업이 완료되기 전에 진행 중인 문제의 상태를 보고 모니터링할 수 있으므로 긴 이메일 체인이나 상태 회의가 필요하지 않습니다. 계획된 이벤트인 작업과 달리, 문제는 Adobe Workfront에서 계획되지 않은 작업 항목을 나타냅니다.
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# 문제 만들기

프로젝트에서 작업하는 동안 예기치 않은 이벤트가 발생할 수 있습니다. 이러한 예기치 않은 이벤트를 특정 프로젝트 또는 작업의 문제로 기록할 수 있습니다. 적절한 액세스 권한이 있는 사용자는 프로젝트 또는 작업이 완료되기 전에 진행 중인 문제의 상태를 보고 모니터링할 수 있으므로 긴 이메일 체인이나 상태 회의가 필요하지 않습니다. 계획된 이벤트인 작업과 달리, 문제는 Adobe Workfront에서 계획되지 않은 작업 항목을 나타냅니다.

요청에 문제를 추가할 수도 있습니다. 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>문제 및 요청은 Workfront에서 서로 교환하여 사용됩니다. 프로젝트 및 작업 모두에 문제를 기록하여 해결해야 하는 예상치 못한 작업을 나타낼 수 있습니다. 요청 큐로 지정된 프로젝트에서 문제로 기록된 요청을 제출할 수도 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>프로젝트나 작업에 문제를 추가하려면 검토 또는 그 이상을 수행합니다</p> <p>요청 큐를 사용하여 문제를 요청으로 추가하도록 요청 이상.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>프로젝트 및 작업에 대한 보기 이상의 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 액세스 수준의 문제에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제를 만드는 작업이나 프로젝트에 문제를 추가하는 기능을 사용하여 기여 또는 더 높은 권한</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a></p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## 문제 만들기의 제한 사항

올바른 액세스 및 권한이 있으면 프로젝트나 작업에 문제를 만들 수 있습니다. 그러나 다음과 같이 문제를 만들 수 없는 경우가 있습니다.

* Workfront 관리자나 그룹 관리자는 프로젝트 환경 설정 영역에서 완료 또는 중단 상태에 있는 프로젝트에 문제를 추가할 수 있도록 설정해야 합니다. 프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 승인 보류 중인 프로젝트에 문제를 추가할 수 없습니다.

## 새 문제 양식 준비

문제를 기록할 시기 및 방법에 대해 조직에서 잘 정의된 프로세스를 준비해야 합니다. 이 프로세스를 구성할 때 첫 번째 단계는 문제 제출에 필요한 양식을 만드는 것입니다. 작업 및 프로젝트에 문제를 직접 추가할 수 있도록 허용할지, 문제가 제출되는 요청 큐가 있는지 여부에 관계없이, 사용자가 새로운 문제를 제출할 때 사용할 수 있는 사용자 지정 필드와 Workfront 필드를 정의할 수 있으며, 이를 완료해야 합니다. 새 문제 양식에는 문제를 신속하게 해결하는 데 유용한 중요한 정보가 포함될 수 있습니다.

프로젝트의 새 문제에 대한 필드는 문제가 기록될 프로젝트의 큐 세부 정보 섹션에 정의되어 있습니다. 프로젝트의 큐 세부 정보 섹션 구성에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

요청을 큐에 제출하여 문제를 만드는 방법에 대한 자세한 내용은 [새 요청을 입력하여 문제 만들기](#create-issues-by-entering-a-new-request) 섹션에 자세히 설명되어 있습니다.

## 새 문제 단추를 사용하여 작업 또는 프로젝트에 문제를 만듭니다

프로젝트에서 새 문제 양식의 필드를 정의한 후 문제 만들기를 시작할 수 있습니다.

작업 또는 프로젝트에 대한 문제를 만들려면 다음을 수행하십시오.

1. 문제를 만들 프로젝트로 이동합니다.
1. (선택 사항) 작업에 대한 문제를 기록하려면 **작업** 영역에서 작업 이름을 클릭합니다.
1. 을(를) 클릭합니다. **문제** 섹션을 참조하십시오.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. 클릭 **새 문제**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (조건부) 프로젝트 작성자가 프로젝트에서 큐 주제 또는 주제 그룹을 만든 경우 새 문제 양식에 추가됩니다. 을(를) 지정합니다. **주제 그룹** 또는 **큐 항목** 새로운 문제 환경에 사용자 지정된 이름을 사용해야 합니다.\
   주제 그룹 만들기에 대한 자세한 내용은 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 큐 항목 만들기에 대한 자세한 내용은 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * 프로젝트에 설정된 큐 항목이 하나만 있으면 자동으로 표시됩니다.
   * 주제 그룹에 대기열 항목 또는 주제 그룹이 없으면 주제 그룹 드롭다운에서 사용할 수 있는 항목이 없습니다.

1. (조건부) 프로젝트 작성자가 **문제 유형** 새 문제 양식에 표시할 필드에서 다음 옵션 중에서 문제 유형을 선택합니다.

   * 버그 신고
   * 순서 변경
   * 문제
   * 요청\
      Workfront 관리자가 프로젝트 환경 설정을 구성한 방식에 따라 문제 유형의 이름이 달라질 수 있습니다.

1. 에서 사용할 수 있는 필드를 지정합니다. **새 문제** 양식. 새 문제를 입력할 때 필드를 정의하는 방법에 대한 자세한 내용은 [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md).
1. (조건부) 큐 항목이 사용자 지정 양식과 연결되어 있으면 해당 사용자 지정 양식이 **새 문제** 양식.\
   또는\
   프로젝트가 큐 세부 정보 영역을 통해 문제 사용자 지정 양식과 연결되어 있으면 양식이 **새 문제** 기본 Workfront 필드 아래에 있는 Form입니다.

   자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 클릭 **새 문제를 저장합니다.**

여러 사용자, 작업 역할 또는 팀에 문제를 할당할 수 있습니다. 요청 지정 및 관리에 대한 자세한 내용은 [작업 및 팀 요청 관리](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## 작업 또는 프로젝트 인라인에 문제 만들기

>[!IMPORTANT]
>
>프로젝트 소유자가 **사용자가 인라인 문제를 추가할 수 있도록 허용** 프로젝트에 대한 문제 설정을 정의할 때 프로젝트 또는 작업에 인라인 문제를 추가할 수 있습니다. 프로젝트에서 문제 설정 구성에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

여러 문제를 빠르게 추가하려면 문제 목록에 추가하여 작업 또는 프로젝트 인라인에 문제를 만들 수 있습니다.

>[!NOTE]
>
>문제를 인라인으로 추가하면 Workfront에서 새 문제 양식을 새 문제에 적용하지 않습니다. 사용자가 문제를 입력할 때 특정 정보를 제공하려면 인라인 문제를 추가하지 않는 것이 좋습니다. 이 경우 문제 보고에 부정적인 영향을 줄 수 있고 나중에 문제에 지정된 사용자가 문제 해결에 필요한 모든 정보를 가질 수 있습니다.

인라인 문제를 만들려면

1. 문제를 만들 프로젝트로 이동합니다.
1. (선택 사항) 작업에 대한 문제를 기록하려면 **작업** 섹션을 클릭한 다음 작업 이름을 클릭합니다.
1. 을(를) 클릭합니다. **문제** 섹션을 참조하십시오.
1. 클릭 **추가 문제**.

   문제 섹션의 문제 목록에 새 줄이 만들어집니다.

   >[!TIP]
   >
   >[프로젝트 편집] 상자에서 [사용자가 문제를 추가할 수 있도록 허용] 인라인 설정이 선택 취소되면 이 옵션은 흐리게 표시됩니다. 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. 이름 필드에 문제 이름을 입력한 다음 인라인으로 문제에 대한 자세한 정보를 계속 추가합니다.

   >[!TIP]
   >
   >인라인을 편집하는 데 사용할 수 있는 필드는 문제 목록에 적용하는 보기에서 사용할 수 있습니다. 다음 유형의 필드를 인라인 편집하지 못할 수 있습니다.
   >   
   >* 다른 개체에 속하는 필드
   >* 편집할 수 있는 액세스 권한이 없는 필드
   >* 계산 필드이며 Workfront에서 자동으로 업데이트하는 필드


1. 입력 을 클릭하여 인라인 편집을 마치고 프로젝트나 작업에 문제를 추가합니다.

## 새 요청을 입력하여 문제 만들기 {#create-issues-by-entering-a-new-request}

문제를 수신하기 위해 프로젝트를 수신하도록 지정할 수 있습니다. 이러한 유형의 프로젝트를 Workfront의 요청 큐라고 합니다. 기본 메뉴의 요청 영역을 통해 요청 큐에 액세스할 수 있습니다.

>[!TIP]
>
>Workfront에서는 &quot;문제&quot;와 &quot;요청&quot;이라는 용어를 서로 바꿔서 사용할 수 있습니다.

문제를 수신하기 위해 프로젝트를 요청 큐로 설정하는 방법에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). 요청 제출에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).
