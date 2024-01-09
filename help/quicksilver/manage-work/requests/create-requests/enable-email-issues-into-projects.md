---
product-area: requests
navigation-topic: create-requests
title: 사용자가 문제를 요청 대기열 프로젝트에 이메일로 보낼 수 있도록 설정
description: 사용자가 문제를 요청 대기열 프로젝트에 이메일로 보낼 수 있도록 설정
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: dad055b0901cfa8114f7f6b13b6f689d70b31205
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# 사용자가 문제를 요청 대기열 프로젝트에 이메일로 보낼 수 있도록 설정

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

사용자가 이메일을 통해 프로젝트에 문제를 추가할 수 있도록 프로젝트를 구성할 수 있습니다. 프로젝트가 요청 대기열로 지정된 경우에만 문제를 프로젝트로 이메일로 보내도록 허용할 수 있습니다. 요청 대기열 프로젝트 만들기에 대한 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

사용자가 이메일을 통해 프로젝트에 문제를 추가할 수 있도록 프로젝트를 구성하려면 다음 전제 조건이 필요합니다.

이 기능을 활성화하기 전에 다음 조건을 충족해야 합니다.

* 이 계정에 문제를 이메일로 보내는 사용자는 Workfront 라이선스가 있는 활성 사용자여야 합니다.
* 이 계정에 문제를 이메일로 보내는 사용자는 프로젝트에 대한 문제 추가 권한이 있어야 합니다.
* 외부 사용자는 문제를 만들 수 있는 액세스 권한이 없으므로 요청 대기열에 문제를 이메일로 보낼 수 없습니다.
* 활성 Workfront 사용자와 연결된 이메일 주소에서 오는 이메일만 프로젝트에 문제를 보낼 수 있습니다. Workfront 계정과 연관되지 않은 이메일에서 활성 Workfront 사용자 이메일로 전달된 이메일은 원래 발신자의 이메일 주소가 활성 Workfront 계정과 연관되어야 하므로 프로젝트에서 문제를 생성할 수 없습니다.
* 프로젝트가 요청 대기열로 설정됩니다.
* 프로젝트와 연결된 이메일 계정이 Workfront 사용자 계정에 연결되어 있지 않습니다.

## Workfront에서 프로젝트 구성

>[!NOTE]
>
>이메일 대기열 설정을 활성화할 때는 다음 사항에 유의하십시오.
>
>* Workfront에서는 모든 클러스터에서 요청 대기열당 하나의 고유한 이메일을 허용합니다. 요청 대기열을 비활성화하도록 선택하면 만든 이메일 주소가 수신 이메일 주소 상자에 있는 한 유지됩니다. 수신 이메일 사용을 중단하기로 선택한 경우 나중에 사용할 수 있도록 수신 이메일 필드에서 해당 수신 이메일을 삭제해야 합니다.
>
>* 요청 대기열에 여러 개의 대기열 주제 또는 주제 그룹이 있는 경우 Workfront은 이메일 요청이 전달될 대기열 주제를 임의로 선택하여 이메일 요청을 관리하기 어렵게 합니다.
>이메일을 통해 요청을 수신하도록 설정한 프로젝트에는 대기열 주제가 두 개 이상 있어서는 안 됩니다. 제출된 요청이 다른 리소스 또는 프로젝트를 위한 경우 제출된 후 수동으로 라우팅하거나 이동해야 합니다.

1. 이메일을 통해 문제를 수신할 수 있도록 활성화할 프로젝트로 이동합니다.
1. 클릭 **대기열 세부 정보** 왼쪽 패널에서 다음을 클릭해야 할 수 있습니다. **더 보기** 첫 번째.
1. 다음에서 **대기열 유형** 영역, 선택 **도움말 요청 대기열로 게시**.

1. 아래로 스크롤하여 **이메일 대기열 설정** 영역을 선택한 다음 을 선택합니다. **이메일을 통한 요청 접수 활성화**.

1. 전자 메일 주소의 시작 부분을 **수신 이메일 주소** 상자.

   고유한 이메일 주소를 만들어야 합니다. 수신 이메일 주소의 일부로 회사 이름을 사용하는 것이 좋습니다.

   >[!CAUTION]
   >
   >* 요청 대기열이 포함된 프로젝트를 삭제한 경우 휴지통에서 이 이메일 주소를 복구할 수 없습니다.
   >
   >* 이 이메일 주소는 고유해야 하므로 삭제하면 나중에 사용할 수 없습니다.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (선택 사항) **이메일을 통해 제출하지 못한 모든 문제 전달**&#x200B;을(를) 클릭한 다음 아래 상자에 전달 이메일 주소를 입력합니다.

   이 이메일 주소는 프로젝트에 제출하지 못한 이메일에 대한 정보를 수신합니다.

1. **저장**&#x200B;을 클릭합니다. 이제 활성 Workfront 계정이 있는 사용자가 이 이메일 주소로 이메일을 보내면 Workfront 프로젝트에 문제가 생성됩니다.

   >[!NOTE]
   >
   >이메일을 통해 제출하려면 프로젝트에 문제를 만들 수 있는 액세스 권한이 있어야 합니다. 고급 설정 아래의 공유 대화 상자에서 이 액세스 권한을 부여할 수 있습니다.
   >
   >외부 사용자는 문제를 만들 수 있는 액세스 권한이 없으므로 요청 대기열에 문제를 이메일로 보낼 수 없습니다.

## Workfront에서 문제 수신

Workfront 사용자가 Workfront으로 이메일을 보낼 때 다음 상황이 발생합니다.

* 이메일의 제목 줄이 문제 이름이 됩니다.
* 이메일의 본문이 문제에 대한 설명이 됩니다.
* 이메일에 첨부된 문서가 있는 경우 해당 문서는 Workfront의 문제에 첨부됩니다.
* 이메일을 보내는 사용자가 Workfront에서 새 문제에 대한 기본 담당자가 됩니다.
* 이메일의 본문은 4,000자를 초과할 수 없습니다.
* 이메일 첨부 파일은 총 7MB를 초과할 수 없습니다.
