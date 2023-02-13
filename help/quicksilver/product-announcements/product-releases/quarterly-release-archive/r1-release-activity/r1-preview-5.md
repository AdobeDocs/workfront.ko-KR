---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 미리 보기 5
description: 이 페이지에서는 R1 Preview 5 릴리스를 통해 미리 보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 3월 16일 미리 보기 환경에서 사용할 수 있었습니다.
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 13%

---

# R1 미리 보기 5

이 페이지에서는 R1 Preview 5 릴리스를 통해 미리 보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 3월 16일 미리 보기 환경에서 사용할 수 있었습니다.

R1에서 수행한 모든 변경 사항 목록은 [R1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## 활용률 보고서를 사용하여 프로젝트 진행 추적

이제 프로젝트에 대한 액세스 관리 권한이 있는 사용자는 활용 보고서를 통해 프로젝트의 진행 상황을 추적할 수 있습니다.

활용률 보고서를 사용하면 주어진 주 또는 월에 대해 예산책정된 시간이나 계획 시간에 대해 또는 전체 프로젝트에 대해 실제 시간이 어떻게 추적되는지 신속하게 확인할 수 있으므로 프로젝트를 예산 내에서 유지할 수 있습니다. 또한 Job 역할이나 개별 사용자별로 분류된 각 범주(예산책정, 계획 및 실제)의 시간 수에 대한 상세 정보를 조회할 수 있습니다.

프로젝트의 사용률 추적에 대한 자세한 내용은 [자원 가동률 보고서 개요](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

시스템 관리자는 사용자가 활용률 탭을 사용할 수 있는지 여부를 구성할 수 있습니다. 기본적으로 활용률 탭은 프로젝트 내의 기타 드롭다운 메뉴에 있습니다. 활용률 탭을 다른 위치로 이동하거나 완전히 숨길 수 있습니다. 조직의 사용자에 대한 사용자 지정 레이아웃 템플릿을 정의한 경우 사용자 정의 레이아웃 템플릿에 사용률 탭을 수동으로 추가해야 합니다.

활용률 탭의 위치 구성에 대한 자세한 내용은 &quot;레이아웃 템플릿 생성 및 관리&quot;에서 &quot;탭 사용자 지정&quot;을 참조하십시오.

## 개별 객체에 대한 기존 전역 승인 프로세스 수정

이제 해당 전역 승인 프로세스를 객체와 연관시킬 때 기존 전역 승인 프로세스를 수정할 수 있습니다. 수정한 사항은 연관되는 객체의 승인 프로세스에만 적용됩니다.

자세한 내용은 [신규 또는 기존 승인 프로세스를 작업물과 연결](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [신규 또는 기존 승인 프로세스를 작업물과 연결](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## 새 Gantt 차트를 기본적으로 표시하도록 보고서 구성

새 옵션 &quot;기본적으로 간트 보기에 이 보고서 표시&quot;를 사용하여 기본적으로 새 간트 차트를 표시하도록 만드는 프로젝트 및 작업 보고서를 구성할 수 있습니다.

새 Gantt 차트를 표시하도록 보고서를 구성하는 방법에 대한 자세한 내용은 [보고서 설정 편집](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

프로젝트 보고서 및 작업 보고서의 간트 차트 보기에 대한 자세한 내용은 [간트 차트에서 정보 보기](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; [간트 차트에서 정보 보기](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## 휴지통 개선: 작업 및 하위 작업은 이전 순서로 복원됩니다.

이제 작업 또는 하위 작업을 삭제한 후 복원하면 삭제하기 전에 나타난 것과 동일한 순서로 작업 또는 하위 작업이 이전 위치(작업 목록 또는 상위 작업 아래)로 복원됩니다.

이 변경 전에 복원된 작업 및 하위 작업은 삭제 전에 표시된 순서에 관계없이 항상 마지막 작업(작업 목록 또는 상위 작업 아래)으로 복원되었습니다.

Workfront에서 개체 복원에 대한 자세한 내용은 [삭제된 항목 복원](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## 이정표 보기 개선 사항

이제 이정표 보기에서 프로젝트 목록 또는 프로젝트 보고서를 볼 때 다음과 같은 개선 사항을 사용할 수 있습니다.

* **진행 상태 및 완료율이 뷰에 표시되는지 여부를 구성합니다.** 진행 상태 아이콘이 이정표 보기에 표시되는지 여부를 구성할 수 있는 새 옵션이 있습니다. 또한 프로젝트 및 작업과 관련된 완료율 정보가 표시되는지를 구성할 수도 있습니다.\
   자세한 내용은 [이정표 보기 사용](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [이정표 보기 사용](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **이정표 보기에서 직접 완료율 편집:** 이제 이정표 보기에서 직접 프로젝트 및 작업의 완료율을 편집할 수 있습니다.\
   자세한 내용은 [이정표 보기 사용](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [이정표 보기 사용](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## 여러 System Setup 페이지의 모양과 느낌을 업데이트했습니다.

설정 영역의 시스템 메뉴에 있는 다음 페이지의 모양과 느낌을 업데이트했습니다(기능은 동일하게 유지됩니다.).

* 진단
* 다음을 포함하는 SSO(Single Sign-On):

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* SSO를 위해 사용자 업데이트

## 이메일 설정 영역에서 이벤트 알림 그룹화가 업데이트되었습니다.

이제 전자 메일 설정 영역에 있는 이벤트 알림의 조직 헤더가 사용자 프로필 설정 영역에서 사용되는 섹션 헤딩과 일치합니다.

이벤트 알림에 대한 자세한 내용은  [시스템의 모든 사용자에 대한 이벤트 알림을 구성합니다](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## 인스턴트 알림 옵트아웃: 컨텍스트 내 다이제스트 구성

이제 인스턴트 이메일 알림 내에서 다음 옵션을 사용할 수 있습니다. 이러한 옵션은 일별 다이제스트 상대가 있는 인스턴트 알림에만 사용할 수 있습니다.

* “일일 요약에 추가”
* &quot;이 유형의 이메일 중지&quot;

이제 인스턴트 이메일 알림을 받으면 해당 알림을 일별 다이제스트 알림에 추가하거나 해당 알림에서 완전히 구독을 취소할 수 있습니다.

이러한 옵션은 이메일 알림 내에서 사용할 수 있습니다. 이메일 알림 수신에 대한 자세한 내용은 [Adobe Workfront 알림](../../../../workfront-basics/using-notifications/wf-notifications.md)

## &#39;필요한 작업&#39; 섹션에서 다른 프로젝트 관련 섹션으로 이동된 다양한 이메일 알림

다음과 같이 사용자 프로필 페이지의 &quot;필요한 작업&quot; 섹션에서 다른 섹션으로 여러 알림이 이동되었습니다.

이메일 알림 구성에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>알림</strong> </th> 
   <th><strong>이전 섹션</strong> </th> 
   <th><strong>새 섹션</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>내가 소유한 프로젝트에 문제가 추가됨</td> 
   <td> <p> 조치 필요 </p> </td> 
   <td>   <p>내가 소유한 프로젝트 정보</p></td> 
  </tr> 
  <tr> 
   <td>내가 진행 중인 프로젝트에 문제가 추가됨</td> 
   <td>   <p>조치 필요</p><p> </p></td> 
   <td> <p> 내가 소유한 프로젝트 정보 </p>   </td> 
  </tr> 
  <tr> 
   <td>미할당 문제를 내가 소유한 프로젝트에 추가합니다.</td> 
   <td>   <p>조치 필요</p></td> 
   <td>   <p>내가 소유한 프로젝트 정보</p></td> 
  </tr> 
  <tr> 
   <td> <p> 내가 진행 중인 프로젝트에 할당 해제된 문제가 추가됨 </p> </td> 
   <td> <p> 조치 필요 </p>   </td> 
   <td> <p> 내가 소유한 프로젝트 정보 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 내 프로젝트 중 하나의 작업에 대한 커밋 일자 변경 </p> </td> 
   <td>   <p>조치 필요</p></td> 
   <td>   <p>내가 소유한 프로젝트 정보</p></td> 
  </tr> 
  <tr> 
   <td> <p> 내 프로젝트 중 하나의 문제에 대한 커밋 일자 변경 </p>   </td> 
   <td>   <p>조치 필요</p></td> 
   <td> <p> 내가 소유한 프로젝트 정보 </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> 나에게 할당된 작업의 기한 변경 </p> </td> 
   <td>   <p>조치 필요</p></td> 
   <td>   <p>나에게 할당된 작업 정보</p></td> 
  </tr> 
  <tr> 
   <td> <p> 내가 할당된 문제의 기한이 변경됩니다. </p> </td> 
   <td> <p> 조치 필요 </p>   </td> 
   <td>   <p>나에게 할당된 작업 정보</p></td> 
  </tr> 
  <tr> 
   <td> <p> 내게 할당된 작업의 상태 변경 </p>   </td> 
   <td> <p> 조치 필요 </p>   </td> 
   <td> <p> 나에게 할당된 작업 정보 </p>   </td> 
  </tr> 
 </tbody> 
</table>

## 새로운 리소스 계획 기능 (R1의 프로덕션에서 사용할 수 없음)

>[!NOTE]
>
>이 기능은 현재 미리 보기 환경에서 사용할 수 있습니다. 이 구성 요소는 프로덕션에 대한 R1 릴리스 약 1개월 전에 미리 보기 환경에서 제거됩니다. 그러면 R2 미리 보기 1의 미리 보기 환경에 다시 도입됩니다.

 

향후 리소스 계획 기능을 지원하기 위해 다음 변경 사항이 추가되었습니다.

* 현재 &quot;리소스 계획&quot; 탭의 이름이 사용자 영역에서 &quot;레거시 리소스 계획&quot;으로 변경되었습니다. 
* 새 기능을 개발할 사용자 영역에 새로운 &quot;리소스 계획&quot; 탭이 도입되었습니다.\
   새 리소스 계획 탭에 대한 자세한 내용은 [리소스 계획 시작](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* 현재 &quot;리소스 풀&quot; 개체의 이름이 &quot;레거시 리소스 풀&quot;으로 변경되었습니다.\
   새 사용자 기반 리소스 풀 만들기에 대한 자세한 내용은 [리소스 풀 개요](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* 새(사용자 기반) 리소스 풀을 지원하기 위해 새 &quot;리소스 풀&quot; 개체가 생성되었습니다.

   >[!NOTE]
   * 현재 기존 레거시 리소스 풀에서 보고서를 실행 중인 경우 기존 보고서는 변경되지 않습니다.
   * 기존(작업 역할 기반) 레거시 리소스 풀에 대해 새 보고서를 만들려면 &quot;레거시 리소스 풀&quot;을 보고서의 개체로 선택해야 합니다.
   * 새(사용자 기반) 리소스 풀에 대한 새 보고서를 만들려면 &quot;리소스 풀&quot;을 보고서의 개체로 선택해야 합니다.

  >   
