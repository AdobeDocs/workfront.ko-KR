---
title: 22.4 프로젝트 개선 사항
description: 22.4 프로젝트 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# 22.4 프로젝트 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.4 릴리스의 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 10월 3일이 있는 주에 사용할 수 있습니다.

22.4 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [22.4 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 이제 전임 작업 세부 정보를 사용할 수 있습니다.

이제 작업의 전임 작업에 대한 세부 정보를 보려면 전임 작업 열의 전임 작업 번호 위로 마우스를 가져가면 됩니다. 세부 정보 상자에는 참조되는 전임 작업 및 프로젝트, 전임 작업에 대한 계획된 시작 및 종료 일자, 전임 작업의 전임 작업 및 후임 작업 수가 표시됩니다. 프로젝트 세부 정보를 확장하여 프로젝트에 대한 자세한 정보를 볼 수 있습니다. 프로젝트 간 전임 작업에 대한 추가 정보가 포함되어 있습니다.

자세한 내용은 [작업 목록에 전임 작업 관계 만들기](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## 작업 또는 문제에 여러 팀 할당

작업 및 문제를 관리하는 방식을 보다 유연하게 수행하기 위해 작업 또는 문제에 여러 팀을 할당할 수 있도록 했습니다. 이전에는 작업 또는 문제에 한 팀만 할당할 수 있었습니다.

>[!NOTE]
>
>이 기능은 현재 팀 영역의 업무 균형자에서 사용할 수 없습니다.

자세한 내용은 [작업 할당](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) 및 [문제 할당](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## 편집 및 세부 정보 영역에서 프로젝트 역할에 대한 스마트 사용자 선택

프로젝트의 편집 상자 및 세부 정보 섹션에서 다음 프로젝트 필드에 추가할 때 사용자가 표시되는 방식이 개선되었습니다.

* 프로젝트 소유자

* 프로젝트 스폰서

* 리소스 관리자

이제 편집 또는 세부 정보 영역에서 이러한 필드에 사용자를 추가하면 이름과 아바타 외에도 기본 역할과 이메일도 표시됩니다. 이러한 수정은 유사하거나 동일한 이름을 가진 여러 사용자를 구별하는 데 도움이 됩니다.

자세한 내용은 [프로젝트 편집](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

참고: 프로젝트, 작업 및 문제에 대한 추가 사용자 필드는 이후 릴리스에서 이 기능으로 업데이트됩니다.

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## 계산된 날짜 필드는 항상 UTC(협정 세계시)를 기반으로 저장됩니다.

이제 사용자 지정 데이터 표현식의 업데이트 방법이나 사용자가 전 세계의 개체를 공동 작업하는 위치에 관계없이 계산된 필드의 모든 날짜 함수가 일관되게 작동하고 모든 사용자에게 동일한 결과를 생성하는지 확인할 수 있습니다.

이제 모든 계산이 조직의 인스턴스 및 개별 사용자 프로필에 대해 설정된 시간대 구성이 아닌 하나의 표준(UTC)에 의해 계산 및 저장됩니다. 그러나 각 사용자의 브라우저에 설정된 개별 시간대를 기반으로 사용자 정의 양식에 계산이 표시됩니다.

이전에는 계산의 시간 설정이 다음과 같은 상황에서 달라질 때 혼동을 일으켰습니다.

* 누군가가 양식 빌더에서 &quot;이전 계산 업데이트&quot;를 사용하여 계산된 필드 표현식을 다시 계산했다면 날짜 함수 결과는 조직의 UTC 시간대로 결정됩니다.

* 누군가 개체를 편집하여 계산된 필드 표현식이 다시 계산되는 경우 날짜 함수 결과는 사용자의 현지 시간대로 결정됩니다. 이 시나리오의 계산된 날짜 필드 결과도 UTC를 기반으로 계산됩니다.

자세한 내용은 [시간대 간 작업](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## 사용자 정의 양식 개선 사항: Adobe XD 및 빠른 필터

사용자 의견을 기반으로 사용자 정의 양식을 관리할 때의 경험을 개선하기 위해 다음과 같은 개선 사항을 도입했습니다.

* Adobe XD 파일을 추가하여 사용자 정의 양식을 보다 시각적으로 유익하게 만듭니다. 양식이 오브젝트에 첨부되어 있으면 오브젝트와 함께 작업하는 사용자는 양식 내에서 XD 파일을 보고 상호 작용할 수 있습니다.

  자세한 내용은 [사용자 정의 양식에서 이미지 또는 기타 에셋 위젯 추가 또는 편집](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* 빠른 필터를 사용하여 현대화된 사용자 정의 양식 및 필드 목록에서 항목을 쉽게 찾을 수 있습니다. 또한 양식 및 필드를 관리하면서 향상된 모양과 느낌을 즐겨보십시오.

  빠른 필터에 대한 자세한 내용은 [목록에 빠른 필터 적용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## 공개 Beta - 프로젝트, 작업 및 문제에 대한 새로운 필터 경험

빠르게 필터를 만들고 공유할 수 있도록 프로젝트, 작업 및 문제 목록의 필터링이 다시 디자인되었습니다. 기능은 다음과 같습니다.

* 새 필터를 만들기 위한 직관적인 &quot;베타 빌더&quot; 인터페이스

* 필터를 즐겨찾기로 표시하는 기능

* 필터 스택(저장된 필터를 두 개 이상 적용)

* 필터 복제

* 필터 공유

* 나와 공유된 필터 제거


새 필터 경험은 타임시트 목록 및 시나리오 플래너에서도 사용할 수 있습니다.

텍스트 모드는 고급 필터 편집에서 계속 사용할 수 있으며 시스템 관리자는 레이아웃 템플릿을 통해 모든 사용자에 대한 기본 필터를 할당할 수 있습니다.

### 이 기능은 어디에서 사용할 수 있습니까?

* 프로젝트/작업/문제 목록

* 시나리오 플래너

* 타임시트


### 피드백을 받고 싶습니다!

이 공개 Beta 사용자에게는 피드백 버튼을 클릭하여 필터 경험을 작업하는 팀에 직접 피드백을 제출할 수 있는 기회가 제공됩니다. 공개 Beta의 새로운 필터 경험에 대해 귀하와 귀하의 사용자로부터 답변을 기다리겠습니다. 귀하의 팀이 추가 피드백을 제공하기 위해 제품을 직접 만나고 싶은 경우, https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25에서 언제든지 회의를 예약하십시오.

### 다음은 무엇입니까?

* 새 그룹화 및 보기(열이라고도 함) 경험

  그룹화 및 보기(열이라고도 함)에 대한 새 경험 작업을 시작하여 새 필터 경험과 일관되고 새 필터 경험과 동일한 몇 가지 훌륭한 기능을 갖게 됩니다.

* Adobe Workfront의 다른 영역에서 새 필터 구현

  제품 전반에 걸쳐 팀과 협력하여 Workfront 전체의 다른 영역에서 새 필터 경험을 구현합니다.


우리는 여러분에게 반복적으로 가치를 전달하고 싶기 때문에 새로운 경험과 다른 영역들이 준비되면 계속 전달할 것입니다. 더 흥미로운 업데이트를 위해 추후에 업데이트될 예정입니다.

자세한 내용은 [필터 개요](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) 및 [Adobe Workfront에서 필터 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412391/)
