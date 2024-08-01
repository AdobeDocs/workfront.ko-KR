---
title: 중복 레코드
description: 테이블 보기에서 기존 레코드를 복제할 수 있습니다. 기존 레코드의 동일한 복사본이 레코드 유형 페이지에 추가됩니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---


# 중복 레코드

<!--update the metadata after GA-->

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드는 레코드 유형의 인스턴스입니다.

테이블 보기에서 기존 레코드를 복제할 수 있습니다. 기존 레코드의 동일한 복사본이 레코드 유형 페이지에 추가됩니다.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Workfront Planning의 조기 액세스 단계에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>새로운 기능: 표준</p>
   <p>현재: 플랜</p>  
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 제어가 없습니다. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역에 대한 Contribute 이상의 권한</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>를 참조하십시오. </p>  
</td>
  </tr>

</tbody>
</table>

*자세한 내용은 [Workfront 설명서에 대한 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## <!--in a record type table (I don't think you can create them elsewhere right now)--> 레코드 복제

기존 레코드를 복제하여 레코드 유형 페이지의 표 보기에서 레코드를 만들 수 있습니다. 기존 레코드와 동일한 레코드가 생성되어 원본 레코드 아래에 추가됩니다.


{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.
선택한 유형의 모든 레코드가 뷰에 표시됩니다.

1. (조건부) 테이블 뷰를 선택합니다.

1. 다음 중 하나를 수행하십시오.

   * 레코드 이름 위로 마우스를 가져간 다음 레코드 이름과 인라인으로 **자세히** 메뉴를 클릭한 다음 **복제** 아이콘 ![](assets/duplicate-icon-gray.png) 을 클릭합니다.

     ![](assets/more-menu-from-record-in-table-view.png)

   * 레코드를 선택한 다음 페이지 아래쪽에 있는 도구 모음에서 **복제** 아이콘 ![](assets/duplicate-icon-white-and-blue.png)을(를) 클릭합니다.

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   원래 레코드 아래에 이름이 같은 동일한 레코드가 만들어집니다. 새 레코드의 모든 필드는 원래 레코드와 동일한 정보로 채워집니다.

1. (선택 사항) 테이블 보기에서 사용할 수 있는 필드에서 새 레코드에 대한 정보 업데이트를 시작하거나 레코드 미리 보기 또는 페이지에서 레코드 및 업데이트 정보를 클릭합니다.

   >[!NOTE]
   >
   >  * 레코드에 대한 필수 필드가 없습니다. 그러나 레코드를 서로 연결할 때 레코드를 식별하는 데 도움이 되므로 레코드의 기본 필드에 대한 정보를 추가하는 것이 좋습니다. 기본 필드에 대한 자세한 내용은 [테이블 보기 관리](/help/quicksilver/planning/views/manage-the-table-view.md) 및 [기본 필드 개요](/help/quicksilver/planning/fields/primary-field-overview.md)를 참조하십시오.
   >
   >  * 다른 레코드 종류 또는 계산된 필드를 참조하는 필드는 읽기 전용 필드입니다.

   레코드 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

1. (선택 사항) 다음 키보드 단축키를 사용하여 표 보기에서 새 레코드 또는 해당 정보를 추가할 때 해당 추가 작업을 취소하거나 다시 실행합니다.

   * CTRL+Z(Mac의 경우 ⌘+Z)
   * 변경 내용을 재실행하려면 CTRL+Shift+Z(Mac의 경우 ⌘+Shift+Z)를 누릅니다.