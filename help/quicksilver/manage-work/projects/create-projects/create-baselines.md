---
product-area: projects
navigation-topic: create-projects
title: 프로젝트 기준 요소 만들기
description: 베이스라인은 프로젝트 초기 계획 또는 프로젝트 수명 동안 지정된 시간에 포함된 주요 정보를 나타내는 프로젝트 스냅샷입니다.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# 프로젝트 기준 요소 만들기

베이스라인은 프로젝트 초기 계획 또는 프로젝트 수명 동안 지정된 시간에 포함된 주요 정보를 나타내는 프로젝트 스냅샷입니다.

기준 요소를 사용하여 현재 계획의 정보 조각을 원래 계획 또는 다른 시점과 비교하여 시간 경과에 따른 문제 작업, 범위 크리프 및 기타 추세를 식별할 수 있습니다.

## 액세스 요구 사항

<!--
drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>참고</b>
   여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>기준선을 보려면 프로젝트 또는 그 이상에 대한 권한을 봅니다</p> <p>프로젝트에 대한 권한을 관리하여 기준 요소 만들기</p> <p> 프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 기준선 작업에 대한 고려 사항

* 프로젝트 수명 동안 여러 번 프로젝트의 진행 상태 스냅샷을 캡처하여 여러 베이스라인을 생성할 수 있습니다.
* 베이스라인을 생성하거나 베이스라인 보고서를 작성하여 프로젝트의 베이스라인에 포함된 정보를 볼 수 있습니다.
* 베이스라인을 생성하면 해당 베이스라인의 베이스라인 작업에도 작업 정보가 캡처됩니다.
* 베이스라인 작업 보고서를 작성하면 베이스라인 작업의 정보를 볼 수 있습니다.

>[!IMPORTANT]
>
>기준 요소는 프로젝트의 이름, 날짜 및 재무 정보에 대한 스냅숏을 만듭니다. 베이스라인에는 프로젝트의 사용자 지정 필드 값이 포함되지 않습니다. 베이스라인에 포함된 재무 정보에 대한 자세한 내용은 [프로젝트 기준에 포함된 프로젝트 재무](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## 기준선 만들기

다음과 같은 방법으로 베이스라인을 생성할 수 있습니다.

* **자동**: Workfront 관리자 또는 그룹 관리자는 프로젝트가 [현재]이 되면 Workfront에 대한 프로젝트 기본 설정을 설정하여 자동으로 베이스라인을 만듭니다. 이 설정을 사용하면 프로젝트 상태가 [현재]가 되면 베이스라인이 생성됩니다. 이 설정을 사용하지 않는 경우에는 수동으로 기준선을 만들어야 합니다.

   프로젝트 환경 설정 구성 및 자동 베이스라인 작성 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!CAUTION]
   >
   >이 설정을 사용하면 프로젝트의 상태가 [현재]로 변경될 때마다 프로젝트에 대한 베이스라인이 자동으로 만들어집니다. 처음 생성된 베이스라인이 기본값입니다. 프로젝트 수명 동안 다른 모든 기준선을 수동으로 만들어야 합니다.

* **수동으로**: 프로젝트가 진행될 때 필요에 따라 프로젝트에 대한 새 베이스라인을 생성할 수 있습니다. 그런 다음 베이스라인을 비교하여 시간이 지남에 따라 프로젝트가 어떻게 진행되는지 확인할 수 있습니다.

베이스라인을 생성하려면 다음과 같이 하십시오.

1. 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **기준선**.

   또는

   클릭 **자세히 표시**&#x200B;를 클릭한 다음 **기준선**.

   ![](assets/nwe-baselines-section-on-project-with-header-350x78.png)

1. 클릭 **새 기준선.**
1. 베이스라인의 이름을 지정합니다.
1. (선택 사항) 첫 번째 베이스라인인 경우 기본값으로 선택할 수 있습니다.
1. **저장**&#x200B;을 클릭합니다.

   기본적으로 생성한 베이스라인에 대한 다음 정보가 표시됩니다.

   * 기준선 이름
   * 베이스라인 시작 날짜
   * 베이스라인 작성 시 프로젝트의 계획된 시작 일자
   * 베이스라인이 작성된 프로젝트의 예상 시작 날짜
   * 베이스라인을 만든 프로젝트의 실제 지속 시간
   * 베이스라인을 만들 때 프로젝트의 완료율
   * 베이스라인이 프로젝트의 기본 베이스라인인지 여부를 표시하는 기본 베이스라인 표시기입니다

      >[!TIP]
      >
      >동일한 보기 또는 보고서에서 두 기준선에서 동시에 정보를 볼 수 없습니다. 동일한 보고서의 지정된 기준 요소 및 기본 기준 요소에서 정보만 볼 수 있습니다. 프로젝트 수명 동안 언제든지 기본 베이스라인(Default baseline)으로 간주되는 베이스라인을 수정할 수 있습니다.

1. (선택 사항) 보기 옆의 드롭다운 화살표를 클릭한 다음, **보기 사용자 지정** 을 클릭하여 보기에 필드를 추가하고 기준 요소 간에 추가 정보를 비교합니다.

## 베이스라인 또는 베이스라인 작업 보고서 작성

베이스라인 정보를 보려면 베이스라인 또는 베이스라인 작업 보고서를 생성할 수도 있습니다. 이렇게 하면 기준선 또는 베이스라인 작업에 대한 여러 필드를 표시하여 하나의 보기에서 비교할 수 있습니다.

>[!TIP]
>
>베이스라인 또는 베이스라인 작업 보고서를 생성하려면 먼저 베이스라인을 생성해야 합니다.

보고서 만들기에 대한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

보다 쉽게 읽을 수 있도록 프로젝트 이름 그룹을 기준선 또는 기준선 보고서에 추가하는 것이 좋습니다.

그룹 생성에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
