---
title: 작업 공간 템플릿 목록
description: 작업 공간은 팀에서 사용하는 운영 레코드 유형 및 분류의 모음이며 팀의 작업 주기를 나타냅니다. Maestro에는 작업 영역을 구축할 때 기본 레코드 유형, 분류 및 필드를 시작할 수 있는 템플릿 세트가 제공됩니다.
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: c4758b87-45dc-4ffd-b086-5e2e907bdf34
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: List of available workspace templates
description: You can use templates to create workspaces. This article provides a list of available workspace templates
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
---

-->

# 작업 공간 템플릿 목록

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe의 새로운 서비스인 Adobe 마에스트로를 참조합니다.
>
>현재 Adobe 마에스트로는 제한된 수의 고객에게 제공되는 베타 프로그램의 일부입니다.
>
>Maestro용 Beta 프로그램 가입에 대한 자세한 내용은 계정 담당자에게 문의하십시오.
>
>자세한 내용은 [Adobe 마에스트로 개요](../maestro-overview.md).

Adobe Maestro에서 작업 공간은 팀에서 사용하는 운영 레코드 유형과 분류 체계의 컬렉션으로, 팀의 작업 주기를 나타냅니다.

Maestro에는 작업 영역을 구축할 때 기본 레코드 유형, 분류 및 필드를 시작할 수 있는 템플릿 세트가 제공됩니다. 작업 공간 만들기에 대한 자세한 내용은 [작업 공간 만들기](../architecture-and-fields/create-workspaces.md).

이 문서에서는 Maestro에서 사용할 수 있는 작업 공간 템플릿에 대해 설명합니다.

## Maestro 템플릿에 대한 고려 사항

* 각 템플릿에는 일련의 운영 레코드 유형과 분류가 함께 제공됩니다. 자세한 내용은 [레코드 유형 및 분류 개요](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).
* 각 작업 레코드 유형 및 분류는 필드 세트와 함께 제공됩니다. 이러한 필드 중 일부는 다른 Maestro 레코드 유형에 대한 연결입니다.
* 모든 템플릿을 사용자 지정할 수 있습니다.

<!-- I modeled this article by the "List of available Blueprints" and that articles does not have an Access area

## Access requirements

You must have the following: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

-->

## Maestro 작업 공간 템플릿

다음은 Maestro의 작업 공간 템플릿과 여기에 포함된 필드 수입니다.

* **마케팅 관리**: 이 템플릿을 사용하면 모든 마케팅 캠페인을 관리할 수 있습니다. 템플릿에는 다음 항목이 포함되어 있습니다.

   * 운영 레코드 유형:

      * **마케팅 계획**: 7개의 필드 및 5개의 연결된 필드
      * **캠페인**: 9개의 필드 및 7개의 연결된 필드
      * **프로그램**: 9개의 필드 및 5개의 연결된 필드
      * **활동**: 6개의 필드 및 5개의 연결된 필드
   * 분류:
      * **대상자**: 3개의 필드 및 3개의 연결된 필드
      * **세그먼트**: 5개의 필드 및 1개의 연결된 필드
      * **고객 여정**: 4개 필드
      * **제품 제공**: 3개의 필드 및 1개의 연결된 필드
      * **지역**: 1개 필드
      * **전술**: 1개 필드
      * **채널**: 1개의 필드 및 1개의 연결된 필드
      * **비즈니스 단위**: 1개 필드
      * **함수**: 1개 필드

* **영업 관리**: 판매 프로세스를 간소화하고 효율성을 개선하는 포괄적인 판매 시스템을 만들 수 있습니다. 템플릿에는 다음 항목이 포함되어 있습니다.

   * 운영 레코드 유형:

      * **영업 기회**: 7개의 필드 및 4개의 연결된 필드
      * **활동**: 4개의 필드 및 5개의 연결된 필드
      * **캠페인**: 5개의 필드 및 3개의 연결된 필드
   * 분류:
      * **계정**: 4개의 필드 및 3개의 연결된 필드
      * **리드**: 12개 필드 및 2개의 연결된 필드
      * **연락처**: 10개의 필드 및 2개의 연결된 필드
      * **지역**: 1개의 필드 및 2개의 연결된 필드
      * **업계**: 1개 필드
      * **구매 센터**: 1개 필드
      * **제품/서비스**: 1개 필드
      * **경쟁**: 1개 필드

* **제품 관리**: 이 템플릿을 사용하여 효율적이고 구조화된 제품 관리 프로세스를 만들 수 있습니다. 템플릿에는 다음 항목이 포함되어 있습니다.

   * 운영 레코드 유형:

      * **테마**: 8개의 필드 및 2개의 연결된 필드
      * **이니셔티브**: 8개의 필드 및 2개의 연결된 필드
      * **Epic**: 9개의 필드 및 3개의 연결된 필드
      * **사용자 스토리**: 9개의 필드 및 2개의 연결된 필드

   * 분류:

      * **고객**: 6개의 필드 및 1개의 연결된 필드
      * **스프린트**: 7개의 필드 및 1개의 연결된 필드
      * **제품 팀**: 3개 필드
      * **기능 요청**: 8개의 필드 및 1개의 연결된 필드
      * **업계**: 1개의 필드 및 1개의 연결된 필드
