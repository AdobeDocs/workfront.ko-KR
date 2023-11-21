---
title: 공식 필드 개요
description: Adobe 마에스트로에서는 함수와 기존 필드를 사용하여 새 사용자 정의 값을 계산하는 공식 필드를 만들 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: edd4aa9556b624de3634af26d6d9efd59f5d2e44
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav - below-->

<!--**********ADD TO TOC************>

<!---
title: Formula fields
description: In Adobe Maestro, you can create formula fields that use functions and existing  fields to calculate a new custom value. 
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# 공식 필드 개요

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront의 새로운 오퍼링인 Adobe Maestro를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다. Maestro 기능을 사용하려면 Workfront 고객이어야 합니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

기존 필드를 참조하고 수식으로 연결하여 Adobe 마에스트로에서 사용자 정의 필드를 만들 수 있습니다. 사용자 정의 공식 유형 필드를 생성하여 이 작업을 수행할 수 있습니다.

공식 필드는 레코드 유형의 다른 필드에 있는 기존 값과 기존 값을 계산하는 방법을 나타내는 함수를 사용하여 새 값을 생성합니다.

자세한 내용은 [필드 만들기](../fields/create-fields.md).

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

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

## 공식 필드에 대한 고려 사항

* 공식 필드는 동일한 레코드 유형에 속하는 필드를 참조합니다. 공식 필드를 만들 때 다른 레코드 유형의 필드를 참조할 수 없습니다. <!--is this still accurate??-->
* 수식 필드를 저장한 후에는 수식 필드의 필드 유형을 변경할 수 없습니다.
* 배합표 필드를 저장한 후 배합표 필드의 계산을 갱신할 수 있으며, 계산 결과는 동일한 유형의 모든 레코드에 대해 자동으로 갱신됩니다.


<!--
## The syntax of Maestro formula fields

## Functions supported in Maestro formula fields - I think this should be its own article, but link from here. 

-->