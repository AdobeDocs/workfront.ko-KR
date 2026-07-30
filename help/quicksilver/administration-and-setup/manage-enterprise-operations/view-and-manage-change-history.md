---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 변경 기록
description: 변경 기록을 사용하면 Workfront 객체에 대한 변경 사항 로그를 볼 수 있습니다
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: de1f426630b8c99cfaca07dafb9c2de0f16f263f
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 2%

---

# 변경 내역 보기 및 관리

{{preview-fast-release-general}}

설정의 변경 추적 영역에서 감사 로그를 포함한 변경 내역을 볼 수 있습니다.

* **감사 로그**&#x200B;는 사용자가 트리거한 변경 사항입니다.
감사 로그 및 감사 로그 영역에 대한 자세한 내용은 [감사 로그 개요](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md) 및 [감사 로그 보기 및 내보내기](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)를 참조하십시오.
* **구성**&#x200B;은(는) 변경 내용 목록에 대해 추적 중인 필드를 표시합니다.
  <span class="preview">Workfront 관리자는 Workfront에서 추적하는 개체 필드와 작업을 구성할 수 있습니다. 예를 들어 Workfront에서 사용자가 시스템 전체에서 문제 이름에 적용한 모든 변경 사항을 추적할 수 있습니다. 문제 이름이 변경되면 변경 기록 로그에 항목으로 나타납니다.</span>

* **변경 기록 목록**&#x200B;을 통해 다음과 같은 특성을 포함하여 Workfront 개체에 대한 변경 사항 로그를 볼 수 있습니다.

  * 오브젝트
  * 오브젝트 유형
  * 변경 유형(작업)
  * 특정 사용자, API, Workfront Fusion, AI LLM 또는 Workfront 시스템과 같은 변경 사항의 Source

  <span class="preview">통합 검토 및 승인 워크플로 활동은 참가자 및 의사 결정을 포함하여 변경 내역에서 추적됩니다.</span>

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
   <td><p>시스템 관리자</p>
       <p><span class="preview">변경 내역을 조회하려면 변경 내역에 대한 관리 액세스</span></p>
       <p><span class="preview">추적된 필드를 구성하려면: 시스템 관리자</span></p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<div class="preview">

## 추적할 필드 추가

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 > 구성**&#x200B;을 클릭합니다.
1. 구성 화면에서 **필드 추가**&#x200B;를 클릭합니다.
1. **필드 추가** 상자에서 개체를 선택합니다. 개체 이름을 입력한 다음 목록에 표시될 때 선택할 수 있습니다.
1. 그런 다음 해당 객체에 대해 추적할 필드 이름을 선택합니다. 필드 이름을 입력한 다음 목록에 나타날 때 필드 이름을 선택할 수 있습니다.

   사용자 정의 필드와 기본 필드는 모두 오브젝트에 사용할 수 있습니다.
   이미 추적 중인 필드가 목록에서 선택된 상태로 표시됩니다.

   ![변경 내용 추적을 위한 필드 추가](assets/change-history-config-add-fields.png)

1. 추적할 모든 필드를 선택한 후 **추가**&#x200B;를 클릭합니다.

   필드가 추적된 필드 목록에 추가됩니다.

## 더 이상 추적하지 않을 필드 제거

Workfront 인터페이스 전체에서 특정 유형의 개체에 대해 시스템에서 추적하지 않으려는 필드를 제거할 수 있습니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 > 구성**&#x200B;을 클릭합니다.
1. 구성 화면에서 추적을 중지할 필드를 선택합니다.

   동일한 필드 이름이 두 번 이상 표시될 수 있습니다. 필드는 정확한 필드를 찾을 수 있도록 오브젝트별로 그룹화됩니다. 화면 상단의 검색 상자를 사용할 수도 있습니다.

1. 화면 하단의 작업 표시줄에서 **삭제**&#x200B;를 선택합니다.
1. 확인 메시지에서 **제거**&#x200B;를 클릭합니다.

   필드는 추적된 필드 목록에서 제거됩니다.

</div>

## 변경 내용 추적을 위한 구성 영역 보기

>[!NOTE]
>
>프로덕션 환경에서 구성은 현재 정보로만 사용할 수 있으며 변경할 수 없습니다. 추적되는 필드를 변경할 수 있는 기능은 가까운 시일 내에 제공될 예정입니다.

추적되는 변경 유형을 보려면 다음과 같이 하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 >**&#x200B;구성**을 클릭합니다.

   필드는 오브젝트 유형별로 그룹화되어 표시됩니다.

1. 특정 개체 아래에 필드를 표시하려면 개체 유형 옆에 있는 드롭다운 화살표를 클릭합니다.

## 변경 내역 목록 보기

Workfront 관리자는 설정 영역에서 변경 내용을 볼 수 있습니다.

변경 내용 목록은 향상된 목록이며 필터, 열, 행 높이, 날짜 선택기 및 검색 막대를 제공합니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **변경 내용 추적 > 변경 내용 목록**&#x200B;을 클릭합니다.

   변경 기록 목록이 열립니다.

1. 변경 내용이 표시되는 날짜를 조정하려면 날짜 선택기를 클릭하고 새 날짜를 선택합니다.

   지난 90일 동안 변경 사항을 사용할 수 있습니다.

1. 특정 용어를 검색하려면 검색 창을 클릭하고 용어를 입력합니다. 입력할 때 목록에 결과가 강조 표시됩니다.
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



