---
title: 운영 레코드 유형 만들기
description: 레코드 유형은 Adobe 마에스트로의 객체 유형입니다. Maestro에서는 조직의 라이프사이클에 필요한 작업 항목을 설명하는 사용자 정의 레코드 유형을 만들 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: d3c22c84a9b246d1a45853c5d2825241f58bebe9
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# 운영 레코드 유형 만들기

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

레코드 유형은 Adobe 마에스트로의 객체 유형입니다. Maestro에서는 조직의 라이프사이클에 필요한 작업 관련 항목을 설명하는 사용자 정의 레코드 유형을 만들 수 있습니다.

레코드 유형은 다음 중 하나일 수 있습니다.

* **운영 레코드 유형**
* **분류**

Maestro 레코드 유형에 대한 자세한 내용은 [레코드 유형 및 분류 개요](../architecture/overview-of-record-types-and-taxonomies.md).

운영 레코드 유형을 만드는 것은 분류 레코드 유형을 만드는 것과 비슷합니다. 이 문서에서는 작업 레코드 유형을 만드는 방법에 대해 설명합니다.

분류 생성에 대한 자세한 내용은 [분류 레코드 유형 만들기](../architecture/create-a-taxonomy.md).

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

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 레코드 유형 만들기에 대한 고려 사항

* 다음 중 하나를 수행하여 작업 영역에서 레코드 유형을 만들 수 있습니다.

   * 자동:
      * 템플릿을 사용하여 작업 공간을 만드는 경우.

        자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).
      * Excel 또는 CSV 파일을 사용하여 가져올 때. 분류 레코드 유형에는 사용할 수 없습니다.
      * 다른 응용 프로그램에서 개체 유형에 대한 연결을 만들 때 레코드 유형에 필드를 추가할 때 이렇게 하면 원본 응용 프로그램의 개체 유형에 연결된 Maestro에 읽기 전용 레코드 유형이 만들어집니다.

     객체 유형을 Maestro 레코드와 연결하는 방법에 대한 자세한 내용은 [레코드 연결](../records/connect-records.md).
   * 수동:

      * 처음부터.

## 작업 공간 템플릿을 사용하여 레코드 유형 만들기

템플릿을 사용하여 작업 공간을 만들 때 레코드 유형을 자동으로 만들 수 있습니다. 각 Maestro 템플릿에는 샘플 운영 및 분류 레코드 유형이 포함되어 있습니다.

작업 공간 만들기에 대한 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).

각 템플릿에 포함된 레코드 유형에 대한 자세한 내용은 [작업 공간 템플릿 목록](../architecture/workspace-templates.md).

## 처음부터 레코드 유형 만들기

이 문서에서는 운영 레코드 유형을 처음부터 만드는 방법에 대해 설명합니다. 운영 레코드 유형을 처음부터 만드는 것은 분류를 만드는 것과 비슷합니다.

분류법에 대한 자세한 내용은 [분류 체계 만들기](../architecture/create-a-taxonomy.md).

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리 또는 **메인 메뉴** 아이콘 ![](assets/main-menu-shell.png)  왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드 유형을 만들 작업 영역을 선택합니다.
1. 클릭 **레코드 유형 추가**.
1. (조건부) 작업 레코드 유형을 만드는 경우 **처음부터**. 분류를 만들 때는 이 옵션을 사용할 수 없습니다.

   레코드 유형 추가 상자가 열립니다.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 다음 정보를 선택합니다.

   * **레코드 이름**: &quot;제목 없는 운영 레코드 유형&quot;을 이후 레코드 유형의 이름으로 바꿉니다. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **모양**: 레코드 종류와 관련된 아이콘의 색상과 모양을 정의합니다. 다음을 수행합니다.
      * 색상을 선택하여 새 레코드 유형을 식별합니다. 레코드 유형 아이콘의 색상입니다. 기본적으로 회색이 선택되어 있습니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

1. 바깥쪽을 클릭합니다. **레코드 유형 추가** 레코드를 저장하는 상자입니다.

   레코드 유형 카드가 선택한 작업 영역에 추가됩니다.
레코드 종류에 포함된 필드 수가 카드에 표시됩니다.
1. (선택 사항) 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 엽니다.

   ![](assets/operational-record-type-blank.png)

   레코드 유형 페이지는 기본적으로 테이블 뷰에 표시됩니다. 표의 열은 새 레코드 종류와 관련된 필드입니다. 각 행은 추가해야 하는 고유한 레코드입니다.

   기본적으로 다음 필드는 작업 레코드 유형의 테이블 보기 열에 표시됩니다.

   * 이름

     이름 필드는 분류법에 대해 자동으로 생성되는 유일한 필드입니다.
   * 설명
   * 시작 일자
   * 종료 일자
   * 상태

1. (선택 사항) 페이지 머리글에서 레코드 유형 이름을 업데이트합니다

   또는

   다음을 클릭합니다. **자세히** 아이콘 ![](assets/more-menu.png) 레코드 유형 이름의 오른쪽에 있는 **이름 바꾸기** 이름을 바꾸려면 다음을 수행하십시오.

1. (선택 사항) **+ 새 &lt; 레코드 유형 이름 >** 선택한 레코드 유형의 레코드를 추가할 수 있습니다. 자세한 내용은 [레코드 만들기](../records/create-records.md).
1. (선택 사항) **+** 레코드 종류에 필드를 더 추가하려면 테이블의 오른쪽 위 모서리에 있는 아이콘을 클릭합니다. 자세한 내용은 [필드 만들기](../fields/create-fields.md).
1. (선택 사항) 선택한 작업 영역으로 돌아가려면 레코드 유형 이름의 왼쪽에 있는 왼쪽 방향 화살표를 클릭합니다.

   레코드 유형 카드에는 레코드 유형에 포함된 필드 및 연결 수가 표시됩니다.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   레코드 추가, 레코드 유형 삭제 또는 편집, 레코드 유형 페이지의 보기 업데이트에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [레코드 만들기](../records/create-records.md)
   * [레코드 유형 삭제](../architecture/delete-record-types.md)
   * [레코드 유형 편집](../architecture/edit-record-types.md)
   * [Adobe Maestro에서 레코드 보기 관리](../views/manage-record-views.md) <!--add information here about the sorting and grouping when available-->

## Excel 또는 CSV 파일을 가져와서 레코드 유형 만들기

Excel 또는 CSV 파일을 사용하여 레코드 유형을 가져올 때는 다음 사항을 고려하십시오.

* Excel 파일의 각 시트는 Maestro의 레코드 유형이 됩니다.
* 각 시트의 열은 각 레코드 유형과 연관된 필드가 됩니다.
* 필드는 해당 레코드 유형에 대해 고유합니다.
* 각 시트의 각 행은 해당 레코드 유형과 연관된 고유한 레코드가 됩니다.
* Excel 파일의 각 시트는 다음을 초과할 수 없습니다.
   * 10,000행
   * 500열
* Excel 파일은 5MB를 초과할 수 없습니다.
* 빈 시트는 지원되지 않습니다.

Excel 파일을 사용하여 레코드 유형을 가져오려면 다음을 수행합니다.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리에서 <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 그런 다음 을 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드 유형을 만들 작업 영역을 선택합니다.
1. 클릭 **레코드 유형 추가**.
1. (조건부) 작업 레코드 유형을 만드는 경우 **Excel/CSV**.

   >[!NOTE]
   >
   >    분류 레코드 유형을 만들 때는 이 옵션을 사용할 수 없습니다.

1. 컴퓨터에 이전에 저장한 Excel 또는 CSV 파일을 끌어서 놓거나 **CSV 또는 Excel 파일 선택** 찾아 봅니다.
1. 클릭 **데이터 검토**.

   미리보기 및 편집(Preview and edit) 상자에 다음 정보가 표시됩니다.

   * 시트 이름 또는 이후 레코드 유형이 왼쪽 패널에 표시됩니다. Maestro는 기본적으로 각 새 레코드 유형의 아이콘과 색상을 선택합니다.
   * 첫 번째 시트 또는 레코드 유형이 선택되고 연관된 필드의 이름이 열 머리글로 표시됩니다. 각 필드의 유형은 기본적으로 선택됩니다.
   * 각 행은 새 레코드를 나타냅니다. 처음 10개의 레코드만 [미리 보기 및 편집] 상자에 표시됩니다.

   ![](assets/preview-and-edit-box.png)

1. (선택 사항) 왼쪽 패널에서 각 시트의 이름을 클릭하여 포함된 정보를 검토합니다.

   >[!NOTE]
   >
   >    비어 있는 시트는 지원되지 않으며 흐리게 표시됩니다.


1. (선택 사항) **가져올 시트 선택** 드롭다운 메뉴를 사용하여 가져오지 않을 시트의 선택을 해제합니다.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   선택을 취소한 시트는 회색 배경과 함께 표시됩니다.

1. 클릭 **가져오기** 파일을 가져올 준비가 되면

   다음 정보는에서 Maestro로 가져옵니다.

   * 새 레코드 유형
   * 각 레코드 유형과 연결된 새 필드
   * 각 레코드 유형과 연결된 새 레코드

   레코드 유형 페이지에서 필드 및 레코드 관리를 시작할 수 있습니다.

   이제 Maestro에 액세스할 수 있는 모든 사용자가 가져온 레코드 종류 및 해당 정보를 보고 편집할 수 있습니다. <!--this will change with permissions-->

## 다른 응용 프로그램의 개체 유형과 레코드 유형 연결

다른 응용 프로그램에서 Maestro 레코드 유형과 객체 유형 간에 연결을 만들 때 레코드 유형을 가져올 수 있습니다. 이렇게 하면 서드파티 애플리케이션의 객체 유형에 해당하는 읽기 전용 레코드 유형이 Maestro에 생성됩니다.

예를 들어 Maestro 레코드 유형을 Workfront 프로젝트와 연결하여 레코드 유형을 만들 수 있습니다. 따라서 Workfront 프로젝트 오브젝트 유형을 읽기 전용 레코드 유형으로 Maestro에 가져옵니다. 기본적으로 레코드 유형의 이름은 &quot;Workfront 프로젝트&quot;로 지정됩니다. <!--has this name changed? Lusine wanted to change it at some point-->

다음 응용 프로그램에서 다음 객체를 가져올 수 있습니다.

* Workfront에서:

   * 프로젝트
   * 포트폴리오
   * 프로그램
   * 회사
   * 그룹

자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).
