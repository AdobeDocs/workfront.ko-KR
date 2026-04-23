---
title: 작업 공간 만들기
description: 작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다. 레코드 유형은 작업 영역의 섹션별로 구성됩니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---


# 작업 공간 만들기

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

Adobe Workfront Planning에서 작업 공간은 팀이 작업을 계획하는 중앙 집중식 위치입니다.

작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다.

작업 영역에 대한 일반적인 정보는 [작업 영역 개요](/help/quicksilver/planning/architecture/workspaces-overview.md)를 참조하십시오.

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
<p>모든 Workfront 또는 워크플로우 패키지</p> 
<p>모든 Workfront Planning 패키지</p>
<p>한 번에 여러 작업 공간을 만들 수 있는 Workfront Planning Prime 이상 패키지</p>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   <p>시스템 관리자가 모범 사례 템플릿 번들을 사용하여 한 번에 여러 작업 공간을 만들 수 있음</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++   

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## 작업 영역 만들기

작업공간을 만들고 여기에 레코드 유형을 추가하여 Workfront Planning에서 객체를 구성할 수 있습니다.

작업 영역 편집에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.

다음과 같은 방법으로 작업 공간을 만들 수 있습니다.

* 처음부터 또는 템플릿에서 작업 공간 만들기

  자세한 내용은 이 문서의 [처음부터 작업 영역 만들기 또는 템플릿에서 작업 영역 만들기](#create-a-workspace-from-scratch-or-from-a-template) 섹션을 참조하십시오.
* AI 기반의 Planning Designer을 사용하여 작업 공간을 하나 만듭니다. 이 기능은 현재 Beta 프로그램의 제한된 고객만 사용할 수 있습니다.

  자세한 내용은 [Adobe Workfront Planning Designer 시작](/help/quicksilver/planning/general/planning-ai-designer.md)을 참조하십시오.

* 모범 사례 다중 작업 영역 템플릿 번들을 사용하여 여러 작업 영역 만들기

  자세한 내용은 이 문서의 [모범 사례 다중 작업 영역 템플릿 번들을 사용하여 여러 작업 영역 만들기](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) 섹션을 참조하십시오

  >[!TIP]
  >
  >모범 사례 템플릿 번들을 사용하는 경우에만 한 번에 여러 작업 공간을 만들 수 있습니다.

### 처음부터 또는 템플릿에서 작업 공간 만들기

{{step1-to-planning}}

1. **작업 영역 만들기** 클릭

   작업 공간 만들기 상자가 표시됩니다. 작업공간을 처음부터 만들거나 사용 가능한 템플릿 중 하나를 사용하여 만들 수 있습니다.

1. (선택 사항 및 조건부) 미리 정의된 다음 작업 영역 템플릿 내에서 **미리 보기**&#x200B;를 클릭합니다.

   * 기본: 마케팅 관리
   * 고급: 마케팅 관리
   * 엔터프라이즈: 마케팅 관리
   * 영업 관리
   * 제품 관리

   템플릿 미리보기 상자가 열립니다.

   각 템플릿과 연관된 운영 레코드 유형, 분류 및 필드 수가 표시됩니다.

   ![작업 영역 템플릿 미리 보기](assets/previewing-a-workspace-template.png)

   Workfront Planning 작업 영역 템플릿에 대한 자세한 내용은 [작업 영역 템플릿 목록](/help/quicksilver/planning/architecture/workspace-templates.md)을 참조하십시오.

1. 템플릿 미리 보기 상자에서 **템플릿 사용**&#x200B;을 클릭하여 선택한 템플릿에서 작업 영역 만들기를 시작합니다

   또는

   **뒤로**&#x200B;를 클릭한 다음 **새 작업 영역**&#x200B;을 클릭하여 작업 영역을 처음부터 만듭니다.

   다음 유형의 작업 공간에 대한 하나가 만들어집니다.

   * 처음부터 작업 영역을 만들 때 레코드 형식을 수동으로 추가할 수 있는 빈 작업 영역(**제목 없는 Workspace**)입니다.
   * 선택한 템플릿 이름을 따라 이름이 지정되고 샘플 레코드 유형으로 채워진 작업 영역입니다. 레코드 유형 및 작업 영역을 추가로 사용자 지정할 수 있습니다.

   Workfront 관리자의 경우 새 작업 영역이 내가 있는 **작업 영역** 탭에 표시됩니다.

   작업 영역을 만들 수 있는 다른 모든 사용자의 경우 **작업 영역** 영역에 새 작업 영역이 표시됩니다.

1. 새 작업 영역의 헤더에서 작업 영역 이름 내부를 클릭하여 이름을 변경한 다음 Enter 키를 누릅니다.

1. (선택 사항 및 조건부) 템플릿에서 작업 영역을 만든 경우 **작업 레코드 종류** 또는 **분류** 섹션의 이름 내부를 클릭합니다

   또는

   섹션의 이름을 마우스로 가리킨 다음 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **이름 바꾸기**&#x200B;를 클릭하여 섹션의 이름을 변경합니다.

   >[!TIP]
   >
   >섹션을 만들지 않았더라도 작업 영역에서 섹션의 이름을 변경할 수 있습니다.

   작업 영역 섹션 편집을 포함하여 작업 영역 편집에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.

1. (선택 사항) **레코드 종류 추가**&#x200B;를 클릭하여 모든 섹션의 작업 영역에 레코드 종류를 추가합니다.

   자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   작업 영역의 레코드 형식을 편집하고 삭제하는 방법에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.

1. (선택 사항) 새 작업 공간 왼쪽에 있는 뒤로 화살표를 클릭하여 Planning 기본 페이지를 엽니다. **내가 있는 작업 영역** 탭에서 새 작업 영역에 대한 새 작업 영역 카드가 만들어집니다.

   작업공간을 생성한 사용자의 이름은 작업공간 카드에 소유자로 저장됩니다.

   >[!TIP]
   >
   >**System**&#x200B;에서 만든 대로 Adobe Admin Console에 추가되지 않은 Workfront 전용 사용자가 만든 작업 영역입니다.
   >

### 모범 사례 다중 작업 영역 템플릿 번들을 사용하여 여러 작업 영역 만들기

>[!IMPORTANT]
>
>모범 사례 템플릿 번들을 사용하여 한 번에 여러 작업 공간을 만드는 것은 다음 전제 조건을 충족해야 사용할 수 있습니다.
>
>* 조직에서 Workfront Planning Prime 또는 Ultimate 패키지를 구매했습니다.
>* 시스템 관리자입니다.

다중 작업 영역 템플릿 번들을 사용하여 한 번의 클릭으로 6개의 작업 영역을 만들 수 있습니다.

번들에 포함된 템플릿에는 Planning 구현을 시작하는 데 도움이 되는 작업 공간, 레코드 유형, 레코드, 보기 및 필드가 포함되어 있습니다.

>[!IMPORTANT]
>
>번들에 포함된 작업 공간 및 레코드의 이름은 예이며 사용자 환경의 반영이 아닙니다.
>
>레코드 유형 및 필드의 이름은 권장 사항에 따라 모든 산업에서 구현을 위한 표준으로 모든 조직에서 사용할 수 있습니다.
>

{{step1-to-planning}}

1. **작업 영역 만들기** 클릭

   작업 공간 만들기 상자가 표시됩니다. 작업공간을 처음부터 만들거나 사용 가능한 템플릿 중 하나를 사용하여 만들 수 있습니다.

1. **여기에서 시작(권장)** 영역에서 **작업 영역 설정 검토**&#x200B;를 클릭합니다.
1. (선택 사항) 미리 정의된 다음 작업 영역 템플릿 내에서 **미리 보기**&#x200B;를 클릭하여 각 템플릿에 대한 미리 보기 상자를 엽니다.

   * &#x200B;1. 글로벌 분류 및 분류

     전역 분류 및 분류 템플릿에는 Workfront Planning의 성공적인 구현을 위해 사용자 환경에서 생성하는 것이 권장되는 모든 레코드 유형 및 필드가 포함되어 있습니다.

     나중에 사용자가 만든 다른 작업 영역에서 이 템플릿의 레코드 유형을 연결하거나 가져올 수 있습니다.
   * &#x200B;2. Fréscopa 글로벌 마케팅
   * 3.Fréscopa 소셜 마케팅
   * 4.Fréscopa 미디어 및 홍보
   * 5.Fréscopa 글로벌 이벤트
   * 6.Fréscopa 경영진 리더십

1. 각 작업 영역 템플릿에 대해 **미리 보기** 상자를 연 후 [뒤로]를 클릭하여 **작업 영역 만들기** 상자로 돌아가거나 [템플릿 사용]을 클릭하여 번들에 포함된 템플릿을 사용하고 작업 영역을 만듭니다.

   작업 영역이 만들어지고 시스템 관리자의 **내가 있는 작업 영역** 및 **모든 작업 영역** 탭에 표시됩니다. 모든 Standard License 사용자는 시스템 관리자가 작업 공간을 만들고 새 작업 공간을 공유하면 작업 공간 영역에서 작업 공간을 볼 수 있습니다.

1. 생성한 작업 영역을 편집하고 조직에 해당하는 레코드 유형, 레코드, 보기 및 필드를 추가합니다.

   Workfront을 구현하는 모범 사례에 대한 자세한 내용은 [Adobe Workfront 계획 모범 사례: 문서 인덱스](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) 섹션의 문서를 참조하십시오.

   작업 영역 편집에 대한 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.



