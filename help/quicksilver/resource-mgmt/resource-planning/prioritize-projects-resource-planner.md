---
product-area: resource-management;projects
navigation-topic: resource-planning
title: 리소스 계획자에서 프로젝트 우선 순위 지정
description: 가장 중요한 프로젝트가 맨 위에 있는 자원 계획자에서 우선 순위 순서로 프로젝트가 나열됩니다.
author: Alina
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 1%

---

# 리소스 계획자에서 프로젝트 우선 순위 지정

가장 중요한 프로젝트가 맨 위에 있는 자원 계획자에서 우선 순위 순서로 프로젝트가 나열됩니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 계획자의 우선순위 및 예산 시간 편집에 대한 액세스 권한을 포함하는 리소스 관리에 대한 액세스 편집</p> <p>재무 데이터, 프로젝트 및 사용자에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 기능을 사용하여 예산을 책정하려는 프로젝트에 대한 권한을 관리합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 리소스 플래너의 기본 프로젝트 순서

기본적으로 프로젝트는 아래 기준을 고려하여 리소스 계획자의 프로젝트 보기에 나열됩니다.

>[!IMPORTANT]
>
>Resource Planner를 처음 열 때만 아래의 세 가지 기준에 따라 프로젝트가 나열됩니다. 그러나 이 기본 우선 순위는 자동으로 사용자 지정 우선 순위가 되며 다음 중 하나를 수행할 때마다 원래 우선 순위로 되돌릴 수 없습니다.
>
>* 언제든지 저장 을 클릭합니다.
>* 수동으로 프로젝트 계획 우선순위를 변경하는 경우. 프로젝트 계획 우선 순위 수동으로 변경에 대한 자세한 내용은 섹션을 참조하십시오 [수동으로 프로젝트 계획 우선순위 변경](#manually-change-the-project-planning-priority) 참조하십시오.
>
>프로젝트 우선 순위가 사용자 지정 우선 순위가 되면 프로젝트 정보의 변경 사항이 이러한 기준을 사용하여 프로젝트의 순서에 더 이상 영향을 주지 않습니다. 이후 프로젝트의 우선 순위는 수동으로만 지정할 수 있습니다.

프로젝트 보기에서 프로젝트를 나열하기 위한 원래 기본 기준은 다음과 같습니다.

1. 프로젝트에 대한 정렬 점수별로.\
   프로젝트의 정렬 점수에 대한 자세한 내용은 다음을 참조하십시오 [프로젝트에 스코어카드를 적용하고 정렬 점수를 생성합니다](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. 프로젝트의 계획 시작 일자까지(정렬 필드가 null이거나 여러 프로젝트에 대해 동일한 경우).
1. 사전순(정렬 필드가 null이거나 동일하고 여러 프로젝트에 대해 계획 시작 날짜가 동일하면)

자원 계획자에서 프로젝트 우선순위를 사용할 때 다음 사항을 고려하십시오.

* 프로젝트 보기를 적용하는 경우에만 프로젝트 우선순위를 수동으로 사용자 지정할 수 있습니다. 이렇게 하면 Resource Planner의 프로젝트 순서가 변경됩니다.
* 리소스 계획자에서 역할 또는 사용자 뷰를 적용하면 프로젝트 뷰에 설정된 우선순위 순서와 동일한 순서로 프로젝트가 나타납니다.
* 리소스 계획자의 프로젝트 순서는 고유한 것입니다. 다른 사용자는 리소스 계획자에서 동일한 프로젝트를 볼 수 있지만 다른 순서로 볼 수 있습니다. 프로젝트 계획 우선순위 필드에 대해서는 보고할 수 없습니다. 이는 리소스 계획자에서만 표시되며 프로젝트 우선 순위를 지정하는 플래그 역할을 합니다.

포트폴리오와 연결된 프로젝트에는 포트폴리오 수준의 우선 순위가 있을 수 있습니다. 자원 계획자 우선순위 외에 자원 계획자에서 프로젝트의 포트폴리오 우선순위를 볼 수 있습니다. 포트폴리오 우선 순위에 따라 프로젝트에 순서를 지정할 수도 있습니다.

## 수동으로 프로젝트 계획 우선순위 변경 {#manually-change-the-project-planning-priority}

자원 계획자에서 프로젝트 순서를 변경하려면 자원 관리에 대한 편집 액세스 및 프로젝트에 대한 관리 권한이 있어야 합니다.

프로젝트에 새로운 우선 순위를 부여함으로써, 여러분은 프로젝트의 중요도에 따라 순위를 정할 수 있습니다.

프로젝트 계획 우선순위를 편집하려면

1. 로 이동합니다. **리소스 플래너**.

1. 번호가 들어 있는 프로젝트 이름의 왼쪽에 있는 필드 내부를 클릭하고 Planning 우선 순위를 변경할 숫자를 입력한 다음 Enter 키를 누릅니다.\
   ![](assets/mceclip4.png)\
   또는\
   프로젝트 이름 위로 마우스를 가져간 다음 프로젝트 이름의 왼쪽에 있는 표시기를 클릭하고 드래그하여 올바른 위치에 놓아 우선순위를 변경합니다.

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   프로젝트에 우선순위를 매길 숫자를 선택하는 경우 우선 순위가 더 높은(더 중요한) 우선 순위의 경우에는 낮은 숫자, 낮은(덜 중요한) 우선 순위의 경우 높은 숫자를 선택합니다. 프로젝트의 우선순위 번호를 낮은 번호(높은 우선순위)로 변경하면 리소스 계획자의 다른 모든 프로젝트가 목록에서 아래로 이동합니다(덜 중요함).\
   프로젝트의 우선순위 수를 더 높은 번호(낮은 우선순위)로 변경하면 리소스 계획자의 다른 모든 프로젝트가 목록에서 위로 이동합니다(더 중요해지기).

1. **저장**&#x200B;을 클릭합니다.\
   프로젝트 순서는 선택에 따라 변경되며 리소스 계획자에서 사용자 지정 프로젝트 우선순위가 됩니다. 다른 사용자는 Resource Planner에서 동일한 프로젝트를 볼 수 있지만 Resource Planner에서 프로젝트의 우선 순위 순서를 볼 수 없습니다.

## 리소스 플래너의 Portfolio 우선 순위에 따라 프로젝트 주문

>[!IMPORTANT]
>
>Portfolio 최적화 프로그램에서 프로젝트의 우선 순위를 정하려면 회사에 Business 또는 Workfront 계획이 있어야 합니다.
>
>Workfront 계획에 대한 자세한 내용은 [Adobe의 계획](https://www.workfront.com/plans).
>
>Portfolio 최적기에서 프로젝트 우선 순위에 대한 자세한 내용은 [Portfolio 최적기에서 프로젝트 우선 순위 지정](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. 를 엽니다. **리소스 플래너** 에서 **프로젝트 보기**.
1. 을(를) 클릭합니다. **설정** 아이콘.
1. 를 활성화합니다 **Portfolio 우선순위 표시** 프로젝트 우선순위를 지정되는 Portfolio에 따라 표시하도록 설정하는 중입니다. 해당 포트폴리오에 따라 프로젝트의 우선순위가 리소스 계획자 우선순위 옆에 표시됩니다. 이 설정은 기본적으로 비활성화됩니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   프로젝트의 포트폴리오 우선순위는 자원 계획자의 프로젝트 뷰에만 표시됩니다.

1. 클릭 **주문** 프로젝트 순서를 포트폴리오 우선 순위에 따라 지정합니다.

   둘 이상의 포트폴리오에 속하는 프로젝트가 있는 경우 리소스 계획자에서 포트폴리오 우선 순위가 동일한 여러 프로젝트를 볼 수 있습니다. 이 경우 포트폴리오 우선 순위가 동일한 프로젝트가 다음 기준으로 이 순서로 나열됩니다.

   1. 정렬 점수
   1. 계획된 시작 일자
   1. 프로젝트 이름

   ![](assets/rp-portfolio-priority-ordered-350x198.png)

1. **저장**&#x200B;을 클릭합니다.

## Project Planning 우선 순위 변경이 사용 가능 시간에 미치는 영향

프로젝트 계획 우선 순위는 사용 가능한 사용자 시간에 영향을 줍니다. 우선 순위가 가장 높은 프로젝트와 연결된 사용자는 일정에 따라 이 프로젝트의 AVL(사용 가능 시간) 열에 대한 최대 가용성을 보여줍니다.

우선순위 순서로 두 번째 프로젝트에 연관된 동일한 사용자는 가용 시간 값의 전체 금액과 예산책정된 시간 열의 첫 번째 프로젝트에 대해 이미 예산책정된 시간 간의 차이인 가용 시간 값을 표시합니다. 리소스 계획자의 예산 책정 자원에 대한 자세한 내용은 [프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

사용자에 대한 첫 번째 프로젝트에 대한 시간(우선 순위) 예산이 책정되지 않았지만 동일한 사용자에 대해 두 번째 프로젝트에 대한 시간 예산이 책정된 경우 두 프로젝트 모두에 대해 사용 가능한 시간의 전체 양이 표시됩니다.

사용자가 항상 사용 가능한 시간을 정확하게 볼 수 있도록 자원 계획자의 프로젝트 순서대로 사용자에 대한 예산책정 시간 열을 갱신하는 것이 좋습니다.

>[!NOTE]
>
>프로젝트 계획 우선순위는 모든 리소스 관리자에 고유하므로 두 번째 우선 순위 프로젝트는 리소스 계획자에서 동일한 프로젝트를 보는 다른 사용자의 첫 번째 우선 순위 프로젝트일 수 있습니다. 다른 리소스 관리자가 첫 번째 프로젝트에 대한 리소스를 예산을 책정하는 경우 해당 변경에 따라 첫 번째 프로젝트에 대한 해당 리소스에 대해 사용 가능한 시간이 줄어듭니다.
>
>시간을 먼저 할당하는 사용자는 해당 리소스를 할당하고 시스템 전체에서 해당 리소스에 대한 사용 가능한 시간 수를 줄입니다. 가용 시간 금액은 Resource Planner에서 자원에 대한 예산책정된 시간이 저장되는 즉시 모든 사용자에 대해 갱신되어야 합니다.
>
>사용 가능한 시간에 대한 자세한 내용은 [자원 가용성 및 할당](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
