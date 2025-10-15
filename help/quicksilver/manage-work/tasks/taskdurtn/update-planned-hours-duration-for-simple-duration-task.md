---
product-area: projects
navigation-topic: task-duration
title: 간단한 기간 유형으로 작업의 계획된 시간 및 기간 업데이트
description: 기본적으로 Adobe Workfront은 계획된 시간을 기반으로 하여 단순 기간 유형으로 작업의 기간을 계산합니다. 그러나 Workfront의 특정 영역에서 계획된 시간 및 단순 기간 작업의 기간을 수동으로 편집할 수도 있습니다.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# 간단한 기간 유형으로 작업의 계획된 시간 및 기간 업데이트

기본적으로 Adobe Workfront은 계획된 시간을 기반으로 하여 단순 기간 유형으로 작업의 기간을 계산합니다. 그러나 Workfront의 특정 영역에서 계획된 시간 및 단순 기간 작업의 기간을 수동으로 편집할 수도 있습니다.

단순한 기간 유형 인라인으로 또는 지정 영역의 작업 레벨에서 작업의 계획된 시간과 기간을 편집할 수 있습니다.

인라인 정보 편집에 대한 자세한 내용은 [Adobe Workfront의 목록에서 인라인 편집 항목](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)을 참조하십시오.

이 문서에서는 지정 영역에서 태스크 레벨에서 간단한 기간 유형으로 태스크에 대한 계획된 시간 및 기간을 갱신하는 방법에 대해 설명합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준 이상</p> 
   <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p> <p>작업에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 액세스 관리 </p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 간단한 기간 유형으로 작업의 계획된 시간 및 기간 업데이트

>[!IMPORTANT]
>
>단순 기간 태스크에서 기간을 수동으로 업데이트하면 Workfront에서 계획된 시간을 기반으로 기간 계산을 중지합니다.

고급 지정 상자에서 단순 기간 유형을 사용하여 작업의 계획된 시간과 기간을 편집하려면

1. 작업 목록에서 기간 유형을 변경할 작업의 이름을 클릭합니다.
1. 다음 중 하나를 수행하십시오.

   * 작업 이름 옆에 있는 **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png)을 클릭하고 **편집**&#x200B;을 클릭한 다음 **할당**&#x200B;을 클릭합니다.
   * 작업 헤더의 할당 영역에서 **할당 대상** 또는 할당 이름을 클릭한 다음 **고급**&#x200B;을 클릭합니다.

1. 모든 할당에 대한 **계획된 시간**&#x200B;의 총 값(예: 10시간)을 입력하십시오. 작업에 할당된 모든 리소스 간에 총 계획된 시간이 균등하게 분배됩니다.
1. (선택 사항) 작업에 할당된 각 자원의 계획된 시간을 수동으로 조정합니다. 리소스에 개별적으로 할당된 새 시간을 반영하도록 작업 업데이트에 대한 총 계획된 시간 수입니다.
1. 작업 **기간**&#x200B;의 값(예: 2일)을 입력하십시오.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. **저장**&#x200B;을 클릭합니다.
