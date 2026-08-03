---
user-type: administrator
product-area: system-administration;setup
title: 변경 내역 보기 및 관리
description: 변경 기록을 사용하면 Workfront 오브젝트 및 필드에 대한 변경 사항 로그를 볼 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 100b900bd7419d78a3135358026ec5e27755fdeb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 3%

---

# 변경 내역 보기 및 관리

{{preview-fast-release-general}}

변경 기록을 사용하면 Adobe Workfront의 오브젝트 및 특정 필드에 대한 변경 사항을 구성하고 추적할 수 있습니다. 유연한 구성을 통해 추적할 오브젝트 및 필드를 설정할 수 있습니다.

변경 기록은 사용자가 정의하는 다음 유형의 데이터를 추적할 수 있습니다.

* 액세스 수준 또는 작업 역할 생성 또는 삭제와 같은 설정 영역의 활동
* 프로젝트 설명 편집 또는 사용자의 레이아웃 템플릿 변경과 같은 필드 수준 업데이트
* 프로젝트 상태 업데이트 또는 사용자 정의 양식을 작업에 첨부하는 등의 오브젝트 업데이트
* <span class="preview">참가자 및 결정을 포함한 통합 검토 및 승인 워크플로 활동</span>

추적할 개체 및 필드를 정의하는 방법에 대한 자세한 내용은 [변경 내역에서 추적할 필드 구성](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md)을 참조하십시오.

변경 내역 목록에서 다음과 같은 속성을 포함하여 Workfront 객체에 대한 변경 로그를 볼 수 있습니다.

* 오브젝트 이름
* 오브젝트 유형
* 변경 유형(작업)
* 변경 날짜 및 시간
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
   <td><span class="preview">변경 기록에 대한 관리 액세스</span></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--
## View the Configuration area for change tracking

>[!NOTE]
>
>In the Production environment, Configuration is currently available only as information and cannot be changed. The ability to change which fields are tracked will be available in the near future.

To view the types of changes that are tracked: 

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
   
   Fields are displayed grouped by object type.

1. To display fields under a specific object, click the dropdown arrow next to the object type.
-->


## 변경 내역 목록 보기

설정 영역에서 변경 내용 로그를 볼 수 있습니다.

변경 내용 목록은 향상된 목록이며 필터, 열, 행 높이, 날짜 선택기 및 검색 막대를 제공합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 > 변경 내용 목록**&#x200B;을 클릭합니다.

   변경 기록 목록이 열립니다.

1. 변경 내용이 표시되는 날짜를 조정하려면 날짜 선택기를 클릭하고 새 날짜를 선택합니다.

   지난 90일 동안 변경 사항을 사용할 수 있습니다.

1. 특정 용어를 검색하려면 검색 상자를 클릭하고 용어를 입력합니다. 입력할 때 목록에 결과가 강조 표시됩니다.
1. (선택 사항) 열을 기준으로 필터링하려면 문서 [고급 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)에서 [고급 목록의 항목 필터링](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list)을 참조하십시오.
1. (선택 사항) 열을 숨기거나 표시하거나 순서를 바꾸려면 문서 [고급 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)에서 [열 사용자 지정](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns)을(를) 참조하십시오.
1. (선택 사항)열을 추가하거나 제거하려면 [고급 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md) 문서에서 [열 관리자로 열 추가 및 제거](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)를 참조하십시오.
1. (선택 사항) 행 높이를 조정하려면 문서 [고급 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)에서 [보기에서 행 높이 변경](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view)을 참조하십시오.

## 변경 내역 내보내기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 > 변경 내용 목록**&#x200B;을 클릭합니다.
1. 목록을 필터링하여 내보낼 항목을 표시합니다.
1. **내보내기** 아이콘 ![내보내기 아이콘](assets/export-icon.png)을 클릭하고 XLSX 또는 CSV 형식으로 저장할지 여부를 선택합니다.

   파일 저장 상자가 열리고 내보낸 파일을 컴퓨터에 저장할 수 있습니다.
   내보낸 파일 저장을 완료합니다. 이제 컴퓨터에서 찾아 다른 사용자와 공유할 수 있습니다.



