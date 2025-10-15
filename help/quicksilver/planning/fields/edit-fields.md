---
title: 필드 설정 편집
description: Adobe Workfront Planning에서 이미 생성된 필드의 필드 설정을 편집할 수 있습니다. 이 문서에서는 Workfront Planning 필드의 설정을 편집하는 방법에 대해 설명합니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 92748bab4eee807d9529a61a9d97ac1c1df9c8cf
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 0%

---


# 필드 설정 편집

<!--leave the choice value information in yellow till January 2026-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

Adobe Workfront Planning에서 기존 필드의 설정을 편집할 수 있습니다.

Adobe Workfront Planning 필드 만들기에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

이 문서에서는 Workfront Planning 필드의 설정을 편집하는 방법에 대해 설명합니다. 레코드의 필드 값 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하십시오.

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

<!--Old:

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
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## 필드 설정 편집에 대한 고려 사항

필드의 구성을 변경하기 전에 다음 사항을 고려해야 합니다.

* 레코드 유형 테이블에서만 필드 설정을 편집할 수 있습니다.
* 레코드 페이지나 표 보기 외부의 다른 보기에서 필드의 설정을 편집할 수는 없습니다.
* 필드를 저장한 후에는 필드 유형을 편집할 수 없습니다.
* 이미 음수 값이 첨부된 레코드에 저장된 경우 숫자, 백분율 또는 통화 필드에 대해 이전에 선택한 음수 허용 설정을 선택 해제할 수 없습니다.
* 필드를 저장한 후 다음 필드 요소의 구성을 편집할 수 있습니다.

   * 모든 필드의 이름 또는 설명
   * 단일 선택 또는 다중 선택 필드의 옵션
   * 공식 필드의 표현식.

  >[!WARNING]
  >
  >수식 표현식이 변경되거나 선택 유형 필드에서 옵션을 추가하거나 제거하면 구성이 수정된 필드에 이미 정보가 저장된 레코드에 대한 데이터가 손실됩니다.
  >
  >필드의 구성을 변경할 때 이 데이터 손실이 발생할 수 있다는 경고나 표시는 없습니다.
  >
  >필드 구성이 변경되었다는 알림이 다른 사용자에게 표시되지 않습니다.

* 연결된 레코드에서 기존 조회 필드를 편집할 수 있습니다.
* 이 문서의 [필드 설정 편집](#edit-field-settings-1) 섹션에 설명된 대로 필드를 편집할 수 있을 뿐만 아니라, <span class="preview">테이블 보기에서 레코드를 편집할 때 필드 값을 업데이트할 때 단일 또는 다중 선택 필드의 선택 항목을 편집할 수 있습니다. 자세한 내용은 이 문서의 표 보기에서 레코드를 편집할 때 [기존 선택 필드에 새 선택 항목 추가](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view) 섹션을 참조하십시오.</span>

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## 필드 설정 편집

{{step1-to-planning}}

1. 레코드 필드를 편집할 작업 영역을 클릭합니다.

   작업공간이 열리고 작업공간의 모든 레코드 유형이 카드에 표시됩니다.

1. 기록 유형의 카드를 클릭합니다.

   레코드 유형의 페이지가 열립니다.

1. (조건부) **테이블 보기**&#x200B;의 탭을 클릭합니다.

   레코드 유형과 연관된 모든 기존 레코드는 테이블 뷰의 행에 표시됩니다.
1. 편집할 필드의 열 머리글 위로 마우스를 가져간 후 필드 이름 뒤에 있는 아래쪽 화살표를 클릭한 다음 **필드 편집**&#x200B;을 클릭합니다

   또는

   필드의 열 머리글을 두 번 클릭합니다.

   ![강조 표시된 테이블 헤더의 필드 이름 뒤 화살표 메뉴](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 필드에 대한 정보를 업데이트하고 **저장**&#x200B;을 클릭합니다.

   자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* 필드를 저장한 후에는 필드 유형을 업데이트할 수 없습니다.
   >
   >* 필드 구성(필드 옵션 또는 수식 표현식)을 수정하면 수정된 필드에 이미 정보가 들어 있는 레코드가 해당 값을 실시간으로 업데이트합니다. 필드 구성 변경에 의해 트리거된 값 변경에 대한 경고 및 감사 로그가 없습니다. 필드를 보는 모든 사용자는 수정 사항이 적용된 새 값을 즉시 볼 수 있습니다.

   필드 정보는 작업 영역을 볼 수 있는 액세스 권한이 있는 모든 사용자에 대해 업데이트됩니다.

1. (조건부) 연결된 레코드 필드의 경우 **조회 필드 편집**&#x200B;을 클릭하고 연결된 레코드 형식에서 조회 필드를 추가하거나 제거합니다.

   자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.


<div class="preview">

## 테이블 보기에서 레코드를 편집할 때 기존 선택 필드에 새 선택 사항을 추가합니다.

<!--some of this information is also available in Edit records article - update both when necessary-->

테이블 보기에서 레코드를 편집할 때 기존 단일 또는 다중 선택 필드에 새 선택 항목을 추가할 수 있습니다.

>[!IMPORTANT]
>
>이 섹션에서 설명하는 기능은 표 보기에서만 사용할 수 있습니다. 단일 또는 다중 선택 필드가 표시되는 다른 영역에서는 사용할 수 없습니다.

**예**

Status 라는 단일 선택 필드에 New 및 Closed 라는 선택 사항이 있을 수 있으며 In 진행 중 상태에 대한 선택 사항을 추가할 수 있습니다. 다음 중 하나를 수행하여 선택 사항을 추가할 수 있습니다.

* 필드 편집 중 자세한 내용은 이 문서의 [필드 설정 편집](#edit-field-settings-1) 섹션을 참조하십시오.
* 아래 설명된 대로 표 보기에서 레코드를 편집하는 동안 새 옵션을 추가합니다.

레코드를 편집할 때 기존 선택 필드에 새 선택을 추가하려면 다음을 수행합니다.

1. 레코드 유형 페이지로 이동하여 테이블 보기를 엽니다.
1. 선택 사항을 추가할 단일 또는 다중 선택 필드를 테이블 보기에 새 열로 추가합니다. 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.
1. 필드의 셀을 두 번 클릭하여 인라인 필드 편집을 시작합니다.
1. 추가할 선택 항목의 이름을 입력한 다음 **선택 항목 추가**&#x200B;를 클릭합니다.

   ![테이블 보기의 단일 선택 필드에 선택 항목 추가](assets/add-choice-in-table-view-for-single-select-field.png)

   새 선택 항목이 단일 선택 필드에 즉시 추가됩니다.

   <!--<span class="preview">A new choice value is also added to each choice. You can use the choice values in API calls or other integrations. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). </span>-->

</div>