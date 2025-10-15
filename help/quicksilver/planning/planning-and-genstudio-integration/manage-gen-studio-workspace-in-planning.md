---
title: Adobe Workfront Planning에서 GenStudio Workspace 관리
description: GenStudio for Performance Marketing 작업 영역은 회사가 제품을 모두 구매하고 Workfront 인스턴스가 회사의 GenStudio 인스턴스와 통합되는 경우 Adobe Workfront Planning에서 사용할 수 있습니다. Planning에서 GenStudio 작업 영역을 보고 두 시스템의 정보를 업데이트할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: f2fe6ef78b3032f7a89d4c816cb11b525634c067
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 0%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# Adobe Workfront Planning에서 GenStudio 작업 공간 관리

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe GenStudio for Performance Marketing 작업 영역은 회사가 제품을 모두 구매하고 Workfront 인스턴스가 회사의 GenStudio 인스턴스와 통합되는 경우 Adobe Workfront Planning에서 사용할 수 있습니다.

Planning에서 GenStudio 작업 영역을 보고 두 시스템의 정보를 업데이트할 수 있습니다.

GenStudio Performance Marketing에서 GenStudio 작업 영역을 사용 및 관리하는 방법에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.

GenStudio-Workfront Planning 통합에 대한 일반적인 정보는 [Adobe Workfront Planning 및 Adobe GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.

>[!IMPORTANT]
>
>이 문서에 설명된 단계는 관리 권한이 있을 때 Workfront Planning에서 GenStudio 작업 영역을 업데이트하는 방법을 보여 줍니다.
>&#x200B;> GenStudio 작업 영역에 대한 Contribute 권한이 있는 경우 일부 기능을 사용할 수 없습니다.
>
>회사에 Workfront 인스턴스가 여러 개 있는 경우 모든 사용자는 Workfront Planning의 GenStudio 작업 영역에 대한 기여 권한을 받습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul> 
<li><p>모든 Workfront 및 모든 Planning 패키지</p></li>
또는
<li><p>모든 워크플로우 및 모든 Planning 패키지</li></ul>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
   <tr> 
<td> 
   <p> 추가 제품</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing 사용자 역할</p></td> 
   <td><p><ul><li>캠페인, 제품 및 가상 사용자에 액세스할 수 있는 모든 GenStudio 사용자 역할</li>
   <li>정품 인증에 액세스하기 위한 GenStudio System Manager <!--and Events--></li></ul>
   자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">사용자 역할 및 권한</a>을 참조하세요. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>  
   <p>Workfront Planning에서: </p>
   <ul>
   <li><p>GenStudio 작업 영역에 새 필드 또는 레코드 유형을 추가할 수 있는 GenStudio 작업 영역에 대한 권한을 관리합니다.</p></li>
   <li><p>GenStudio 작업 영역에서 레코드를 추가, 업데이트 또는 삭제할 수 있는 GenStudio 작업 영역 기여 권한</p> </li>  
   </ul>
   <p>어떤 사용자도 Workfront Planning의 GenStudio 작업 영역에서 GenStudio for Performance Marketing 레코드 유형 또는 필드를 제거할 수 없습니다</p>
   <p>Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing의 모든 권한</p></li>
   <li><p> Adobe GenStudio for Performance Marketing에서 항목을 만들 수 있는 권한 만들기</p></li></ul>
   </td>  
</tbody> 
</table>

Adobe Workfront Planning 액세스에 대한 자세한 내용은 [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.

Adobe GenStudio for Performance Marketing에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations ****** and Events*********</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to add new fields or record types to the GenStudio workspace</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   </ul>
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Workfront Planning에서 GenStudio 작업 공간 관리에 대한 고려 사항

* Workfront Planning에서 Adobe GenStudio for Performance Marketing 작업 영역을 보려면 먼저 조직에서 GenStudio을 구매해야 합니다.

* 조직에 있는 Workfront 인스턴스 수에 따라 Planning의 GenStudio 작업 영역에 대해 자동으로 다음 권한을 갖습니다.

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>Workfront 인스턴스 1개</p></td> 
      <td> 
   <p>GenStudio 작업 영역은 Workfront Planning 인스턴스에 표시됩니다</p>
   <p>Workfront 관리자는 Planning의 GenStudio 작업 영역에 대한 관리 권한이 있습니다.</p>
   <p>다른 모든 사용자는 Planning의 GenStudio 작업 영역에 대한 기여 액세스 권한을 가집니다</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> Workfront의 여러 인스턴스</p> </td> 
      <td> 
      <p>GenStudio 작업 영역은 모든 Workfront 인스턴스에서 볼 수 있습니다</p>
   <p>GenStudio for Performance Marketing 및 Workfront Planning에 대한 액세스 권한이 있는 모든 사용자는 Planning의 GenStudio에 대한 기여자 권한을 가집니다</p> </td> 
   </tr>
      </tbody> 
   </table>

* GenStudio 작업 영역에 대한 작업 영역 구성, 레코드 유형, 보기 및 필드를 업데이트하는 것은 Workfront Planning 작업 영역을 해당 요소로 업데이트하는 것과 동일합니다.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Workfront Planning에서 GenStudio 작업 공간 관리

>[!NOTE]
>
>GenStudio 작업 영역을 관리하기 전에 문서 [Workfront 계획 및 GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.
>

1. GenStudio에 액세스할 수 있는 사용자로 Workfront에 로그인합니다.
1. 왼쪽 상단의 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 계획]**&#x200B;을 클릭합니다.

   Workfront Planning 기본 페이지가 열립니다.

1. **다른 작업 영역**&#x200B;을 클릭하고 **System**&#x200B;에서 만든 표시가 있고 카드에 **GenStudio** 태그가 있는 작업 영역을 찾습니다.

   ![태그가 있는 GenStudio 작업 영역 카드](assets/genstudio-card-with-tag-highlighted.png)

1. **GenStudio 작업 영역 카드**&#x200B;를 클릭하여 Workfront Planning에서 GenStudio 작업 영역을 엽니다.
1. 기본적으로 다음 GenStudio 레코드 유형이 만들어지고 Workfront Planning에서 표시됩니다.

   * 캠페인
   * 제품
   * 페르소나
   * 활성화
   * 채널
   * 지역

   GenStudio 레코드 유형 카드에 원래 GenStudio에서 생성되었다는 표시가 있습니다.

   <!--check screen shot-->

   ![태그가 있는 GenStudio 레코드 유형 카드](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. 작업 영역 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 후 다음 중 하나를 클릭합니다.

   * **편집**

     자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. 작업 영역을 다른 사람과 공유하려면 오른쪽 상단의 **공유**&#x200B;를 클릭하세요.

   자세한 내용은 [작업 영역 공유](/help/quicksilver/planning/access/share-workspaces.md)를 참조하십시오.

1. 해당 유형의 레코드를 보려면 레코드 유형 카드를 클릭합니다.

   레코드 종류, 보기 및 필드를 관리하려면 이 문서의 [Workfront Planning에서 GenStudio 레코드 종류 관리](#manage-genstudio-record-types-from-workfront-planning) 섹션을 참조하십시오.


## Workfront Planning의 GenStudio 작업 공간에서 레코드 유형, 보기 및 레코드 관리

>[!NOTE]
>
>GenStudio 작업 영역을 관리하기 전에 문서 [Workfront 계획 및 GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.
>

1. 이 문서의 [GenStudio Planning에서 GenStudio 작업 영역 관리](#manage-the-genstudio-workspace-from-workfront-planning) 섹션에 설명된 대로 Workfront Planning의 Workfront 작업 영역으로 이동하여 레코드 유형 페이지를 엽니다.

1. 레코드 형식 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 후 다음 중 하나를 클릭합니다.

   * **편집**

     자세한 내용은 [레코드 종류 편집](/help/quicksilver/planning/architecture/edit-record-types.md)을 참조하세요.
   * **자동화 관리**

     자세한 내용은 [Adobe Workfront Planning 자동화 구성](/help/quicksilver/planning/records/configure-automations-to-create-records.md)을 참조하십시오.
   * **요청 양식 관리**

     여러 요청 양식을 만들 수 있습니다. 요청 양식은 Workfront의 요청 영역에서 사용할 수 있으며 공개적으로 또는 링크와 공유할 수도 있습니다.

     자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

1. 보기 또는 레코드 유형을 공유하려면 다음을 수행하십시오.

   * 레코드 종류 페이지의 오른쪽 상단에서 **공유**&#x200B;를 클릭한 후 다음 중 하나를 클릭합니다.
      * **레코드 종류 공유**
자세한 내용은 [레코드 종류 공유](/help/quicksilver/planning/access/share-record-types.md)를 참조하십시오.
      * **현재 보기 공유**
자세한 내용은 [보기 공유](/help/quicksilver/planning/access/share-views.md)를 참조하십시오.
      * **보기 링크 복사**
보기에 대한 링크가 클립보드에 복사됩니다.
      * **현재 보기 내보내기**
자세한 내용은 [테이블 보기에서 레코드 내보내기](/help/quicksilver/planning/records/export-records-from-the-table-view.md)를 참조하십시오.

1. 레코드 유형 보기를 관리하려면 다음을 수행합니다.

   * GenStudio 레코드 형식에 대한 보기를 만들려면 **+ 보기**&#x200B;를 클릭하십시오.

     자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

   * **전체 화면** 아이콘 ![전체 화면으로 전체 보기 열기](assets/open-full-screen-icon.png)를 클릭하여 전체 화면 모드로 보기를 엽니다.

   * 모든 보기에서 보기 요소를 관리합니다.

     예를 들어 사용 가능한 경우 보기의 필터, 그룹화, 정렬, 설정을 변경할 수 있습니다.

     자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

1. 레코드를 추가하려면 다음 중 하나를 수행합니다.

   * 모든 보기에서 **새 레코드**&#x200B;을 클릭하여 처음부터 레코드를 만듭니다.

   * 표 보기에서 Excel 또는 CSV 파일을 사용하여 레코드 가져오기

   * 타임라인 또는 달력 보기에서 아무 곳이나 클릭하여 레코드를 추가합니다.

     자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.

     레코드는 Workfront 및 GenStudio 모두에서 볼 수 있습니다.

     >[!NOTE]
     >
     >활성화 레코드 유형에 대한 레코드를 추가할 수 없습니다.

1. 레코드를 편집하려면 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 인라인 레코드 편집

   * 보기에서 레코드를 클릭하여 세부 정보 페이지를 엽니다.

     자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

     Planning의 GenStudio 작업 영역에서 변경한 사항은 GenStudio에서 즉시 볼 수 있습니다.

1. 테이블 보기에서 레코드를 선택한 다음 **삭제**&#x200B;를 클릭합니다.

   자세한 내용은 [레코드 삭제](/help/quicksilver/planning/records/delete-records.md)를 참조하십시오.

   삭제된 레코드는 GenStudio에서 즉시 제거됩니다.

   >[!TIP]
   >
   >삭제된 레코드는 Workfront Planning의 테이블 보기에서 최근에 삭제된 저장소를 복구할 수 있습니다. GenStudio에서 삭제된 레코드는 Workfront Planning의 최근에 삭제된 빈에서도 복구할 수 있습니다.

   자세한 내용은 [삭제된 레코드 복원](/help/quicksilver/planning/records/restore-deleted-records.md)을 참조하세요.

1. 표 보기의 오른쪽 위 모서리에 있는 + 아이콘을 클릭하여 다음을 만듭니다.

   * 레코드 필드

     자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하세요.

   * 레코드 연결

     자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

     GenStudio 작업 영역에서 생성된 필드는 다음 영역에 표시됩니다.

      * Workfront Planning 보기
      * Workfront Planning 레코드 세부 정보
      * GenStudio 레코드 세부 정보

     >[!TIP]
     >
     >Workfront Planning에서 생성된 필드는 GenStudio의 목록 보기에 표시되지 않습니다.

1. 테이블 보기의 필드 위로 마우스를 가져간 다음 드롭다운 메뉴를 클릭하여 다음 중 하나를 수행합니다.

   * 정렬 기준:
   * 숨기기
   * 설정 편집
     <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

     <!--GenStudio-native fields are note removed from GenStudio. -->

     >[!NOTE]
     >
     >GenStudio에서 관리 권한이 있는 경우에만 필드의 구성을 편집하고 필드를 추가할 수 있습니다.

