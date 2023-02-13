---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 큐 항목 만들기
description: 큐 항목은 라우팅 규칙과 함께 작동하여 들어오는 작업을 사용자, 작업 역할, 팀에 자동으로 할당하거나 프로젝트에 배치하도록 합니다. 대기열 항목은 공정순서 규칙을 구현하기 위해 존재해야 하는 조건을 정의합니다.
author: Alina
feature: Work Management
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# 큐 항목 만들기

큐 항목은 라우팅 규칙과 함께 작동하여 들어오는 작업을 사용자, 작업 역할, 팀에 자동으로 할당하거나 프로젝트에 배치하도록 합니다. 대기열 항목은 공정순서 규칙을 구현하기 위해 존재해야 하는 조건을 정의합니다.

주제 그룹이나 프로젝트에 지정할 수 있는 큐 주제 수에는 제한이 없습니다. 큐 항목은 보고서 가능한 개체 유형입니다.

## 액세스 요구 사항

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오

## 대기열 항목 만들기

1. 대기열 항목과 연결하려는 경우 공정순서 규칙, 주제 그룹 및 사용자 정의 양식을 생성합니다.\
   라우팅 규칙, 항목 그룹 또는 사용자 정의 양식을 만드는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. 도움말 요청 대기열로 활성화하도록 선택한 프로젝트 및 새 큐 항목을 만들 위치로 이동합니다.\
   프로젝트를 도움말 요청 큐로 지정하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.\
   [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

   관련 대기열 항목을 항목 그룹 아래의 또는 도움말 요청 대기열로 지정된 프로젝트에서 직접 구성할 수 있습니다. 이렇게 하면 요청자에게 요청을 할 때 일련의 드롭다운 메뉴가 제공됩니다.\
   도움말 요청 대기열로 지정된 프로젝트 아래에서 주제 그룹 없이 바로 큐 항목을 중첩할 수 있습니다.

   항목 그룹 만들기에 대한 내용은 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. 클릭 **큐 항목** 왼쪽 패널에 표시됩니다. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **큐 항목**.
1. 클릭 **새 큐 항목**.
1. 설정 **새 큐 항목** 양식에서 다음을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>이름</strong> </td> 
      <td> 큐 항목의 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>설명</strong> </td> 
      <td>요청 큐를 설명합니다. 사용자가 새 요청을 제출하는 프로세스에서 큐 항목을 선택하면 설명이 표시됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>주제 그룹에 추가</strong> </td> 
      <td> 프로젝트에 주제 그룹이 없으면 프로젝트 이름이 기본적으로 주제 그룹으로 설정됩니다.<br>여기에서 주제 그룹을 추가로 만들려면 다음을 선택합니다 <strong>새 주제 그룹 만들기</strong> 를 클릭합니다.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 정의 양식</strong> </td> 
      <td>큐 항목과 연결할 사용자 지정 양식을 선택합니다. 문제에 대한 사용자 지정 양식을 만든 후에 큐 주제에 연결할 수 있습니다. 사용자 지정 양식 만들기에 대한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 지정 양식 만들기 또는 편집</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 승인</td> 
      <td> <p>승인 프로세스를 이 큐 항목과 연결합니다. 이 드롭다운 메뉴에는 문제 승인 프로세스만 표시됩니다. 이 큐에 제출된 모든 문제가 이 승인 프로세스와 연결됩니다. 큐 항목에 연결하려면 먼저 Adobe Workfront 관리자가 시스템 수준 승인 프로세스를 정의해야 합니다. <span>승인 프로세스에 대한 관리자 액세스 권한이 있는 사용자도 그룹별 승인 프로세스를 만들 수 있습니다.</span> 승인 프로세스 생성에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">작업 항목에 대한 승인 프로세스 생성</a>.<br></p> 
       <div> 
        <p>중요 사항: 프로젝트 그룹이 변경되면 기존 문제에 첨부된 그룹별 승인 프로세스가 단일 사용 승인 프로세스가 됩니다. 프로젝트 그룹의 변경 사항이나 승인 프로세스의 변경 사항이 승인 설정에 미치는 영향에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">그룹 및 승인 프로세스 변경이 지정된 승인 프로세스에 미치는 영향</a>.</p> 
        <p>대기열 항목에 승인 프로세스를 추가할 때 다음 사항을 고려하십시오. </p> 
        <ul style="list-style-type: circle;"> 
         <li>활성 승인 프로세스만 목록에 표시됩니다. </li> 
         <li> <p>시스템 전체 및 그룹별 승인 프로세스가 목록에 표시됩니다. 프로젝트 이외의 그룹과 연관된 승인 프로세스가 목록에 표시되지 않습니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 기간</strong> </td> 
      <td>요청의 기본 기간이며 요청의 계획 완료 일자는 이 값을 기반으로 계산됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 경로</strong> </td> 
      <td>대기열 항목과 연관시킬 공정순서 규칙을 지정합니다. 공정순서 규칙을 대기열 항목에 첨부하려면 먼저 공정순서 규칙을 생성해야 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>요청 유형</strong> </td> 
      <td> <p>이 큐 항목이 저장하는 요청의 종류를 선택합니다. 표시되는 옵션은 <strong>큐 세부 정보</strong> 탭으로 이동합니다. 필수 필드입니다. </p> <p>참고: 요청 유형은 대기열 세부 사항 및 대기열 항목 페이지 모두에서 요청 유형을 선택한 경우에만 요청 영역에 선택 항목으로 표시됩니다. 프로젝트의 큐 세부 정보 영역 설정에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a>. </p> <p>다음 유형 중에서 선택합니다.</p> 
       <ul> 
        <li>버그 신고</li> 
        <li>순서 변경</li> 
        <li>문제</li> 
        <li>요청</li> 
       </ul> <p>Workfront 관리자가 이러한 옵션 중 일부의 이름을 변경했을 수 있습니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-queue-topic-box-nwe-350x375.png)

1.  
1. **저장**&#x200B;을 클릭합니다.\
   이제 큐 항목을 사용할 수 있으며, 요청 큐 및 항목 그룹을 선택한 후 Workfront의 요청 영역에 표시됩니다.
