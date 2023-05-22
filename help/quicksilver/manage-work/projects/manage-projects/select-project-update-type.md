---
product-area: projects
navigation-topic: manage-projects
title: 프로젝트 업데이트 유형 선택
description: 프로젝트에 대한 업데이트 유형을 선택하여 프로젝트의 타임라인에 대한 변경 사항이 상위 작업 또는 프로젝트에 저장되는 빈도를 제어할 수 있습니다.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# 프로젝트 업데이트 유형 선택

프로젝트에 대한 업데이트 유형을 선택하여 프로젝트의 타임라인에 대한 변경 사항이 상위 작업 또는 프로젝트에 저장되는 빈도를 제어할 수 있습니다.

프로젝트 타임라인이 업데이트되면 프로젝트, 프로젝트 작업 또는 타임라인이 종속된 다른 프로젝트에 대한 변경 사항을 기반으로 프로젝트 타임라인이 다시 계산됩니다.

예를 들어 프로젝트의 작업에 대한 다음 변경 사항은 프로젝트의 타임라인에 대한 업데이트를 트리거합니다.

* 작업 날짜 업데이트
* 작업의 전임 작업 관계 변경
* 작업 제한이나 기간 유형을 변경하는 것 외에 할당을 추가 또는 제거하는 상위-하위 관계를 변경합니다.

## 액세스 요구 사항

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 프로젝트의 업데이트 유형 업데이트

작업이 업데이트되면 해당 상위 개체(상위 작업 또는 프로젝트)가 업데이트 유형에 표시된 시점에 업데이트됩니다.  프로젝트의 업데이트 유형을 지정하려면 다음을 수행합니다.

1. 업데이트 유형을 지정할 프로젝트로 이동합니다.
1. 기타 메뉴 클릭 ![](assets/more-icon.png) 프로젝트 이름 옆에 있는 을(를) 클릭한 다음 **편집** .

1. 클릭  **프로젝트** **설정**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. 다음에서 **업데이트 유형** 필드에서는 변경 사항이 있을 때 Workfront에서 프로젝트의 타임라인을 매일 자동으로 계산할지 또는 프로젝트 관리자가 수동으로 계산할지 여부를 선택합니다.

   아래 목록의 옵션에서 선택하십시오. 

   >[!IMPORTANT]
   >
   >프로젝트의 타임라인이 15년을 초과하는 경우 Workfront은 타임라인을 자동으로 또는 변경 시 계산하지 않습니다. 15년 이상 프로젝트의 업데이트 유형은 항상 수동입니다.

   * **자동 및 변경 시:** 기본 설정입니다. 프로젝트 또는 타임라인이 종속된 다른 프로젝트에서 변경 사항이 발생할 때마다 프로젝트 타임라인이 업데이트됩니다. 프로젝트 타임라인도 매일 밤 업데이트됩니다. \
      이 설정은 프로젝트 타임라인이 항상 최신 상태인지 확인하므로 권장됩니다.

      작업 또는 프로젝트를 업데이트하고 타임라인 재계산을 트리거하면 사용 가능한 모든 날짜가 즉시 표시되어 작업을 계속할 수 있습니다. 작업이 100개를 초과하는 프로젝트의 경우 계산이 더 긴 날짜가 흐리게 표시됩니다.

      ![](assets/dates-dimmed-when-insline-editing-350x146.png)

      이는 재계산이 아직 완료되지 않았으며, 날짜가 변경될 수 있음을 나타냅니다.

   * **변경만:** 프로젝트 타임라인은 프로젝트 또는 타임라인이 종속된 다른 프로젝트에서 변경 사항이 발생할 때마다 업데이트되며 예약된 업데이트는 발생하지 않습니다.\
      시스템 성능이 걱정되고 프로젝트나 타임라인이 종속된 다른 프로젝트에서 변경 사항이 거의 발생하지 않는 경우 이 옵션을 선택할 수 있습니다.

   * **자동만:** 프로젝트 타임라인은 매일 밤 업데이트되며, 변경 후 바로 업데이트되지 않습니다.\
      시스템 성능이 걱정되고 프로젝트 또는 타임라인이 종속된 다른 프로젝트에서 매일 많은 변경 사항이 발생하는 경우 이 옵션을 선택할 수 있습니다.

      >[!NOTE]
      >
      >프로젝트가 Planning 상태인 경우 매일 밤 자동으로 다시 계산되지 않습니다. 변경 시에만 다시 계산됩니다.

   * **수동만:** 다음 옵션을 선택하는 경우에만 프로젝트 타임라인이 업데이트됩니다. **타임라인 다시 계산**&#x200B;문서의 &quot;수동 재계산&quot; 섹션에 설명된 대로 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
      한 번에 프로젝트를 여러 번 변경하고, 각 개별 변경 내용이 아닌 모든 변경 내용이 적용된 후에 타임라인 재계산을 수행하려는 경우 이 옵션을 선택할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.
