---
product-area: projects
navigation-topic: update-work-in-a-project
title: 프로젝트 상태 업데이트
description: 프로젝트 상태 는 프로젝트와 관련된 작업이 원활하게 진행되고 있는지 또는 장애물이 발생했는지 여부를 나타내기 위해 프로젝트에 배치되는 플래그입니다. 현재 진행 중인지 여부를 나타내는 프로젝트 상태와 다릅니다.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 2d8ad8baa6c470fd82b61202cb42443f568b1968
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 프로젝트 상태 업데이트

프로젝트 상태 는 프로젝트와 관련된 작업이 원활하게 진행되고 있는지 또는 장애물이 발생했는지 여부를 나타내기 위해 프로젝트에 배치되는 플래그입니다. 현재 진행 중인지 여부를 나타내는 프로젝트 상태와 다릅니다.

프로젝트의 상태를 자동 또는 수동으로 설정할 수 있습니다. 프로젝트의 상태를 수동으로 변경하려면 프로젝트 소유자 또는 프로젝트 관리 권한이 있어야 합니다.

[사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)에 설명된 대로 Adobe Workfront 관리자는 사용자 환경에 대한 사용자 지정 조건을 만들 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
  <p>표준</p>
   <p>플랜</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p> <p>작업 및 문제에 대한 액세스 편집 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 문제에 대한 또는 그 이상의 권한을 보고 해당 조건 보기</p>
   <p>작업 및 문제에 대한 권한을 관리하여 조건 업데이트</p>
     </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the new licenses:
  <p>Standard</p>
   
   For current licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
     </td> 
  </tr> 
 </tbody> 
</table>-->

## 자동으로 조건 설정

프로젝트의 상태를 자동으로 설정하는 것은 프로젝트의 상태 유형에 의해 결정됩니다. Workfront이 프로젝트의 상태를 자동으로 설정하려면 상태 유형 을 진행 상태로 설정해야 합니다.

Workfront 또는 그룹 관리자는 설정 영역에서 프로젝트 환경 설정을 지정할 때 시스템의 새 프로젝트에 대한 상태 유형 필드의 기본값을 결정합니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

프로젝트를 만들 때 프로젝트의 상태가 해당 시점의 프로젝트 진행 상태와 일치하도록 자동으로 설정됩니다. 프로젝트의 진행 상태는 프로젝트에 대한 작업의 진행 상황을 기반으로 합니다.

프로젝트 상태 및 진행 상태를 기반으로 프로젝트 상태를 계산하는 방법에 대한 자세한 내용은 [프로젝트 진행 상태 개요](../../../manage-work/projects/planning-a-project/project-progress-status.md)를 참조하십시오.

## 프로젝트의 상태 수동 업데이트

진행 상태 대신 프로젝트의 상태 유형을 수동으로 설정하는 경우 프로젝트의 상태를 수동으로 업데이트할 수 있습니다.

1. 조건을 업데이트할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **프로젝트 세부 정보** 섹션을 클릭합니다.

1. **조건 유형** 필드가 **수동**(으)로 설정되어 있는지 확인하십시오.

   ![](assets/project-details-overview-select-condition.png)

1. **조건** 필드에서 연결된 작업이 원활하게 진행되는지 또는 지연되는지 여부에 대해 이해한 것과 일치하는 옵션을 선택합니다.

   * **대상**
   * **위험 상태**
   * **문제 발생**

   프로젝트 상태에 대한 자세한 내용은 [프로젝트 상태 및 상태 형식 개요](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)를 참조하십시오.

   >[!NOTE]
   >
   >사용자 환경에 맞게 조건을 사용자 정의할 수 있으므로 사용자 환경에서 조건에 대한 세 가지 이상의 옵션을 찾을 수 있습니다. 조건의 이름은 위에 나열된 조건과 다를 수 있습니다. Workfront에서 조건을 사용자 지정하는 방법에 대한 자세한 내용은 [사용자 지정 조건 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)을 참조하십시오.

1. **변경 내용 저장**&#x200B;을 클릭합니다.
