---
title: 기록 유형에 대한 교차 작업 영역 기능 구성
description: 레코드 유형을 다른 작업 공간에 추가하거나 다른 작업 공간에서 연결할 수 있습니다.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 8f4c1be156094d18df4bc3628d4f1fca90372119
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# 레코드 유형에 대한 작업 영역 간 기능 구성

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

Adobe Workfront Planning에서 다른 작업 공간에 추가되거나 다른 작업 공간에서 연결될 레코드 유형을 지정할 수 있습니다.

작업 영역 관리자가 레코드 유형을 다른 작업 영역에서 연결하거나 다른 작업 영역으로 가져오려면 먼저 레코드 유형의 작업 영역 간 기능을 정의해야 합니다.

레코드 유형을 만들거나 편집할 때 레코드 유형의 작업 영역 간 기능을 정의합니다.

자세한 내용은 다음 문서 중 하나를 참조하십시오.

* [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)
* [레코드 유형 편집](/help/quicksilver/planning/architecture/edit-record-types.md)

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
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
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 다른 작업 공간에 레코드 유형 추가 구성

작업 영역 관리자는 레코드 유형을 작성하거나 편집할 때 다른 작업 영역에 추가할 레코드 유형을 구성할 수 있습니다.

다른 작업공간에 레코드 유형 추가를 구성할 때 작업공간 관리자는 해당 작업공간에서 관리하는 작업공간 중 하나로 레코드 유형 및 모든 정보를 가져올 수 있습니다.

레코드 유형을 편집할 때 다른 작업 공간에 레코드 유형 추가를 구성하려면 다음과 같이 하십시오.

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업 영역을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다.
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 연 다음 레코드 유형 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭합니다.
1. **편집**&#x200B;을 클릭합니다.

   ![레코드 종류 카드의 추가 메뉴 옵션](assets/more-menu-options-from-record-type-card.png)

1. **레코드 종류 편집** 상자에서 **고급 설정** 탭을 선택합니다.
1. **다른 작업 영역에 이 레코드 형식을 추가할 수 있도록 허용** 설정을 사용합니다.

   ![다른 작업 영역에 추가를 사용하여 고급 설정 편집](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. **이 레코드 종류를 자신이 관리하는 작업 영역에 추가할 수 있는 사용자를 선택하십시오** 필드에서 이 레코드 종류를 자신이 관리하는 작업 영역에 추가할 사용자를 추가하십시오.

   필드에 이름이 자동으로 추가됩니다.

   이 레코드 유형을 추가할 개인 사용자, 그룹, 팀, 작업 역할 또는 회사를 자신이 관리하는 작업 공간에 추가할 수 있습니다.

   레코드 유형을 저장한 후 이 필드를 편집할 수 있습니다.
1. (선택 사항) **이 레코드 종류를 관리할 작업 영역에 추가할 수 있는 사용자를 선택하십시오** 필드에서 이름을 제거합니다.

1. **저장**&#x200B;을 클릭합니다.

   다음과 같은 상황이 발생합니다.

   * 이제 지정한 사용자가 레코드 종류 및 해당 필드를 다른 작업 영역에 추가할 수 있습니다.
   * 레코드 유형 카드는 구성에 지정한 관리자가 있는 모든 작업 영역에 레코드 유형을 추가할 수 있음을 나타내는 전역 아이콘 ![전역 레코드 유형 아이콘](assets/global-icon.png)을 표시합니다.
   * 시스템 생성 **Workspace** 필드가 레코드 형식에 추가되었습니다.

     Workspace 필드에는 각 레코드가 생성된 작업 영역이 표시됩니다.

     이 필드는 읽기 전용이므로 삭제할 수 없습니다.

## 다른 작업 영역의 레코드 유형에 대한 연결 구성

레코드 유형을 작성하거나 편집할 때 다른 작업 공간에서 연결하도록 레코드 유형을 구성할 수 있습니다.

레코드 유형을 편집할 때 다른 작업 공간에서 연결하도록 레코드 유형을 구성하려면 다음과 같이 하십시오.

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업 영역을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류의 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에서 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 열고 레코드 유형 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다.

   ![레코드 종류 카드의 추가 메뉴 옵션](assets/more-menu-options-from-record-type-card.png)

1. **레코드 종류 편집** 상자에서 **고급 설정** 탭을 선택합니다.
1. **다른 작업 영역에서 이 레코드 형식에 연결할 수 있도록 허용** 설정을 사용합니다. <!-- check the setting name, this is the suggested UI text to be edited by Lilit and team-->

   ![다른 작업 공간에서 연결을 사용하도록 설정한 고급 설정 탭](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   활성화되면 기록 유형에 액세스하고 다른 작업 공간에서 연결할 수 있습니다.

1. 레코드 종류에 액세스할 수 있는 작업 공간을 선택합니다. 다음 옵션 중에서 선택합니다.

   * **시스템 전체**: 사용자는 관리 권한이 있는 모든 작업 영역에서 이 레코드 형식에 연결할 수 있습니다.
   * **특정 작업 영역**: 작업 영역 관리자가 이 레코드 형식에 연결할 수 있는 작업 영역의 이름을 추가합니다.
1. **편집**&#x200B;을 클릭합니다.

   다음과 같은 상황이 발생합니다.

   * 이제 지정한 작업 영역에서 레코드 유형 및 해당 필드를 연결할 수 있습니다.
   * 레코드 유형 카드에 작업 영역 간 연결 아이콘 ![작업 영역 간 연결 아이콘](assets/connect-from-other-workspaces-icon.png)이 표시되어 구성에 지정한 작업 영역에서 레코드 유형을 연결할 수 있음을 나타냅니다.






