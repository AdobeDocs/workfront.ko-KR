---
title: Adobe Workfront Planning에서 GenStudio Workspace 관리
description: GenStudio for Performance Marketing 작업 영역은 회사가 제품을 모두 구매하고 Workfront 인스턴스가 회사의 GenStudio 인스턴스와 통합되는 경우 Adobe Workfront Planning에서 사용할 수 있습니다. Planning에서 GenStudio 작업 영역을 보고 두 시스템의 정보를 업데이트할 수 있습니다.
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

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

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

Adobe GenStudio for Performance Marketing 작업 영역은 회사가 제품을 모두 구매하고 Workfront 인스턴스가 회사의 GenStudio 인스턴스와 통합되는 경우 Adobe Workfront Planning에서 사용할 수 있습니다.

Planning에서 GenStudio 작업 영역을 보고 두 시스템의 정보를 업데이트할 수 있습니다.

GenStudio Performance Marketing에서 GenStudio 작업 영역을 사용 및 관리하는 방법에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.

GenStudio-Workfront Planning 통합에 대한 일반적인 정보는 [Adobe Workfront Planning 및 Adobe GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Adobe Workfront 워크플로 패키지</p>
<p>모든 Adobe Workfront Planning 패키지</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio 패키지</p></td> 
   <td> 
<p>??? GEN STUDIO에 이를 지원하는 패키지가 있습니까???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p> 표준</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio 라이선스</p></td> 
   <td><p> ??? GEN STUDIO에는 이를 지원하는 특정 라이센스가 필요합니까???</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> 추가 제품</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
   <p>GenStudio 구성: ???GEN에 필요한 액세스 수준은 무엇입니까???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한*</p></td> 
   <td>  
   <p>Workfront Planning에서: </p>
   <ul>
   <li><p>작업 공간 및 레코드 유형에 대한 또는 그 이상의 권한 기여  </p> </li> 
   <li><p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p></li>
   </ul>
   <p>Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing의 모든 권한</p></li>
   <li><p> Adobe GenStudio for Performance Marketing에서 항목을 만들 수 있는 권한 만들기</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
*Adobe GenStudio for Performance Marketing에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.

+++   

## Workfront Planning에서 GenStudio 작업 공간 관리에 대한 고려 사항

* Workfront Planning에서 Adobe GenStudio for Performance Marketing 작업 영역을 보려면 먼저 조직에서 GenStudio을 구매해야 합니다.

* Workfront 사용자가 Workfront Planning에서 GenStudio 작업 영역을 보려면 GenStudio에 액세스할 수 있어야 합니다.

* Workfront Planning에서 GenStudio 작업 공간에 대한 다음 정보를 업데이트할 수 있습니다.

   * 작업 영역 설정 <!--check to see if this is correct? is this editable or read only from Planning??--> 편집
   * 레코드 종류 및 해당 필드 <!--check on this--> 편집
   * 보기 공유, 편집 및 추가
   * 새 레코드 유형 추가
   * 레코드 편집, 추가 또는 삭제

* GenStudio 작업 영역에 대한 작업 영역 구성, 레코드 유형, 보기 및 필드를 업데이트하는 것은 Workfront Planning 작업 영역을 해당 요소로 업데이트하는 것과 동일합니다.

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## Workfront Planning에서 GenStudio 레코드 유형 관리

>[!NOTE]
>
>GenStudio 작업 영역을 관리하기 전에 문서 [Workfront Planning 및 GenStudio for Performance Marketing 통합 시작](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)을 참조하십시오.

1. GenStudio에 액세스할 수 있는 사용자로 Workfront에 로그인합니다.
1. 왼쪽 상단의 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 계획]**&#x200B;을 클릭합니다.

   Workfront Planning 기본 페이지가 열립니다.

1. **다른 작업 영역**&#x200B;을 클릭하고 **System**&#x200B;에서 만든 표시가 있고 카드에 **GenStudio** 태그가 있는 작업 영역을 찾습니다.

   ![태그가 있는 GenStudio 작업 영역 카드](assets/genstudio-card-with-tag-highlighted.png)

1. **GenStudio 작업 영역 카드**&#x200B;를 클릭하여 Workfront Planning에서 GenStudio 작업 영역을 엽니다.
1. 기본적으로 다음 GenStudio 레코드 유형이 만들어지고 Workfront Planning에서 표시됩니다.

   * 캠페인
   * 제품
   * 활성화
   * 채널
   * 지역

   GenStudio 레코드 유형 카드에 원래 GenStudio에서 생성되었다는 표시가 있습니다.

   <!--check screen shot-->

   ![태그가 있는 GenStudio 레코드 유형 카드](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. 해당 유형의 레코드를 보려면 레코드 유형 카드를 클릭합니다.

1. 다음 중 하나를 수행하십시오.

   * 레코드 종류 페이지의 오른쪽 상단에서 **공유**&#x200B;를 클릭한 후 다음 중 하나를 클릭합니다.
      * 레코드 형식에 대한 링크를 공유하려면 **보기 링크를 복사**&#x200B;하십시오.
      * CSV 또는 Excel 파일로 내보내려면 **현재 보기를 내보냅니다**.
테이블 뷰만 내보낼 수 있습니다. <!--check on this later; is this true or are there more options in the Share button-->

   * GenStudio 레코드 형식에 대한 보기를 만들려면 **+ 보기**&#x200B;를 클릭하십시오.

     자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

   * **전체 화면** 아이콘 ![전체 화면으로 전체 보기 열기](assets/open-full-screen-icon.png)를 클릭하여 전체 화면 모드로 보기를 엽니다.

   * 모든 보기에서 보기 요소를 관리합니다.

     예를 들어 사용 가능한 경우 보기의 필터, 그룹화, 정렬, 설정을 변경할 수 있습니다.

     자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

   * 표 또는 타임라인 보기에서 레코드를 추가합니다.

     처음부터 만들거나 CSV 또는 Excel 파일을 가져와야 레코드를 만들 수 있습니다.

     자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.

     레코드는 Workfront 및 GenStudio 모두에서 볼 수 있습니다.

   * 테이블 보기에서 인라인으로 레코드를 편집하거나 레코드를 클릭하여 세부 정보 페이지를 엽니다.

     자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

   * 테이블 보기에서 레코드를 삭제합니다.

     자세한 내용은 [레코드 삭제](/help/quicksilver/planning/records/delete-records.md)를 참조하십시오.

     삭제된 레코드는 Workfront에서 삭제할 경우 Workfront Planning의 테이블 보기 휴지통에서 복구할 수 있습니다.

     자세한 내용은 [삭제된 레코드 복원](/help/quicksilver/planning/records/restore-deleted-records.md)을 참조하세요.

   * 필드를 정렬하거나 숨기려면 테이블 보기의 필드 위로 마우스를 가져갑니다.

     >[!NOTE]
     >
     >GenStudio에서 관리 권한이 있는 경우에만 필드의 구성을 편집하고 필드를 추가할 수 있습니다. <!--check to see if this is true??-->
