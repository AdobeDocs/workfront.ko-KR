---
title: 레코드 유형 편집
description: 레코드 유형을 저장한 후 편집할 수 있습니다. 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: bda3dc43828032fd5a8862b12d851c56cf9b6cbd
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# 레코드 유형 편집

{{planning-important-intro}}

레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. 사용자 또는 다른 사용자가 만든 레코드 유형의 모양을 편집할 수 있습니다. Workfront Planning 레코드 유형을 만드는 방법에 대한 자세한 내용은 [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
   <p> Adobe Workfront</p> <p>Adobe Workfront Planning 레코드 유형을 Experience Manager Assets과 연결하려면 Adobe Experience Manager Assets 라이선스가 있어야 하며, 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>새로운 기능: 표준</p>
   <p>현재: 플랜</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>를 참조하십시오. </p>  
</td>
  </tr>

</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 레코드 유형 편집

{{step1-to-planning}}

1. 레코드 유형을 편집할 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.
1. 레코드 종류의 카드 위에 마우스를 올려 놓고 레코드 종류 카드의 오른쪽 상단에서 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭합니다.

   ![](assets/more-menu-options-from-record-type-card.png)

1. **레코드 종류 편집** 상자에서 다음 정보를 업데이트하십시오.

   * 필요한 경우 레코드 유형 이름을 편집합니다. <!--did they add a field label for this? -->
   * **설명**: 레코드 형식에 대한 자세한 내용을 포함하여 설명을 편집하거나 추가합니다.
   * 레코드 종류와 관련된 아이콘의 색 및 모양을 편집합니다. 다음을 수행합니다.
      * 레코드 유형을 식별할 색상을 선택합니다. 레코드 유형 아이콘의 색상입니다. 기본적으로 회색이 선택되어 있습니다.
      * 목록에서 아이콘을 선택하거나 아이콘 이름을 입력하여 아이콘이 나타내는 내용을 설명한 다음 표시될 때 선택합니다. 레코드 유형의 아이콘입니다. 기본적으로 파일 아이콘이 선택되어 있습니다.

     ![](assets/update-record-type-box.png)

1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 작업 영역 영역에서 레코드 유형 카드를 클릭하여 레코드 유형의 페이지를 엽니다.
1. 레코드 종류 이름의 오른쪽에 있는 **자세히** 메뉴를 클릭한 다음 **편집**&#x200B;을 클릭하여 레코드 종류에 대한 정보를 업데이트합니다.

   >[!TIP]
   >
   >   헤더에서 레코드 유형의 이름을 바꿀 수 있습니다.

   ![](assets/more-menu-options-from-record-type-page.png)

   <!--check this screen shot - not sure this is valid ???-->

1. (선택 사항) 다른 레코드 유형을 편집하려면 레코드 유형 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드 유형을 검색한 다음 목록에 표시될 때 선택합니다.
