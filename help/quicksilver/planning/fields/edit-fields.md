---
title: 필드 설정 편집
description: Adobe Workfront Planning에서 이미 생성된 필드의 필드 설정을 편집할 수 있습니다. 이 문서에서는 Workfront Planning 필드의 설정을 편집하는 방법에 대해 설명합니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---


# 필드 설정 편집

{{planning-important-intro}}

Adobe Workfront Planning에서 이미 생성된 필드의 필드 설정을 편집할 수 있습니다.

Adobe Workfront Planning 필드 만들기에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

이 문서에서는 Workfront Planning 필드의 설정을 편집하는 방법에 대해 설명합니다. 레코드의 필드 값 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
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
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


<!--
OLD

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## 필드 설정 편집에 대한 고려 사항

필드의 구성을 변경하기 전에 다음 사항을 고려해야 합니다.

* 필드가 속한 작업 영역에 대한 관리 권한이 있는 경우 사용자가 만든 필드나 다른 사용자가 만든 필드를 편집할 수 있습니다.
* 레코드 유형 테이블에서 필드를 편집할 수 있습니다.
* 레코드 페이지나 테이블 보기 외부의 다른 보기에서는 필드를 편집할 수 없습니다.
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

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 필드에 대한 정보를 업데이트하고 **저장**&#x200B;을 클릭합니다. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* 필드를 저장한 후에는 필드 유형을 업데이트할 수 없습니다.
   >
   >* 필드 구성(필드 옵션 또는 수식 표현식)을 수정하면 수정된 필드에 이미 정보가 들어 있는 레코드가 해당 값을 실시간으로 업데이트합니다. 필드 구성 변경에 의해 트리거된 값 변경에 대한 경고 및 감사 로그가 없습니다. 필드를 보는 모든 사용자는 수정 사항이 적용된 새 값을 즉시 볼 수 있습니다.

   필드 정보는 작업 영역을 볼 수 있는 액세스 권한이 있는 모든 사용자에 대해 업데이트됩니다.

1. (조건부) 연결된 레코드 필드의 경우 **조회 필드 편집**&#x200B;을 클릭하고 연결된 레코드 형식에서 필드를 추가하거나 제거합니다.

   자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

