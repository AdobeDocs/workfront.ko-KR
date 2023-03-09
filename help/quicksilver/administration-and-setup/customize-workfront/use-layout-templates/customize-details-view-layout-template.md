---
title: 레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Workfront 관리자는 작업, 문제, 문서, 프로그램 또는 포트폴리오를 보는 동안 사용자가 왼쪽 패널에서 세부 정보 섹션을 선택할 때 레이아웃 템플릿을 사용하여 표시되는 정보를 결정할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리보기 환경에서만 사용할 수 있습니다.</span>

Adobe Workfront 관리자는 레이아웃 템플릿을 사용하여 사용자가 세부 정보 아이콘을 클릭할 때 표시되는 정보를 확인할 수 있습니다 ![](assets/project-details-icon.png) 작업, 문제, 문서, 프로그램 또는 포트폴리오를 보는 동안 왼쪽 패널에서

<!--
or billing record
-->

이 정보가 표시되는 정보의 순서를 변경할 수도 있습니다. 예를 들어, 사용자가 보는 모든 작업에 대해 사용자 정의 Forms 정보를 사용자가 보는 모든 작업에 대한 세부 정보 보기의 맨 위로 이동할 수 있습니다.

객체에 대한 세부 정보 보기의 변경 사항은 사용자가 다음 영역에서 볼 수 있는 필드의 가용성과 순서를 결정합니다.

* 새 작업 및 새 문제와 같은 &quot;새 개체&quot; 상자

   ![](assets/new-task-dialog.png)

* 작업 편집, 문제 편집 및 프로젝트 편집과 같은 &quot;개체 편집&quot; 화면

   ![](assets/edit-task-screen.png)


* <span class="preview">프로젝트 편집과 같이 프로젝트를 일괄 편집할 때 &quot;오브젝트 편집&quot; 화면</span>

   <span>![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)</span>
-->

* 요약 ![](assets/summary-panel-icon.png) 작업 및 문제 목록 패널

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >레이아웃 템플릿을 변경하면 로그인한 사용자에게 할당된 작업 및 문제에 대해서만 요약 패널의 필드 순서 및 가용성에 영향을 줍니다.

* 문제를 작업으로 변환 또는 문제를 프로젝트로 변환 상자와 같은 변환 상자.

   ![문제를 작업 상자로 변환](assets/convert-issue-to-task-box.png)

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 세부 정보 보기에 표시되는 사용자 지정

1. 에 설명된 대로 레이아웃 템플릿에서 작업 시작 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 아래쪽 화살표 클릭 ![](assets/dropdown-arrow-12x12.png) 아래에 **사용자에게 표시되는 항목 맞춤화**&#x200B;을 클릭한 다음 을 클릭합니다 **프로젝트**, **작업**, **문제**, **프로그램**, 또는 **Portfolio.**
<!--
, or billing record
-->

1. 다음에서 **세부 사항** 섹션에서 다음 중 하나를 수행하여 사용자가 세부 정보 보기에 표시되는 내용을 사용자 지정합니다.

   * 섹션 머리글을 드래그합니다 ![](assets/move-icon---dots.png) 주문을 변경하려고 합니다.
   * 아래의 옵션 활성화 또는 비활성화 **개요** 및 **사용자 지정 Forms** 표시하거나 숨깁니다.

      이러한 섹션 중 하나에 있는 모든 필드를 숨기면 전체 섹션이 숨겨집니다.

      모든 필드는 기본적으로 활성화되어 있습니다.

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.
