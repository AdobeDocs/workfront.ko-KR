---
title: Adobe Workfront에서 Flash 기반 도구 교체
description: Adobe Workfront에서 Flash 기반 도구 교체
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '2705'
ht-degree: 0%

---

# Adobe Workfront에서 Flash 기반 도구 교체

Adobe Workfront Classic에서 모든 Flash 기반 도구를 제거했습니다.

현재 표준을 기반으로 하는 교체 도구는 Workfront에서 사용할 수 있습니다. 이러한 변경 사항은 Adobe이 발표한 Flash 제품 지원 종료와 일치합니다.

## 중요 날짜

다음 날짜는 Workfront에 있는 모든 Flash 기반 도구의 제거 프로세스에 중요합니다.

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **2020년 11월 19일**: 모든 Flash 기반 도구는 모든 Workfront 제품에서 제거되었습니다.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## 기존 Flash 기반 도구

다음 섹션에 나열된 도구는 Workfront 시스템에서 제거되고 새 솔루션으로 대체되었습니다.

교체 도구에 대한 자세한 내용은 [기존 Flash 기반 도구 및 그 교체](#legacy-flash-based-tools-and-their-replacements) 참조하십시오.

### 리소스 관리

* 사용자 영역의 기존 리소스 계획 탭과 탭에 포함된 모든 도구에는 다음이 포함됩니다.

   * 리소스 예산 관리자
   * 수용작업량 플래너
   * 리소스 추정치
   * 리소스 그리드\
      자세한 내용은 [Adobe Workfront의 리소스 계획](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* 프로젝트의 업무 사례에서 레거시 자원 예상 영역

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
* 이전 스케줄링 영역 또는 Team Builder를 제거하는 프로젝트의 스태핑 탭의 스케줄링 하위 탭에 있는 새 스케줄링 영역 사용 옵션 이 경우 기본적으로 예약 타임라인이 표시됩니다.
* 사용자 프로필 아래의 할당 탭

### 보고서

다음 보고 기능 및 보고서가 제거되었습니다.

* 제거된 보고 기능:

   * 사용자 보고서의 리소스 그리드 옵션
   * 프로젝트 또는 작업 보고서의 기존 Gantt 옵션\
      자세한 내용은 [간트 차트에서 정보 보기](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* 제거된 보고서:

   * 레거시 리소스 풀 보고서
   * 리소스 예상 보고서

   >[!NOTE]
   >
   >보고서나 API(기존 자원 풀, 기존 예산책정된 비용, 기존 비용, 이전 예산책정된 시간, 레거시 예산책정된 노무비 등)를 통해 액세스되는 모든 레거시 필드는 다양한 보고서에 표시되지만 새 정보로 채우지는 않습니다.

### 레거시 간트

* 프로젝트 및 작업 목록의 모든 기존 Gantt 보기, 보고서 및 보고 옵션
* Portfolio 및 프로그램의 기존 Gantt 하위 탭
* 템플리트의 템플리트 태스크 목록, 템플리트 태스크의 하위 태스크 탭, 템플리트 태스크 보고서의 기존 간트 뷰 및 템플리트 태스크 보고서의 기존 간트 하위 탭

### 증명

레거시 언어 교정 뷰어가 대부분의 고객을 위한 새 Web Proofing Viewer 및 Desktop Proofing Viewer로 대체되었으며 2020년 11월에 모든 고객을 위해 제거되었습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

자세한 내용은 다음 리소스를 참조하십시오.

* [Web Proofing Viewer에서 증명 검토](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [데스크탑 교정 뷰어에서 증명 검토](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

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

## 기존 Flash 기반 도구 및 그 교체 {#legacy-flash-based-tools-and-their-replacements}

별도로 지정하지 않는 경우를 제외하고 다음 표에 표시된 대로 모든 이전 피쳐가 새 피쳐로 대체되었습니다.

>[!CAUTION]
>
>기존 Flash 기반 도구가 모든 환경에서 제거되었습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>기존 도구</strong> </p> </th> 
   <th> <p><strong>새 도구</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>레거시 리소스 풀</strong> </p> <p>레거시 리소스 풀은 프로젝트를 완료하기 위해 동시에 필요한 작업 역할의 그룹이나 컬렉션입니다. 레거시 리소스 풀에는 다음과 같은 많은 단점들이 있습니다.</p> 
    <ul> 
     <li> 사용자를 하나의 레거시 리소스 풀과 연결할 수 있지만 보고용으로만 사용되었습니다. 레거시 리소스 풀이 추상 작업 역할 엔티티로 작동했으므로 사용자의 일정 예외 및 휴가가 고려되지 않아 리소스 가용성에 대한 데이터가 부정확합니다. </li> 
    </ul> 
    <ul> 
     <li>프로젝트당 하나의 레거시 리소스 풀만 지정할 수 있으므로, 서로 독립적으로 작동하며 리소스를 공유하지 않는 개별 그룹의 흐름만 지원하는 여러 레거시 리소스 풀이 있습니다. 다른 모든 경우에는 시스템에 모든 리소스를 포함하는 하나의 레거시 리소스 풀을 유지하는 것이 좋습니다. 이로 인해 많은 양의 프로젝트 및 데이터에 성능 문제가 발생했습니다.</li> 
    </ul> </td> 
   <td> <p><strong>리소스 풀</strong> </p> <p>새 리소스 풀은 프로젝트 완료와 동시에 필요한 사용자 모음입니다. Workfront은 또한 전문 사용자가 별도로 작업을 할당받아야 하는 경우가 있다는 것을 알고 있습니다. 따라서 이제 작업 역할 대신 사용자에게 예산을 할당할 수 있습니다. </p> 레거시 리소스 풀에 비해 리소스 풀의 장점은 다음과 같습니다. 
    <ul>
     <li>리소스 풀은 사용자를 기반으로 하므로 사용자 및 역할 가용성 계산을 위해 시간 초과 및 예약 예외가 이미 고려됩니다. 이를 통해 정확한 최신 데이터를 얻을 수 있으므로 예산 결정을 올바르게 내릴 수 있고 프로젝트가 진행 중일 때 변경 가능성을 최소화할 수 있습니다.</li>
     <li>이제 리소스 가용성과 데이터 정확성을 더욱 강력하게 제어할 수 있으므로 Workfront에서 여러 리소스 풀을 프로젝트와 연결할 수 있습니다. 여러 프로젝트에서 동시에 사용할 수 있는 여러 기술이 있는 경우 한 사용자가 둘 이상의 리소스 풀에 속할 수도 있습니다. </li>
    </ul><p>이러한 데이터 제어를 통해 사용 가능한 예산을 분배하기 위한 모든 리소스를 포함하는 자원 풀이 더 이상 필요하지 않습니다. 사실 이 방법은 권장되지 않습니다. 대신 리소스 풀을 다양화하고 관련 리소스 풀을 프로젝트와 연결하기만 하면 됩니다.</p><p> 리소스 풀에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 리소스 풀 개요 </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 예산 관리자</strong> </p> <p>리소스 예산 관리자를 사용하여 여러 리소스 풀에서 작업 역할 리소스의 가용성을 지정할 수 있습니다. 그러나 레거시 리소스 풀의 단점으로 인해 이 기능은 거의 사용되지 않았습니다. 이 기능을 사용하면 사용자가 작업 역할의 가용성을 수동으로 입력하여 예산을 더 정확하게 작성할 수 있습니다. 예약 예외 및 사용자의 휴가가 고려되지 않았습니다.</p> </td> 
   <td> <p>자원 풀의 사용자를 기반으로 가용성을 자동으로 계산하면 자원 예산 관리자가 더 이상 필요하지 않습니다. 가용성 계산을 위한 모든 수동 작업과 함께 도구가 제거되었습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 추정치</strong> </p> <p>각 레거시 리소스 풀 아래의 리소스 예상 탭은 하나의 레거시 리소스 풀 컨텍스트에서만 리소스 예산 관리자와 동일한 목적을 수행했습니다. 이 도구는 리소스 예산 관리자 및 레거시 리소스 풀과 동일한 제한 사항을 제공합니다. 부정확한 데이터 및 가용성의 수동 입력 </p> </td> 
   <td> <p>사용자 가용성을 자동으로 계산하여 리소스 추정이 더 이상 사용되지 않으며 제거되었습니다.</p> <p>이 툴은 프로젝트의 비즈니스 사례에서 레거시 리소스 풀 및 레거시 리소스 추정치에서 제거됩니다. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>수용작업량 플래너</strong> </p> <p>Capacity Planner는 자원의 가용성에 따라 Legacy Resource Pool 내의 프로젝트 우선 순위를 지정하고 자원을 예산책정하는 Workfront 도구입니다. 자원 예상 및 능력 계획자에 대한 정보를 제공하는 자원 예산 관리자의 데이터가 불완전할 경우, 프로젝트 우선 순위를 사용자 가용성에 대해 두 번 확인해야 합니다.</p> <p>시스템에서 모든 작업 역할을 포함하는 단일 레거시 리소스 풀을 사용하는 것은 가장 일반적인 시나리오였으며, 이로 인해 많은 수의 프로젝트를 로드하려고 하는 용량 계획자가 성능 문제를 일으켰습니다.</p> </td> 
   <td> <p><strong>리소스 플래너의 프로젝트 뷰</strong> </p> <p>자원 계획자의 프로젝트 기반 뷰에서 자원을 예산을 책정하고 레거시 능력 계획자에서 그렇게 하기 위해 사용한 것과 유사한 방법으로 프로젝트에 우선순위를 지정할 수 있습니다. 기존 도구와 달리 이제 더 많은 데이터가 지원되며, 사용 가능한 정보는 사용자의 휴식과 예약 예외 모두를 고려하여 더 정확하게 제공됩니다.</p> <p>사용 가능, 계획 및 예산책정된 정보는 한 눈에 표시되므로 자원 관리자는 작업을 수행할 충분한 인력이 있는지 여부와 프로젝트 계획이 초기 예산 추정치를 초과하는지 여부를 모두 확인할 수 있습니다.</p> <p> 리소스 계획자에서 프로젝트 뷰를 사용하는 방법에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a></p> <p><strong>시나리오 플래너</strong> </p> <p>장기 용량 계획, what-if 시나리오 모델링 및 우선 순위를 위해 Workfront 시나리오 플래너 도 도입했습니다. </p> <p>시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">시나리오 계획자 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>기존 리소스 예상(비즈니스 사례)</strong> </p> <p>업무 사례의 이전 자원 예상 영역을 사용하여 프로젝트 계획 및 자원 요청의 일부로 일정 양의 노무 시간과 비용을 예산할 수 있습니다. 이 보기는 리소스의 가용성에 대한 가시성을 제공하지 않았으므로, 리소스에 대한 대략적인 요청과 거부된 프로젝트 작업에 대한 가능성이 높아졌습니다.</p> </td> 
   <td> <p><strong>자원 예산 책정(업무 사례)</strong> </p> <p>업무 사례 아래의 자원 예산 섹션은 Resource Planner 기능을 업무 사례에 가져와서 사용자 및 역할 가용성을 확인하고 사용자 레벨에서 예산을 편성할 수 있습니다. </p> <p> Business Case의 Resource Budgeting 영역에 대한 자세한 내용은 <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">비즈니스 사례 영역 개요</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 예상 보고서</strong> </p> <p>자원 관리를 위한 레거시 도구를 사용할 때 업무 사례에서 예산책정된 시간과 계획된 시간을 보고할 수 있습니다. 이를 통해 특정 기간의 각 작업 역할에 대한 총 예산책정된 작업 및 계획된 작업 내용을 보여 주는 매트릭스 보고서를 작성할 수 있습니다. 이 보고서를 편집할 수 없으므로 보고서 결과를 기반으로 리소스의 예산을 변경할 수 없습니다. </p> </td> 
   <td> <p><strong>활용률 보고서</strong> </p> <p>기본 가동률 보고서는 계획, 예산책정됨 및 실제 시간, 원가 및 수익을 나란히 표시합니다. </p> <p>활용률 보고서 사용에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">자원 사용률 정보 보기 </a>. </p> 
    <div> 
     <p><strong>보고 가능 예산책정 시간</strong> </p> 
     <p>Resource Planner에서 설정한 시간을 보고서 형식으로 검토하기 위해 예산책정된 시간에 대한 보고서를 생성합니다. </p> 
     <p>예산책정된 시간에 대한 자세한 내용은 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe Workfront 용어 설명</a>.</p> 
     <p>보고서 만들기에 대한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">사용자 지정 보고서 만들기</a>.</p> 
    </div> <p><strong>리소스 계획자의 역할 보기</strong> </p> <p>레거시 리소스 관리 도구의 업무 사례에서 예산책정된 시간 및 계획된 시간은 이제 자원 계획자의 역할 기반 보기인 새로운 기본 뷰에서 사용할 수 있습니다. 이 뷰에서는 사용 가능, 계획 및 예산책정 시간 정보를 한 눈에 제공하며, 동일한 위치에서 예산 편성을 제어하고 변경할 수 있습니다. 따라서 높은 수준의 작업 역할 계획 시 더 나은 의사 결정을 내릴 수 있습니다. </p> <p> 리소스 계획자의 역할 뷰의 예산 책정 자원에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">프로젝트 및 역할 보기를 사용하여 예산 자원 </a> 섹션 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>리소스 그리드</strong> </p> <p>리소스 그리드를 통해 프로젝트가 완료될 때 특정 사용자의 할당을 파악할 수 있습니다. </p> <p>예를 들어 프로젝트 팀의 누군가가 자신의 작업을 일찍 수행한 시점과 작업이 지연된 시점과 특정 기간 동안 초과 할당 또는 덜 할당된 상태인지를 쉽게 확인할 수 있습니다. </p> <p>불행하게도, 당신은 같은 시각으로 그 정보에 대해 행동할 수 없었습니다. 초과 할당 문제를 해결하려면 프로젝트로 이동하여 작업 결과에 대한 가시성 없이 수동으로 정보를 조정해야 합니다.</p> </td> 
   <td> <p>리소스 그리드가 두 개의 새 도구로 대체되었습니다. 자신이 찾는 리소스 계획의 단계에 따라 다음 도구를 사용할 수 있습니다.</p> 
    <ul> 
     <li> <p><strong>분석 단계의 경우:</strong> </p> 
      <ul> 
       <li> <p><strong>작업 로드 밸런서</strong>: 작업 로드 밸런서를 사용하여 사용자의 작업 로드를 보다 세부적인 수준에서 봅니다. 작업 로드 밸런서를 사용할 때 작업 로드에서 사용 가능한 사용자를 확인하여 작업 시간을 완료할 수 있습니다. 여기에는 시간 초과 및 예약 예외 세부 사항이 포함됩니다. </p> <p>작업 로드 밸런서에 대한 자세한 내용은 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">작업 로드 밸런서 개요</a>.</p> </li> 
       <li> <p><strong>리소스 계획자의 사용자 보기</strong><strong>:</strong> 사용자가 할당된 프로젝트를 상위 레벨에서 이해하려고 할 때 리소스 계획자의 사용자 뷰를 사용합니다. 이를 통해 사용자가 작업 중인 내용과 특정 기간 동안의 초과 및 저할당을 확인할 수 있습니다. 또한 Resource Planner는 전체 사용자 할당 시각화와 실제 시간 기록됨 가시성을 제공하며, 이는 작업 진행 상황을 분석하는 데 유용합니다. </p> <p>리소스 계획자에서 사용자 뷰를 사용하는 방법에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">사용 가능, 계획 및 실제 시간 또는 FTE를 보려면 사용자 뷰를 사용하십시오 </a> 섹션 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">리소스 플래너 개요</a></p> </li> 
      </ul> </li> 
     <li><strong>전술 단계:</strong> 
      <ul> 
       <li><strong>작업 로드 밸런서</strong> 작업 로드 밸런서를 사용하여 다음을 수행할 수 있습니다. 
        <ul>
         <li>사용자에게 작업을 할당합니다.</li>
         <li>작업 항목에 대한 사용자의 할당을 관리합니다. </li>
         <li>작업 로드 밸런서를 사용자 영역에 대한 가시성이 없는 다른 사용자와 공유합니다. 공유 가능한 링크 기능을 사용하여 작업 로드 밸런서에 대한 링크를 공유하고 사용자 지정 대시보드에 포함합니다. 사용자 보기에 액세스할 수 있는 모든 사용자는 대시보드를 공유할 때 이러한 대시보드를 볼 수 있습니다.</li>
        </ul><p>작업 로드 밸런서는 사용자 영역에서 사용할 수 있습니다. </p><p>작업 로드 밸런서에 대한 자세한 내용은 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">작업 로드 밸런서 개요</a>.</p></li> 
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
   <td> <p><strong>기존 Gantt 차트, 작업 목록</strong> </p> <p> 작업 목록의 기존 Gantt 차트는 사용자가 데이터베이스의 변경 사항을 커밋하지 않고 프로젝트의 타임라인을 시각적으로 보고 가능한 시나리오 계획을 수행할 수 있는 기능을 제공합니다. 기존 Gantt 차트는 보안 위험을 보여주는 Flash 기술을 기반으로 했습니다. </p> </td> 
   <td> <p><strong>간트 차트,</strong> <strong>작업 목록</strong></p> <p> 새 HTML 기반 Gantt 차트가 기존 Gantt 차트와 동일한 목적을 제공하고 있습니다. 사용자는 작업 목록 도구 모음에서 수동 저장 옵션으로 변경하여 데이터베이스 변경 사항을 커밋하지 않고 프로젝트의 타임라인을 시각화하고 가능한 시나리오 계획을 수행할 수 있습니다. </p> <p>새로운 Gantt 차트는 자동 저장 옵션을 사용할 때 대화형이며, 변경 내용이 발생할 때 자동으로 저장할 때 사용할 수 있습니다. </p> <p>새로운 작업 목록 Gantt 차트는 최신 기술을 기반으로 구축되어 있으며 신뢰할 수 있습니다. 이 새로운 Gantt 차트는 작업 목록에 바로 있으며 탭을 전환하거나 보기를 변경하지 않고 작업 목록에서 작업하는 동안 쉽게 액세스할 수 있습니다. </p> <p>새 Gantt 차트는 이전 차트와 동일한 기능을 제공하지만 기존 Gantt와 비교하여 기능에 몇 가지 차이가 있습니다. </p> <p> 템플리트의 템플리트 태스크 목록에 있는 기존 Gantt 하위 탭, 템플리트 태스크의 하위 태스크 탭에 있는 기존 Gantt 뷰 및 템플리트 태스크 보고서에 있는 기존 Gantt 차트도 HTML 기반 Gantt 차트로 대체되었습니다. </p> <p>기존 Gantt 차트를 주로 단순 보기 및 빠른 편집에 사용하고 실제 차트를 사용하지 않는 경우 새 타임라인 계획 옵션을 사용하여 주요 계획 필드를 빠르게 변경할 수 있습니다. 작업 목록 도구 모음에서 자동 저장 대신 타임라인 계획을 선택할 수 있습니다.</p> <p>타임라인 계획 옵션을 사용하여 작업 목록을 저장하는 방법에 대한 자세한 내용은 문서의 "타임라인 계획 옵션을 선택할 때 수동으로 작업 목록에 변경 내용 저장" 섹션을 참조하십시오 <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">목록의 작업 편집</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>프로젝트 목록에 대한 기존 Gantt 차트</strong> </p> <p>프로젝트 목록의 기존 Gantt 차트를 통해 사용자는 프로젝트 및 해당 작업을 하나의 보기에서 볼 수 있습니다. 프로젝트 목록의 컨텍스트를 종료하지 않고 프로젝트 간의 종속성과 프로젝트의 작업에 대한 세부 정보를 볼 수 있습니다. 프로젝트 목록의 기존 Gantt 차트는 보안 위험을 보여주는 Flash 기술을 기반으로 했습니다. </p> </td> 
   <td> <p><strong>간트 차트, 프로젝트 목록</strong> </p> <p>HTML 기반 Gantt 차트는 기존 Gantt 차트와 동일한 목적을 제공합니다. 사용자는 프로젝트 및 해당 작업을 하나의 보기에서 보고 프로젝트 및 작업 간의 종속성을 시각적으로 식별할 수 있습니다. 프로젝트 목록 간트 차트는 프로젝트 목록에 바로 있습니다. 새로운 Gantt 차트는 최신 인터페이스와 최신 기술을 기반으로 설계되었습니다.</p> <p>프로젝트 목록 Gantt 차트에 대한 자세한 내용은 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">간트 차트에서 정보 보기 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>보고서, 달력 및 문서에 대한 공유 대화 상자</strong> </p> <p>보고서, 달력 및 문서를 공유할 때 사용된 대화 상자는 Flash 기술을 기반으로 했습니다.</p> </td> 
   <td> <p>Workfront에서 보고서, 달력 및 문서를 공유할 때의 경험은 변경되지 않았습니다. 하지만 경험은 더 이상 Flash에 의존하지 않습니다.</p> <p>이러한 항목 공유에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">개체에 대한 권한 공유 개요</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>레거시 교정 뷰어</strong> </p> <p>레거시 교정 뷰어는 정적, 비디오 및 대화형 증명을 위한 교정 기능을 제공하는 웹 기반 교정 뷰어였습니다.</p> </td> 
   <td> <p><strong>웹 언어 교정 뷰어 및 데스크탑 언어 교정 뷰어</strong> </p> <p>Web Proofing Viewer는 정적 및 비디오 증명을 위한 교정 기능을 제공합니다.</p> <p>Desktop Proofing Viewer는 정적 및 비디오 증명을 완벽하게 지원할 뿐만 아니라 대화형 증명을 위한 교정을 제공합니다.</p> <p>SWF 파일 형식은 더 이상 주요 공급자가 지원하지 않으며, 교정을 위한 HTML5 배너로 교체되었습니다. </p> <p>사용 가능한 언어 교정 뷰어 간의 차이에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Web Proofing Viewer와 Desktop Proofing Viewer 개요의 차이점</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
