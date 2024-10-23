---
content-type: overview
navigation-topic: business-case-and-scorecards
title: 비즈니스 사례 영역 개요
description: 이 문서에서는 프로젝트의 비즈니스 사례 영역에 대해 설명합니다.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1603'
ht-degree: 2%

---

# 비즈니스 사례 영역 개요

이 문서에서는 프로젝트의 비즈니스 사례 영역에 대해 설명합니다.

프로젝트의 비즈니스 사례를 만드는 방법에 대한 자세한 내용은 [프로젝트의 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md)를 참조하십시오.

Adobe Workfront 관리자 또는 그룹 관리자는 비즈니스 사례의 모든 섹션을 활성화해야 프로젝트 정보 섹션을 제외하고 프로젝트에 표시됩니다. 프로젝트 정보 섹션은 기본적으로 활성화되어 있습니다.

비즈니스 사례 영역 활성화에 대한 자세한 내용은 의 &quot;비즈니스 사례&quot; 섹션을 참조하십시오.  [시스템 전체 프로젝트 환경 설정을 구성합니다](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

다음은 프로젝트의 비즈니스 사례에 있는 영역입니다.

* 프로젝트 정보
* 목표
* 경비
* 리소스 예산 책정
* 위험
* 스코어카드
* 사용자 정의 양식
* 비즈니스 사례 요약

## 프로젝트 정보

Workfront 관리자가 비즈니스 사례의 **프로젝트 정보** 영역을 구성할 수 없습니다. 모든 프로젝트에는 비즈니스 사례에 프로젝트 정보 영역이 있습니다. 

비즈니스 사례의 프로젝트 정보 섹션에는 프로젝트가 실제로 시작되기 전의 프로젝트 기본 정보가 포함됩니다.

다음 필드를 편집하는 것이 좋습니다.

* **설명**: 프로젝트에 대한 설명을 지정하십시오.
* **프로젝트 소유자**

  기본적으로 프로젝트를 만드는 사용자도 프로젝트 소유자입니다. 이 필드를 편집하고 다른 활성 사용자를 프로젝트 소유자로 표시할 수 있습니다.

* **프로젝트 스폰서**

  프로젝트 소유자 이외의 사용자를 프로젝트의 스폰서로 추가하는 것이 좋습니다. 스폰서는 비즈니스 사례의 승인을 받습니다. 

* **Portfolio**: 프로젝트의 Portfolio을 지정하십시오. 이 드롭다운 메뉴에서 Portfolio을 선택하려면 먼저 해당 사용자를 만들어 **활성** 상태로 만들어야 합니다.

  포트폴리오에 대한 자세한 내용은 [Adobe Workfront의 Portfolio 개요](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)를 참조하십시오.

  Portfolio 만들기에 대한 자세한 내용은 [포트폴리오 만들기](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)를 참조하십시오.

* **계획된 이익**: 이 프로젝트가 완료될 때 조직에 대해 계획된 금전적 이익을 예측합니다. 어떤 통화량이든 될 수 있으며 양의 값이어야 합니다. 예를 들어 $10,000입니다.
* **상태**: 기본적으로 프로젝트 요청의 상태는 **아이디어**(으)로 설정됩니다.

  상태를 Idea 또는 Planning 이외의 다른 항목으로 변경하면 비즈니스 사례 요약 영역에서 **제출** 단추가 사라지고 승인을 위해 비즈니스 사례를 더 이상 제출할 수 없습니다. 

* **고정 시작 날짜**: 프로젝트를 시작할 날짜를 지정합니다.
* **고정 종료 날짜**: 프로젝트를 종료할 날짜를 지정합니다.

  >[!NOTE]
  >
  >비즈니스 사례의 고정 시작 및 종료 일자는 프로젝트의 계획된 시작 및 완료 일자에 영향을 주지 않습니다. 이는 프로젝트가 이상적으로 개발될 시기에 대해 프로젝트 작성자가 요청한 날짜를 나타냅니다. 대신, 프로젝트의 계획된 시작 및 계획된 완료 일자에 프로젝트의 작업을 기반으로 하는 프로젝트의 계획된 타임라인이 표시됩니다.

## 목표

목표는 프로젝트의 목표를 정의합니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되어 있지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다. 이 필드에는 우선 순위 순으로 목표가 표시됩니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>프로젝트의 개별 비즈니스 사례에 연결되지 않은 조직의 전략적 목표를 생성할 수 있습니다. 전략적 목표를 만들려면 Adobe Workfront 목표에 액세스할 수 있어야 합니다. 그런 다음 비즈니스 사례 이외의 프로젝트와 연결할 수 있습니다. Workfront 목표를 사용하여 목표를 만드는 방법에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../../workfront-goals/goal-management/wf-goals-overview.md)를 참조하십시오.

목표를 정의하는 것은 프로젝트가 Portfolio 최적화 도구에서 점수를 받는 데 선택 사항입니다. 이 섹션은 비즈니스 사례에서 유일한 선택적 섹션입니다. 비즈니스 사례의 다른 모든 섹션은 프로젝트가 Portfolio 최적화 도구에서 채점되기 전에 완료되어야 합니다. 목표를 생성할 때 목표에 대한 우선순위 수준을 나타낼 수 있습니다.

목표에 대한 자세한 내용은  [비즈니스 사례 목표 만들기](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## 경비

경비는 프로젝트 수명 동안 발생할 수 있는 비인적 비용을 나타냅니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되어 있지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다. 

비즈니스 사례에 입력하는 모든 경비는 프로젝트의 경비 탭에 계획된 경비로 입력됩니다.

경비는 프로젝트의 다음 필드에 영향을 줍니다.

* 예산 비용
* 순 가치

예산 비용 및 순 가치에 대한 자세한 내용은 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md)를 참조하십시오.

경비에 대한 자세한 내용은  [프로젝트 경비 관리](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

Workfront 관리자는 사용자 정의 경비 유형을 설정할 수 있습니다.

사용자 지정 경비 유형 만들기에 대한 자세한 내용은 [사용자 지정 경비 유형 만들기](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md)를 참조하십시오. 

## 리소스 예산 책정

비즈니스 사례의 리소스 예산 책정 영역에서 다음 작업을 수행할 수 있습니다.

* 리소스 풀을 프로젝트와 연결합니다.
* 프로젝트 수준에서 리소스 예산을 책정합니다.

프로젝트의 자원에 대해 예산 책정된 시간이 비즈니스 사례의 자원 예산 책정 영역에 표시되어 프로젝트의 예산 책정된 인건비를 생성합니다. 비즈니스 사례의 이 영역은 기본적으로 활성화되어 있습니다.

비즈니스 사례에서 프로젝트의 리소스 예산 책정에 대한 자세한 내용은 [비즈니스 사례의 리소스 예산](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)을 참조하십시오.

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

비즈니스 사례의 리소스 예산 책정 섹션을 볼 때는 다음 사항을 고려하십시오.

* 다음 도구를 사용하여 여기에서 리소스 정보의 예산을 책정할 수 있습니다.

   * 리소스 플래너

     자세한 내용은 [리소스 플래너를 사용한 비즈니스 사례의 리소스 예산](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md)을 참조하세요.

   * 회사에서 Adobe 시나리오 플래너에 대한 추가 라이선스를 구입한 경우 시나리오 플래너 .

     자세한 내용은 [시나리오 플래너를 사용하여 비즈니스 사례에서 리소스 예산](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)을 참조하세요.

     시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이선스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 플래너 개요](../../../scenario-planner/scenario-planner-overview.md)를 참조하십시오.

* 여기에 표시되는 정보는 시스템 레벨 리소스 플래너 또는 시나리오 플래너에도 표시됩니다. 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* 자원의 예산을 책정한 후, 역할이 시간당 비용 비율과 연관된 경우 프로젝트의 예산 인건비가 자원 예산 책정 영역에 표시됩니다. 예산 인건비는 프로젝트 통화로 표시됩니다.

  >[!IMPORTANT]
  >
  >예산 인건비는 프로젝트의 역할과 연관된 비용이며 사용자와 연관되지 않습니다. 사용자의 모든 예산 인건비 합계는 사용자와 연관된 직무 역할의 예산 인건비와 동일하거나 동일하지 않을 수 있습니다. 

  예산 인건비에 대한 자세한 내용은 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md)를 참조하십시오.

  작업 역할을 만들고 시간당 비용을 해당 역할과 연결하는 방법에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

## 위험

위험은 프로젝트가 정시 또는 예산으로 끝나지 않도록 하는 요소입니다. 이러한 요소를 정의하는 것은 Portfolio 관리자 또는 프로젝트 스폰서가 프로젝트 승인에 대해 교육적으로 결정하는 데 중요합니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되어 있지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다.

잠재적 비용을 발생해야 하는 경우에 정의하는 위험과 연결할 수 있습니다. 프로젝트의 위험 비용은 프로젝트의 순 가치에 영향을 미칩니다. 

프로젝트 순 가치에 대한 자세한 내용은 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md)를 참조하십시오.

위험 생성에 대한 자세한 내용은  [프로젝트에 대한 위험 만들기 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Workfront 관리자는 사용자 정의 위험 유형을 설정할 수 있습니다.

사용자 지정 위험 유형을 만들고 편집하는 방법에 대한 자세한 내용은 [위험 유형 편집 및 만들기](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md)를 참조하십시오.

## 스코어카드

스코어카드는 프로젝트의 정렬을 측정합니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되어 있지만 Workfront 관리자가 표시하지 않도록 선택할 수 있습니다.

프로젝트에 스코어카드를 적용하고 정렬 점수를 생성하는 방법에 대한 자세한 내용은 [프로젝트에 스코어카드 적용 및 정렬 점수 생성](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)을 참조하십시오.

스코어카드를 적용하려면 Workfront 관리자가 스코어카드를 만들어야 합니다. 스코어카드를 만들지 않으면 비즈니스 사례의 **스코어카드** 영역이 표시되지 않습니다.

스코어카드 만들기에 대한 자세한 내용은  [스코어카드를 만듭니다](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## 사용자 정의 양식

비즈니스 사례를 정의할 때 프로젝트에 사용자 지정 Forms을 첨부할 수 있습니다. 이 영역은 비즈니스 사례에서 기본적으로 활성화되지 않습니다. Workfront 관리자는 이를 활성화하여 비즈니스 사례에 표시해야 합니다.

비즈니스 사례 영역 활성화에 대한 자세한 내용은 [시스템 차원의 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

사용자 정의 양식을 적용하려면 Workfront 관리자가 먼저 사용자 정의 양식을 만들어야 합니다.

사용자 정의 양식 만들기에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

사용자 정의 양식을 사용하여 비즈니스 사례의 다른 필드에 표시되지 않는 추가 정보를 수집할 수 있습니다.

사용자 정의 양식을 적용하는 방법에 대한 자세한 내용은 [비즈니스 사례에 사용자 정의 양식 첨부](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md)를 참조하십시오.

## 비즈니스 사례 요약

* [비즈니스 사례 요약 개요](#overview-of-the-business-case-summary)
* [비즈니스 사례 내보내기](#export-the-business-case)

### 비즈니스 사례 요약 개요 {#overview-of-the-business-case-summary}

비즈니스 사례 의 오른쪽 위 모서리에 있는 비즈니스 사례 요약 패널에서 주요 프로젝트 재무 및 프로젝트가 스코어카드와 정렬되었는지 여부에 대한 요약을 볼 수 있습니다.

비즈니스 사례 요약을 편집할 수 없습니다. 재무 필드 및 스코어카드와 관련된 프로젝트의 상태를 간단하게 볼 수 있습니다. \
 

비즈니스 사례 요약에는 다음 필드가 표시됩니다.

* 프로젝트 순 가치
* 프로젝트 예산 비용
* 잠재적 위험 비용
* 계획된 이익
* 정렬 점수

이러한 필드에 대한 자세한 내용은 [비즈니스 사례 재무 필드 개요](../../../manage-work/projects/define-a-business-case/business-case-finances.md)를 참조하십시오.

### 비즈니스 사례 내보내기 {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

인쇄하거나 보다 압축된 형식으로 이메일에 첨부해야 하는 경우 비즈니스 사례를 PDF 파일로 내보낼 수 있습니다. 

자세한 내용은 [프로젝트의 비즈니스 사례 내보내기](../../../manage-work/projects/define-a-business-case/export-business-case.md)를 참조하십시오.

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
—&gt;
