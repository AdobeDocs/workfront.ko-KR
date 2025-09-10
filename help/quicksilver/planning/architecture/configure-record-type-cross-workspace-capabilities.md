---
title: 기록 유형에 대한 교차 작업 영역 기능 구성
description: 레코드 유형을 다른 작업 공간에 추가하거나 다른 작업 공간에서 연결할 수 있습니다.
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# 레코드 유형에 대한 작업 영역 간 기능 구성

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

다음은 레코드 유형의 작업 영역 간 기능입니다.

* 레코드 유형을 중앙 집중식으로 지정할 수 있습니다. 사용자는 자신이 관리할 수 있는 다른 작업 공간에 중앙 집중식 레코드 유형을 추가할 수 있습니다.
* 레코드 종류를 연결 가능한 것으로 지정할 수 있습니다. 사용자는 다른 작업 영역에서 이 레코드 유형에 연결할 수 있습니다.

작업 영역 관리자가 레코드 유형을 다른 작업 영역에서 연결하거나 다른 작업 영역에 추가하기 전에 먼저 레코드 유형의 작업 영역 간 기능을 정의해야 합니다.

레코드 유형을 만들거나 편집할 때 레코드 유형의 작업 영역 간 기능을 정의합니다.

자세한 내용은 다음 문서 중 하나를 참조하십시오.

* [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)
* [레코드 유형 편집](/help/quicksilver/planning/architecture/edit-record-types.md)

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
<ul><li><p>모든 Workfront 패키지</p></li>
And
<li><p>Planning Plus 패키지</p></li></ul>
또는:
<ul><li><p>모든 워크플로우 패키지</p> </li>
And
<li><p>Prime 또는 Ultimate 패키지 계획</p></li></ul>
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++   

## 중앙 집중식 레코드 유형 구성

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

작업 영역 관리자는 레코드 유형을 중앙 집중식 레코드 유형으로 구성할 수 있습니다. 다른 작업 공간에 중앙 집중식 레코드 유형을 추가할 수 있습니다.

작업 영역 관리자는 관리하는 작업 영역에 중앙 집중식 레코드 유형을 추가할 수 있습니다. 레코드 유형의 원본 필드도 추가됩니다.

사용자는 Contribute 권한이 있고 원래 작업 영역을 포함하여 중앙 집중식 레코드 유형이 추가된 작업 영역에서 중앙 집중식 레코드 유형에 레코드를 추가할 수 있습니다. 보기 권한만 있는 작업 영역에서 레코드를 볼 수 있습니다.

자세한 내용은 [중앙 집중식 레코드 종류 개요](/help/quicksilver/planning/architecture/centralized-record-types-overview.md)를 참조하세요.

레코드 유형 추가를 중앙 집중식 레코드 유형으로 구성하려면 다음을 수행합니다.

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업공간을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다.
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 연 다음 레코드 유형 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭합니다.
1. **편집**&#x200B;을 클릭합니다.

   ![레코드 종류 카드의 추가 메뉴 옵션](assets/more-menu-options-from-record-type-card.png)

   >[!TIP]
   >
   >레코드 유형이 이미 중앙 집중식 레코드 유형으로 지정되어 있고 다른 작업 공간에 추가된 경우 편집 옵션이 흐리게 표시됩니다.

1. **레코드 종류 편집** 상자에서 **고급 설정** 탭을 선택합니다.
1. **다른 작업 영역에 이 레코드 형식을 추가할 수 있도록 허용** 설정을 사용합니다.

   ![다른 작업 영역에 추가를 사용하여 고급 설정 편집](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >다른 작업 영역에 중앙 집중식 레코드 유형을 추가한 후에는 이 설정을 더 이상 비활성화할 수 없습니다.

1. **이 레코드 형식을 자신이 관리하는 작업 영역에 추가할 수 있는 사용자 선택** 필드에서 이 레코드 형식을 자신이 관리하는 작업 영역에 추가하도록 허용할 엔터티를 추가합니다.

   필드에 이름이 자동으로 추가됩니다.

   이 레코드 유형을 자신이 관리하는 작업 공간에 추가하도록 허용할 개인 사용자, 그룹, 팀, 작업 역할 또는 회사를 추가할 수 있습니다.

   이 설정을 활성화할 수 있는 엔터티(사용자, 팀, 그룹, 역할 또는 회사)를 하나 이상 지정해야 합니다.

   레코드 유형을 저장한 후 이 필드를 편집할 수 있습니다.

1. (선택 사항) **이 레코드 종류를 관리할 작업 영역에 추가할 수 있는 사용자를 선택하십시오** 필드에서 이름을 제거합니다.

1. **저장**&#x200B;을 클릭합니다.

   다음과 같은 상황이 발생합니다.

   * 이제 지정한 사용자가 레코드 종류 및 해당 필드를 다른 작업 영역에 추가할 수 있습니다.

   >[!NOTE]
   >
   >레코드 유형의 모양 및 설정과 원본 필드는 원본 작업 공간에서만 편집할 수 있습니다.

   * 레코드 유형 카드에 중앙 집중식 아이콘 ![중앙 집중식 레코드 유형 아이콘](assets/global-icon.png)이 표시되어 레코드 유형을 다른 작업 영역에 추가할 수 있음을 나타냅니다.
   * 시스템 생성 **Workspace** 필드가 레코드 종류 및 해당 레코드의 세부 정보에 대한 테이블 보기에 추가됩니다.

     Workspace 필드에는 각 레코드가 생성되는 작업 영역이 표시됩니다.

     이 필드는 읽기 전용이므로 삭제할 수 없습니다.
1. (선택 사항) 다른 작업 영역으로 이동하여 기존 레코드 유형을 사용하여 레코드 유형을 만듭니다. 위의 단계에서 활성화한 레코드 유형을 선택합니다.

   자세한 내용은 [기존 레코드 종류 추가](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md)를 참조하십시오.

## 연결 가능한 레코드 유형 구성

<!--this is a UI term; don't change the title of this section-->

레코드 유형을 작성하거나 편집할 때 다른 작업 영역에서 연결할 레코드 유형을 구성할 수 있습니다.

레코드 유형을 편집할 때 다른 작업 공간에서 연결하도록 레코드 유형을 구성하려면 다음과 같이 하십시오.

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업공간을 클릭합니다.

   작업 영역 페이지가 열리고 레코드 유형이 표시됩니다.
1. 다음 중 하나를 수행하십시오.

   * 레코드 종류의 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에서 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다
또는
   * 레코드 유형 카드를 클릭하여 레코드 유형 페이지를 열고 레코드 유형 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**&#x200B;을 클릭합니다.

   ![레코드 종류 카드의 추가 메뉴 옵션](assets/more-menu-options-from-record-type-card.png)

1. **레코드 종류 편집** 상자에서 **고급 설정** 탭을 선택합니다.
1. **다른 작업 영역에서 이 레코드 형식에 연결 허용** 설정을 사용합니다. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![다른 작업 공간에서 연결을 사용하도록 설정한 고급 설정 탭](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   활성화되면 레코드 유형에 액세스하고 다른 작업 공간에서 연결할 수 있습니다.

1. 레코드 종류에 액세스할 수 있는 작업 공간을 선택합니다. 다음 옵션 중에서 선택합니다.

   * **시스템 전체**: 사용자는 관리 권한이 있는 모든 작업 영역에서 이 레코드 형식에 연결할 수 있습니다.
   * **특정 작업 영역**: 작업 영역 관리자가 이 레코드 형식에 연결할 수 있는 작업 영역의 이름을 추가합니다.
1. **저장**&#x200B;을 클릭합니다.

   다음과 같은 상황이 발생합니다.

   * 이제 지정한 작업 영역에서 레코드 유형 및 해당 필드에 연결할 수 있습니다.
   * 레코드 유형 카드는 구성에 지정한 모든 작업 영역에서 레코드 유형을 연결할 수 있음을 나타내는 작업 영역 간 연결 아이콘 ![작업 영역 간 연결 아이콘](assets/connect-from-other-workspaces-icon.png)을 표시합니다.

   지정된 작업공간에서에 연결할 수 있는 레코드 유형이 제공됩니다.
1. (선택 사항) 다른 작업 영역으로 이동하여 위의 단계에서 작업 영역 간 연결을 활성화한 레코드 유형에 연결을 추가합니다.

   자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.









