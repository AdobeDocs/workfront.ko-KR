---
title: 필드 삭제
description: Adobe Workfront planning에서 더 이상 관련이 없는 사용자 정의 필드를 삭제할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Maestro, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# 필드 삭제

{{maestro-important-intro}}

Adobe Workfront planning에서 사용자 정의 필드를 만들어 레코드에 대한 정보를 저장할 수 있습니다.

Workfront Planning에서 사용자 정의 필드를 만드는 방법에 대한 자세한 내용은 [필드 만들기](../fields/create-fields.md).

더 이상 관련이 없는 Workfront 계획 필드는 삭제할 수 있습니다.

## Workfront 계획 필드 삭제에 대한 고려 사항:

* 레코드 유형 테이블 보기에서만 필드를 삭제할 수 있습니다.
* 레코드의 기본 필드는 삭제할 수 없습니다.
* 필드에 저장된 모든 정보는 삭제되며 복구할 수 없습니다.
* 연결된 레코드 필드를 삭제하면 연결된 모든 조회 필드도 연결된 레코드 유형에서 삭제됩니다. 연결된 레코드 종류의 연결된 레코드 필드는 삭제되지 않습니다.

  자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## 액세스 요구 사항

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>조직은 Adobe Workfront planning Beta 프로그램에 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Workfront 계획에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 필드 삭제

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-maestro}}

그러면 Workfront planning에서 마지막으로 액세스한 작업 영역이 열립니다.
1. 필드를 삭제할 레코드 유형의 카드를 클릭합니다.
1. (조건부) 선택 **표 보기** 다음에서 **보기** 레코드 유형 페이지의 오른쪽 위 모서리에 있는 드롭다운 메뉴.
1. 열 헤더에서 삭제할 필드를 찾고 열 헤더 위로 마우스를 가져간 다음 필드 이름 뒤에 있는 아래쪽 방향 화살표를 클릭합니다.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 클릭 **삭제**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 클릭 **삭제** 확인할 수 있습니다.

   필드가 삭제되고 복구할 수 없으며 더 이상 레코드와 연결할 수 없습니다.
