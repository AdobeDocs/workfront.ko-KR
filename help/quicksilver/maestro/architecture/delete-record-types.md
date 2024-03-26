---
title: 레코드 유형 삭제
description: 더 이상 관련이 없는 레코드 유형은 삭제할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# 레코드 유형 삭제

{{maestro-important-intro}}

더 이상 관련이 없는 레코드 유형은 삭제할 수 있습니다.

그러나 레코드 유형을 삭제하면 레코드 유형과 관련된 모든 정보도 삭제됩니다. 자세한 내용은 [레코드 유형 삭제 시 고려 사항](#considerations-when-deleting-record-types) 이 문서의 섹션.

레코드 유형에 대한 자세한 내용은 [레코드 유형 개요](../architecture/overview-of-record-types-and-taxonomies.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td> <p>Adobe Workfront 계획에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 레코드 유형 삭제 시 고려 사항

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 관리 권한이 있는 작업 공간에서는 레코드 유형만 삭제할 수 있습니다.
* 레코드 유형을 삭제하면 레코드 유형과 관련된 다음 정보가 제거됩니다.

   * 해당 유형의 모든 레코드.
   * 레코드 유형과 연결된 모든 필드.
   * 레코드 종류의 모든 보기(필터, 그룹화 및 정렬 기준 포함).
* 기록 유형은 작업 영역에 액세스하는 모든 사용자에서 제거됩니다.
* 삭제된 레코드 종류 또는 해당 정보는 복구할 수 없습니다.
* 삭제하기 전에 다른 레코드 유형에서 삭제하려는 레코드 유형과 연관된 레코드 및 필드를 다시 만드는 것이 좋습니다.

## 레코드 유형 삭제

{{step1-to-maestro}}

기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드 유형을 삭제할 작업 영역을 선택합니다.

   작업공간이 열리고 작업공간과 연관된 레코드 유형 및 분류가 표시됩니다.
1. 삭제할 레코드 유형의 카드를 클릭합니다.

   레코드 유형의 페이지가 열립니다.
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png) 레코드 유형 이름의 오른쪽에 있는 **삭제**.
1. 클릭 **삭제** 확인할 수 있습니다.

   선택한 레코드 종류, 해당 필드, 연결된 레코드 및 보기가 삭제됩니다.
