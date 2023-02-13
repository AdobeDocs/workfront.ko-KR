---
product-area: requests
navigation-topic: create-requests
title: 초안에서 요청 만들기
description: 새 요청을 입력할 때 Workfront에서 제안하는 사용 가능한 초안을 사용하는 것 외에도 초안 섹션에서 초안 요청에 액세스하여 여기에서 제출을 완료할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 2%

---

# 초안에서 요청 만들기

새 요청을 입력할 때 Workfront에서 제안하는 사용 가능한 초안을 사용하는 것 외에도 초안 섹션에서 초안 요청에 액세스하여 여기에서 제출을 완료할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 초안에서 요청을 만들기 위한 사전 요구 사항

초안에서 요청을 만들려면 먼저 다음을 수행해야 합니다. 

* 요청 만들기를 시작합니다. 이렇게 하면 요청이 초안 섹션에 자동으로 초안으로 저장됩니다.

   요청 만들기에 대한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).

## 초안에서 요청 만들기

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 상단 모서리에서
1. 클릭 **요청** > **초안**.

   각 요청 큐의 각 큐 항목에 대한 초안이 이 목록에 표시됩니다.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. 초안 목록의 다음 열에서 각 초안에 대한 정보를 검토합니다.

   | 주제 | 요청을 만들 때 지정한 이름입니다. |
   |---|---|
   | 경로 | 원래 요청을 제출하려는 요청 큐, 항목 그룹 및 큐 항목의 이름입니다. |
   | 시작 날짜 | 요청 만들기를 시작한 날짜입니다. |
   | 마지막 업데이트 날짜 | 마지막 업데이트. 요청을 처음 시작한 후 업데이트하지 않은 경우 입력 날짜 및 마지막 업데이트 날짜가 같아야 합니다. |

   {style=&quot;table-layout:auto&quot;}

1. (선택 사항) **요청 유형별 필터링** 초안 목록의 오른쪽 위 모서리에서 표시할 초안이 포함된 요청 큐를 선택합니다.
1. 초안의 이름을 클릭하여 엽니다.
1. 에 설명된 대로 요청에 대한 정보를 업데이트합니다. [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (선택 사항 및 조건부) 요청을 입력하는 동안 언제든지 **삭제** 초안을 삭제하려면 초안입니다. 이렇게 하면 복구할 수 없는 초안이 삭제됩니다. 초안 삭제에 대한 자세한 내용은 [요청 초안 삭제](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (선택 사항) **취소** 작업을 되돌리고 초안을 유지하려면 페이지의 왼쪽 아래 모서리에 있는 을 클릭합니다.

1. 요청에 대한 정보를 완료한 후 다음 중 하나를 수행합니다.

   * 클릭 **제출** 요청을 제출할 준비가 된 경우. 요청이 제출됨 섹션에 저장됩니다. 요청 큐의 라우팅 규칙에 따라 이 요청은 요청 큐로 지정된 프로젝트가 아닌 다른 프로젝트로 라우팅될 수 있습니다. 라우팅 규칙에 대한 자세한 내용은 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      또는

      클릭 **닫기** 아직 제출할 준비가 되지 않았는데 나중에 다시 와서 완료할 수 있습니다. 요청은 초안 섹션에 저장되며, 다음에 이 요청 큐에 대한 요청을 제출할 때 사용할 수 있습니다.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

      요청을 제출하면 초안이 삭제되고 복원할 수 없습니다.
