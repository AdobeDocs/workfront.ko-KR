---
title: 필드 삭제
description: Adobe Maestro에서 더 이상 관련이 없는 사용자 정의 필드를 삭제할 수 있습니다.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 필드 삭제

>[!IMPORTANT]
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe Maestro에서 사용자 정의 필드를 만들어 레코드에 대한 정보를 저장할 수 있습니다.

Maestro에서 사용자 정의 필드를 만드는 방법에 대한 자세한 내용은 [필드 만들기](../architecture-and-fields/create-fields.md).

더 이상 관련이 없는 Maestro 필드는 삭제할 수 있습니다.

## Maestro 필드 삭제에 대한 고려 사항:

* 생성한 필드나 다른 사용자가 생성한 필드를 삭제할 수 있습니다. <!--this will change with access levels/ permissions-->
* 레코드 유형 테이블에서만 필드를 삭제할 수 있습니다.
* 필드에 저장된 모든 정보는 삭제되며 복구할 수 없습니다.
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>모든</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>모든</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">액세스 수준</td>
   <td> <p>모든</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">레이아웃 템플릿</td>
   <td> <p>시스템 관리자가 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/grant-access.md">Adobe 마에스트로에 대한 액세스 권한 부여</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 필드 삭제

<!--When they release the sharing of fields between other records, revise this section.  -->

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리에서 <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 그런 다음 을 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   이렇게 하면 Maestro에서 마지막으로 액세스한 작업 영역이 열립니다.
1. 필드를 삭제할 레코드 유형의 카드를 클릭합니다.
1. (조건부) 선택 **표 보기** 다음에서 **보기** 레코드 유형 페이지의 오른쪽 위 모서리에 있는 드롭다운 메뉴.
1. 열 헤더에서 삭제할 필드를 찾고 열 헤더 위로 마우스를 가져간 다음 필드 이름 뒤에 있는 아래쪽 방향 화살표를 클릭합니다.
1. 클릭 **삭제**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 클릭 **삭제** 확인할 수 있습니다.

   필드가 삭제되고 복구할 수 없으며 더 이상 레코드와 연결할 수 없습니다.