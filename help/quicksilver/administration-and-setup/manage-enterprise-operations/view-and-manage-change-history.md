---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 변경 기록
description: 변경 기록을 사용하면 Workfront 객체에 대한 변경 사항 로그를 볼 수 있습니다.
author: Lisa and Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c58c4365016f8fe855003cdbbd457f95483d08bc
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 4%

---

# 변경 내역 보기 및 관리

설정의 변경 추적 영역에서 감사 로그를 포함한 변경 내역을 볼 수 있습니다.

* **감사 로그**&#x200B;는 사용자가 트리거한 변경 사항입니다.감사 로그 및 감사 로그 영역에 대한 자세한 내용은 [감사 로그 개요](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)를 참조하십시오.
* **구성**&#x200B;은(는) 변경 내용 목록에 대해 추적 중인 필드를 표시합니다.구성은 현재 정보로만 사용할 수 있으며 변경할 수 없습니다. 추적되는 필드를 변경할 수 있는 기능은 가까운 시일 내에 제공될 예정입니다.
* 변경 내역 목록을 사용하면 다음과 같은 속성을 포함하여 Workfront 객체에 대한 변경 사항 로그를 볼 수 있습니다.

   * 오브젝트
   * 오브젝트 유형
   * 변경 유형(작업)
   * 특정 사용자, API, Workfront Fusion, AI LLM 또는 Workfront 시스템과 같은 변경 사항의 Source

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>변경 기록을 보려면 Workfront 관리자여야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 감사 로그 보기 및 관리

감사 로그를 보고 관리하려면 [감사 로그 보기 및 내보내기](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)를 참조하세요.

## 변경 내용 추적을 위한 구성 영역 보기

>[!NOTE]
>
>구성은 현재 정보로만 사용할 수 있으며 변경할 수 없습니다. 추적되는 필드를 변경할 수 있는 기능은 가까운 시일 내에 제공될 예정입니다.

추적되는 변경 유형을 보려면 다음과 같이 하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적** ![변경 내용 아이콘](assets/change-history-icon.png)을 클릭합니다.
1. **구성**&#x200B;을 클릭합니다.

   필드는 오브젝트 유형별로 그룹화되어 표시됩니다.

1. 특정 개체 아래에 필드를 표시하려면 개체 유형 옆에 있는 드롭다운 화살표를 클릭합니다.

## 변경 내역 목록 보기

Workfront 관리자는 설정 영역에서 변경 내용을 볼 수 있습니다.

변경 내용 목록은 향상된 목록이며 필터, 열, 행 높이, 날짜 선택기 및 검색 막대를 제공합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적** ![변경 내용 아이콘](assets/change-history-icon.png)을 클릭합니다.
1. **변경 목록**&#x200B;을 클릭합니다.

   변경 기록 목록이 열립니다.

1. 변경 내용이 표시되는 날짜를 조정하려면 날짜 선택기를 클릭하고 새 날짜를 선택합니다.

   지난 90일 동안 변경 사항을 사용할 수 있습니다.
1. 특정 용어를 검색하려면 검색 창을 클릭하고 용어를 입력합니다. 입력한 대로 결과가 필터링됩니다.
1. (선택 사항) 열을 기준으로 필터링하려면 향상된 목록 사용 문서에서 [향상된 목록의 항목 필터링](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list)을 참조하십시오.
1. (선택 사항) 열을 숨기거나 표시하거나 순서를 바꾸려면 향상 목록 사용 문서에서 [열 사용자 지정](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns)을(를) 참조하십시오.
1. 열을 추가하거나 제거하려면 향상된 목록 사용 문서에서 [열 관리자로 열 추가 및 제거](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)를 참조하십시오.
1. 행 높이를 조정하려면 향상된 목록 사용 문서에서 [보기에서 행 높이 변경](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view)을 참조하십시오.





