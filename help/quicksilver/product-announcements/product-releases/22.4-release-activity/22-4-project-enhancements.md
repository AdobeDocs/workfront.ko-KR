---
title: 22.4 프로젝트 개선 사항
description: 22.4 프로젝트 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 2%

---

# 22.4 프로젝트 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.4 릴리스로 수행된 모든 프로젝트 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 10월 3일이 있는 주에 제공될 예정입니다.

22.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.4 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 이전 버전 세부 사항은 이제 사용할 수 있습니다

이제 선행 작업의 세부 사항을 보려면 선행 작업 열의 선행 작업 번호를 마우스로 가리키면 됩니다. 세부 정보 상자에는 참조된 선행 작업 및 프로젝트, 선행 작업의 계획 시작 및 종료 날짜, 선행 작업 및 후속 작업 수가 표시됩니다. 프로젝트 세부 사항을 확장하여 프로젝트에 대한 자세한 정보를 볼 수 있습니다. 프로젝트 간 선행 작업을 위한 추가 정보가 포함되어 있습니다.

자세한 내용은 [작업 목록에서 선행 관계 만들기](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## 작업 또는 문제에 여러 팀 할당

작업 및 문제를 관리하는 방법에 대해 보다 유연하게 대처할 수 있도록 여러 팀을 작업이나 문제에 할당할 수 있도록 했습니다. 이전에는 한 팀만 작업이나 문제에 할당할 수 있었습니다.

>[!NOTE]
>
>현재 팀 영역의 작업 로드 밸런서에서 이 기능을 사용할 수 없습니다.

자세한 내용은 [작업 할당](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) 및 [문제 할당](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## 편집 및 세부 정보 영역에서 프로젝트 역할에 대한 스마트 사용자 선택

프로젝트의 편집 상자 및 세부 정보 섹션에서 다음 프로젝트 필드에 추가할 때 사용자가 표시되는 방식이 개선되었습니다.

* 프로젝트 소유자

* 프로젝트 스폰서

* 리소스 관리자

이제, 사용자를 편집 또는 세부 정보 영역의 이러한 필드에 추가하면 사용자의 이름과 아바타 외에도 기본 역할 및 전자 메일도 표시됩니다. 이러한 수정은 유사하거나 동일한 이름을 가진 여러 사용자를 구별하는 데 도움이 됩니다.

자세한 내용은 [프로젝트 편집](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

참고: 프로젝트, 작업 및 문제에 대한 추가 사용자 필드는 향후 릴리스에서 이 기능을 사용하여 업데이트됩니다.

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## 계산된 날짜 필드는 항상 UTC(Coordinated Universal Time)를 기반으로 저장됩니다

이제 사용자 지정 데이터 표현식의 업데이트 방식이나 전 세계 사용자가 개체를 공동 작업하고 있는 위치에 상관없이 계산된 필드의 모든 날짜 기능이 일관되게 작동하고 모든 사람에게 동일한 결과를 제공하는지 확인할 수 있습니다.

이제 모든 계산은 조직의 인스턴스 및 개별 사용자 프로필에 대해 설정된 표준 시간대 구성이 아닌 하나의 표준(UTC)에 의해 계산되고 저장됩니다. 하지만 계산은 브라우저에 설정된 각 사용자의 개별 시간대를 기반으로 사용자 지정 양식에 표시됩니다.

이전에는 이러한 상황에서 계산의 시간 설정이 변경되면 혼동했었습니다.

* 양식 빌더에서 &quot;이전 계산 업데이트&quot;를 사용하여 계산된 필드 표현식을 다시 계산한 경우, 날짜 함수 결과는 조직의 UTC 표준 시간대로 결정됩니다.

* 개체를 편집하고 계산된 필드 표현식이 다시 계산되는 경우 날짜 함수 결과는 사용자의 로컬 시간대로 결정됩니다. 이 시나리오의 계산된 날짜 필드 결과는 UTC를 기반으로 계산됩니다.

자세한 내용은 [시간대 작업](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## 사용자 지정 양식 개선 사항: Adobe XD 및 빠른 필터

사용자의 피드백을 기반으로 사용자 지정 양식을 관리할 때 경험을 개선하기 위해 다음과 같은 개선 사항이 도입되었습니다.

* Adobe XD 파일을 추가하여 사용자 지정 양식을 보다 시각적이고 유용한 방식으로 만들 수 있습니다. 양식이 개체에 첨부된 경우 개체를 사용하여 작업하는 사용자는 양식 내에서 XD 파일을 보고 상호 작용할 수 있습니다.

   자세한 내용은 [사용자 지정 양식에서 이미지 또는 기타 자산 위젯을 추가하거나 편집합니다](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* 빠른 필터 를 사용하여 현대화된 사용자 지정 양식 및 필드 목록에서 항목을 쉽게 찾을 수 있습니다. 또한 양식 및 필드를 관리할 때 모양과 느낌을 향상시킬 수 있습니다.

   빠른 필터에 대한 자세한 내용은 [목록에 빠른 필터 적용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## 공개 베타 - 프로젝트, 작업 및 문제에 대한 새로운 필터 환경

프로젝트, 작업 및 문제 목록의 필터링은 필터를 신속하게 만들고 공유할 수 있도록 다시 디자인되었습니다. 기능은 다음과 같습니다.

* 새로운 필터를 만드는 직관적인 &quot;베타 빌더&quot; 인터페이스

* 필터를 즐겨찾기로 표시 기능

* 필터 스택(저장된 필터를 두 개 이상 적용)

* 필터 복제

* 공유 필터

* 공유된 필터 제거


새 필터 경험은 작업표 목록 및 시나리오 플래너에서도 사용할 수 있습니다.

텍스트 모드는 고급 필터 편집에 사용할 수 있으며 시스템 관리자는 레이아웃 템플릿을 통해 모든 사용자에 대한 기본 필터를 할당할 수 있습니다.

### 이 기능은 어디에서 사용할 수 있습니까?

* 프로젝트/작업/문제 목록

* 시나리오 플래너

* 타임시트


### 피드백을 원합니다!

이 공개 베타 사용자는 피드백 버튼을 클릭하여 필터 환경에서 작업하는 팀에 직접 피드백을 제출할 수 있습니다. 공개 베타에서 새로운 필터 경험에 대한 사용자와 사용자의 의견을 듣기를 기대합니다. 추가 피드백을 제공하기 위해 제품을 직접 만나려면 여기에서 모임을 예약할 수 있습니다. https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### 다음은 무엇입니까?

* 새로운 그룹화 및 보기(열이라고도 함) 경험

   그룹화 및 보기(열이라고도 함)에 대한 새로운 경험에 대해 작업하기 시작하므로 새로운 필터 경험과 일치하고 새로운 필터 경험과 동일한 우수한 기능 중 일부를 제공합니다.

* Adobe Workfront의 다른 영역에서 새 필터 구현

   Adobe는 제품 전체에서 팀과 협력하여 Workfront의 다른 영역에서 새 필터 경험을 구현합니다.


Adobe는 새로운 경험과 다른 영역이 준비되는 대로 앞으로도 계속 전달할 수 있도록 고객에게 가치를 전달하려고 합니다. 더 흥미로운 업데이트를 위해 채널을 고정하세요.

자세한 내용은 [Adobe Workfront의 필터 개요](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) 및 [Adobe Workfront에서 필터 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[이 기능에 대한 비디오 데모를 봅니다.](https://video.tv.adobe.com/v/3412391/)
