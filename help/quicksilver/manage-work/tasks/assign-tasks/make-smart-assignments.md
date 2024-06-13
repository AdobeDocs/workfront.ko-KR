---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 스마트 할당 만들기
description: 스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 작업 항목을 리소스에 할당할 때 Adobe Workfront이 사용자에게 제공하는 사용자, 역할 또는 팀에 대한 제안입니다. 스마트 할당에 대한 자세한 내용은 스마트 할당 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# 스마트 할당 만들기

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객의 미리보기 환경 또는 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서만 사용할 수 있습니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 활성화 또는 비활성화](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">현재 릴리스에 대한 자세한 내용은 [2024년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다.

스마트 할당은 작업 항목을 리소스에 할당할 때 Adobe Workfront이 사용자에게 제공하는 사용자, 역할 또는 팀에 대한 제안입니다. Workfront은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 제안을 합니다.

<span class="preview">Workfront에는 작업 및 문제에 대한 두 개의 분리된 알고리즘이 있습니다. </span>

스마트 할당 결정에 사용되는 기준에 대한 자세한 내용은 [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>새로운 기능: 표준</p>
      또는
      <p>현재: 작업 시간 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 문제에 대한 액세스 편집</p> <p>프로젝트에 대한 보기 또는 상위 액세스 권한</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 문제에 할당할 수 있는 권한으로 기여하거나 더 높은 권한 부여</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 스마트 할당 만들기

스마트 할당은 Workfront에서 할당할 수 있는 대부분의 위치에서 사용할 수 있습니다.

1. 다음 영역으로 이동하여 **할당** 또는 **할당 대상:** 필드:

   * 작업 또는 문제 목록 또는 보고서
   * 작업 또는 문제 헤더
   * 작업 또는 문제 요약 패널
   * <span class="preview">새 작업 또는 문제를 프로젝트에 추가할 때 표시되는 새 작업 또는 새 문제 상자</span>
   * 홈 영역에 나열된 항목에 대한 지정 필드
   * 업무 균형자의 작업 또는 문제

1. 할당 필드에 커서를 놓고 2초 동안 기다립니다.

   <div class="preview">
   스마트 할당 제안을 포함하는 다음 섹션 중 하나 또는 여러 섹션이 표시됩니다.

   * **제안된 할당**: 작업용으로 표시됩니다.

     >[!TIP]
     >
     >   목록 헤더가 표시됩니다. **다음은 몇 가지 권장 사항입니다** 대신 **제안된 할당** 프로덕션 환경에서.
     >
   * **기타 할당**: 작업 및 문제에 대해 표시됩니다.
   * **사용자 및 팀**: 작업 및 문제에 대해 표시됩니다.
   * **작업 역할**: 작업 및 문제를 표시합니다.
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   작업의 경우, 스마트 할당은 알고리즘 계산에서 할당을 식별하는 단계에 따라 다음 섹션에 표시됩니다.

   * **제안된 할당**: 작업 스마트 할당의 알고리즘 계산 첫 번째 단계에서 확인된 할당입니다. <span class="preview">이 섹션은 문제에 사용할 수 없습니다.</span>
   * <span class="preview">**기타 할당**, **사용자 및 팀**, 또는 **작업 역할**: 작업 스마트 할당의 알고리즘 계산 두 번째 단계에서 식별된 할당입니다. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   자세한 내용은 [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Recommendations 목록에서 해당 이름을 클릭하여 사용자를 선택합니다.

1. (선택 사항) **나에게 할당** 작업 항목을 자신에게 할당합니다.

   >[!TIP]
   >
   >제안이 없으면 제안 목록이 열리지 않습니다.

1. (선택 사항) 스마트 할당 목록에서 권장되는 사용자 중 하나를 사용하지 않으려면 원하는 리소스 이름을 입력하고 목록에 표시될 때 해당 이름을 선택합니다.
1. 클릭 **입력** 할당에 사용됩니다.

   선택한 사용자가 작업 또는 문제에 할당되었습니다.
