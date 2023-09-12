---
title: 분류 레코드 유형 만들기
description: 분류는 Adobe Workfront Maestro의 운영 레코드 유형에 대한 속성을 캡처하는 재사용 가능한 레코드 유형의 유형입니다.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 분류 레코드 유형 만들기

>[!IMPORTANT]
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 비공개 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

분류는 Adobe Maestro의 운영 레코드 유형에 대한 속성을 캡처하는 레코드 유형입니다.

예를 들어 Campaign은 운영 레코드 유형일 수 있습니다. 다음은 캠페인 레코드 유형에 대한 속성을 캡처하는 분류입니다(지역, 대상자, 국가).

Maestro 레코드 유형에 대한 자세한 내용은 [레코드 유형 및 분류 개요](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
 <tr>
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

## 분류 생성에 대한 고려 사항

* 작업 영역에서 분류를 만들려면 먼저 작업 영역을 만들어야 합니다.

  작업 공간에 대한 자세한 내용은 [작업 공간 만들기](../architecture-and-fields/create-workspaces.md).
* 다음 중 하나를 수행하여 분류 레코드 유형을 만들 수 있습니다.
   * 템플릿을 사용하여 작업 공간을 만들 때 자동으로 만듭니다. 자세한 내용은 [작업 공간 만들기](../architecture-and-fields/create-workspaces.md).
   * 처음부터 직접 만듭니다.
   * 외부 목록의 정보를 붙여 넣어 수동으로 만듭니다.

  <!--this is not possible yet:
  * You can taxonomies to a workspace by doing one of the following:
    * Create a connection to object types from other systems, when adding fields to a taxnomy record type. This creates a read-only record type in Maestro.  - update this sentence when you can connect taxonomies as well as operational records to a third-party system.-->

* 새로 생성된 모든 분류는 다음 필드와 함께 제공됩니다.

   * 이름 <!--if there won't be any more fields, consider rephrasing this-->

  또한 사용자 지정 필드를 분류법에 추가할 수 있습니다. 자세한 내용은 [필드 만들기](../architecture-and-fields/create-fields.md).

  >[!NOTE]
  >
  >    작업 영역 템플릿을 사용할 때 생성되는 분류에는 추가 필드가 있습니다.

## 분류 체계 만들기

분류를 만드는 것은 처음부터 또는 작업 영역 템플릿에서 작업 기록 유형을 만드는 것과 비슷합니다.

자세한 내용은 이 문서의 &quot;처음부터 레코드 유형 만들기&quot; 섹션을 참조하십시오 [레코드 유형 만들기](../architecture-and-fields/create-record-types.md).

템플릿에서 작업 영역을 생성할 때 분류를 자동으로 생성하는 방법에 대한 자세한 내용은 [작업 공간 만들기](../architecture-and-fields/create-workspaces.md).
