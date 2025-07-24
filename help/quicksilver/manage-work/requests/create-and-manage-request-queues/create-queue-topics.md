---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 대기열 주제 만들기
description: 대기열 항목은 라우팅 규칙과 함께 작동하여 들어오는 작업을 자동으로 사용자, 작업 역할, 팀에 할당하거나 프로젝트에 배치합니다. 대기열 항목은 라우팅 규칙을 구현하기 위해 존재해야 하는 조건을 정의합니다.
author: Alina
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 3563d5e7136d8bd70504a0b7762c4be06e5a9c56
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 2%

---

# 대기열 주제 만들기

<!-- Audited: 12/2023 -->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

대기열 항목은 라우팅 규칙과 함께 작동하여 들어오는 작업을 자동으로 사용자, 작업 역할, 팀에 할당하거나 프로젝트에 배치합니다. 대기열 항목은 라우팅 규칙을 구현하기 위해 존재해야 하는 조건을 정의합니다.

주제 그룹 또는 프로젝트에 할당할 수 있는 대기열 주제 수에는 제한이 없습니다. 대기열 주제는 보고 가능한 객체 유형입니다.

개별 프로젝트 또는 프로젝트 템플릿에 대한 대기열 주제를 만들 수 있습니다.

만든 후에는 프로젝트 또는 템플릿 간에 대기열 주제를 이동할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
    <p>새로운 기능: 표준</p>
    <p>또는</p>
    <p>현재: 플랜</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 대기열 주제 만들기

1. 라우팅 규칙, 주제 그룹 및 사용자 정의 양식을 작성하여 대기열 주제와 연결하십시오.\
   라우팅 규칙, 주제 그룹 또는 사용자 정의 양식을 만드는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. 도움말 요청 대기열로 사용하기 위해 선택한 프로젝트 또는 템플릿과 새 대기열 주제를 만들 위치로 이동합니다.\
   프로젝트를 도움말 요청 대기열로 지정하는 방법에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.

   주제 그룹 아래에서 관련 대기열 주제를 구성할 수 있습니다. 이렇게 하면 요청을 할 때 요청자에게 일련의 드롭다운 메뉴를 제공합니다.

   또는

   주제 그룹 없이 도움말 요청 대기열로 지정된 프로젝트 아래에 대기열 주제를 직접 중첩할 수 있습니다.

   주제 그룹 만들기에 대한 자세한 내용은 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)를 참조하십시오.

1. 왼쪽 패널에서 **주제 큐**&#x200B;를 클릭합니다.
1. **새 대기열 주제**&#x200B;를 클릭합니다.
1. **새 대기열 주제** 양식에서 다음을 입력합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>이름</strong> </td> 
      <td> 대기열 주제 이름.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>설명</strong> </td> 
      <td>요청 대기열에 대해 설명합니다. 사용자가 새 요청을 제출하는 과정에서 대기열 주제를 선택하면 설명이 표시됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>주제 그룹에 추가</strong> </td> 
      <td> 프로젝트에 주제 그룹이 없는 경우 프로젝트 이름은 기본적으로 주제 그룹으로 설정됩니다.<br>여기에서 추가 주제 그룹을 만들려면 드롭다운 메뉴에서 <strong>새 주제 그룹 만들기</strong>를 선택하십시오.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 정의 양식</strong> </td> 
      <td>대기열 주제와 연결할 사용자 정의 양식을 선택합니다. 대기열 주제에 연결하려면 먼저 문제에 대한 사용자 정의 양식을 만들어야 합니다. 사용자 정의 양식 만들기에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">사용자 정의 양식 만들기</a>를 참조하십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 승인</strong></td> 
      <td> <p>승인 프로세스를 이 대기열 주제와 연결합니다. 문제 승인 프로세스만 이 드롭다운 메뉴에 표시됩니다. 이 대기열에 제출된 모든 문제는 이 승인 프로세스와 연결됩니다. 대기열 주제에 연결하려면 먼저 Adobe Workfront 관리자가 시스템 수준 승인 프로세스를 정의해야 합니다. <span>승인 프로세스에 대한 관리자 액세스 권한이 있는 사용자는 그룹별 승인 프로세스를 만들 수도 있습니다.</span> 승인 프로세스 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">작업 항목에 대한 승인 프로세스 만들기</a>를 참조하십시오.<br></p> 
       <div> 
        <p>중요: 프로젝트 그룹이 변경되면 기존 문제에 첨부된 그룹별 승인 프로세스가 일회용 승인 프로세스가 됩니다. 프로젝트 그룹 변경 또는 승인 프로세스 변경 내용이 승인 설정에 미치는 영향에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">그룹 및 승인 프로세스 변경 내용이 할당된 승인 프로세스에 미치는 영향</a>을 참조하십시오.</p> 
        <p>대기열 주제에 승인 프로세스를 추가할 때는 다음 사항을 고려하십시오. </p> 
        <ul style="list-style-type: circle;"> 
         <li>활성 승인 프로세스만 목록에 표시됩니다. </li> 
         <li> <p>시스템 전체 및 그룹별 승인 프로세스가 목록에 표시됩니다. 프로젝트 그룹 이외의 그룹과 연결된 승인 프로세스가 목록에 표시되지 않습니다.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 기간</strong> </td> 
      <td>요청의 기본 기간이며, 요청의 계획된 완료 일자 는 이 값을 기반으로 계산됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 경로</strong> </td> 
      <td>대기열 주제와 연결할 라우팅 규칙을 지정합니다. 라우팅 규칙을 만들어 대기열 주제에 첨부해야 합니다. 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">라우팅 규칙 만들기</a>를 참조하십시오. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>요청 유형</strong> </td> 
      <td> <p>이 대기열 주제가 저장할 요청 종류를 선택합니다. 프로젝트의 <strong>큐 세부 정보</strong> 탭에서 표시되는 옵션이 설정됩니다. 필수 필드입니다. </p> 
       <p><b>참고</b>:</p>
      <p>유형은 [대기열 세부 정보] 및 [대기열 주제] 페이지에서 [요청 유형]이 선택된 경우에만 [요청] 영역에 선택 항목으로 표시됩니다. 프로젝트의 대기열 세부 정보 영역 설정에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a>를 참조하십시오. </p> <p>다음 유형 중에서 선택합니다.</p> 
       <ul> 
        <li>버그 신고</li> 
        <li>순서 변경</li> 
        <li>문제</li> 
        <li>요청</li> 
       </ul> <p>Workfront 관리자가 이러한 옵션 중 일부의 이름을 변경했을 수 있습니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![새 대기열 주제 상자](assets/new-queue-topic-box.png)

1. **저장**&#x200B;을 클릭합니다.\
   이제 대기열 주제를 사용할 수 있으며, 요청 대기열 및 주제 그룹을 선택한 후에 Workfront의 요청 영역에 표시됩니다.

## 대기열 주제 편집

기존 대기열 주제를 편집하려면:

1. 편집할 대기열 주제가 포함된 프로젝트 또는 템플릿으로 이동합니다.
1. 왼쪽 패널에서 **주제 큐**&#x200B;를 클릭합니다.
1. 프로덕션 환경에서 편집할 대기열 주제를 선택합니다. 화면에 표시되는 세부 정보 페이지에서 **대기열 주제 편집**&#x200B;을 클릭합니다.
1. <span class="preview">미리 보기 환경에서 편집할 대기열 주제를 선택한 다음 편집 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.</span>

