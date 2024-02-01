---
title: 필드 편집
description: Adobe Maestro에서 이미 만들어진 필드의 필드 설정을 편집할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# 필드 편집

{{maestro-important-intro}}

이미 만들어진 필드의 필드 설정을 편집할 수 있습니다.

Adobe 마에스트로 필드 생성에 대한 자세한 내용은 [필드 만들기](../fields/create-fields.md).

이 문서에서는 Maestro 필드의 설정을 편집하는 방법을 설명합니다. Maestro 레코드의 필드 값 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/maestro/records/edit-records.md).

## 필드 정보 편집에 대한 고려 사항

* 필드가 속한 작업 영역에 대한 관리 권한이 있는 경우 사용자가 만든 필드나 다른 사용자가 만든 필드를 편집할 수 있습니다.
* 레코드 유형 테이블에서 필드를 편집할 수 있습니다.
* 레코드의 세부 정보 페이지나 타임라인 보기에서 필드를 편집할 수 없습니다.
* 필드를 저장한 후에는 필드 유형을 편집할 수 없습니다.
* 이미 음수 값이 첨부된 레코드에 저장된 경우 숫자, 백분율 또는 통화 필드에 대해 이전에 선택한 음수 허용 설정을 선택 해제할 수 없습니다.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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
<p>Adobe Maestro Closed Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   <td> <p>Maestro에 대한 액세스 제어가 없습니다.</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 필드 편집

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-workfront.png) Workfront의 오른쪽 위 모서리 또는 **메인 메뉴** 아이콘 ![](assets/main-menu-shell.png)  왼쪽 위 모서리에서 사용 가능한 경우 을(를) 클릭합니다. **마에스트로** ![](assets/maestro-icon.png).

   기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드 유형을 삭제할 작업 영역을 선택합니다.

   작업공간이 열리고 작업공간과 연관된 레코드 유형 및 분류가 표시됩니다.
1. 편집할 필드를 포함하는 레코드 유형 또는 분류법에 대한 카드를 클릭합니다.

   레코드 유형의 페이지가 열립니다.
1. (조건부) 선택 **표 보기** 다음에서 **보기** 레코드 유형 페이지의 오른쪽 위 모서리에 있는 드롭다운 메뉴.
1. 편집할 필드의 열 헤더 위로 마우스를 가져간 다음 필드 이름 뒤에 있는 아래쪽 화살표를 클릭하고 **필드 편집**

   또는

   필드의 열 머리글을 두 번 클릭합니다.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 필드에 대한 정보를 업데이트하고 **저장**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >필드를 저장한 후에는 필드 유형을 업데이트할 수 없습니다.


1. (조건부) 연결된 레코드 필드의 경우 **조회 필드 편집** 연결된 레코드 종류에서 필드를 추가하거나 제거합니다.

   자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).
