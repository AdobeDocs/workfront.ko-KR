---
title: 레코드 연결
description: 레코드 종류 간에 연결을 만든 후에는 개별 레코드를 서로 연결할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: d3c22c84a9b246d1a45853c5d2825241f58bebe9
workflow-type: tm+mt
source-wordcount: '1975'
ht-degree: 0%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# 레코드 연결

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe Maestro 레코드를 서로 연결하거나 다른 응용 프로그램의 개체에 연결할 수 있습니다.

먼저 두 개의 레코드 형식을 함께 연결하거나 다른 응용 프로그램의 개체 형식에 레코드 형식을 연결해야 합니다. 그런 다음 레코드 형식의 표 보기를 사용하여 레코드를 서로 연결하거나 레코드를 다른 개체에 연결할 수 있습니다.

레코드 형식을 서로 연결하거나 다른 응용 프로그램의 개체 형식에 연결하는 방법에 대한 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

레코드 종류 연결에 대한 예는 [레코드 종류 및 레코드 연결의 예](../architecture/example-connect-record-types-and-records.md).

다음을 연결할 수 있습니다.

* Maestro 운영 기록
* Maestro 운영 레코드를 분류 레코드로 변환
* 다른 응용 프로그램의 Maestro 운영 기록 및 객체

  다음 응용 프로그램에서 아래 나열된 형식의 개체에 Maestro 레코드를 연결할 수 있습니다.

   * Adobe Workfront

      * 프로젝트
      * 포트폴리오
      * 프로그램
      * 회사
      * 그룹

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <td><p>Any, to create Maestro records</p> 
<p>Workfront에서 프로젝트를 보려면 작업 이상</p>
  <p>자세한 내용은 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Adobe Workfront 라이선스 개요</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">액세스 수준</td>
   <td> <p>Any, to create Maestro records</p>
<p>프로젝트, Portfolio, 프로그램에 대한 보기 이상의 액세스 권한</p> 
<p>그룹 및 회사에 대한 추가 액세스 권한(보기 그룹 또는 회사 사용자가 소속되어 있지 않은 경우)</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td> <p>Maestro 레코드와 연결할 개체에 대한 이상의 사용 권한 보기  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/grant-access.md">Adobe 마에스트로에 대한 액세스 권한 부여</a>. </p></td>
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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
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

## 레코드 연결

### 레코드 연결에 대한 고려 사항

* 레코드 유형 간의 연결이 설정되면 연결된 레코드 유형이 연결된 레코드 유형의 테이블에 연결된 레코드 필드로 표시됩니다.
* 연결된 레코드 필드에서 연결된 레코드와 개체 유형의 레코드와 개체를 찾아보고 추가할 수 있습니다.
* 연결된 레코드 유형의 필드를 연결할 레코드 유형의 테이블에 추가할 수 있습니다.
* 연결 중인 레코드의 연결된 필드 값은 수동으로 업데이트할 수 없습니다.

  연결된 레코드에서 연결된 필드의 값은 자동으로 연결되는 Maestro 레코드를 채웁니다.

* Maestro에 액세스할 수 있는 모든 사용자는 Maestro 레코드 간 또는 Maestro 레코드와 Workfront 오브젝트 간 연결을 볼 수 있습니다. 또한 다른 모든 사용자의 연결을 보고 편집할 수 있습니다. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* 하나의 Maestro 레코드를 다른 애플리케이션에서 하나 또는 여러 객체에 연결할 수 있습니다.
* 분류법을 레코드 유형이나 다른 응용 프로그램의 개체에 연결할 수 없습니다. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Maestro 레코드를 Workfront 오브젝트와 연결하려면 다음이 필요합니다.

   * Workfront 개체입니다. 예를 들어 먼저 Workfront에서 프로젝트, 포트폴리오, 프로그램, 회사 또는 그룹을 만들어야 합니다.
   * Maestro 작업 공간, 레코드 유형 및 레코드. 자세한 내용은 다음 문서를 참조하십시오.

      * [작업 공간 만들기](../architecture/create-workspaces.md)
      * [레코드 유형 만들기](../architecture/create-record-types.md)
      * [레코드 만들기](../records/create-records.md)

   * 레코드 유형 간 또는 레코드 유형과 다른 응용 프로그램의 개체 간 연결입니다. 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md)

### Connect Maestro 레코드

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리 또는 **메인 메뉴** 아이콘 ![](assets/main-menu-shell.png)  왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드를 연결할 작업 영역을 선택합니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. 선택 **표** 다음에서 보기 **보기** 레코드 유형 페이지의 오른쪽 위 모서리에 있는 드롭다운 메뉴.
1. 선택한 레코드 유형에서 다른 레코드 또는 개체 유형에 연결을 추가합니다. 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

   연결된 레코드 종류를 표시하는 새 열이 표에 추가됩니다.

1. 테이블에 새 행을 추가하여 선택한 레코드 유형에 레코드를 추가합니다. 자세한 내용은 [레코드 만들기](../../maestro/records/create-records.md).
1. 표 보기에 나열된 레코드에서 연결된 레코드 열로 이동하여 다른 Maestro 레코드와 연결할 레코드에 해당하는 셀을 마우스로 가리킨 다음 **+** 아이콘.

   다음 **오브젝트 연결** 상자가 표시됩니다.

   ![](assets/connected-objects-table-for-records.png)

1. 검색 상자에 레코드 이름을 입력한 다음 목록에 표시될 때 선택합니다

   또는

   상자에서 하나 이상의 레코드 이름을 선택한 다음 **오브젝트 연결** 을 클릭합니다.

   다음이 추가됩니다.

   * 연결된 레코드는 3단계에서 선택한 레코드의 연결된 레코드 필드에 표시됩니다. 연결된 레코드를 업데이트하면 연결할 레코드의 연결된 레코드 필드가 자동으로 업데이트됩니다. <!--ensure the number of the step stays accurate-->
   * 연결된 레코드에 속하는 연결된 필드는 원래 연결된 레코드의 정보로 자동으로 채워집니다. 연결된 필드는 수동으로 편집할 수 없습니다.

     >[!TIP]
     >
     >* &quot;연결된 필드&quot;와 &quot;조회 필드&quot;를 서로 교환하여 사용합니다.
     >
     >* 레코드 유형을 연결할 때 여러 레코드 허용 설정을 활성화한 경우, 선택한 여러 개체의 필드 값이 쉼표로 구분되어 표시되거나 선택한 집계기에 따라 집계됩니다.

1. (선택 사항) Maestro 레코드 유형 페이지를 닫고 선택한 작업 영역으로 이동합니다.
1. 연결한 레코드 종류의 카드를 클릭합니다.

   예를 들어 캠페인 레코드를 제품 레코드와 연결한 경우 **제품** 카드.

   레코드 유형 카드가 표 보기에서 열립니다.

   Campaign 연결된 레코드 필드는 제품 레코드 유형 페이지에서 제품에 연결한 캠페인의 이름을 표시합니다. Campaign 정보를 업데이트하면 제품 레코드 유형에 대한 Campaign 연결 레코드 필드가 자동으로 업데이트됩니다.

### Maestro 레코드를 Workfront 오브젝트에 연결

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Maestro 레코드 유형과 Workfront 객체 유형 간에 연결을 만든 후 개별 Maestro 레코드를 Workfront의 객체에 연결할 수 있습니다. Workfront 객체의 필드를 Maestro 레코드 유형에 연결할 수도 있습니다.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리 또는 **메인 메뉴** 아이콘 ![](assets/main-menu-shell.png)  왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드를 연결할 작업 영역을 선택합니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. 다음에서 테이블 뷰를 선택합니다. **보기** 레코드 유형 페이지의 오른쪽 위 모서리에 있는 드롭다운 메뉴.
1. Workfront에서 선택한 레코드 유형의 오브젝트 유형에 새 연결을 추가합니다. Workfront 섹션 아래의 다음 객체 중에서 선택합니다.

   * 프로젝트
   * 포트폴리오
   * 프로그램
   * 회사
   * 그룹

   자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

   연결된 객체 유형을 표시하기 위해 새 열이 테이블에 추가됩니다.

1. 테이블에 새 행을 추가하여 선택한 레코드 유형에 개별 레코드를 추가합니다. 자세한 내용은 [레코드 만들기](../../maestro/records/create-records.md).
1. 표 보기에 나열된 레코드에서 연결된 개체 열로 이동하여 Workfront의 다른 개체와 연결할 레코드에 해당하는 셀을 마우스로 가리킨 다음 **+** 아이콘. <!--change Workfront to other applications, when this will be possible-->

   다음 **오브젝트 연결** 상자가 표시됩니다.

   ![](assets/connect-objects-box-to-select-projects.png)

1. 검색 상자에 Workfront 개체 이름을 입력한 다음 목록에 표시될 때 선택합니다

   또는

   상자에서 하나 이상의 개체 이름을 선택한 다음 **오브젝트 연결** 을 클릭합니다.

   Maestro에 추가된 항목은 다음과 같습니다.

   * 선택한 Workfront 개체가 연결된 레코드 필드에 추가됩니다.
   * 연결된 레코드에 필드를 추가할 때 선택한 모든 연결된 필드에 대해 새 연결된 필드(또는 조회 필드)가 만들어집니다.
   * &quot;Workfront 개체&quot;라는 새 레코드 유형은 연결하려는 Maestro 레코드와 동일한 작업 영역에서 만들어집니다. 개체 이름은 이 레코드 종류 이름의 일부입니다. 예를 들어 Workfront 프로젝트에 연결하면 Maestro에서 Workfront 프로젝트 레코드 유형이 생성됩니다.

     이 레코드 유형은 읽기 전용이며 Maestro 레코드에서 만든 새 연결된 오브젝트 필드에서 선택한 Workfront 오브젝트를 표시합니다. 연결된 개체의 연결된 필드는 읽기 전용 연결된 Workfront 레코드에도 표시됩니다.

     >[!IMPORTANT]
     >
     > 읽기 전용 Workfront 개체 레코드 유형은 개별 프로젝트가 Maestro 레코드에 추가될 때만 만들어집니다. Maestro 레코드 유형과 Workfront 객체 유형 간에 연결을 만들기만 하면 Workfront 레코드 유형이 만들어지지 않습니다.

     Workfront 개체 필드의 기존 정보는 연결된 필드 또는 조회 필드에 표시됩니다.

     >[!TIP]
     >
     >
     >* 복수 레코드 허용 설정을 활성화한 경우, 복수 객체 값은 쉼표로 구분되어 표시되거나 선택한 집계기에 따라 집계됩니다.
     >
     >* 연결된 Workfront 개체에 대해 Maestro 연결된 레코드에 연결된 레코드 필드가 만들어지지 않습니다.


1. (선택 사항) Maestro 레코드 유형 페이지를 닫고 선택한 작업 영역으로 이동합니다.
1. Workfront 개체 레코드 유형에 대한 카드를 클릭합니다. 예를 들어 **Workfront 프로젝트** 카드(Workfront 프로젝트에 연결된 경우) 읽기 전용 Workfront 레코드 유형 카드가 표 보기에서 열립니다.

   >[!NOTE]
   >
   >    * Workfront 레코드 유형 페이지에 나열된 레코드는 읽기 전용 Workfront 개체입니다. Workfront 레코드 유형에서 연결된 필드도 읽기 전용 열로 표시되며, Workfront에서 채워질 때 자동으로 채워집니다.
   >    * Maestro에서 Workfront 필드는 수동으로 업데이트할 수 없습니다. Workfront 개체 필드는 Workfront에서 채워야 하며 필드 값은 Maestro의 Workfront 레코드에 자동으로 표시됩니다.
   >
   >    * 타임라인 보기에서 Workfront 개체 레코드 유형을 표시하려면 읽기 전용 Workfront 레코드 유형 페이지의 테이블 보기에 두 개 이상의 날짜 필드가 표시되어야 합니다.

1. (선택 사항) Maestro에서 Workfront 객체 레코드 세부 사항 페이지를 열려면 다음 중 하나를 수행하십시오.

   * 연결한 레코드 유형에서 Workfront 개체로 연결된 레코드 필드로 이동하여 Workfront 개체의 이름을 클릭합니다.
   * 다음에서 **표** Workfront 레코드 유형 페이지에서 Workfront 개체의 이름을 클릭합니다

     또는

     다음을 클릭합니다. **자세히** 메뉴를 사용하여 Workfront 개체 이름 오른쪽에서 **보기**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   링크된 Workfront 객체의 Maestro 세부 정보 페이지가 열립니다. 읽기 전용 페이지입니다.

1. (선택 사항) Workfront에서 연결된 Workfront 개체를 열려면 다음 중 하나를 수행하십시오.

   * 다음에서 **표** Workfront 레코드 유형 페이지를 보고 Workfront 개체의 이름을 클릭합니다.

   또는

   다음을 클릭합니다. **자세히** 메뉴를 사용하여 Workfront 개체 이름 오른쪽에서 **소스로 이동**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Workfront 개체 페이지가 열립니다. 권한이 있는 경우 Workfront 개체에 대한 정보를 편집할 수 있습니다.

1. (선택 사항) **필드 추가** 아이콘 ![](assets/add-fields-icon.png) Workfront 레코드 유형 페이지의 표 보기 오른쪽 상단 모서리에서 Workfront 레코드 유형에서 Workfront 필드를 추가하거나 제거합니다.

   >[!NOTE]
   >
   >  Workfront 개체 레코드 유형 페이지에서 추가하거나 제거하는 필드는 Workfront 개체 유형에 연결되는 Maestro 레코드 유형에서 추가되거나 제거되지 않습니다. 필드는 읽기 전용 Workfront 레코드 유형 페이지에만 표시되므로 Maestro에서 검토할 수 있습니다.

1. (선택 사항 및 조건부) 두 개 이상의 날짜 필드를 Workfront 개체에 추가한 경우 **보기** Workfront 개체 레코드 유형 페이지의 드롭다운 메뉴에서 **타임라인** 보기. Workfront 연결 개체가 타임라인 보기에 표시됩니다.
