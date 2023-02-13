---
product-area: projects
navigation-topic: update-work-in-a-project
title: 문제 상태 업데이트
description: 문제 상태를 업데이트하여 문제가 어디에서 어떻게 진행되는지 다른 사람에게 알릴 수 있습니다.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# 문제 상태 업데이트

문제 상태를 업데이트하여 문제가 어디에서 어떻게 진행되는지 다른 사람에게 알릴 수 있습니다.

## 액세스 요구 사항

<!--drafted for P&P;

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제 상태

다음은 Workfront의 문제에 대한 기본 상태입니다.

* 신규
* 진행 중
* 대기 중인 피드백
* 보류 중
* 해결되지 않음
* 다시 열림
* 마감됨
* 해결됨

Adobe Workfront 관리자는 조직의 문제에 대한 사용자 지정 상태를 추가할 수 있습니다. 문제 유형에 따라 상태를 사용할 수도 있습니다.

사용자 지정 상태 및 문제 유형에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [문제 만들기](../../../manage-work/issues/manage-issues/create-issues.md)

문제 상태를 수동으로 업데이트하거나, 특정 작업이 발생하면 Workfront에서 자동으로 업데이트하도록 할 수 있습니다.

## 수동으로 문제 상태 업데이트

문제 상태를 업데이트할 때 새 상태에 대한 설명을 추가하고 커밋 날짜와 같은 기타 문제 정보를 변경할 수도 있습니다.

1. 상태를 업데이트할 이 할당된 문제로 이동합니다.
1. 을(를) 클릭합니다. **상태** 문제 헤더의 필드를 작성하고 새 상태를 선택합니다.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. 문제 완료에 대한 시각적 표시를 제공하려면 아래의 버블을 드래그 또는 두 번 클릭합니다 **완료율** 를 입력합니다.

   또는

   문제 헤더에서 버블 내부를 클릭하여 백분율을 입력합니다.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (선택 사항) 업데이트에 대한 추가 정보를 제공하려면 다음 중 하나를 수행한 다음 를 클릭합니다 **업데이트** 또는 문제에 완료와 관련된 상태가 있으면 **완료:**

   * 업데이트에 대한 메모를 추가하려면 **업데이트** 섹션을 클릭하고 **새 업데이트 시작**&#x200B;을 입력한 다음 메모를 입력합니다.

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 특정 사용자에게 업데이트에 대해 알리려면 **알림** 업데이트에 대한 메모를 입력할 때 표시되는 상자입니다. 자세한 내용은 [업데이트에 다른 사용자에게 태그 지정](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 문제 조건을 업데이트하려면 **조건**&#x200B;그런 다음 문제의 현재 조건을 가장 잘 반영하는 조건을 선택합니다. 다음 옵션 중에서 선택합니다.

      * 매끄럽게 진행 중
      * 일부 우려 사항
      * 주요 장애물
   * 문제의 커밋 날짜를 업데이트하려면 **커밋 날짜** 드롭다운 달력에서 새 날짜를 선택합니다.


## 문제 상태 자동 업데이트

Workfront은 아래 표에 나열된 작업이 발생하면 문제의 기존 상태를 자동으로 다른 상태로 업데이트합니다.

>[!NOTE]
>
>다음 표의 상태는 기본 시스템 상태입니다. Workfront 관리자 또는 그룹 관리자는 Workfront 인스턴스에서 상태의 이름을 변경할 수 있습니다. Workfront에서 상태 만들기 및 관리에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>개 액션</td> 
   <td>원래 상태</td> 
   <td>새 상태</td> 
  </tr> 
  <tr> 
   <td>문제 완료 비율을 100%로 업데이트</td> 
   <td>신규 또는 진행 중</td> 
   <td>마감됨</td> 
  </tr> 
  <tr> 
   <td>문제 완료 비율을 100%에서 낮은 숫자로 업데이트합니다</td> 
   <td>마감됨 </td> 
   <td>진행 중</td> 
  </tr> 
  <tr> 
   <td>문제에 연결된 해결 개체의 상태 업데이트</td> 
   <td>다양한 상태</td> 
   <td> <p>다양한 상태</p> <p>객체 해결 및 해당 객체가 문제 상태에 미치는 영향에 대한 자세한 내용은 문서의 "해결 가능한 객체의 상태와 해결 객체 간의 동기화" 섹션을 참조하십시오 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 가능한 객체 해결 및 해결 방법 개요 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>사용자에게 할당된 문제에 대한 작업을 수락하려면 문제 시작 단추를 클릭하십시오</span> </td> 
   <td><span>신규</span> </td> 
   <td> <p>홈 팀 설정의 문제 시작 단추와 연관된 모든 상태입니다. </p> <p>Work On It 단추를 Start Issue 단추로 대체하는 방법에 대한 자세한 내용은 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Work On It 단추를 시작 단추로 바꿉니다.</a></span><span>.</span> </p> <p>팁: 클릭 <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">실행 취소 단추</span> 시작 문제를 클릭하면 상태가 새로 고침으로 되돌아갑니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
