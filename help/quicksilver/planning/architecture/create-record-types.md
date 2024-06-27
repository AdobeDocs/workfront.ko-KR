---
title: 레코드 유형 만들기
description: 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 조직의 라이프사이클에 필요한 작업 항목을 설명하는 사용자 정의 레코드 유형을 생성할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '1273'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# 레코드 유형 만들기

{{planning-important-intro}}

레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 조직의 라이프사이클에 필요한 작업 관련 항목을 설명하는 사용자 정의 레코드 유형을 생성할 수 있습니다.

레코드 유형에 대한 자세한 내용은 [레코드 유형 개요](/help/quicksilver/planning/architecture/overview-of-record-types.md).

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
   <td> Adobe Workfront
   </td>
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
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>현재: 플랜</p>
   또는
   <p>새로운 기능: 표준 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 레코드 유형 만들기에 대한 고려 사항

* 다음과 같은 방법으로 작업 영역에서 레코드 유형을 만들 수 있습니다.

   * 자동:
      * 템플릿을 사용하여 작업 공간을 만드는 경우.

        자세한 내용은 [작업 공간 만들기](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Excel 또는 CSV 파일을 사용하여 가져올 때.

        >[!IMPORTANT]
        >
        >이 기능은 2024년 3월 21일부터 일시적으로 비활성화되었습니다. 이 기능은 나중에 활성화됩니다.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * 수동:

      * 처음부터.

        이 문서에서는 처음부터 레코드 유형을 만드는 방법을 설명합니다.

* 한 섹션 내에서 또는 작업 영역의 한 섹션에서 다른 섹션으로 레코드 유형을 이동할 수 있습니다. 한 작업 영역에서 다른 작업 영역으로 레코드 유형을 이동할 수 없습니다.

## 작업 공간 템플릿을 사용하여 레코드 유형 만들기

Workfront Planning 템플릿을 사용하여 작업 공간을 만들 때 레코드 유형을 자동으로 만들 수 있습니다. 각 템플릿에는 샘플 레코드 유형이 포함되어 있습니다.

템플릿에서 작업 공간을 만들 때 레코드 유형은 다음 섹션으로 그룹화됩니다.

* 운영 레코드 유형
* 분류

운영 레코드 유형 및 분류 섹션에서 레코드 유형을 수동으로 추가할 수 있습니다.

작업 공간 만들기에 대한 자세한 내용은 [작업 공간 만들기](/help/quicksilver/planning/architecture/create-workspaces.md).

각 템플릿에 포함된 레코드 유형에 대한 자세한 내용은 [작업 공간 템플릿 목록](/help/quicksilver/planning/architecture/workspace-templates.md).

## 처음부터 레코드 유형 만들기

{{step1-to-planning}}

1. 레코드 유형을 만들 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.
1. (선택 사항) **섹션 추가** 작업공간에 새 섹션을 추가합니다.
1. 클릭 **레코드 유형 추가**.
1. (조건부) Excel 또는 CSV 파일을 가져와서 레코드 유형을 만드는 것이 활성화되어 있으면 **처음부터**. 그렇지 않으면 **레코드 유형 추가** 상자가 열립니다.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 다음 정보를 업데이트합니다.

   * &quot;제목 없는 레코드 유형&quot;을 이후 레코드 유형의 이름으로 바꿉니다. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **설명**: 레코드 유형에 대한 정보를 더 추가합니다.
   * 레코드 유형과 연관된 아이콘의 색과 모양을 선택합니다. 다음을 수행합니다.
      * 색상을 선택하여 새 레코드 유형을 식별합니다. 레코드 유형 아이콘의 색상입니다. 기본적으로 회색이 선택되어 있습니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

1. Click **Create**.

   레코드 유형 카드가 선택한 섹션 및 작업 영역에 추가됩니다.
레코드 유형의 설명이 카드에 표시됩니다.

   ![](assets/record-type-card-with-description.png)

1. (선택 사항) 레코드 유형 카드에 마우스를 가져다 대고 **자세히** 아이콘 ![](assets/more-menu.png) 오른쪽 상단에서 을(를) 클릭한 다음 **편집** 레코드 유형에 대한 정보를 수정합니다.
1. (선택 사항) 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 엽니다.

   ![](assets/operational-record-type-blank.png)

   레코드 유형 페이지는 기본적으로 테이블 뷰에 표시됩니다. 표의 열은 새 레코드 종류와 관련된 필드입니다. 각 행은 추가해야 하는 고유한 레코드입니다.

   >[!TIP]
   >
   >    Excel 또는 CSV 파일에서 레코드 형식을 가져오는 경우 레코드도 가져옵니다.

   기본적으로 다음 필드는 작업 레코드 유형의 테이블 보기 열에 표시됩니다.

   * 이름
   * 설명
   * 시작 일자
   * 종료 일자
   * 상태

1. (선택 사항) 페이지 헤더에서 레코드 유형 이름을 업데이트합니다

   또는

   다음을 클릭합니다. **자세히** 아이콘 ![](assets/more-menu.png) 레코드 유형 이름의 오른쪽에 있는 **편집** 이름을 바꾸거나 정보를 변경합니다. 자세한 내용은 [레코드 유형 편집](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (선택 사항) **+ 새 레코드** 선택한 레코드 유형의 레코드를 추가할 수 있습니다. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md).
1. (선택 사항) **+** 레코드 종류에 필드를 더 추가하려면 테이블의 오른쪽 위 모서리에 있는 아이콘을 클릭합니다.

   필드 만들기에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md).

1. (선택 사항) 헤더에서 레코드 유형 이름의 왼쪽에 있는 왼쪽 화살표를 클릭하여 선택한 작업 영역으로 돌아갑니다.

1. (선택 사항) 작업 공간에서 레코드 유형 카드를 클릭하여 원하는 위치에 레코드 유형을 끌어다 놓거나 다른 섹션으로 이동합니다.

   변경 사항은 자동으로 저장됩니다.

   레코드 추가, 레코드 유형 삭제 또는 편집, 레코드 유형 페이지의 보기 업데이트에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [레코드 만들기](/help/quicksilver/planning/records/create-records.md)
   * [레코드 유형 삭제](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [레코드 유형 편집](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)

## Excel 또는 CSV 파일을 가져와서 레코드 유형 만들기

>[!IMPORTANT]
>
>이 기능은 2024년 3월 21일부터 일시적으로 비활성화되었습니다. 이 기능은 나중에 활성화됩니다.

Excel 또는 CSV 파일을 사용하여 레코드 유형을 가져올 때는 다음 사항을 고려하십시오.

* Excel 파일의 각 시트는 레코드 유형이 됩니다.
* 각 시트의 열은 각 레코드 유형과 연관된 필드가 됩니다.
* 필드는 해당 레코드 유형에 대해 고유합니다.
* 각 시트의 각 행은 해당 레코드 유형과 연관된 고유한 레코드가 됩니다.
* Excel 파일의 각 시트는 다음을 초과할 수 없습니다.
   * 50,000행
   * 500열
* Excel 파일은 5MB를 초과할 수 없습니다.
* 빈 시트는 지원되지 않습니다.

Excel 파일을 사용하여 레코드 유형을 가져오려면 다음을 수행합니다.

{{step1-to-planning}}

1. 레코드 유형을 만들 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.
1. 클릭 **레코드 유형 추가**.
1. 클릭 **Excel/CSV**.
1. 컴퓨터에 이전에 저장한 Excel 또는 CSV 파일을 끌어서 놓거나 **CSV 또는 Excel 파일 선택** 찾아 봅니다.
1. 클릭 **데이터 검토**.

   미리보기 및 편집(Preview and edit) 상자에 다음 정보가 표시됩니다.

   * 시트 이름 또는 이후 레코드 유형이 왼쪽 패널에 표시됩니다. Workfront Planning에서는 기본적으로 각 새 레코드 유형에 대해 아이콘과 색상을 선택합니다.
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

   다음 정보는에서 Workfront Planning으로 가져옵니다.

   * 새 레코드 유형
   * 각 레코드 유형과 연결된 새 필드
   * 각 레코드 유형과 연결된 새 레코드

   레코드 유형 페이지에서 필드 및 레코드 관리를 시작할 수 있습니다.

   이제 Workfront Planning에 액세스할 수 있는 모든 사용자는 가져온 레코드 유형과 해당 정보를 보고 편집할 수 있습니다. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
-->