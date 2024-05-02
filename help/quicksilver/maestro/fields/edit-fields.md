---
title: 필드 편집
description: Adobe Workfront Planning에서 이미 생성된 필드의 필드 설정을 편집할 수 있습니다. 이 문서에서는 Workfront Planning 필드의 설정을 편집하는 방법에 대해 설명합니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

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

Adobe Workfront Planning에서 이미 생성된 필드의 필드 설정을 편집할 수 있습니다.

Adobe Workfront Planning 필드 생성에 대한 자세한 내용은 다음을 참조하십시오. [필드 만들기](../fields/create-fields.md).

이 문서에서는 Workfront Planning 필드의 설정을 편집하는 방법에 대해 설명합니다. 레코드의 필드 값 편집에 대한 자세한 내용은 [레코드 편집](/help/quicksilver/maestro/records/edit-records.md).

## 필드 설정 편집에 대한 고려 사항

필드의 구성을 변경하기 전에 다음 사항을 고려해야 합니다.

* 필드가 속한 작업 영역에 대한 관리 권한이 있는 경우 사용자가 만든 필드나 다른 사용자가 만든 필드를 편집할 수 있습니다.
* 레코드 유형 테이블에서 필드를 편집할 수 있습니다.
* 레코드 페이지나 테이블 보기 외부의 다른 보기에서는 필드를 편집할 수 없습니다.
* 필드를 저장한 후에는 필드 유형을 편집할 수 없습니다.
* 이미 음수 값이 첨부된 레코드에 저장된 경우 숫자, 백분율 또는 통화 필드에 대해 이전에 선택한 음수 허용 설정을 선택 해제할 수 없습니다.

<!--this is not true yet, but will be with the release of RTBE for field configuration changes: 

* You can edit the configuration of the following fields, after they are saved:

    * The Name or the Description of any field
    * The Options of a Single-select or a Multi-select field.
    * The expression of a Formula field.-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
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
<p>조직은 Adobe Workfront Planning Beta 프로그램에 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   <td> <p>Workfront Planning에 대한 액세스 제어가 없습니다.</p>  
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
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 필드 설정 편집

{{step1-to-maestro}}

    기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드 유형을 삭제할 작업 영역을 선택합니다.

   작업공간이 열리고 작업공간과 연관된 레코드 유형이 표시됩니다.
1. 편집할 필드가 있는 레코드 유형의 카드를 클릭합니다.

   레코드 유형의 페이지가 열립니다.
1. (조건부) **표 보기**.
1. 편집할 필드의 열 헤더 위로 마우스를 가져간 다음 필드 이름 뒤에 있는 아래쪽 화살표를 클릭하고 **필드 편집**

   또는

   필드의 열 머리글을 두 번 클릭합니다.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 필드에 대한 정보를 업데이트하고 **저장**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >필드를 저장한 후에는 필드 유형을 업데이트할 수 없습니다.

   필드 정보는 작업 영역을 볼 수 있는 액세스 권한이 있는 모든 사용자에 대해 업데이트됩니다.

   <!--After the release of the RTBE for field configurations, replace the tip with this:

    >[!TIP]
    >
    >* You cannot update the field type after the field is saved.
    >
    >* When you modify field configurations (field options or formula expressions), records that already contain information in the modified fields will update their values in real-time. There is no warning and no audit log for the value changes triggered by field configuration changes. All users who view the fields will immediately see the new values with the modifications. 
    -->


1. (조건부) 연결된 레코드 필드의 경우 **조회 필드 편집** 연결된 레코드 종류에서 필드를 추가하거나 제거합니다.

   자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).
