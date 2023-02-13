---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 미리 보기 3
description: 이 페이지에서는 R1.3 릴리스를 통해 미리 보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 2월 1일 미리 보기 환경에서 사용할 수 있었습니다.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 1%

---

# R1 미리 보기 3

이 페이지에서는 R1.3 릴리스를 통해 미리 보기 환경에서 사용할 수 있는 모든 변경 사항에 대해 설명합니다. 이 페이지의 기능은 2017년 2월 1일 미리 보기 환경에서 사용할 수 있었습니다.

R1에서 수행한 모든 변경 사항 목록은 [R1 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 외부 파일 연결 방법이 개선되었습니다.

외부 소스(예: Google 드라이브, 상자, Dropbox 등)에서 문서를 연결하는 옵션이 문서 영역에서 보다 눈에 띄는 위치에 있습니다. 

또한 해당 공급자에서 파일을 처음으로 연결하기 전에 문서 공급자를 승인하는 작업이 이제 더 직관적이 됩니다(외부 공급자에서 파일을 연결할 때 추가 단계일 수 있음).

이러한 변경 전에 외부 소스의 파일을 연결하는 옵션이 문서 영역 내의 문서 추가 대화 상자 내에 있었습니다. 외부 소스에서 문서를 처음으로 연결하기 전에 문서 연결 사용자가 설정 영역에서 해당 문서 공급자를 승인해야 했습니다.

자세한 내용은  [외부 응용 프로그램에서 문서 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## 일정에 따라 작업하는 팀이 업데이트되었습니다.

이제 팀에서 사용할 수 있는 작업 일정 에는 추가 기능과 업데이트된 모양 및 느낌이 포함되어 있습니다. 이제 팀 작업 달력이 프로젝트의 리소스 예약 도구와 유사하게 작동합니다.

업데이트된 팀 작업 일정에는 다음과 같은 개선 사항이 포함됩니다.

* 사용자를 알파벳순으로 보거나 역할별로 그룹화합니다.
* 프로젝트 우선순위, 상태 및 개별 프로젝트별로 예약 타임라인을 필터링합니다. 역할 및 사용자별로 예약 타임라인을 필터링할 수도 있습니다. (필터 영역에는 프로젝트에 대한 리소스를 예약할 때보다 더 적은 선택 사항이 포함됩니다.)
* 예약 타임라인에 문제를 포함합니다.
* 사용자 할당을 표시하고 사용자가 각 날의 특정 작업 및 문제에 할당된 시간 수를 수정합니다.
* 사용자가 지정된 날짜에 너무 많이 할당되는 시기를 보여주는 지표를 봅니다.
* 완료된 작업이 예약 타임라인에 표시되는지 여부를 구성합니다.

프로젝트에 대한 리소스를 예약할 때 리소스 예약 툴과 차이가 있습니다.

* 모든 팀 구성원이 작업 일정에 표시됩니다.\
   프로젝트에 대한 리소스를 예약할 때 [지정되지 않음] 영역에서 하나 이상의 작업 역할과 일치하는 역할과 연관된 역할이 있는 사용자만 표시됩니다.
* 교체 도구는 Working On 일정에 포함되어 있지 않습니다.
* 모든 팀 구성원은 Working On 일정에서 변경할 수 있습니다.\
   프로젝트에 대한 리소스를 스케줄링할 때 자원 관리자만 프로젝트에 대한 자원 결정을 수행할 수 있습니다.
* Working On 일정에 기본적으로 문제가 표시됩니다.\
   프로젝트에 대한 리소스를 예약할 때 기본적으로 문제는 표시되지 않습니다.

업데이트된 팀 작업 일정 사용에 대한 자세한 내용은 [리소스 예약](../../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

## 리소스 예약 개선 사항

예약 타임라인에는 다음과 같은 개선 사항이 포함됩니다.

* [필터를 사용하여 예약 타임라인에 표시되는 사용자를 제어합니다.](#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline)
* [작업 할당 후 타임라인에 남아 있는 사용자](#users-remain-on-the-timeline-after-being-assigned-a-task)

### 필터를 사용하여 예약 타임라인에 표시되는 사용자를 제어합니다. {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

이제 필터를 사용하여 미지정 영역에 표시되는 작업 및 문제와 함께 예약 타임라인에 표시되는 사용자를 제어할 수 있습니다. 필터에서 사용자를 선택하면 [지정되지 않음] 영역에서 작업의 역할 할당과 일치하는 역할 할당이 있는지 여부에 관계없이 선택한 사용자만 표시됩니다. 해당 사용자에게 현재 할당된 모든 작업도 표시됩니다.

이 변경 전에 필터는 [지정되지 않음] 영역에 표시된 작업 및 문제만 제어했습니다. 사용자가 지정되지 않은 영역에서 작업의 역할 할당과 일치한 경우에만 예약 타임라인에 표시됩니다.

필터를 사용하여 예약 타임라인에 표시되는 내용을 제어하는 방법에 대한 자세한 내용은  [예약 영역에서 정보를 필터링합니다.](../../../../resource-mgmt/resource-scheduling/filter-scheduling-area.md), 및  [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 작업 할당 후 타임라인에 남아 있는 사용자 {#users-remain-on-the-timeline-after-being-assigned-a-task}

사용자에게 작업 또는 문제가 할당되면, 일치하는 역할 할당이 있는 남은 작업 또는 문제가 없는 경우에도 예약 타임라인에 남아 있습니다. 이를 통해 사용자를 지정한 후 필요한 사항을 변경할 수 있습니다.

이 변경 전에 동일한 역할 할당이 있는 [지정되지 않음] 영역에 남은 작업이나 문제가 없을 경우, 작업 또는 문제가 지정된 직후에 예약 타임라인에서 사용자가 사라집니다.

자세한 내용은  [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## 개체 이름을 변경하여 Workfront 용어 사용자 지정

이제 특정 개체의 이름을 변경하여 Workfront 용어를 사용자 지정할 수 있습니다.\
이제 레이아웃 템플릿을 사용하여 조직의 요구 사항에 맞게 다음 작업 객체의 이름을 변경할 수 있습니다.

* 포트폴리오
* 프로그램
* 프로젝트
* 작업
* 문제

예를 들어 조직에서 프로젝트 대신 캠페인으로 작업하는 경우 &quot;프로젝트&quot; 개체의 이름을 &quot;캠페인&quot;으로 바꿀 수 있습니다.

이 대체 작업을 수행하면 응용 프로그램의 다음 영역에 객체의 업데이트된 이름이 표시됩니다.

* 전역 탐색 모음
* 모든 탭
* 모든 메뉴 
* Report Builder 및 보고 요소(보기, 필터 및 그룹화)
* 저장 단추
* 내보낸 파일
* 이메일

다음 영역에는 객체의 업데이트된 이름이 표시되지 않습니다.

* 리소스 추정치
* 리소스 예산 관리자
* 수용작업량 플래너
* 리소스 그리드
* 팀 빌더
* Portfolio 최적화 프로그램 
* 모바일 앱
* Outlook 추가 기능

레이아웃 템플릿을 사용하여 Workfront 용어를 사용자 지정하는 방법에 대한 자세한 내용은 의 &quot;레이아웃 템플릿 만들기 및 관리&quot;에서 &quot;용어 사용자 지정&quot; 섹션과 &quot;개체 이름 사용자 지정에 대한 의미 이해&quot; 섹션을 참조하십시오 [Adobe Workfront의 개체 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 보고서에 승인 시작 및 종료 날짜 포함

이제 보고서를 만들거나 수정할 때 다음 필드를 포함할 수 있습니다.

* 승인 경로 시작 일자
* 승인 경로 완료 날짜

이러한 필드를 사용하면 현재 또는 가장 최근 승인 경로가 시작된 시기와 승인 경로가 완료로 표시된 시기를 알 수 있습니다.

이러한 필드에 대한 자세한 내용은 [Adobe Workfront 용어 설명](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

승인 경로, 승인 경로가 생성 및 트리거되는 방법 및 승인 프로세스에서 제공하는 기능에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 생성](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

다음 필드는 Workfront에서 제거되어 더 이상 보고서에 포함할 수 없습니다(이러한 필드는 승인 자체에 대한 정보가 아니라 프로젝트에 대한 정보를 제공했으며 종종 오용됨).

* 승인 계획 시작 날짜
* 승인 예상 시작 일자
* 승인 예상 시작 일자

## &quot;수행한 요청&quot;에 대한 새 이메일 다이제스트 옵션

일별 다이제스트 게재 옵션이 알림 설정의 &quot;요청 수행&quot; 영역에 추가되었습니다.

자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

이 기능을 테스트할 수 있도록 계정과 연결된 이메일 주소를 업데이트해야 합니다. 미리 보기 샌드박스는 모든 사용자의 이메일 주소를 지우므로 필요합니다.

## 문서 승인 전자 메일 알림의 모양과 느낌을 업데이트했습니다.

&quot;문서 승인&quot;에 대한 알림 모양과 느낌을 새 UI로 업데이트했습니다.

이메일 알림에 대한 자세한 내용은 [Adobe Workfront 알림](../../../../workfront-basics/using-notifications/wf-notifications.md).

이 기능을 테스트할 수 있도록 계정과 연결된 이메일 주소를 업데이트해야 합니다. 미리 보기 샌드박스는 모든 사용자의 이메일 주소를 지우므로 필요합니다.

## 이정표 보기의 개선 사항

이제 프로젝트 목록 또는 프로젝트 보고서를 볼 때 사용할 수 있는 이정표 보기에는 다음과 같은 개선 사항이 포함됩니다.

* 계획 날짜는 편집 가능합니다
* 프로젝트 및 작업에 대한 완료율이 표시됩니다

이 변경 전에 완료 날짜 또는 보기 백분율을 편집하려면 개별 작업으로 이동해야 합니다.

자세한 내용은 [이정표 보기 사용](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
