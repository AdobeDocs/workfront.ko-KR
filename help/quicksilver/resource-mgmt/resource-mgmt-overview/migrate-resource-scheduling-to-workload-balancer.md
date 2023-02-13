---
filename: migrate-resource-scheduling-to-workload-balancer
product-area: resource-management
navigation-topic: resource-management-overview
title: 리소스 예약에서 다음으로 마이그레이션 [!UICONTROL 작업 로드 밸런서]
description: 마이그레이션 계획을 설계하도록 지원함으로써 가능한 한 적은 작업 중단을 경험하시기 바랍니다. 아래 단계는 작업 로드 밸런서로 전환하기 위한 최적의 시간을 파악하여 팀의 교육을 받는 데 도움이 됩니다.
author: Alina
exl-id: 4bc08d5f-99c7-40e2-85d6-1de0b585aef8
source-git-commit: d2a8380e3383b97b8245bd2b6d3cb9ff75306e4f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# 리소스에서 마이그레이션 [!UICONTROL 예약] 변환 후 [!UICONTROL 작업 로드 밸런서]

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 환경에서만 사용할 수 있습니다.</span>

<!-- drafted for res scheduling deprecation blurb for PREVIEW release - Oct 2022 - CHANGE THIS BLURB TO SOMETHING ELSE AT PRODUCTION:-->

>[!CAUTION]
>  
>  
> <span class="preview">예약 영역이 미리 보기 환경에서 제거되었으며 의 프로덕션 환경에서 제거됩니다 **2023년 1월**. </span>\
> <span class="preview"> 2023년 1월 이후에는 작업 로드 밸런서에서 리소스를 예약해야 합니다. </span>
>  
><span class="preview"> 작업 로드 밸런서를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [작업 로드 밸런서](../../resource-mgmt/workload-balancer/workload-balancer.md).</span>

이 문서의 정보는 리소스의 리소스 일정을 관리한 경우에만 적용됩니다 [!UICONTROL 예약] Adobe Workfront 지역. Workfront이 [!UICONTROL 예약] 는 2020년 11월 도구에서 [!UICONTROL 작업 로드 밸런서].

의 사용 중단 계획에 대한 자세한 내용은 [!UICONTROL 리소스 예약] 도구 및 타임라인을 통해 [!UICONTROL 작업 로드 밸런서]를 참조하십시오. [Adobe Workfront의 리소스 예약 도구 사용 중단](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

마이그레이션 계획을 설계하도록 지원함으로써 가능한 한 적은 작업 중단을 경험하시기 바랍니다. 아래 단계에서는 팀의 교육을 받고 전환 시간을 결정할 수 있습니다 [!UICONTROL 작업 로드 밸런서].

## 리소스 예약 도구를 찾습니다

사용자와 팀이 일부 리소스를 사용하고 있을 수 있습니다 [!UICONTROL 예약] Workfront의 다음 영역에 있는 도구:

* 다음 [!UICONTROL 예약] 의 섹션 [!UICONTROL 리소스] 영역
* 다음 [!UICONTROL 예약] 프로젝트의 섹션
* 다음 [!UICONTROL 예약] 팀의 섹션

이 사용 중단 시 [!UICONTROL 작업 로드 밸런서] 모두 바꾸기  [!UICONTROL 리소스 예약] 위에 나열된 모든 영역의 도구.

## 1단계: 팀 교육

교육 시작 [새로운 Adobe Workfront 경험을 위한 리소스 관리 프로그램](https://one.workfront.com/s/resource-management-program-nwe) (75분) Workfront One.

로그인하거나 교육 과정에 액세스하는 데 어려움이 있다면 고객 지원 센터에 문의하십시오. 자세한 내용은 [고객 지원에 문의](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## 2단계: 마이그레이션할 최적의 시간 결정 {#step-2-determine-the-best-time-to-migrate}

아래 절차에 따라 마이그레이션해야 하는 최적의 시간이 언제인지 결정하십시오.

1. 리소스의 기능 확인 [!UICONTROL 예약] 팀에서 가장 많이 사용하는 도구를 사용하고 [!UICONTROL 작업 로드 밸런서]. 에서 현재 사용할 수 있는 기능에 대한 자세한 내용은 [!UICONTROL 작업 로드 밸런서]를 참조하려면 문서의 &quot;기능 가용성&quot; 섹션을 참조하십시오 [Adobe Workfront의 리소스 예약 도구 사용 중단](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

   >[!IMPORTANT]
   >
   >스케줄링 도구의 거의 모든 기능이 이제 작업 로드 밸런서에 있습니다.

1. 지정 시 팀이 사용자 할당을 관리하는지 여부를 결정합니다. 사용자 할당을 조정하거나 수정하는 것은 작업 항목의 지속 시간 동안 각 사용자에 대한 일별 계획 시간을 수정하는 것을 의미합니다.

   예약 도구에서 편집한 할당은 작업 로드 밸런서로 전송되지 않습니다. 기본적으로 시스템은 품목의 전체 기간 동안 작업 항목의 총 계획 시간을 균등하게 분배합니다.

   할당이 스케줄링 도구에 있는 할당과 일치하도록 작업 로드 밸런서에서 수동으로 할당을 관리해야 합니다. 자세한 내용은 [작업 로드 밸런서에서 사용자 할당 관리](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. 예약 영역에 저장된 모든 필터는 작업 로드 밸런서로 자동으로 전송되지 않습니다. 작업 로드 밸런서에서 필요한 필터를 생성할 시간을 지정합니다. 작업 로드 밸런서에서 필터 만들기에 대한 자세한 내용은 [작업 로드 밸런서에서 정보 필터링](../workload-balancer/filter-information-workload-balancer.md).

<!--
1. Using the information gathered from Steps 1 and Step 2, decide which version of Step 3 you should continue with based on the needs of your organization.
-->

## 3단계: 으로 마이그레이션 [!UICONTROL 작업 로드 밸런서]{#step-3-migrate-to-the-workload-balancer}

2단계의 결과에 따라 이 단계의 다음 버전을 식별했습니다.

* [3a단계: 사용자 또는 팀이 [!UICONTROL 예약] 도구를 사용하지만 사용자 할당은 수정하지 않습니다.](#step-3a-you-or-your-teams-use-the-scheudling-tools-but-do-not-modify-user-allocation)
* [3b단계: 사용자 또는 팀이 [!UICONTROL 예약] 도구](#step-3b-you-or-your-teams-manage-user-allocations-in-the-scheduling-tools)

### 3a단계: 사용자 또는 팀이 [!UICONTROL 예약] 도구를 사용하지만 사용자 할당은 수정하지 않습니다.

사용자 또는 팀이 작업 할당에서 일별 시간 할당을 수정하지 않으면 예약 리소스를 [!UICONTROL 작업 로드 밸런서].

![](assets/nwe-workload-balancer-global-350x125.png)

다음을 수행합니다.

* 전환 날짜를 선택합니다.

   >[!TIP]
   >
   >전환 날짜 이전에 작업 로드 밸런서 사용에 대한 교육을 받을 시간을 팀에 제공합니다. 교육에 대한 자세한 내용은 섹션을 참조하십시오 [자원 스케줄링에서 작업 로드 밸런서로 마이그레이션](#migrate-from-resource-uicontrol-scheduling-to-the-uicontrol-workload-balancer) 참조하십시오.

* 팀을 지원하려면 다음 지침을 따르십시오.

   * 팀원이 [개요 [!UICONTROL 작업 로드 밸런서]](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) 페이지 및 여기에서 연결된 모든 페이지를 확인하여 [!UICONTROL 작업 로드 밸런서] 작동합니다.
   * 전환 1주일 전에 질문에 답변하고 전환한 다음 다른 FAQ 회의를 열어 후속 질문에 답변합니다.
   * 상단 도구 모음의 피드백 단추를 사용하여 Workfront에 피드백을 제출합니다. Adobe의 제품 개발자들은 Adobe가 제공하는 방법에 대한 사용 사례를 듣는 데 항상 관심이 있습니다 [!UICONTROL 작업 로드 밸런서] 더 많은 값을 제공합니다.

### 3b단계: 사용자 또는 팀이 [!UICONTROL 예약] 도구

워크플로우가 이 시나리오와 일치하는 경우 전환 계획에서 더 전략적이어야 합니다. 에 표시되는 일별 할당 [!UICONTROL 예약] 도구는에 표시되는 일별 할당이 아닌 다른 데이터베이스에 저장됩니다 [!UICONTROL 작업 로드 밸런서]. 이는 리소스에서 수행하는 일별 할당 조정을 의미합니다 [!UICONTROL 예약] 도구는에서 일별 할당으로 전송되지 않습니다 [!UICONTROL 작업 로드 밸런서].

>[!CAUTION]
>
>언제까지 **2023년 1월** 스케줄링 영역에서 사용자 할당이 프로덕션 환경에서 작업 로드 밸런서의 할당과 일치하는지 확인합니다. 이때 프로덕션 환경에서 예약 도구를 제거합니다. 작업 로드 밸런서에서 할당을 수동으로 조정하여 예약 도구의 할당과 일치해야 합니다. <span class="preview">예약 도구가 미리 보기 환경에서 이미 제거되었습니다.</span>


로 전환할 때 다음 사항을 고려하십시오 [!UICONTROL 작업 로드 밸런서] 사용 시 [!UICONTROL 예약] 기능:

* 에서 할당 관리를 보류합니다. [!UICONTROL 예약] 리소스 관리자의 도구 전환 방법은 다음과 같습니다.

   * 현재 프로젝트에서 작업의 평균 기간을 확인하고 사용자 할당 관리를 보류해야 하는 시간을 결정할 때 이를 고려하십시오.

      >[!TIP]
      >
      >현재 또는 계획 프로젝트만 확인해야 합니다. 이 프로젝트들은 팀에서 할당을 수행하고 일별 할당을 관리하는 프로젝트입니다.

   * 작업 보고서를 만들고 보기에 작업 기간 필드를 추가하고 프로젝트 이름으로 그룹화합니다. 평균 보기 로 기간 열을 요약한 다음 보고서를 저장합니다.

      보고서 만들기에 대한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) .

   * 작업 보고서를 분석합니다. 예를 들어 평균 작업 기간이 3일인 경우 1주 전환이 가장 좋을 수 있습니다. 팀이 1주일 동안 사용자 할당 관리를 중지하도록 합니다. 다음 주에 팀을 [!UICONTROL 작업 로드 밸런서] 다음 주에 사용자 할당 관리를 시작합니다.
   >[!NOTE]
   >
   >평균 작업 기간이 예약 도구를 제거할 때까지 남은 시간보다 긴 경우 이 제안이 작동하지 않을 수 있습니다.


   ![](assets/timeline-stop-using-resource-scheduler-callouts-350x178.png)

   >[!TIP]
   >
   >전환 기간 동안 계속 작업 및 문제 지정을 수행할 수 있습니다. 지정된 할당은 자원 스케줄러와 [!UICONTROL 작업 로드 밸런서].

* 수백 개의 프로젝트에 대한 리소스를 관리하는 팀이 있는 더 큰 조직의 경우 [!UICONTROL 예약] 도구 [!UICONTROL 작업 로드 밸런서] 한 번에 한 포트폴리오. 에서 사용자 지정된 필터를 만들어 단계적 롤아웃을 고려하십시오 [!UICONTROL 작업 로드 밸런서] 한 번에 하나의 특정 포트폴리오를 살펴보십시오.

* 리소스 관리자가 팀을 구성할 수 있도록 허용: 한 사람의 검토 과제를  [!UICONTROL 리소스 예약] 도구 및 [!UICONTROL 작업 로드 밸런서]. 두 개의 툴로 구성된 해당 팀이 두 툴을 모두 조정하면 워크플로우를 [!UICONTROL 작업 로드 밸런서].

## 추가 지원 필요

이 마이그레이션에 대한 추가 정보가 필요한 경우 사용자 지정 지원에 문의하십시오. 지원에 문의하는 방법에 대한 자세한 내용은 [고객 지원에 문의](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
