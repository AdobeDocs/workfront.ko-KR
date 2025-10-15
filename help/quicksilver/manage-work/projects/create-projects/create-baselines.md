---
product-area: projects
navigation-topic: create-projects
title: 프로젝트 기준선 만들기
description: 기준선은 초기 프로젝트 계획 또는 프로젝트 수명 동안 주어진 시간에 포함된 주요 정보를 나타내는 프로젝트 스냅샷입니다.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 프로젝트 기준선 만들기

<!-- Audited: 08/2025 -->

기준선은 초기 프로젝트 계획 또는 프로젝트 수명 동안 주어진 시간에 포함된 주요 정보를 나타내는 프로젝트 스냅샷입니다.

기준선을 사용하여 현재 계획의 해당 정보를 원래 계획 또는 다른 시점과 비교하여 문제 작업, 범위 변경 및 시간에 따른 기타 추세를 식별할 수 있습니다.

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
    <td><p>표준</p>
        <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 또는 그 이상에 대한 권한을 보고 기준선을 봅니다.</p> <p>프로젝트에 대한 권한을 관리하여 기준선 만들기</p> </td> 
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
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
    <td><p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 기준선 작업 고려 사항

* 프로젝트 기간 동안 프로젝트의 진행 상황에 대한 스냅샷을 여러 번 캡처하여 여러 기준선을 만들 수 있습니다.
* 베이스라인을 작성하거나 베이스라인 보고서를 작성하여 프로젝트의 베이스라인에 포함된 정보를 볼 수 있습니다.
* 베이스라인을 생성하면 작업 정보가 해당 베이스라인의 베이스라인 작업에도 캡처됩니다.
* 기준선 작업 보고서를 작성하여 기준선 작업 정보를 볼 수 있습니다.

>[!IMPORTANT]
>
>기준선은 프로젝트의 이름, 날짜 및 재무 정보에 대한 스냅샷을 만듭니다. 기준선에는 프로젝트의 사용자 정의 필드 값이 포함되지 않습니다. 기준선에 포함된 재무 정보에 대한 자세한 내용은 [프로젝트 기준선에 포함된 프로젝트 재무](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md)을 참조하십시오.

## 기준선 만들기

다음과 같은 방법으로 베이스라인을 생성할 수 있습니다.

* **자동으로**: Workfront 관리자 또는 그룹 관리자는 프로젝트가 현재 상태가 되면 자동으로 기준선을 만들 수 있도록 Workfront에 대한 프로젝트 환경 설정을 설정합니다. 이 설정을 사용하면 프로젝트 상태가 현재가 되면 베이스라인이 만들어집니다. 이 설정이 활성화되지 않은 경우 기준선을 수동으로 만들어야 합니다.

  프로젝트 환경 설정 구성 및 자동 기준선 만들기 설정에 대한 자세한 내용은 [시스템 차원의 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

  >[!CAUTION]
  >
  >이 설정을 사용하면 프로젝트의 상태가 현재로 변경될 때마다 프로젝트에 대한 기준선이 자동으로 만들어집니다. 처음 생성된 베이스라인이 기본 베이스라인입니다. 프로젝트 기간 동안 다른 모든 기준선을 수동으로 만들어야 합니다.

* **수동으로**: 프로젝트가 진행될 때 필요에 따라 프로젝트에 대한 새 기준선을 만들 수 있습니다. 그런 다음 기준선을 비교하여 시간이 지남에 따라 프로젝트가 어떻게 진행되었는지 확인할 수 있습니다.

베이스라인을 생성하려면 다음을 수행합니다.

1. 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **기준선**&#x200B;을 클릭합니다.

   프로젝트의 ![기준선 섹션](assets/baselines-section-on-project-with-header.png)

1. **새 기준선을 클릭합니다.**
1. 베이스라인의 이름을 지정합니다.
1. (선택 사항) 첫 번째 기준선인 경우 이를 기본값으로 선택할 수 있습니다.
1. **저장**&#x200B;을 클릭합니다.

   기본적으로 사용자가 생성한 베이스라인에 대해 다음 정보가 표시됩니다.

   * 기준선 이름
   * 베이스라인 입력 일자
   * 베이스라인이 생성된 프로젝트의 계획된 시작 일자
   * 베이스라인이 생성된 프로젝트의 예상 시작 일자
   * 기준선이 생성될 때의 실제 프로젝트 기간
   * 베이스라인이 생성될 때의 프로젝트 완료율 %
   * 베이스라인이 프로젝트의 기본 베이스라인인지 여부를 보여 주는 기본 베이스라인 표시기

     >[!TIP]
     >
     >동일한 보기 또는 보고서에서 두 베이스라인의 정보를 동시에 볼 수 없습니다. 동일한 보고서에서 지정된 기준 요소 및 기본 기준 요소의 정보만 볼 수 있습니다. 프로젝트 기간 동안 언제든지 기본 베이스라인으로 간주되는 베이스라인을 수정할 수 있습니다.

1. (선택 사항) **보기** 단추를 클릭한 다음 새 보기를 만들거나 현재 보기를 편집하여 보기에 필드를 추가하고 기준선 간의 추가 정보를 비교합니다. 자세한 내용은 [Adobe Workfront에서 보기 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)을 참조하세요.

## 기준선 또는 기준선 작업 보고서 만들기

기준 요소 정보를 보려면 기준 요소 또는 기준 요소 작업 보고서를 생성할 수도 있습니다. 이를 통해 하나의 보기에서 베이스라인 또는 베이스라인 작업에 대한 필드를 원하는 수만큼 표시하여 비교할 수 있습니다.

>[!TIP]
>
>베이스라인 또는 베이스라인 작업 보고서를 생성하려면 먼저 베이스라인을 생성해야 합니다.

보고서 만들기에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)를 참조하십시오.

보다 쉽게 읽을 수 있도록 기준선 또는 기준선 작업 보고서에 프로젝트 이름 그룹화를 추가하는 것이 좋습니다.

그룹화 만들기에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)를 참조하십시오.
