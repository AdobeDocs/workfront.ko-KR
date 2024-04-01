---
title: 레코드 삭제
description: 사용자 또는 다른 사용자가 만든 레코드를 삭제할 수 있습니다. 삭제된 레코드는 복구할 수 없습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 레코드 삭제

{{maestro-important-intro}}

Adobe Workfront Planning에서 더 이상 관련이 없는 레코드를 삭제할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
<p>조직은 Adobe Workfront Planning Beta 프로그램에 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p>
   </td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역에 대한 상위 권한 기여</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 레코드 삭제에 대한 고려 사항

* 사용자 또는 다른 사용자가 만든 레코드를 삭제할 수 있습니다.
* 삭제된 레코드는 복구할 수 없습니다. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 삭제된 레코드가 다른 레코드와 연결된 경우 연결된 레코드는 삭제되지 않지만 삭제된 레코드의 정보도 삭제됩니다.
* 레코드를 일괄적으로 삭제할 수 없습니다. <!--this will probably change-->
* 타임라인 보기에서 레코드를 삭제할 수 없습니다.

## 레코드 삭제

다음 영역에서 레코드를 삭제할 수 있습니다.

* [레코드 페이지에서](#delete-a-record-from-the-records-page)
* [레코드 유형의 테이블 보기에서](#delete-a-record-from-the-record-type-table-view)

### 레코드 페이지에서 레코드 삭제

{{step1-to-maestro}}

마지막으로 액세스한 작업공간이 열립니다.

1. 레코드 유형을 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름을 클릭합니다.
   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **보기**

     ![](assets/contextual-menu-for-record-row.png)
   * 타임라인 보기에서 레코드 모음을 클릭합니다.

   레코드 페이지가 열립니다.

1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png) 레코드 이름 오른쪽에서 **삭제**, 그런 다음 **삭제** 다시 한 번 확인해 보십시오.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
레코드가 삭제되어 복구할 수 없습니다.

### 레코드 유형 테이블 보기에서 레코드 삭제

{{step1-to-maestro}}

마지막으로 액세스한 작업 영역이 열립니다.

1. 레코드 유형을 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. (조건부) **보기** 테이블 왼쪽 위 모서리에 있는 드롭다운 메뉴에서 테이블 뷰를 선택합니다. 레코드 유형에 마지막으로 액세스했을 때 타임라인 보기에서 확인하지 않은 경우 기본 보기여야 합니다.

   선택한 레코드 유형과 연관된 레코드가 테이블 뷰에 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 행을 마우스 오른쪽 단추로 클릭한 다음 **삭제**.
   * 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png) 레코드 이름 오른쪽에서 **삭제**

     ![](assets/contextual-menu-for-record-row.png)

   * 다음을 클릭합니다. **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png) 를 클릭하여 레코드의 세부 정보가 있는 상자를 열고 **자세히** ![](assets/more-menu.png) 레코드 이름의 오른쪽에 있는 경우 **삭제**.

   레코드가 삭제되어 복구할 수 없습니다.

1. (선택 사항) 다음 키보드 단축키를 사용하여 레코드 삭제를 실행 취소하거나 재실행할 수 있습니다.

   * CTRL+Z(Mac의 경우 ⌘+Z)
   * 변경 내용을 재실행하려면 CTRL+Shift+Z(Mac의 경우 ⌘+Shift+Z)
