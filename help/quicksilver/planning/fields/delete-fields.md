---
title: 필드 삭제
description: Adobe Workfront Planning에서 더 이상 관련이 없는 사용자 정의 필드를 삭제할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Planning, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# 필드 삭제

{{planning-important-intro}}

Adobe Workfront Planning에서 사용자 정의 필드를 만들어 레코드에 대한 정보를 저장할 수 있습니다.

Workfront Planning에서 사용자 정의 필드를 만드는 방법에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

더 이상 관련이 없는 Workfront Planning 필드를 삭제할 수 있습니다.

## Workfront Planning 필드 삭제에 대한 고려 사항:

* 레코드 유형 테이블 보기에서만 필드를 삭제할 수 있습니다.
* 레코드의 기본 필드는 삭제할 수 없습니다.
* 필드에 저장된 모든 정보는 삭제되며 복구할 수 없습니다.
* 연결된 레코드 필드를 삭제하면 연결된 모든 조회 필드도 사용자가 연결한 레코드 유형에서 삭제됩니다. 연결하는 레코드 유형의 연결된 레코드 필드도 연결하는 레코드에서 삭제됩니다.

  예를 들어 캠페인을 제품이라는 다른 레코드 유형에 연결하고 캠페인에서 제품 연결 필드와 제품 상태 조회 필드를 삭제하면 다음 항목이 삭제됩니다.

   * 캠페인의 제품 연결 필드
   * 캠페인의 제품 상태 조회 필드
   * 제품의 Campaign 연결 필드.

  자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <p> Adobe Workfront</p> </td>
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
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="/help/quicksilver/planning/access/access-overview.md">액세스 개요</a>를 참조하십시오. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
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

## 필드 삭제

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. 레코드 필드를 삭제할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.

1. 기록 유형의 카드를 클릭합니다.

1. (조건부) 아직 선택하지 않은 경우 레코드 유형 페이지에서 **테이블 보기**&#x200B;의 탭을 클릭합니다.

   레코드 유형과 연관된 모든 기존 레코드는 테이블 뷰의 행에 표시됩니다.

1. 열 헤더에서 삭제할 필드를 찾고 열 헤더 위로 마우스를 가져간 다음 필드 이름 뒤에 있는 아래쪽 방향 화살표를 클릭합니다.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. **삭제**&#x200B;를 클릭합니다. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 확인하려면 **삭제**&#x200B;를 클릭하세요.

   필드가 삭제되고 복구할 수 없으며 더 이상 레코드와 연결할 수 없습니다.
