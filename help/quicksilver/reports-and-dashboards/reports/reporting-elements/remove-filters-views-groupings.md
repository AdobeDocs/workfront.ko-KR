---
product-area: reporting
navigation-topic: reporting-elements
title: 필터, 보기 및 그룹화 제거
description: 목록 및 보고서를 만들었거나 사용자와 공유한 경우, 목록 및 보고서에서 필터, 보기 또는 그룹화를 제거할 수 있습니다. 기본 필터, 보기 또는 그룹화는 제거할 수 없습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 1%

---

# 필터, 보기 및 그룹화 제거

<!-- Audited: 11/2024 -->

목록 및 보고서를 만들었거나 사용자와 공유한 경우, 목록 및 보고서에서 필터, 보기 또는 그룹화를 제거할 수 있습니다. 기본 필터, 보기 또는 그룹화는 제거할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> 
      <p>신규:</p>
         <ul>
         <li><p>기여자 이상</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>요청 이상</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td><p>필터, 보기, 그룹화에 대한 보기 또는 상위 액세스</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td><p>제거할 필터, 보기 또는 그룹화에 대한 공유 액세스 권한이 있는 권한 보기</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 표준 빌더를 사용하여 필터 제거 또는 삭제

표준 빌더 인터페이스를 사용하여 프로젝트, 작업 또는 문제 목록에서 사용자와 공유된 필터를 제거할 수 있습니다. 표준 빌더 인터페이스는 다른 개체, 보기 또는 그룹화에는 사용할 수 없습니다.

표준 빌더 인터페이스를 사용하여 프로젝트, 작업 또는 문제 목록에서 소유한 필터를 삭제할 수도 있습니다.

시스템 기본 필터는 제거하거나 삭제할 수 없습니다.

### 표준 빌더를 사용하여 필터 제거 또는 삭제에 대한 고려 사항

표준 빌더를 사용하여 필터를 제거하거나 삭제하는 시나리오는 다음과 같습니다.

* 필터를 공유한 후 제거한 경우 해당 필터는 귀하만 제거됩니다. 원래 필터를 만든 사용자와 공유한 다른 사용자는 필터에 계속 액세스할 수 있습니다.
* 필터를 소유하고 있는데 삭제하면 Workfront 시스템에서 필터가 제거됩니다. 이전에 공유한 사용자는 필터를 더 이상 사용할 수 없습니다.
* Workfront 관리자인 경우 필터를 삭제할 수 있으며 소유자를 포함한 모든 사용자에 대해 필터가 영구적으로 삭제됩니다.

### 표준 빌더를 사용하여 필터 제거

1. 프로젝트, 작업, 문제, 포트폴리오, 프로그램, 사용자, 템플릿 또는 그룹 목록으로 이동합니다.
1. **필터** 아이콘 ![필터 아이콘](assets/filter-nwepng.png)을 클릭합니다.
1. **나와 공유** 아래의 필터에 마우스를 가져다 대고 **자세히** 메뉴 ![기타 아이콘](assets/more-icon-spectrum.png)을 클릭한 다음 **제거**&#x200B;를 클릭합니다.
1. 필터를 영구적으로 제거하려면 확인 메시지에서 **제거**&#x200B;를 선택합니다.

### 표준 빌더를 사용하여 필터 삭제

1. 프로젝트, 작업, 문제, 포트폴리오, 프로그램, 사용자, 템플릿 또는 그룹 목록으로 이동합니다.
1. **필터** 아이콘 ![필터 아이콘](assets/filter-nwepng.png)을 클릭합니다.
1. 삭제할 권한이 있는 필터에 마우스를 가져다 대고 **자세히** 메뉴 ![추가 아이콘](assets/more-icon-spectrum.png)을 클릭한 다음 **삭제**&#x200B;를 클릭합니다.

   ![필터 삭제](assets/new-filters-more-menu-options-with-delete.png)

1. (선택 사항) 삭제를 방지하고 필터 목록으로 돌아가려면 확인 메시지에서 **취소**&#x200B;를 클릭합니다.
1. 삭제를 확인하려면 확인 메시지에서 **삭제**&#x200B;을(를) 클릭합니다.

   사용자 및 이 필터에 대한 권한이 있는 모든 사용자에 대해 필터가 삭제됩니다.

## 기존 빌더를 사용하여 필터, 보기 또는 그룹화 제거

기존 빌더 인터페이스를 사용하여 모든 객체 목록에 대한 필터, 보기 또는 그룹화를 제거할 수 있습니다.

### 기존 빌더를 사용하여 필터, 보기 및 그룹화 제거에 대한 고려 사항

보고 요소를 제거하는 방법은 처음에 보고 요소를 만들었는지 아니면 사용자와 공유했는지 여부에 따라 다릅니다.

필터, 보기 또는 그룹화를 제거할 때 다음과 같은 시나리오가 있습니다.

* **요소를 만들어 제거한 경우** 요소가 Workfront 시스템에서 제거됩니다. 이전에 공유한 사용자는 더 이상 사용할 수 없습니다.
* **요소가 귀하와 공유되어 제거되었으면** 해당 요소는 귀하만을 위해 제거됩니다. 처음 만든 사용자와 공유한 다른 모든 사용자는 여전히 액세스할 수 있습니다.

### 기존 빌더를 사용하여 필터, 보기 또는 그룹화 제거

1. 객체 목록 또는 보고서로 이동합니다.
1. (조건부) 목록에서 **필터**, **보기** 또는 **그룹화** 아이콘을 클릭한 다음 제거할 필터, 보기 또는 그룹화 위로 마우스를 가져간 다음 **자세히** 아이콘 ![기타 아이콘](assets/more-icon.png), **제거**&#x200B;를 클릭합니다. 필터, 보기 또는 그룹화가 제거됩니다.
1. (조건부) 보고서에서 **그룹화**, **필터** 또는 **보기** 드롭다운 메뉴를 클릭하고 **그룹화 제거**, **필터 제거** 또는 **보기 제거**&#x200B;를 선택합니다.

   **내 그룹화**, **내 필터,** 또는 **내 보기** 대화 상자가 표시됩니다.

   제거할 권한이 있는 모든 보고 요소를 제거할 수 있습니다. 다른 보고 요소는 흐리게 표시됩니다.

1. 제거할 보고 요소 옆의 **x** 아이콘을 클릭합니다.
1. (조건부) 자신이 만들었다가 나중에 다른 사람과 공유한 필터, 보기 또는 그룹화를 삭제하려면 **예, 삭제**&#x200B;를 클릭합니다. 이렇게 하면 Workfront 시스템에서 필터, 보기 또는 그룹화가 삭제됩니다.

   >[!TIP]
   >
   >다른 사용자와 공유하지 않고 만든 필터, 보기 또는 그룹화를 제거하면 확인을 요구하지 않고 시스템에서 제거됩니다.

1. **완료**&#x200B;를 클릭합니다.

