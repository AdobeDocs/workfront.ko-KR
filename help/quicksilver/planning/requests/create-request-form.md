---
title: Adobe Workfront Planning에서 요청 양식 만들기
description: Adobe Workfront Planning 영역에서 레코드 유형을 선택한 후 해당 레코드 유형과 연결된 요청 양식을 작성하고 이에 대한 링크를 다른 내부 또는 외부 사용자와 공유할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# Adobe Workfront Planning에서 요청 양식 만들기

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Adobe Workfront Planning 영역에서 레코드 유형을 선택한 후 요청 양식을 만들어 해당 레코드 유형과 연결할 수 있습니다. 그런 다음 다른 내부 또는 외부 사용자와 링크를 공유할 수 있습니다. <!--double-check on the external part of it-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

Workfront Planning에 액세스하려면 다음 항목이 있어야 합니다.

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
<p>임의 </p>   </td>

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
   <td>
   <p>표준</p>
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
   <td>
   <ul>
   <li><p>작업 공간에 대한 권한 관리</p></li>
    <li><p>시스템 관리자는 자신이 만들지 않은 작업 공간을 관리할 수 있습니다. </p></li>
    </ul>
   <p>Workfront Planning 객체의 권한 공유에 대한 자세한 내용은  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning의 공유 권한 개요</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 유형에 대한 요청 양식 만들기

{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.

1. 페이지 헤더의 레코드 형식 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **요청 양식 만들기**&#x200B;를 클릭합니다.
1. 요청 양식 이름을 업데이트합니다. 기본적으로 양식 이름은 **제목 없는 요청 양식**&#x200B;입니다. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (선택 사항) 요청 양식에 대해 **설명**&#x200B;을(를) 추가합니다.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Click **Create**. 선택한 레코드 유형에 대한 요청 양식이 열립니다.

   요청 양식에는 기본적으로 다음 정보가 포함되어 있습니다.

   * **기본 섹션**: Workfront이 요청 양식에 적용하는 기본 섹션 구분입니다. 기본 섹션의 이름을 변경하거나 제거할 수 없습니다.
   * **제목** 필드: Workfront에서 요청을 식별하는 필드입니다. 이 기능은 아직 사용할 수 없습니다.
   * 레코드 유형과 연결된 모든 필드.

   요청 양식에 포함된 필드는 이 레코드 유형에 요청을 제출하는 모든 사람에게 표시됩니다.

1. (선택 사항) **제목** 필드는 Workfront Planning에 표시되지 않으므로 제거합니다. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. 제거할 양식의 모든 필드 위에 마우스를 올려 놓습니다. 양식 왼쪽의 **필드** 탭에 추가됩니다.
1. 필드를 클릭한 다음 양식의 오른쪽에 있는 컨트롤을 사용하여 필드에 대한 다음 정보를 정의합니다.

   * **레이블**: 요청 양식에 표시되는 필드 이름입니다. 레코드 필드의 이름은 변경되지 않습니다.
   * **지침**: 필드에 대한 정보를 더 추가합니다.
   * **필수 필드 만들기**: 선택한 경우 필드에 값이 있어야 합니다. 그렇지 않으면 양식을 제출할 수 없습니다.
   * **논리 추가**: 필드가 표시되거나 숨겨지기 위해 충족되어야 하는 조건을 정의합니다.

1. 양식 오른쪽에 있는 콘텐츠 요소 탭을 클릭하고 다음 요소 중 하나를 추가합니다.

   * 설명 텍스트
   * 섹션 구분

   사용자 지정 양식을 작성하는 방법에 대한 자세한 내용은 [양식 디자이너를 사용하여 양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)을 참조하십시오.





