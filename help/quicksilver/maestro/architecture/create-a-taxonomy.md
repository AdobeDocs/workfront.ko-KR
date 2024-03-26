---
title: 분류 레코드 유형 만들기
description: 템플릿을 사용하여 작업 영역을 생성하면 작업 레코드 유형 및 분류 섹션에 레코드 유형이 생성됩니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 3%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 분류 레코드 유형 만들기

{{maestro-important-intro}}

템플릿을 사용하여 작업공간을 생성하면 다음 섹션에 레코드 유형이 생성됩니다.

* 운영 레코드 유형
* 분류

작업 영역의 분류 섹션에 있는 레코드 유형은 동일한 작업 영역의 작업 레코드 유형 섹션에서 레코드 유형에 대한 속성을 캡처합니다.

예를 들어 Campaign은 운영 레코드 유형일 수 있습니다. 다음은 캠페인 레코드 유형에 대한 속성을 캡처하는 분류입니다(지역, 대상자, 국가).

레코드 유형에 대한 자세한 내용은 [레코드 유형 개요](../architecture/overview-of-record-types-and-taxonomies.md).

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
   <p> Adobe Workfront</p> <p>기록 유형을 Experience Manager Assets과 연결하려면 Adobe Experience Manager Assets 라이선스가 있어야 하며, 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Workfront Planning 마감된 Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
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
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 공간에 대한 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다
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

* 작업 영역의 분류 섹션에서 레코드 유형을 만들려면 먼저 템플릿을 사용하여 작업 영역을 만들어야 합니다.

  작업 공간에 대한 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).
* 다음 중 하나를 수행하여 작업 공간의 분류 섹션에서 레코드 유형을 생성할 수 있습니다.
   * 템플릿을 사용하여 작업 공간을 만들 때 자동으로 만듭니다. 자세한 내용은 [작업 공간 만들기](../architecture/create-workspaces.md).
   * 작업 영역의 분류 섹션에서 처음부터 수동으로 만듭니다.

* 새로 생성된 모든 분류에는 기본적으로 다음 필드가 있습니다.

   * 이름
   * 설명
   * 시작 일자
   * 종료 일자
   * 상태

  또한 사용자 지정 필드를 분류법에 추가할 수 있습니다. 자세한 내용은 [필드 만들기](../fields/create-fields.md).

  >[!NOTE]
  >
  >    작업 영역 템플릿을 사용할 때 생성되는 분류 레코드 유형에는 추가 필드가 있습니다.

## 분류 레코드 유형 만들기

분류 레코드 유형을 만드는 것은 레코드 유형을 만드는 것과 비슷합니다.

자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).
