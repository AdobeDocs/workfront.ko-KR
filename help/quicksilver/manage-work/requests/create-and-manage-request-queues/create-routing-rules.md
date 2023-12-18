---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 라우팅 규칙 만들기
description: 라우팅 규칙은 Adobe Workfront이 요청 대기열에 제출될 때 발생하는 문제를 제어합니다. 요청 대기열 만들기에 대한 자세한 내용은 요청 대기열 만들기를 참조하십시오.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: e971f08a1ee9bbf27a78916dbec57ca729407c03
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 1%

---

# 라우팅 규칙 만들기

<!-- Audited: 12/2023 -->

라우팅 규칙은 Adobe Workfront이 요청 대기열에 제출될 때 발생하는 문제를 제어합니다. 요청 대기열 만들기에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

라우팅 규칙은 제출된 문제 또는 요청을 해결하기 위해 가장 잘 갖추어진 특정 사용자 또는 작업 역할에 문제를 보냅니다. 라우팅 규칙은 일반적으로 대기열 주제와 연결되며, 문제 또는 요청에 적용할 라우팅 규칙을 제어하는 데 사용됩니다.

## 액세스 요구 사항

<!--drafted - replace the table at P&P:

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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>
    <p>새로운 기능: 표준</p>
    <p>또는</p>
    <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 라우팅 규칙 만들기

1. 요청에 대한 라우팅 규칙을 추가할 프로젝트로 이동합니다.
1. 클릭 **라우팅 규칙** 왼쪽 패널에서 다음을 클릭해야 할 수 있습니다. **더 보기**, 그런 다음 **라우팅 규칙**.
1. 클릭 **새 라우팅 규칙** 새 규칙을 추가합니다.
1. 공정순서 규칙에 대해 다음 정보를 입력합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>이름</strong> </td> 
      <td>라우팅 규칙의 이름입니다. 프로젝트에 대한 이 정보를 볼 수 있는 액세스 권한이 있는 경우 라우팅 규칙을 볼 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>설명</strong> </td> 
      <td>라우팅 규칙에 대한 설명을 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 담당자*</strong> </td> 
      <td>새 문제를 할당해야 하는 활성 사용자 또는 활성 작업 역할을 추가합니다. 이 필드에는 기본 피할당자를 한 명만 가질 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 팀*</strong> </td> 
      <td>새 문제를 할당해야 하는 활성 팀을 추가합니다. 이 필드에는 기본 팀이 하나만 있을 수 있습니다.

   <p><b>메모</b></p>

   문제가 제출되면 해당 할당을 편집하고 다른 사용자, 역할 또는 팀을 할당할 수 있습니다. 자세한 내용은  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">문제 할당</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>프로젝트로의 경로</strong> </td> 
      <td>문제가 추가되는 프로젝트입니다.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*사용자, 작업 역할 또는 팀이 라우팅 규칙과 연결된 후 비활성화되면 요청이 계속 라우팅됩니다. 모든 공정순서 규칙의 재고를 정기적으로 가져오고 비활성화된 지정을 활성 지정으로 대체해야 합니다.

   문제를 프로젝트로 라우팅하면 문제에 대한 권한이 있는 사용자가 해당 프로젝트에 대해 설정된 권한을 받습니다. 프로젝트에 대한 권한 설정에 대한 자세한 내용은 [Adobe Workfront에서 프로젝트 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![새 라우팅 규칙 상자](assets/new-routing-rule-box.png)

1. **저장**&#x200B;을 클릭합니다.

   이 프로세스는 라우팅 규칙만 정의합니다. 문제가 요청 대기열로 제출될 때 라우팅되도록 하려면 **대기열 세부 정보** 아래의 탭 **기본 경로**.

   요청 대기열에 기본 경로 추가에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   여러 라우팅 규칙을 요청 대기열과 연결하려면 여러 대기열 주제를 만들고 각 대기열 주제를 별도의 라우팅 규칙과 연결해야 합니다. 대기열 주제를 만드는 방법에 대한 자세한 내용은 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
