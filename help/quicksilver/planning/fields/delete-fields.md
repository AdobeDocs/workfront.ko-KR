---
title: 필드 삭제
description: Adobe Workfront Planning에서 더 이상 관련이 없는 사용자 정의 필드를 삭제할 수 있습니다.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EusoK7-jmYJHg9nqyvvQamsfVeUy802p36EyDmLGwik
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 733
ht-degree: 1%

---

# 필드 삭제

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


{{planning-important-intro}}

Adobe Workfront Planning에서 사용자 정의 필드를 만들어 레코드에 대한 정보를 저장할 수 있습니다.

Workfront Planning에서 사용자 정의 필드를 만드는 방법에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

더 이상 관련이 없는 Workfront Planning 필드를 삭제할 수 있습니다.

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
<li><p>모든 워크플로우 및 모든 Planning 패키지</p></li></ul>

<p>글로벌 레코드 유형에서 필드를 삭제하려면</p>
<ul><li><p>모든 Workfront 패키지 및 Planning Plus 패키지</p></li>
또는
<li><p>모든 워크플로우 및 Planning Prime 및 Ultimate 패키지</p></li></ul>

<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table>
-->

## Workfront Planning 필드 삭제에 대한 고려 사항:

* 레코드 유형 테이블 보기에서만 필드를 삭제할 수 있습니다.
* 레코드의 기본 필드는 삭제할 수 없습니다.
* 필드에 저장된 모든 정보는 삭제되며 복구할 수 없습니다.
* 연결된 레코드 필드를 삭제하면 연결된 모든 조회 필드도 사용자가 연결한 레코드 유형에서 삭제됩니다. 연결하는 레코드 유형의 연결된 레코드 필드도 연결하는 레코드에서 삭제됩니다.

  예를 들어, Campaigns를 Product라는 다른 레코드 유형에 연결하고 Campaign에서 Product connected 필드 및 Product의 Status 조회 필드를 삭제하면 다음 항목이 삭제됩니다.

   * 캠페인의 제품 연결 필드
   * 캠페인의 제품 상태 조회 필드
   * 제품의 Campaign 연결 필드

  자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* 보조 작업 영역에서 보조 작업 영역에 추가된 글로벌 레코드에서는 필드를 삭제할 수 없습니다.

## 필드 삭제

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. 레코드 필드를 삭제할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.

1. 기록 유형의 카드를 클릭합니다.

1. (조건부) 아직 선택하지 않은 경우 레코드 유형 페이지에서 **테이블 보기**&#x200B;의 탭을 클릭합니다.

   레코드 유형과 연관된 모든 기존 레코드는 테이블 뷰의 행에 표시됩니다.

1. 열 헤더에서 삭제할 필드를 찾고 열 헤더 위로 마우스를 가져간 다음 필드 이름 뒤에 있는 아래쪽 방향 화살표를 클릭합니다.

   ![강조 표시된 테이블 헤더의 필드 이름 뒤 화살표 메뉴](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. **삭제**&#x200B;를 클릭합니다. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. <span class="preview">(조건부) 삭제하려는 필드가 요청 양식의 일부인 경우 **필드 삭제** 상자가 표시되어 변경 사항의 영향을 받을 양식을 나타냅니다. 다음 중 하나를 실행하십시오.</span>

   <div class="preview">

   * 오른쪽 화살표를 클릭하여 변경의 영향을 받는 양식을 표시한 다음, 양식 이름을 클릭하여 양식을 새 탭에서 열고 필드를 양식에 유지할지 또는 양식을 추가로 변경할지 결정합니다.
   * 필드가 표시되는 모든 영역에서 필드를 삭제하려면 **삭제**&#x200B;를 클릭합니다.

   </div>

   삭제된 필드는 복구할 수 없습니다.

   삭제한 필드 유형에 따라 다음 상황이 발생합니다.

   * 선택한 레코드에 속하는 필드를 삭제하면 필드가 삭제되며 더 이상 레코드와 연결할 수 없습니다. 이 필드가 다른 레코드에 조회 필드로 추가되면 해당 필드도 삭제됩니다.
   * 연결 필드를 삭제하면 선택한 레코드에서 필드가 삭제됩니다. 또한 원본 레코드에서 해당 연결 필드도 삭제됩니다.
   * 연결된 레코드에서 추가된 조회 필드를 삭제하면 선택한 레코드 유형에서 필드가 삭제되지만 원래 레코드 유형에는 남아 있습니다.
   * 기본 작업 영역의 글로벌 레코드 유형에서 필드를 삭제하면 해당 레코드 유형이 추가된 모든 작업 영역에서 삭제됩니다. 보조 작업 영역에서는 글로벌 레코드 유형에서 필드를 삭제할 수 없습니다.
