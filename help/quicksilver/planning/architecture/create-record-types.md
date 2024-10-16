---
title: 레코드 유형 만들기
description: 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 조직의 라이프사이클에 필요한 작업 항목을 설명하는 사용자 정의 레코드 유형을 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 2%

---


<!--this is linked to the UI in an empty workspace screen-->

# 레코드 유형 만들기

{{planning-important-intro}}

레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 조직의 라이프사이클에 필요한 작업 관련 항목을 설명하는 사용자 정의 레코드 유형을 생성할 수 있습니다.

레코드 형식에 대한 자세한 내용은 [레코드 형식 개요](/help/quicksilver/planning/architecture/overview-of-record-types.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 계획*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


<!--
OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Current: Plan</p>
   Or
   <p>New: Standard </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
-->

## 레코드 유형 만들기에 대한 고려 사항

* 다음과 같은 방법으로 작업 영역에서 레코드 유형을 만들 수 있습니다.

   * 자동:
      * 템플릿을 사용하여 작업 공간을 만드는 경우.

        자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

     <!--* When you import them using an Excel or CSV file. 

            >[!IMPORTANT]
            >
            >This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.-->

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

작업 영역 만들기에 대한 자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

각 템플릿에 포함된 레코드 종류에 대한 자세한 내용은 [작업 영역 템플릿 목록](/help/quicksilver/planning/architecture/workspace-templates.md)을 참조하세요.

## 처음부터 레코드 유형 만들기

{{step1-to-planning}}

1. 레코드 유형을 만들 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.
1. (선택 사항) 작업 영역에 새 섹션을 추가하려면 **섹션 추가**&#x200B;를 클릭합니다.
1. **레코드 종류 추가**&#x200B;를 클릭합니다.

   레코드 유형 추가 상자가 열립니다.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. 다음 정보를 업데이트합니다.

   * &quot;제목 없는 레코드 유형&quot;을 이후 레코드 유형의 이름으로 바꿉니다. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **설명**: 레코드 형식에 대한 정보를 더 추가합니다.
   * 레코드 유형과 연관된 아이콘의 색과 모양을 선택합니다. 다음을 수행합니다.
      * 색상을 선택하여 새 레코드 유형을 식별합니다. 레코드 유형 아이콘의 색상입니다. 기본적으로 회색이 선택되어 있습니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

1. Click **Create**.

   레코드 유형 카드가 선택한 섹션 및 작업 영역에 추가됩니다.
레코드 유형의 설명이 카드에 표시됩니다.

   ![](assets/record-type-card-with-description.png)

1. (선택 사항) 레코드 종류 카드 위로 마우스를 가져간 후 오른쪽 상단의 **자세히** 아이콘 ![](assets/more-menu.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭하여 레코드 종류에 대한 정보를 수정합니다.
1. (선택 사항) 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 엽니다.

   ![](assets/operational-record-type-blank.png)

   레코드 유형 페이지는 기본적으로 테이블 뷰에 표시됩니다. 표의 열은 새 레코드 종류와 관련된 필드입니다. 각 행은 추가해야 하는 고유한 레코드입니다.

   <!--TIP: If you import a record type from an Excel or CSV file, records are also imported.-->

   기본적으로 다음 필드는 작업 레코드 유형의 테이블 보기 열에 표시됩니다.

   * 이름
   * 설명
   * 시작 일자
   * 종료 일자
   * 상태

1. (선택 사항) 페이지 헤더에서 레코드 유형 이름을 업데이트합니다

   또는

   레코드 형식 이름 오른쪽에 있는 **자세히** 아이콘 ![](assets/more-menu.png)을(를) 클릭하고 **편집**&#x200B;을(를) 클릭하여 이름을 바꾸거나 레코드 형식 정보를 변경합니다. 자세한 내용은 [레코드 종류 편집](/help/quicksilver/planning/architecture/edit-record-types.md)을 참조하세요.

1. (선택 사항) **+ 새 레코드**&#x200B;을(를) 클릭하여 선택한 레코드 종류의 레코드를 추가합니다. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
1. (선택 사항) 레코드 종류에 필드를 더 추가하려면 표의 오른쪽 상단에 있는 **+** 아이콘을 클릭합니다.

   필드 만들기에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

1. (선택 사항) 헤더에서 레코드 유형 이름의 왼쪽에 있는 왼쪽 화살표를 클릭하여 선택한 작업 영역으로 돌아갑니다.

1. (선택 사항) 작업 공간에서 레코드 유형 카드를 클릭하여 원하는 위치에 레코드 유형을 끌어다 놓거나 다른 섹션으로 이동합니다.

   변경 사항은 자동으로 저장됩니다.

   레코드 추가, 레코드 유형 삭제 또는 편집, 레코드 유형 페이지의 보기 업데이트에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [레코드 만들기](/help/quicksilver/planning/records/create-records.md)
   * [레코드 유형 삭제](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [레코드 유형 편집](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)

<!--
## Create record types by importing an Excel or CSV file

>[!IMPORTANT]
>
>This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.

Consider the following when importing record types using an Excel or CSV file: 

* Each sheet of the Excel file becomes a record type. 
* The columns of each sheet become the fields associated with each record type. 
* Fields are unique for their respective record types. 
* Each row in each sheet becomes a unique record associated with its respective record type. 
* Each sheet of the Excel file should not exceed the following: 
    * 50,000 rows
    * 500 columns
* The Excel file should not be larger than 5MB.
* Empty sheets are not supported. 

To import record types using an Excel file: 

{{step1-to-planning}}

1. Click the workspace where you want to create record types, 

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name, search for a workspace, then select it when it displays in the list.
1. Click **Add record type**. 
1. Click **Excel/CSV**.
1. Drag and drop an Excel or CSV file previously saved on your computer, or click **Select a CSV or Excel file** to browse for one. 
1. Click **Review your data**.
    
    The Preview and edit box displays with the following information: 

    * The names of the sheets or of the future record types display in the left panel. Workfront Planning selects an icon and a color for each new record type by default.
    * The first sheet or record type is selected and the names of the fields associated with it display as the column headers. The type of each field is selected by default. 
    * Each row represents a new record. Only the first 10 records display in the Preview and edit box. 

    ![](assets/preview-and-edit-box.png)

1. (Optional) Click the name of each sheet in the left panel to review the information it contains. 

    >[!NOTE]
    >
    >    Sheets that are empty are not supported and are dimmed. 


1. (Optional) Click the **Select sheets to import** drop-down menu and deselect the sheets that you don't want to import. 

    ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

    Sheets you deselected display with a gray background. 

1. Click **Import** when you are ready to import your file. 

    The following information imports in to Workfront Planning:

    * New record types
    * New fields associated with each record type
    * New records associated with each record type

    You can start managing fields and records on the record types pages. 
    
    Everyone with access to Workfront Planning can now view and edit the imported record types and their information.-->

