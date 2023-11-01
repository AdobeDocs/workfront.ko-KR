---
title: 레코드 삭제
description: 사용자 또는 다른 사용자가 만든 레코드를 삭제할 수 있습니다. 삭제된 레코드는 복구할 수 없습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 1dcc267f04242782efea4a219410380ca5a01e1d
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# 레코드 삭제

>[!IMPORTANT]
>이 문서의 정보는 Adobe의 새로운 서비스인 Adobe 마에스트로를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe 마에스트로에서 더 이상 관련되지 않는 레코드를 삭제할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>모든</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>모든</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">액세스 수준</td>
   <td> <p>모든</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/grant-access.md">Adobe 마에스트로에 대한 액세스 권한 부여</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 레코드 삭제에 대한 고려 사항

* 사용자 또는 다른 사용자가 만든 레코드를 삭제할 수 있습니다.
* 삭제된 레코드는 복구할 수 없습니다. <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 삭제된 레코드가 다른 레코드와 연결된 경우 연결된 레코드는 삭제되지 않지만 삭제된 레코드의 정보도 삭제됩니다.
* 레코드를 일괄적으로 삭제할 수 없습니다. <!--this will probably change-->
* 타임라인 보기에서 레코드를 삭제할 수 없습니다.
* 다른 애플리케이션에서 연결된 레코드 유형은 삭제할 수 없습니다. 예를 들어 Maestro 레코드를 Workfront 객체에 연결하는 경우 Workfront 객체 레코드 페이지에서 Workfront 객체를 삭제할 수 없습니다.

## 레코드 삭제

다음 영역에서 레코드를 삭제할 수 있습니다.

* [레코드의 세부 정보 페이지에서](#delete-a-record-from-the-records-details-page)
* [레코드 유형의 테이블 보기에서](#delete-a-record-from-the-record-type-table-view)

### 레코드의 세부 정보 페이지에서 레코드 삭제

1. 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-workfront.png) 오른쪽 상단 또는 **메인 메뉴** ![](assets/main-menu-shell.png) 왼쪽 상단 모서리에서 사용 가능한 경우 Maestro 를 클릭합니다.

   마지막으로 액세스한 작업공간이 열립니다.
1. 레코드 유형을 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름을 클릭합니다.
   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **보기**

     ![](assets/contextual-menu-for-record-row.png)
   * 타임라인 보기에서 레코드 모음을 클릭합니다.

   레코드 **세부 사항** 페이지가 열립니다.

1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png) 레코드 이름 오른쪽에서 **삭제**, 그런 다음 **삭제** 다시 한 번 확인해 보십시오.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
레코드가 삭제되어 복구할 수 없습니다.

### 레코드 유형 테이블 보기에서 레코드 삭제

1. 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-workfront.png) 오른쪽 상단 또는 **메인 메뉴** ![](assets/main-menu-shell.png) 왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **마에스트로**.

   마지막으로 액세스한 작업 영역이 열립니다.
1. 레코드 유형을 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. (조건부) **보기** 테이블 오른쪽 위 모서리에서 드롭다운 메뉴를 사용하여 테이블 뷰를 선택합니다. 레코드 유형에 마지막으로 액세스했을 때 타임라인 보기에서 확인하지 않은 경우 기본 보기여야 합니다.

   선택한 레코드 유형과 연관된 레코드가 테이블 뷰에 표시됩니다.
1. 레코드 행을 마우스 오른쪽 단추로 클릭한 다음 **삭제**.

   ![](assets/contextual-menu-for-record-row.png)

   레코드가 삭제되어 복구할 수 없습니다.
