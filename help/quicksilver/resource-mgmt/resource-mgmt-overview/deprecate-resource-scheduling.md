---
content-type: reference
product-area: resource-management
keywords: 워크로드,밸런서
navigation-topic: resource-management-overview
title: Adobe Workfront의 리소스 예약 도구 사용 중단
description: 현재 Adobe Workfront에서 모든 예약 도구를 사용하지 않고 작업 로드 밸런서로 교체하는 중입니다.
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Adobe Workfront의 리소스 예약 도구 사용 중단

>[!IMPORTANT]
>  
><span class="preview">이 문서에 설명된 예약 기능은 2023년 1월 23.1 릴리스부터 Adobe Workfront에서 더 이상 사용되지 않고 제거됩니다.   </span>
>  
> <span class="preview"> 이 문서는 2023년 초에 23.1 릴리스 직후 제거됩니다. 지금은 이에 따라 책갈피를 업데이트하는 것이 좋습니다. </span>
> 
><span class="preview"> 이제 작업 로드 밸런서를 사용하여 자원에 대한 작업 일정을 예약할 수 있습니다. </span>
>  
> <span class="preview">작업 로드 밸런서를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [작업 로드 밸런서](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--
We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.
-->

## 준비 방법

스케줄과 작업 로드 밸런서 간 전환을 준비하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [자원 스케줄링에서 작업 로드 밸런서로 마이그레이션](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

현재 예약 도구를 사용하는 경우 해당 도구를 중단하고 작업 로드 밸런서 사용을 시작하는 것이 좋습니다.

![글로벌 자원 스케줄링 영역](assets/resource-scheduler-global-350x127.png)

이제 작업 로드 밸런서에서 이전에 예약 영역에서 사용할 수 있었던 거의 모든 기능을 사용할 수 있습니다. 자세한 내용은 섹션을 참조하십시오 [기능 가용성](#feature-availability) 참조하십시오. 작업 로드 밸런서에서 작업에만 사용할 리소스를 계속 예약할 수 있습니다.

![전역 작업 로드 밸런서 영역](assets/workload-balancer-pti-350x111.png)

## 작업 로드 밸런서로 전송되지 않는 정보

다음 정보는 스케줄링 도구에서 작업 로드 밸런서로 전송되지 않습니다.

* **사용자에 대한 일별 할당**: 동일한 사용자 할당을 조정하기 위해 스케줄링 및 작업 로드 밸런서를 동시에 사용해서는 안 됩니다. 스케줄링 도구에서 관리 사용자 할당이 있는 경우 조정된 일별 할당이 작업 로드 밸런서로 전송되지 않습니다. 마찬가지로, 작업 로드 밸런서에서 사용자 할당을 조정한 경우 예약 도구로 전송되지 않습니다. 이 전환을 준비할 수 있도록 작업 로드 밸런서에서 일별 할당이 정확한지 확인하는 것이 좋습니다. 자세한 내용은 [작업 로드 밸런서에서 사용자 할당 관리](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **필터**: 예약 영역에 필터를 저장한 경우 작업 로드 밸런서로 전송되지 않습니다. 작업 로드 밸런서에서 필터를 다시 생성해야 합니다. 자세한 내용은 [작업 로드 밸런서에서 정보 필터링](../workload-balancer/filter-information-workload-balancer.md).

## 사용 중단 타임라인 강조 표시

>[!IMPORTANT]
>
>이 문서를 사용하여 예약 도구 사용 중단에 대한 최신 타임라인을 파악합니다. 이 타임라인에 대한 모든 업데이트는 이 문서와 공지 센터 메시지에 전달됩니다.

다음은 리소스 예약 도구의 사용 중단 프로세스에 대한 타임라인입니다.

* [2020.4 릴리스(2020년 11월)](#2020-4-release-november-2020)
* [2021.4 릴리스(2021년 10월)](#2021-4-release-october-2021)
* [2022.4 - 2023.1 릴리스(2022년 10월 - 2023년 1월)](#2022-4-2023-1-releases)

### 2020.4 릴리스(2020년 11월) {#2020-4-release-november-2020}

* 예약 솔루션에 대한 새로운 기능 기능이 더 이상 구현되지 않습니다
* High 및 Critical Severity 결함만 Fix를 위해 우선 순위가 지정됩니다
* Workfront에 추가된 새로운 작업 로드 밸런서 기능

### 2021.4 릴리스(2021년 10월) {#2021-4-release-october-2021}

* 작업 로드 밸런서는 Workfront의 처음 사용자에 대해 기본값으로 설정됩니다
* 공유 및 추가 필드를 포함할 수 있는 향상된 필터

### 2022.4 - 2023.1 릴리스(2022년 10월 - 2023년 1월) {#2022-4-2023-1-releases}

* 2022.4 또는 2023.1 릴리스 중 및 이후 수정 사항에 대해 우선 순위가 지정되지 않습니다
* 모든 예약 영역이 미리 보기 환경에서 제거됩니다(**2022년 10월 20일**)
* 모든 예약 영역이 프로덕션 환경에서 제거됩니다(**2023년 1월**)
* 작업 로드 밸런서는 Workfront에서 사용할 수 있는 유일한 리소스 예약 도구입니다 **2023년 1월**)

## 기능 가용성 {#feature-availability}

별도로 지정하지 않는 한 모든 리소스 스케줄링 기능이 작업 로드 밸런서에서 사용되었거나 사용할 수 있게 됩니다. 작업 로드 밸런서에 대한 자세한 내용은 [작업 로드 밸런서 개요](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

작업 로드 밸런서에는 기존 기능 외에도 다음 표와 같이 리소스 스케줄링 도구에 존재하지 않았던 새 기능이 있거나 있을 것입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>기능</b></span> </td> 
   <td rowspan="2"> <b>리소스 예약 도구 기능 가용성</b></td> 
   <td colspan="3"><b>작업 로드 밸런서 기능 가용성</b></td> 
  </tr> 
  <tr> 
   <td><b>지금 사용 가능</b></td> 
   <td><b>곧 제공</b></td> 
   <td><b>계획되지 않음</b></td> 
  </tr> 
  <tr> 
   <td> <p>리소스 영역에서 액세스 도구</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>지정되지 않은 작업 및 할당된 작업 영역 분리</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>지정되지 않음 및 할당된 작업에 대한 필터 적용 및 만들기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>도구에서 직접 작업 항목에 액세스</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>수동으로 작업 및 문제 지정 또는 할당 취소</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>개별 할당 조정</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>문제 시간 포함</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>예상 날짜 표시 </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>완료된 작업 표시</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>사용자 시간 초과, 주말 및 예약 예외 표시</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>역할에 따라 신속하게 사용자 할당*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>신속한 사용자 교체*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>사용자 할당 취소 속도 향상*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>팀에서 도구 액세스</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>프로젝트에서 도구 액세스</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr>
   <td>작업 라이선스 사용자는 프로젝트에서 작업 로드 밸런서에 액세스할 때 사용자 할당을 조정할 수 있습니다 </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>지정되지 않은 작업 영역에 문제 표시</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>끌어다 놓아 작업 및 문제 할당 및 할당 취소*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로젝트에서 리소스 관리자를 지정하지 않고 모든 계획 사용자가 볼 수 있습니다.</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로젝트별 정보 그룹화</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>리소스 영역에 대한 액세스 권한이 없는 사용자와 작업 로드 밸런서를 공유합니다</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>주별 할당 표시 및 조정</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>도구에서 직접 사용자 액세스</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>요약 패널을 사용하여 다른 곳으로 이동하지 않고 작업 항목에 대한 자세한 정보에 액세스*</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>백분율 값으로 할당 표시 및 조정 </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>사용 가능한 시간과 할당된 시간 간의 차이를 표시합니다</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>차트에 사용자 가용성 표시</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>프로젝트 상태별 색상 코드 작업 항목 및 프로젝트</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>사용자 할당을 조정할 때 계획 시간을 자동으로 갱신합니다(단순 기간 유형이 있는 작업의 경우).</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>사용자의 지정 패턴, 기존 역할 또는 팀 지정에 따라 지정을 제안합니다</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>공유 및 추가 필드를 포함할 수 있는 향상된 필터</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>고급 할당</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr>

<tr> 
   <td><span>프로젝트 및 프로젝트 상태별 색상 코드 작업 항목</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td>

<tr> 
   <td>프로젝트 팀에 사용자 추가(재배치됨) <b>사람</b> 프로젝트의 탭) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td> </td>

</tr>
   <tr> 
   <td>작업 및 문제 자동 할당</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr>

</tbody> 
</table>

*이러한 기능은 새 Adobe Workfront 경험에서만 사용할 수 있습니다.
