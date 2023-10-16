---
title: 레코드 편집
description: Adobe 마에스트로에서 레코드 정보를 편집할 수 있습니다. 레코드 만들기 및 편집을 시작하려면 먼저 레코드 유형을 만들어야 합니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 4895a85084c1554cfd773cf51ea0c922f7701414
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 2%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 레코드 편집

>[!IMPORTANT]
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe 마에스트로에서 레코드 정보를 편집할 수 있습니다. 레코드 만들기 및 편집을 시작하려면 먼저 레코드 유형을 만들어야 합니다.
자세한 내용은 [레코드 유형 만들기](../architecture-and-fields/create-record-types.md).

&lt;!— 여기에서 세부 사항 보기의 필드가 표 보기의 필드와 동일하다고 언급하십시오. 이 문서는 레코드 관리 보기에서 연결되어 이 정보를 참조합니다—>

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

## 레코드 편집에 대한 고려 사항

* 사용자 또는 다른 사용자가 만든 레코드를 편집할 수 있습니다. <!--will change with access levels-->
* 다른 레코드에서 연결된 필드나 계산이 들어 있는 필드는 편집할 수 없습니다.
* 표시되는 레코드가 다른 레코드에 연결되어 있는 경우 편집 중인 레코드의 새 정보가 연결된 레코드에 반영됩니다.
* 레코드를 일괄적으로 편집할 수 없습니다. <!--this will probably change-->
* URL은 http://, https://, ftp:// 또는 www로 시작하는 경우에만 한 줄 텍스트 필드 유형에서 링크로 인식됩니다. .
* 단락 유형 필드를 편집할 때 다음과 같은 서식 있는 텍스트 서식 옵션을 사용할 수 있습니다.

   * 볼드체
   * 이탤릭체
   * 밑줄
   * 링크 추가
   * 글머리 기호 목록 추가
   * 번호 매기기 목록 추가

## 레코드 편집

다음 영역에서 레코드를 편집할 수 있습니다.

* [레코드의 세부 정보 페이지에서](#edit-a-record-from-the-records-details-page)
* [레코드 유형의 테이블 보기에서](#edit-a-record-from-the-record-type-table-view)

### 레코드의 세부 정보 페이지에서 레코드 편집

1. 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-workfront.png) 오른쪽 상단 또는 **메인 메뉴** ![](assets/main-menu-shell.png) 왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **마에스트로**.

   마지막으로 액세스한 작업공간이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.
1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름을 클릭합니다.
   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **보기**

     ![](assets/contextual-menu-for-record-row.png)
   * 타임라인 보기에서 레코드 모음을 클릭합니다.

   레코드 **세부 사항** 페이지가 열립니다.

1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png) 레코드 이름 오른쪽에서 **편집**

   또는

   세부 정보 페이지의 편집 가능한 필드 내부를 클릭하여 정보를 편집합니다.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. 클릭 **변경 내용 저장**. <!--logged a bug for this - this needs to be "Save"-->

### 레코드 유형 테이블 보기에서 레코드 편집

1. 다음을 클릭합니다. **메인 메뉴** ![](assets/main-menu-workfront.png) 오른쪽 위 모서리에서 <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it is available,--> 그런 다음 을 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.
1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. (조건부) **보기** 테이블 오른쪽 위 모서리에서 드롭다운 메뉴를 사용하여 테이블 뷰를 선택합니다. 레코드 유형에 마지막으로 액세스했을 때 타임라인 보기에서 확인하지 않은 경우 기본 보기여야 합니다.

   선택한 레코드 유형과 연관된 레코드가 테이블 뷰에 표시됩니다.
1. 레코드 행 내부를 클릭하여 인라인 레코드에 대한 정보 편집을 시작합니다.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. 누르기 **입력** 키보드에서 를 클릭하거나 행 외부를 클릭하여 변경 내용을 저장합니다. 변경 사항은 자동으로 저장됩니다.