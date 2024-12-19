---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 스마트 할당 만들기
description: 스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다. 스마트 할당은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 작업 항목을 리소스에 할당할 때 Adobe Workfront이 사용자에게 제공하는 사용자, 역할 또는 팀에 대한 제안입니다. 스마트 할당에 대한 자세한 내용은 스마트 할당 개요를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 스마트 할당 만들기

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">이 페이지에서 강조 표시된 정보는 빠른 릴리스를 사용하도록 설정한 고객의 프로덕션 환경에서만 사용할 수 있는 기능을 참조합니다.</span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>을 참조하세요.

<span class="preview"> 이 기능은 2025년 1월에 25.1 릴리스로 빠른 릴리스를 활성화한 고객의 프로덕션 환경에서 제거됩니다. 25.1 릴리스에 대한 자세한 내용은 [2025년 1분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)를 참조하십시오.

스마트 할당을 사용하여 작업을 완료하는 데 가장 적합한 사용자를 식별할 수 있습니다.

스마트 할당은 작업 항목을 리소스에 할당할 때 Adobe Workfront이 사용자에게 제공하는 사용자, 역할 또는 팀에 대한 제안입니다. Workfront은 작업에 가장 적합한 리소스를 결정하는 알고리즘을 기반으로 제안을 합니다.

<span class="preview">Workfront에는 작업과 문제에 대해 다르게 작동하는 스마트 할당을 계산하는 두 가지 알고리즘이 있습니다.</span>

스마트 할당을 결정하는 데 사용되는 기준에 대한 자세한 내용은 [스마트 할당 개요](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td> <p>작업 및 문제에 대해 할당할 수 있는 Contribute 이상의 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 스마트 할당 만들기

스마트 할당은 Workfront에서 할당할 수 있는 대부분의 위치에서 사용할 수 있습니다.

1. 다음 영역으로 이동하여 **할당** 또는 **할당 대상** 필드를 클릭합니다.

   * 작업 또는 문제 목록 또는 보고서
   * 작업 또는 문제 헤더
   * 작업 또는 문제 요약 패널
   * <span class="preview">새 작업</span> 또는 새 문제 상자 <span class="preview">새 작업</span> 또는 문제를 프로젝트에 추가할 때
   * 업무 균형자의 작업 또는 문제

1. 지정 필드에 커서를 놓고 2초 동안 기다립니다.

   문제의 경우 스마트 할당이 다음 섹션에 표시됩니다.

   * **사용자 및 팀**
   * **작업 역할**

   ![](assets/smart-assignments-issue-header.png)

   작업의 경우, 스마트 할당은 알고리즘 계산에서 할당을 식별하는 단계에 따라 다음 섹션에 표시됩니다.

   * <span class="preview">**제안된 할당**: 작업 스마트 할당 알고리즘의 첫 번째 단계에서 식별된 할당을 표시합니다.</span>
   * **사용자 및 팀**, **작업 역할** 또는 <span class="preview">**등급 카드 작업 역할**</span>: 작업 스마트 할당의 알고리즘 계산의 두 번째 단계에서 확인된 할당입니다.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   자세한 내용은 [스마트 할당 개요](../../../manage-work/tasks/assign-tasks/smart-assignments.md)를 참조하십시오.

1. 이름을 클릭하여 권장 사항 목록에서 리소스를 선택합니다.

1. (선택 사항) 자신에게 작업 항목을 할당하려면 **나에게 할당**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >제안이 없으면 제안 목록이 열리지 않습니다.

1. (선택 사항) 스마트 할당 목록에서 권장되는 사용자 중 하나를 사용하지 않으려면 원하는 리소스 이름을 입력하고 목록에 표시될 때 해당 이름을 선택합니다.
1. 할당하려면 **Enter**&#x200B;를 클릭하세요.

   선택한 사용자가 작업 또는 문제에 할당되었습니다.
