---
product-area: requests
navigation-topic: create-requests
title: 제출된 요청 재요청 초안 삭제
description: 제출된 요청이나 요청 초안을 삭제할 수 있습니다.
author: Becky
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 3%

---

# 제출된 요청 또는 요청 초안 삭제

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리 보기 환경이나 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서만 사용할 수 있습니다.</span>

제출된 요청이나 새 요청 경험에서 만든 요청 초안을 삭제할 수 있습니다. Workfront 관리자 및 Planning 작업 영역 관리자는 요청을 삭제할 수도 있습니다.

기존 요청 경험에서 요청 초안을 삭제할 수 있습니다. 제출된 요청은 삭제할 수 없습니다.

자세한 내용은 다음을 참조하십시오.

* [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [초안에서 요청 만들기](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>생성하지 않은 요청을 삭제하려면 Workfront 관리자 또는 Planning 작업 공간 관리자여야 합니다.</p><p>기존 요청 경험에서 초안을 삭제하려면 문제에 대한 편집 액세스 권한이 있어야 합니다.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>새 요청 경험에서 삭제하려면 요청 또는 초안을 만들어야 합니다.</p><p>기존 요청 경험에서 초안을 삭제하려면 문제에 대한 편집 액세스 권한이 있어야 합니다.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 제품</td> 
   <td> <ul><li>Adobe Workfront</li><li>Planning 요청 또는 요청 양식을 보려면 Adobe Workfront Planning이 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


<div class="preview">

## 새 요청 경험에서 <!--or request drafts --> 요청을 삭제합니다.

Workfront의 요청 영역이나 홈의 내 요청 위젯에서 요청을 삭제할 수 있습니다.

* Workfront 관리자는 조직의 <!-- and drafts--> 요청을 삭제할 수 있습니다.
* Workfront Planning 작업 영역 관리자는 자신이 관리하는 Planning 작업 영역에서 <!--and drafts--> 요청을 삭제할 수 있습니다.
* 사용자가 제출한 <!--and drafts--> 요청을 삭제할 수 있습니다.

### 점 3개 메뉴에서 요청 삭제

{{step1-to-requests}}

1. 홈에서 내 요청 위젯에 액세스하려면 다음을 수행하십시오.

   {{step1-to-home}}

   1. 내 요청 위젯을 찾습니다.

      내 요청 위젯에 대한 자세한 내용은 [내 요청 위젯 사용](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)을 참조하십시오.

1. 요청 목록 또는 내 요청 위젯에서 삭제할 요청 <!--or draft -->을(를) 마우스로 가리킵니다.

   3점 추가 메뉴가 나타납니다.
   ![](assets/more-menu.png)

1. 요청 **이름 오른쪽에 있는**&#x200B;자세히<!--or draft--> 메뉴를 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   또는

   선택한 요청을 마우스 오른쪽 단추로 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   >[!TIP]
   >
   >문제를 만들 수 있는 액세스 권한이 없는 경우 관리자가 요청 만들기를 제한했다는 경고가 표시됩니다.

1. 대화 상자가 열리면 **삭제**&#x200B;를 클릭합니다.

   <!--or draft--> 요청이 삭제되었습니다.

### 대량 삭제 요청

{{step1-to-requests}}

1. 홈에서 내 요청 위젯에 액세스하려면 다음을 수행하십시오.

   {{step1-to-home}}

   1. 내 요청 위젯을 찾습니다.

      내 요청 위젯에 대한 자세한 내용은 [내 요청 위젯 사용](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)을 참조하십시오.

1. 요청 목록 또는 내 요청 위젯에서 삭제할 각 요청의 왼쪽에 있는 상자를 클릭합니다.
1. 페이지 하단의 파란색 막대에서 **삭제**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >파란색 막대에 삭제 옵션이 표시되지 않으면 선택한 요청 중 하나 이상을 삭제할 권한이 없습니다.

</div>

## 기존 요청 경험에서 요청 초안 삭제

더 이상 관련이 없는 경우 초안으로 저장된 후 초안을 삭제할 수 있습니다. 삭제된 초안 요청은 복구할 수 없습니다.

### 요청 초안 삭제 사전 요구 사항

요청 초안을 삭제하려면 먼저 다음 작업을 수행해야 합니다.

* 요청 만들기를 시작합니다. 초안 섹션에 요청이 자동으로 초안으로 저장됩니다.

  요청 만들기에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md)을 참조하십시오.

### 요청 초안 삭제

{{step1-to-requests}}

1. 왼쪽 패널에서 **초안**&#x200B;을 선택합니다.

   모든 요청 대기열의 모든 초안이 이 목록에 표시됩니다.

1. (선택 사항) 초안 목록의 오른쪽 상단 모서리에서 **요청 유형별로 필터링**&#x200B;을 클릭한 다음, 표시할 초안이 포함된 요청 큐를 선택하십시오.
1. 목록에서 초안을 선택한 다음 목록의 맨 위에서 **삭제**&#x200B;를 클릭합니다.
1. **예, 삭제**&#x200B;를 클릭합니다.

   초안이 삭제되어 복구할 수 없습니다.
