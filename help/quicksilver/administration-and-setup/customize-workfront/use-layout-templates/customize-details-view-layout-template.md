---
title: 레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Workfront 관리자는 작업, 문제, 문서, 프로그램 또는 포트폴리오를 보는 동안 사용자가 왼쪽 패널에서 세부 정보 섹션을 선택할 때 레이아웃 템플릿을 사용하여 표시되는 정보를 결정할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Adobe Workfront 관리자는 작업, 문제, 문서, 프로그램 또는 포트폴리오를 보는 동안 사용자가 왼쪽 패널의 세부 정보 아이콘 ![세부 정보 아이콘](assets/project-details-icon.png)을 클릭할 때 표시되는 정보를 결정할 때 레이아웃 템플릿을 사용할 수 있습니다.

<!--
or billing record
-->

이 정보가 표시되는 정보의 순서를 변경할 수도 있습니다. 예를 들어, 사용자가 보는 모든 작업에 대해 사용자 정의 Forms 정보를 사용자가 보는 모든 작업에 대한 세부 정보 보기의 맨 위로 이동할 수 있습니다.

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

객체에 대한 세부 정보 보기의 변경 사항은 사용자가 다음 영역에서 볼 수 있는 필드의 가용성과 순서를 결정합니다.


* Create Task와 같은 &quot;Create object&quot; 상자

  ![새 작업 대화 상자](assets/new-task-dialog.png)


* 작업 편집, 문제 편집 및 프로젝트 편집과 같이 오브젝트를 편집할 때 &quot;오브젝트 편집&quot; 화면

  ![작업 화면 편집](assets/edit-task-screen.png)


* 오브젝트를 일괄 편집할 때 &quot;오브젝트 편집&quot; 화면이 표시됩니다. 현재 이 기능은 프로젝트 일괄 편집에 대해 지원됩니다.

  ![프로젝트 편집 사용자 지정](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* 작업 및 문제 목록에 대한 요약 패널 ![요약 패널](assets/summary-panel-icon.png)

  ![요약 영역](assets/summary-area.png)

  >[!NOTE]
  >
  >레이아웃 템플릿을 변경하면 로그인한 사용자에게 할당된 작업 및 문제에 대해서만 요약 패널의 필드 순서 및 가용성에 영향을 줍니다.

* 문제를 작업으로 변환 또는 문제를 프로젝트로 변환 상자와 같은 변환 상자.

  ![문제를 작업 상자로 변환](assets/convert-issue-to-task-box.png)

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>새로운 기능: 표준</p>
  <p> 현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 세부 정보 보기에 표시되는 사용자 지정

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.
1. ![사용자에게 표시되는 내용을 사용자 지정](assets/dropdown-arrow-12x12.png)에서 아래쪽 화살표 **아래쪽 화살표**&#x200B;를 클릭한 다음 **프로젝트**, **작업**, **문제**, **프로그램** 또는 **Portfolio을 클릭합니다.**
<!--
, or billing record
-->

1. **세부 정보** 섹션에서 다음 중 하나를 수행하여 사용자가 세부 정보 보기에서 보는 내용을 사용자 지정합니다.

   * 순서를 변경하려면 섹션 머리글 ![이동 아이콘](assets/move-icon---dots.png)을 끕니다.
   * 다양한 영역(예: **개요**, **재무** 및 **사용자 지정 Forms**)에서 옵션을 활성화하거나 비활성화하여 표시하거나 숨깁니다.

     이러한 섹션 중 하나에 있는 모든 필드를 숨기면 전체 섹션이 숨겨집니다.

     모든 필드는 기본적으로 활성화되어 있습니다. 영역의 **모두 선택** 확인란을 선택하거나 선택 취소하여 해당 영역의 모든 필드를 표시하거나 숨길 수 있습니다.

   ![레이아웃 템플릿의 세부 정보 보기](assets/layout-template-details-view.png)

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.
