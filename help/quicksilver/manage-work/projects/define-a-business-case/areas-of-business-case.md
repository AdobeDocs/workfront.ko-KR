---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 비즈니스 사례 영역 개요
description: 이 문서에서는 프로젝트의 비즈니스 사례 영역에 대해 설명합니다.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 2%

---

# 비즈니스 사례 영역 개요

이 문서에서는 프로젝트의 비즈니스 사례 영역에 대해 설명합니다.

프로젝트에 대한 비즈니스 사례 생성에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

프로젝트 정보 섹션을 제외하고 프로젝트에 비즈니스 사례 섹션을 모두 표시해야 Adobe Workfront 관리자 또는 그룹 관리자가 이 섹션을 활성화해야 합니다. 프로젝트 정보 섹션은 기본적으로 활성화되어 있습니다.

Business Case 영역 활성화에 대한 자세한 내용은  [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

다음은 프로젝트의 Business Case에 있는 영역입니다.

* 프로젝트 정보
* 목표
* 경비
* 리소스 예산 책정
* 위험
* 스코어카드
* 사용자 정의 양식
* 비즈니스 사례 요약

## 프로젝트 정보

다음 **프로젝트 정보** 비즈니스 케이스의 영역은 Workfront 관리자가 구성할 수 없습니다. 모든 프로젝트에는 비즈니스 케이스에 프로젝트 정보 영역이 있습니다. 

비즈니스 케이스의 프로젝트 정보 섹션에는 프로젝트가 실제로 시작되기 전에 프로젝트의 기본 정보가 포함됩니다.

다음 필드를 편집하는 것이 좋습니다.

* **설명**: 프로젝트에 대한 설명을 지정합니다.
* **프로젝트 소유자**

   기본적으로 프로젝트를 만드는 사용자도 프로젝트 소유자입니다. 이 필드를 편집하고 다른 활성 사용자를 프로젝트 소유자로 표시할 수 있습니다.

* **프로젝트 스폰서**

   프로젝트 소유자가 아닌 다른 사람을 프로젝트의 스폰서로 추가하는 것이 좋습니다. 후원자는 비즈니스 사건의 승인을 받습니다. 

* **Portfolio**: 프로젝트에 대한 Portfolio을 지정합니다. Portfolio을 만들고 다음 상태에 배치해야 합니다. **활성** 먼저 이 드롭다운 메뉴에서 을(를) 선택할 수 있습니다.

   포트폴리오에 대한 자세한 내용은 [Adobe Workfront의 Portfolio 개요](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   Portfolio 만들기에 대한 자세한 내용은 [포트폴리오 만들기](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **계획된 혜택**: 이 프로젝트가 완료될 때 조직에 대해 계획된 금전적 이익을 예측합니다. 모든 통화 금액일 수 있으며 양수 값이어야 합니다. 예를 들어 $10,000입니다.
* **상태**: 기본적으로 프로젝트 요청에 대한 상태 는 로 설정됩니다 **아이디어**.

   상태를 Idea 또는 Planning 이외의 것으로 변경하는 경우 **제출** 버튼이 비즈니스 사례 요약 영역에서 사라지므로 더 이상 비즈니스 사례를 제출하여 승인을 받을 수 없습니다. 

* **고정 시작 날짜**: 프로젝트를 시작할 날짜를 지정합니다.
* **고정 종료 날짜**: 프로젝트를 종료하려는 날짜를 지정합니다.

   >[!NOTE]
   >
   >업무 사례의 고정 시작 및 종료 일자는 프로젝트의 계획 시작 및 완료 일자에 영향을 주지 않습니다. 이것은 프로젝트 작성자가 프로젝트를 이상적으로 개발할 시기에 대해 요청한 날짜를 나타냅니다. 대신 프로젝트의 계획 시작 및 계획 완료 일자는 프로젝트의 작업을 기반으로 하는 프로젝트에 대한 계획 타임라인을 표시합니다.

## 목표

목표는 프로젝트의 목표를 정의합니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다. 이 필드에는 우선 순위 순서대로 목표가 표시됩니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
프로젝트의 개별 비즈니스 사례에 연결되지 않은 조직에 대한 전략적 목표를 만들 수 있습니다. 전략적 목표를 만들려면 Adobe Workfront 목표에 액세스할 수 있어야 합니다. 그런 다음 해당 비즈니스 사례 외부의 프로젝트에 연결할 수 있습니다. Workfront 목표를 사용하여 목표를 만드는 방법에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../../workfront-goals/goal-management/wf-goals-overview.md).

목표 정의는 프로젝트가 Portfolio 최적기에서 점수를 받는 데 선택 사항입니다. 이 섹션은 비즈니스 사례에서 유일한 선택적 섹션입니다. Portfolio 최적기에서 프로젝트 점수가 매겨지기 전에 비즈니스 사례의 다른 모든 섹션을 완료해야 합니다. 목표를 만들 때 목표에 대한 우선순위 수준을 나타낼 수 있습니다.

목표에 대한 자세한 내용은  [비즈니스 사례 목표 생성](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## 경비

비용은 프로젝트 수명 동안 발생할 수 있는 비인적 비용을 나타냅니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다. 

업무 사례에 입력하는 모든 비용은 프로젝트의 비용 탭에 계획 비용으로 표시됩니다.

비용은 프로젝트의 다음 필드에 영향을 줍니다.

* 예산 비용
* 순 가치

예산책정된 비용 및 순 값에 대한 자세한 내용은 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

비용에 대한 자세한 내용은  [프로젝트 비용 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

Workfront 관리자는 사용자 정의 비용 유형을 설정할 수 있습니다.

사용자 지정 비용 유형 생성에 대한 자세한 내용은 [사용자 지정 비용 유형 만들기](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## 리소스 예산 책정

업무 사례의 자원 예산 관리 영역에서 다음 작업을 수행할 수 있습니다.

* 리소스 풀을 프로젝트와 연결합니다.
* 프로젝트 수준에서 리소스 예산을 책정합니다.

프로젝트 자원에 대한 예산책정된 시간이 업무 사례의 자원 예산 영역(Resource Budgeting)에 표시되어 프로젝트의 예산책정된 노무비를 생성합니다. 비즈니스 케이스의 이 영역은 기본적으로 활성화되어 있습니다.

업무 사례에서 프로젝트에 대한 예산 책정 자원에 대한 자세한 내용은 [비즈니스 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

업무 사례의 자원 예산 관리 섹션을 볼 때 다음 사항을 고려하십시오.

* 다음 도구를 사용하여 여기에 자원 정보를 예산을 편성할 수 있습니다.

   * 리소스 플래너

      자세한 내용은 [자원 계획자를 사용하여 업무 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * 시나리오 플래너 (회사에서 Adobe 시나리오 플래너에 대한 추가 라이센스를 구입한 경우)

      자세한 내용은 [시나리오 계획자를 사용하여 비즈니스 사례의 예산 자원](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 계획자 개요](../../../scenario-planner/scenario-planner-overview.md).

* 여기에 표시되는 정보는 시스템 레벨 자원 계획자 또는 시나리오 계획자에도 표시됩니다. 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* 자원 예산 편성 후 역할이 시간당 원가와 연관되어 있는 경우 프로젝트의 예산책정된 노무비가 자원 예산 책정 영역에 표시됩니다. 예산책정된 노무비는 프로젝트의 통화로 표시됩니다.

   >[!IMPORTANT]
   예산책정된 노무비는 사용자가 아닌 프로젝트의 역할과 연관된 비용입니다. 사용자에 대한 모든 예산책정된 노무비 합계는 사용자와 연관된 Job 역할의 예산책정된 노무비 합과 다를 수 있습니다. 

   예산책정된 노무비에 대한 자세한 내용은 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   작업 역할 생성 및 시간당 비용 연관 방법에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## 위험

위험 요소는 프로젝트가 제 시간에 또는 예산에 따라 끝나지 않도록 막을 수 있는 요소들입니다. 이러한 요소를 정의하는 것은 Portfolio 관리자 또는 프로젝트 후원자가 프로젝트 승인에 대해 교육적인 결정을 내리는 데 중요합니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다.

잠재적 비용과 발생 시 정의한 위험을 연관시킬 수 있습니다. 프로젝트의 위험 비용이 프로젝트의 순 값에 영향을 줍니다. 

프로젝트 순 값에 대한 자세한 내용은 다음을 참조하십시오 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

위험 생성에 대한 자세한 내용은  [프로젝트에서 위험 요소 생성 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Workfront 관리자는 사용자 지정 위험 유형을 설정할 수 있습니다.

사용자 지정 위험 유형 만들기 및 편집에 대한 자세한 내용은 [위험 유형 편집 및 생성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## 스코어카드

스코어카드는 프로젝트의 정렬을 측정합니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다.

프로젝트에 스코어카드를 적용하고 정렬 점수를 생성하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [프로젝트에 스코어카드를 적용하고 정렬 점수를 생성합니다](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

스코어카드를 적용하려면 Workfront 관리자가 스코어카드를 만들어야 합니다. 다음 **스코어카드** 스코어카드가 만들어지지 않는 경우 Business Case 영역이 표시되지 않습니다.

스코어카드 만들기에 대한 자세한 내용은  [스코어카드 만들기](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## 사용자 정의 양식

비즈니스 사례를 정의할 때 프로젝트에 사용자 지정 Forms 를 첨부할 수 있습니다. 이 영역은 비즈니스 케이스에서 기본적으로 활성화되지 않습니다. Workfront 관리자가 비즈니스 사례에 표시할 수 있도록 설정해야 합니다.

Business Case 영역 활성화에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

사용자 지정 양식을 적용하려면 Workfront 관리자가 먼저 사용자 지정 양식을 만들어야 합니다.

사용자 지정 양식 만들기에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

사용자 지정 양식을 사용하여 비즈니스 케이스의 다른 필드에 표시되지 않는 추가 정보를 수집할 수 있습니다.

사용자 지정 양식 적용에 대한 자세한 내용은 [비즈니스 사례에 사용자 지정 양식 첨부](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## 비즈니스 사례 요약

* [비즈니스 사례 요약 개요](#overview-of-the-business-case-summary)
* [비즈니스 사례 내보내기](#export-the-business-case)

### 비즈니스 사례 요약 개요 {#overview-of-the-business-case-summary}

비즈니스 사례 요약 패널의 비즈니스 사례 오른쪽 상단 모서리에서 주요 프로젝트 재무 및 프로젝트가 스코어카드에 정렬되었는지 여부를 요약하여 볼 수 있습니다.

비즈니스 사례 요약을 편집할 수 없습니다. 이것은 재무 필드 및 스코어카드와 관련된 프로젝트의 상태에 대한 빠른 보기입니다. \
 

비즈니스 사례 요약에 다음 필드가 표시됩니다.

* 프로젝트 순 값
* 프로젝트 예산책정된 원가
* 잠재적 위험 비용
* 계획된 혜택
* 정렬 점수

이러한 필드에 대한 자세한 내용은 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### 비즈니스 사례 내보내기 {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

비즈니스 사례를 인쇄하거나 보다 압축된 형식으로 전자 메일에 첨부해야 하는 경우 PDF 파일로 내보낼 수 있습니다. 

자세한 내용은 [프로젝트의 비즈니스 사례 내보내기](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
