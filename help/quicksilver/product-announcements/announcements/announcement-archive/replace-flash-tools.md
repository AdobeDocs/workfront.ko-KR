---
title: Adobe Workfront에서 Flash 기반 도구 교체
description: Adobe Workfront에서 Flash 기반 도구 교체
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '2702'
ht-degree: 0%

---

# Adobe Workfront에서 Flash 기반 도구 교체

Adobe Workfront Classic에서 모든 Flash 기반 도구를 제거했습니다.

현재 표준을 기반으로 하는 대체 도구를 이제 Workfront에서 사용할 수 있습니다. 이러한 변경 사항은 Adobe에서 발표한 Flash 제품에 대한 지원 종료와 일치합니다.

## 중요 날짜

다음 날짜는 Workfront에서 모든 Flash 기반 도구를 제거하는 프로세스에 중요합니다.

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **2020년 11월 19일**: 모든 Flash 기반 도구가 모든 Workfront 제품에서 제거되었습니다.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## 기존 Flash 기반 도구

다음 섹션에 나열된 도구는 Workfront 시스템에서 제거되고 새 솔루션으로 대체되었습니다.

교체 도구에 대한 자세한 내용은 [기존 Flash 기반 도구 및 그 대체 요소](#legacy-flash-based-tools-and-their-replacements) 이 문서에서.

### 리소스 관리

* 사람 영역의 레거시 리소스 계획 탭과 탭에 포함된 모든 도구(다음 포함).

   * 리소스 예산 관리자
   * 수용작업량 플래너
   * 리소스 추정치
   * 리소스 그리드\
     자세한 내용은 [Adobe Workfront의 리소스 계획](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* 프로젝트의 비즈니스 사례에서 레거시 리소스 견적 영역

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

  .

* 프로젝트의 스태핑 탭에 있는 자원 그리드 하위 탭
* 기존 스케줄링 영역 또는 팀 빌더를 제거하는 프로젝트의 스태핑 탭에 있는 스케줄링 하위 탭의 신규 스케줄링 영역 사용 옵션. 이 경우 이제 예약 타임라인이 기본적으로 표시됩니다.
* 사용자 프로필 아래의 할당 탭

### 보고서

다음 보고 기능 및 보고서가 제거되었습니다.

* 제거된 보고 기능:

   * 사용자 보고서의 리소스 그리드 옵션
   * 프로젝트 또는 작업 보고서의 레거시 간트 옵션\
     자세한 내용은 [간트 차트에서 정보 보기](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* 제거된 보고서:

   * 레거시 리소스 풀 보고서
   * 리소스 견적 보고서

  >[!NOTE]
  >
  >보고서 또는 API(레거시 리소스 풀, 레거시 예산 비용, 레거시 비용, 레거시 예산 시간, 레거시 예산 인건비 등)를 통해 액세스하는 모든 레거시 필드는 다양한 보고서에 표시되지만 새 정보로 채우지는 않습니다.

### 레거시 간트

* 프로젝트 및 작업 목록과 보고서 및 보고 옵션의 모든 레거시 간트 보기
* Portfolio 및 프로그램의 기존 간트 하위 탭
* 템플릿의 템플릿 작업 목록에 있는 레거시 간트 하위 탭, 템플릿 작업의 하위 작업 탭에 있는 레거시 간트 보기 및 템플릿 작업 보고서에 있는 레거시 간트 보기

### 증명

기존 증명 뷰어는 대부분의 고객을 위한 새로운 웹 증명 뷰어 및 데스크탑 증명 뷰어로 교체되었으며 2020년 11월에 모든 고객에 대해 제거되었습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

자세한 내용은 다음 리소스를 참조하십시오.

* [웹 증명 뷰어에서 증명 검토](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Desktop Proofing Viewer에서 증명 검토](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## 기존 Flash 기반 도구 및 그 대체 요소 {#legacy-flash-based-tools-and-their-replacements}

별도로 지정된 경우를 제외하고 모든 레거시 피쳐는 다음 표와 같이 새 피쳐로 대체됩니다.

>[!CAUTION]
>
>기존 Flash 기반 도구는 모든 환경에서 제거되었습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>레거시 도구</strong> </p> </th> 
   <th> <p><strong>새 도구</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>레거시 리소스 풀</strong> </p> <p>레거시 리소스 풀은 프로젝트 완료에 동시에 필요한 작업 역할의 그룹 또는 컬렉션입니다. 레거시 리소스 풀에는 다음과 같은 여러 가지 단점이 있었습니다.</p> 
    <ul> 
     <li> 사용자를 하나의 레거시 리소스 풀과 연결할 수 있지만 보고 용도로만 사용되었습니다. 레거시 리소스 풀은 추상 작업 역할 엔티티로 작동했으므로 사용자의 일정 예외 및 휴무를 고려하지 않았으므로 리소스 가용성에 대한 데이터가 부정확했습니다. </li> 
    </ul> 
    <ul> 
     <li>프로젝트당 하나의 레거시 리소스 풀만 지정할 수 있으므로 여러 레거시 리소스 풀이 서로 독립적으로 작동하며 리소스를 공유하지 않는 개별 그룹의 흐름만 지원합니다. 그 외의 모든 경우에는 시스템에 모든 리소스를 포함하는 하나의 레거시 리소스 풀을 유지하는 것이 좋았고, 이로 인해 대량의 프로젝트 및 데이터에 성능 문제가 발생했습니다.</li> 
    </ul> </td> 
   <td> <p><strong>리소스 풀</strong> </p> <p>새 리소스 풀은 프로젝트 완료에 동시에 필요한 사용자 컬렉션입니다. Workfront 역시 전문 이용자에게 업무를 따로 할당해 줘야 하는 경우가 있다는 점을 실감하고 있다. 따라서 이제 작업 역할 대신 사용자 예산을 책정할 수 있습니다. </p> 레거시 리소스 풀과 비교하여 리소스 풀의 장점은 다음과 같습니다. 
    <ul>
     <li>리소스 풀은 사용자를 기반으로 하므로 해당 사용자의 휴무와 일정 예외는 사용자 및 역할 가용성 계산에 이미 고려됩니다. 이를 통해 정확한 최신 데이터를 얻을 수 있으므로 올바른 예산 결정을 가능하게 하고 프로젝트가 진행 중일 때 변경 가능성을 최소화할 수 있습니다.</li>
     <li>이제 리소스의 가용성과 데이터의 정확성에 대해 보다 세밀하게 제어할 수 있으므로 Workfront에서 여러 리소스 풀을 프로젝트와 연결할 수 있습니다. 한 사용자가 여러 프로젝트에서 동시에 사용할 수 있는 여러 기술을 보유한 경우 두 명 이상의 리소스 풀에 속할 수도 있습니다. </li>
    </ul><p>이러한 데이터 제어를 통해 사용 가능한 예산을 분배하기 위해 모든 리소스를 포함하는 리소스 풀을 더 이상 보유할 필요가 없습니다. 사실, 우리는 이것을 추천하지 않습니다. 대신, 리소스 풀을 다양화하고 관련 리소스 풀을 프로젝트와 연결하는 것이 좋습니다.</p><p> 리소스 풀에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 리소스 풀 개요 </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 예산 관리자</strong> </p> <p>리소스 예산 관리자를 사용하여 여러 리소스 풀에서 작업 역할 리소스의 가용성을 지정할 수 있습니다. 그러나 레거시 리소스 풀의 단점으로 인해 이 기능은 거의 사용되지 않았습니다. 이를 사용할 때는 사용자가 작업 역할의 가용성을 수동으로 입력하여 예산을 보다 정확하게 책정하도록 했습니다. 일정 예외 및 사용자의 휴무 등은 고려하지 않았다.</p> </td> 
   <td> <p>리소스 풀의 사용자를 기준으로 가용성을 자동으로 계산하므로 리소스 예산 관리자는 더 이상 필요하지 않습니다. 가용성 계산을 위한 모든 수동 작업과 함께 도구가 제거되었습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 추정치</strong> </p> <p>각 레거시 리소스 풀 아래의 리소스 예상 탭은 하나의 레거시 리소스 풀 컨텍스트에서만 리소스 예산 관리자와 동일한 용도로 사용됩니다. 이 툴은 리소스 예산 관리자 및 레거시 리소스 풀과 동일한 제한 사항을 제시했습니다. 부정확한 데이터 및 가용성의 수동 입력입니다. </p> </td> 
   <td> <p>사용자 가용성이 자동으로 계산됨에 따라 리소스 예측이 더 이상 사용되지 않으며 제거되었습니다.</p> <p>프로젝트의 비즈니스 사례에서 레거시 리소스 풀 및 레거시 리소스 추정치를 사용하는 경우 도구가 제거됩니다. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>수용작업량 플래너</strong> </p> <p>용량 플래너는 리소스 예산을 책정하고 리소스의 가용성에 따라 레거시 리소스 풀 내에서 프로젝트의 우선 순위를 지정하는 Workfront 도구입니다. 리소스 추정치 및 용량 플래너에 대한 정보를 제공하는 리소스 예산 관리자의 데이터가 불완전할 경우, 프로젝트 우선 순위를 사용자의 가용성과 비교하여 두 번 확인해야 했습니다.</p> <p>시스템의 모든 작업 역할을 포함하는 단일 레거시 리소스 풀을 사용하는 것이 가장 일반적인 시나리오였으며, 이로 인해 용량 플래너가 많은 수의 프로젝트를 로드하려고 할 때 성능 문제가 발생했습니다.</p> </td> 
   <td> <p><strong>리소스 플래너의 프로젝트 보기</strong> </p> <p>리소스 플래너의 프로젝트 기반 보기에서 레거시 용량 플래너에서 리소스 예산을 책정하고 프로젝트 우선 순위를 정했던 방식과 유사하게 지정할 수 있습니다. 기존 도구와 달리 이제 더 많은 데이터가 지원되며, 사용자의 휴무 및 예약 예외를 모두 고려하여 사용 가능한 정보를 더 정확하게 지정할 수 있습니다.</p> <p>사용 가능, 계획 및 예산 정보가 한눈에 표시되므로 리소스 관리자는 작업을 수행할 수 있는 충분한 인력이 있는지 여부와 프로젝트 계획이 초기 예산 추정치를 초과하는지 여부를 모두 확인할 수 있습니다.</p> <p> 리소스 플래너에서 프로젝트 보기 사용에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a></p> <p><strong>시나리오 플래너</strong> </p> <p>장기 용량 계획, 가정 시나리오 모델링 및 우선 순위 지정의 경우 Workfront 시나리오 플래너 도 도입했습니다. </p> <p>시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이선스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">시나리오 플래너 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>레거시 리소스 추정치(비즈니스 사례)</strong> </p> <p>비즈니스 사례의 레거시 리소스 견적 영역을 사용하여 프로젝트 계획 및 리소스 요청의 일부로 특정 노동 시간 및 비용을 예산할 수 있습니다. 이 보기는 리소스의 가용성에 대한 가시성을 제공하지 않았으므로 리소스에 대한 대략적인 요청과 거부된 프로젝트 작업의 가능성이 증가했습니다.</p> </td> 
   <td> <p><strong>리소스 예산 책정(비즈니스 사례)</strong> </p> <p>비즈니스 사례 아래의 리소스 예산 편성 섹션은 비즈니스 사례에 리소스 플래너 기능을 가져와서 사용자 및 역할 가용성에 대한 가시성을 제공하며 사용자 수준에서 예산을 편성할 수 있습니다. </p> <p> 비즈니스 사례의 리소스 예산 편성 영역에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">비즈니스 사례 영역 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 견적 보고서</strong> </p> <p>리소스 관리를 위한 레거시 도구를 사용하는 경우 비즈니스 사례에서 예산 및 계획된 시간을 보고할 수 있습니다. 이를 통해 특정 시간대의 각 작업 역할에 대한 총 예산 및 계획된 작업을 표시하는 매트릭스 보고서를 작성할 수 있습니다. 이 보고서는 편집할 수 없으며 보고서 결과를 기반으로 리소스 예산을 변경할 수 없습니다. </p> </td> 
   <td> <p><strong>활용성 보고서</strong> </p> <p>기본 제공 활용성 보고서에는 계획, 예산 및 실제 시간, 비용 및 수익이 나란히 표시됩니다. </p> <p>활용률 보고서 사용에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">자원 가동률 정보 보기 </a>. </p> 
    <div> 
     <p><strong>보고 가능한 예산 시간</strong> </p> 
     <p>예산 시간에 대한 보고서를 생성하여 보고서 양식의 리소스 플래너에서 예산 책정된 시간을 검토합니다. </p> 
     <p>예산 시간에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe Workfront 용어 목록</a>.</p> 
     <p>보고서 만들기에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> 
    </div> <p><strong>리소스 플래너의 역할 보기</strong> </p> <p>레거시 리소스 관리 도구의 비즈니스 사례에서 예산 및 계획된 시간을 이제 리소스 플래너의 역할 기반 보기인 새로운 기본 보기에서 사용할 수 있습니다. 이 보기는 사용 가능 시간, 계획 시간 및 예산 시간 정보를 한눈에 제공하며, 이를 통해 동일한 위치에서 예산 책정을 제어하고 변경할 수 있습니다. 이를 통해 고위직 역할 계획 시 더 나은 의사 결정을 할 수 있다. </p> <p> 리소스 플래너의 역할 보기에서 리소스 예산 책정에 대한 자세한 내용은 다음을 참조하십시오. <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">프로젝트 및 역할 보기를 사용하여 리소스 예산 책정 </a> 의 섹션 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 그리드</strong> </p> <p>리소스 그리드는 프로젝트가 완료로 진행될 때 특정 사용자의 할당을 볼 수 있도록 해줍니다. </p> <p>예를 들어 프로젝트 팀의 누군가가 작업을 일찍 완료하고 누군가가 뒤처진 경우를 비롯하여 특정 기간에 초과 할당되었는지 또는 과소 할당되었는지 등을 쉽게 확인할 수 있습니다. </p> <p>안타깝게도, 당신은 같은 견해로 그 정보에 대해 조치를 취할 수 없었습니다. 초과 할당 문제를 해결하려면 프로젝트로 이동하여 작업의 결과를 표시하지 않고 정보를 수동으로 조정해야 했습니다.</p> </td> 
   <td> <p>리소스 그리드 가 두 개의 새 도구로 대체되었습니다. 자원 계획의 단계에 따라 다음 도구를 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>분석 단계의 경우:</strong> </p> 
      <ul> 
       <li> <p><strong>업무 균형자</strong>: 업무 균형자 를 사용하여 사용자의 업무를 보다 세분화된 수준에서 볼 수 있습니다. 업무 균형자 를 사용할 때 어느 사용자가 업무 균형자에서 제 시간에 작업을 완료할 수 있는지 확인할 수 있습니다. 여기에는 휴무와 일정 예외 세부 사항이 포함됩니다. </p> <p>업무 균형자에 대한 자세한 내용은 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">업무 균형자 개요</a>.</p> </li> 
       <li> <p><strong>리소스 플래너의 사용자 보기</strong><strong>:</strong> 사용자가 할당되는 프로젝트를 더 높은 수준에서 이해하려고 할 때 리소스 플래너의 사용자 보기를 사용합니다. 이를 통해 작업 중인 사용자와 특정 시간대에 초과 및 과소 할당을 확인할 수 있습니다. 리소스 플래너는 또한 전체적으로 사용자의 전체 할당에 대한 시각화를 제공하고, 기록된 실제 시간에 대한 가시성을 제공하므로 수행된 작업의 진행 상황을 분석하는 데 도움이 됩니다. </p> <p>리소스 플래너에서 사용자 보기 사용에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">사용자 보기를 사용하여 가용, 계획 및 실제 근로시간 또는 FTE 보기 </a> 의 섹션 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a></p> </li> 
      </ul> </li> 
     <li><strong>전략 단계:</strong> 
      <ul> 
       <li><strong>업무 균형자</strong> 업무 균형자 를 사용하여 다음과 같은 작업을 수행할 수 있습니다. 
        <ul>
         <li>사용자에게 작업을 할당합니다.</li>
         <li>작업 항목에 대한 사용자의 할당을 관리합니다. </li>
         <li>사용자 영역에 대한 가시성이 없을 수 있는 다른 사용자와 업무 균형자 를 공유합니다. 공유 가능한 링크 기능을 사용하여 업무 균형자에 대한 링크를 공유하고 사용자 정의 대시보드에 포함합니다. 사용자 보기 액세스 권한이 있는 모든 사용자는 이러한 대시보드를 공유할 때 볼 수 있습니다.</li>
        </ul><p>업무 균형자 는 사람 영역에서 사용할 수 있습니다. </p><p>업무 균형자에 대한 자세한 내용은 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">업무 균형자 개요</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>레거시 간트 차트, 작업 목록</strong> </p> <p> 작업 목록의 레거시 간트 차트는 프로젝트의 타임라인을 시각적으로 보고 데이터베이스에 변경 사항을 커밋하지 않고 가정 시나리오 계획을 수행할 수 있는 기능을 제공합니다. 레거시 간트 차트는 보안 위험을 나타내는 Flash 기술을 기반으로 했습니다. </p> </td> 
   <td> <p><strong>간트 차트,</strong> <strong>작업 목록</strong></p> <p> 새 HTML 기반 간트 차트는 기존 간트와 동일한 용도로 사용됩니다. 사용자는 작업 목록 도구 모음에서 수동 저장 옵션을 변경하여 데이터베이스에 변경 사항을 적용하지 않고 프로젝트의 타임라인을 시각화하고 가정 시나리오 계획을 수행할 수 있습니다. </p> <p>변경 사항이 발생할 때 자동으로 저장할 때 사용할 수 있는 자동 저장 옵션을 사용할 때 새로운 간트 차트는 대화형입니다. </p> <p>새로운 작업 목록 간트 차트 는 최신 기술을 기반으로 구축되었으며 신뢰할 수 있습니다. 이 새로운 간트 차트는 작업 목록에 바로 표시되며, 탭을 전환하거나 보기를 변경하지 않고도 작업 목록에서 작업할 때 쉽게 액세스할 수 있습니다. </p> <p>새 간트 차트는 이전 차트와 동일한 기능을 제공하지만 기존 간트와 비교하여 기능에는 몇 가지 차이점이 있습니다. </p> <p> 템플릿의 템플릿 작업 목록에 있는 레거시 간트 하위 탭, 템플릿 작업의 하위 작업 탭에 있는 레거시 간트 보기 및 템플릿 작업 보고서에 있는 레거시 간트 차트가 HTML 기반 간트 차트로 대체되었습니다. </p> <p>단순한 보기와 빠른 편집 위주로 이전 간트 차트를 사용하고 실제 차트를 사용하지 않는 경우, 새로운 타임라인 계획 수립 옵션을 사용하면 주요 계획 수립 필드를 빠르게 변경할 수 있습니다. 작업 목록 도구 모음에서 자동 저장 대신 타임라인 계획 수립을 선택할 수 있습니다.</p> <p>타임라인 계획 수립 옵션을 사용하여 작업 목록을 저장하는 방법에 대한 자세한 내용은 문서의 "타임라인 계획 수립 옵션을 선택할 때 수동으로 작업 목록에 변경 사항 저장" 섹션을 참조하십시오 <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">목록에서 작업 편집</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>프로젝트 목록에 대한 레거시 간트 차트</strong> </p> <p>프로젝트 목록의 레거시 간트 차트는 프로젝트와 해당 작업을 하나의 보기에서 볼 수 있는 기능을 사용자에게 제공합니다. 프로젝트 목록의 컨텍스트를 종료하지 않으면 프로젝트의 작업에 대한 세부 정보와 프로젝트 간의 종속성을 볼 수 있습니다. 프로젝트 목록의 레거시 간트 차트는 보안 위험을 나타내는 Flash 기술을 기반으로 했습니다. </p> </td> 
   <td> <p><strong>간트 차트, 프로젝트 목록</strong> </p> <p>HTML 기반 간트 차트는 기존 간트 차트와 동일한 용도로 사용됩니다. 사용자는 프로젝트와 작업을 하나의 보기에서 보고 프로젝트뿐만 아니라 작업 간의 종속성을 시각적으로 식별할 수 있습니다. 프로젝트 목록 간트 차트는 프로젝트 목록에 바로 있습니다. 새로운 간트 차트는 최신 인터페이스를 갖추고 있으며 최신 기술을 기반으로 구축되었습니다.</p> <p>프로젝트 목록 간트 차트에 대한 자세한 내용은 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">간트 차트에서 정보 보기 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>보고서, 캘린더 및 문서의 공유 대화 상자</strong> </p> <p>보고서, 캘린더 및 문서를 공유할 때 사용된 대화 상자는 Flash 기술을 기반으로 했습니다.</p> </td> 
   <td> <p>Workfront에서 보고서, 캘린더 및 문서를 공유할 때의 환경이 변경되지 않았습니다. 그러나 경험은 더 이상 Flash에 의존하지 않습니다.</p> <p>이러한 항목 공유에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">오브젝트에 대한 공유 권한 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>기존 증명 뷰어</strong> </p> <p>기존 증명 뷰어는 정적, 비디오 및 대화형 증명에 대한 증명 기능을 제공하는 웹 기반 증명 뷰어였습니다.</p> </td> 
   <td> <p><strong>웹 증명 뷰어 및 데스크탑 증명 뷰어</strong> </p> <p>웹 증명 뷰어는 정적 증명 및 비디오 증명에 대한 증명 기능을 제공합니다.</p> <p>Desktop Proofing Viewer는 정적 증명 및 비디오 증명에 대한 모든 지원을 제공할 뿐만 아니라 대화형 증명에 대한 증명 기능을 제공합니다.</p> <p>SWF 파일 형식은 더 이상 주요 공급자에서 지원되지 않으며 증명을 위해 HTML 5 배너로 대체되었습니다. </p> <p>사용 가능한 증명 뷰어 간의 차이에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">웹 증명 뷰어와 데스크탑 증명 뷰어의 차이점 개요</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
