---
title: 레코드 유형 편집
description: 레코드 유형을 저장한 후 편집할 수 있습니다. 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 2%

---


# 레코드 유형 편집

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. 사용자 또는 다른 사용자가 만든 레코드 유형의 모양을 편집할 수 있습니다. Workfront Planning 레코드 유형을 만드는 방법에 대한 자세한 내용은 [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항 보기..

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
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준 </p>
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
   <td>   <p>작업 영역 <span class="preview"> 및 레코드 종류</span>에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
   <p>시스템 관리자만 다른 작업 영역에서 레코드 유형을 연결할 수 있습니다.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## 레코드 유형 편집

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업 영역을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류의 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에서 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**을 클릭합니다
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 열고 레코드 유형 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다.

   ![레코드 종류 카드의 추가 메뉴 옵션](assets/more-menu-options-from-record-type-card.png)

1. **레코드 종류 편집** 상자에서 기본적으로 **모양** 탭이 열립니다.

   ![레코드 종류 상자 모양 편집 탭 ](assets/edit-record-type-box-appearance-tab.png)

   **모양** 탭에서 다음 정보를 업데이트합니다.

   * 필요한 경우 레코드 유형 이름을 편집합니다. <!--did they add a field label for this?-->
   * **설명**: 레코드 형식에 대한 자세한 내용을 포함하여 설명을 편집하거나 추가합니다.
   * 레코드 종류와 관련된 아이콘의 색 및 모양을 편집합니다. 다음을 수행합니다.
      * 레코드 유형을 식별할 색상을 선택합니다. 레코드 유형 아이콘의 색상입니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

1. (조건부) 시스템 관리자인 경우 **레코드 종류 편집** 상자에서 **고급 설정** 탭을 클릭합니다. <!--the info here is duplicated in the Create record types article-->

   ![레코드 종류 상자 고급 설정 탭](assets/edit-record-type-box-advanced-settings-tab.png)

1. (조건부) **고급 설정** 탭에서 다음 정보를 업데이트합니다.

   * **다른 작업 영역에서 연결** 설정을 사용하도록 설정합니다. 활성화되면 기록 유형에 액세스하고 다른 작업 공간에서 연결할 수 있습니다.
   * 레코드 종류에 액세스할 수 있는 작업 공간을 선택합니다. 다음 옵션 중에서 선택합니다.

      * **시스템 전체**: 사용자는 관리 권한이 있는 모든 작업 영역에서 이 레코드 형식에 연결할 수 있습니다.
      * **특정 작업 영역**: 작업 영역 관리자가 이 레코드 형식에 연결할 수 있는 작업 영역의 이름을 추가합니다.

1. **저장**&#x200B;을 클릭합니다.

   작업 영역의 레코드 유형 카드에 오른쪽 상단의 연결 아이콘 ![다른 작업 영역에서 연결](assets/connect-from-other-workspaces-icon.png)이 표시되어 이제 다른 작업 영역에서 레코드에 액세스할 수 있음을 나타냅니다.

1. (선택 사항) 작업 영역 영역에서 레코드 유형 카드를 클릭하여 레코드 유형의 페이지를 연 다음 헤더에서 레코드 유형의 이름을 변경합니다.

1. (선택 사항) 다른 레코드 유형을 편집하려면 레코드 유형 페이지에서 레코드 유형 이름의 오른쪽에 있는 아래쪽 화살표를 확장하고 레코드 유형을 검색한 다음 목록에 표시될 때 선택합니다.

   ![검색 상자가 있는 레코드 종류 페이지의 레코드 종류 드롭다운](assets/record-type-drop-down-on-record-type-page-with-search-box.png)