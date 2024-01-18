---
title: 20.4 향상된 프로젝트 관리 기능
description: 20.4 향상된 프로젝트 관리 기능
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 0%

---

# 20.4 향상된 프로젝트 관리 기능

이 페이지에서는 미리보기 환경에 대한 20.4 릴리스의 모든 프로젝트 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2020년 11월 9일이 있는 주에 프로덕션 환경에서 사용할 수 있습니다.

20.4 릴리스에서 사용할 수 있는 모든 변경 사항의 목록은 을 참조하십시오. [20.4 릴리스 개요](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 관리자용 새로운 기능: 사용자 정의 필드 공유 방법 제어

사용자가 만든 사용자 정의 필드를 편집, 삭제 및 사용할 수 있는 사용자를 보다 세밀하게 제어할 수 있도록 원하는 공유 방식을 정확하게 구성하는 기능이 추가되었습니다.

지금까지 사용자 정의 필드를 만들 때 시스템의 모든 사용자가 편집할 수 있었습니다. 여전히 사용자 정의 필드의 기본 상태이지만, 이제 사용자 정의 필드를 특정 사용자, 역할, 팀, 그룹 및 회사로 공유하는 것을 제한할 수 있습니다. 또한 수신자가 사용자 정의 필드를 관리할 수 있는지 또는 볼 수만 있는지 여부를 결정할 수 있습니다.

또한 사용자에게 친숙한 이 경험을 제공하기 위해 이 기능이 Workfront 전체에서 공유하는 다른 오브젝트 영역과 유사하도록 사용자 인터페이스를 설계했습니다.

자세한 내용은 [사용자 정의 필드 및 위젯에 대한 공유 구성](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md).

## 관리자를 위한 새로운 기능: 표준화된 사용자 정의 양식 공유

이미 알고 있는 것과 동일한 Workfront 개체 공유 프로세스를 사용할 수 있도록 사용자 지정 Forms에 대한 공유를 표준화했습니다. 또한 새로운 공유 환경을 통해 사용자가 만든 사용자 정의 Forms을 편집, 삭제 및 사용할 수 있는 사용자를 보다 세밀하게 제어할 수 있습니다. 사용자 정의 양식에 대한 공유를 특정 사용자, 역할, 팀, 그룹 및 회사로 제한할 수 있습니다. 또한 이러한 수신자가 사용자 정의 양식을 보거나 관리할 수 있는지 여부를 결정할 수 있습니다.

자세한 내용은 [사용자 정의 양식 공유](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## 프로젝트, 작업 또는 문제의 세부 정보 섹션에서 사용자 정의 양식 및 개요 정보 내보내기

이제 사용자 정의 양식 정보를 .pdf 파일로 내보낼 수 있습니다. 객체의 세부 정보 섹션에서 양식에 액세스할 때 프로젝트, 작업 또는 문제에서 사용자 정의 양식을 내보낼 수 있습니다.

이제 프로젝트, 작업 및 문제의 사용자 정의 양식을 내보낼 수 있을 뿐만 아니라 내보낸 pdf에 개요 영역을 포함할 수도 있습니다.

개체에서 사용자 정의 양식을 내보내는 방법에 대한 자세한 내용은 [사용자 정의 양식 및 개체 세부 정보 내보내기](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## 신속하게 반복 추가

>[!NOTE]
>
>이 기능은 프로덕션 환경에서 일시적으로 제거되었습니다. 기능을 사용할 수 있게 되면 이 페이지가 업데이트됩니다.

이터레이션 작성 간소화를 위해 이터레이션 탭에서 이터레이션을 추가할 수 있는 새 버튼을 추가했습니다. 여기에서 반복을 만든 다음 나중에 작업 및 문제를 추가할 수 있습니다.

이전처럼 백로그 태그에 반복을 만들 수 있습니다.

자세한 내용은 [반복 만들기](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## 프로젝트에서 사용할 수 있는 새 지표 섹션

이제 시간을 절약하고 프로젝트의 전체 상태에 대한 이해를 높이기 위해 프로젝트에서 다음 사항에 대한 정보가 포함된 지표 섹션을 사용할 수 있습니다.

* 완료, 미완료, 기한 초과 및 예정된 작업
* 상태 또는 우선 순위별로 그룹화된 작업 및 문제 금액
* 각 사용자에게 할당된 작업 노력

차트에서 선택하여 프로젝트의 작업 및 문제의 다양한 측면을 확인하고 특정 요소를 클릭하여 작업 정보를 표시할 수 있습니다.

이 기능은 이제 [플래너 기본 사항, 3부 학습 경로](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) Workfront One.

## 관리자용 새로운 기능: 그룹에 비즈니스 리더 할당

그룹을 구성하고 정의하는 데 도움이 되도록 사용자를 그룹(또는 하위 그룹)에 대한 비즈니스 리더로 할당하는 기능을 추가했습니다. 비즈니스 리더는 그룹에 대한 비즈니스 결정을 내리는 Workfront 사용자입니다.

새 비즈니스 리더 필드는 보고서 필터, 보기 및 그룹화에 사용할 수 있습니다. 예를 들어 특정 비즈니스 리더를 기준으로 필터링하여 해당 역할에 할당된 그룹만 나열할 수 있습니다.

자세한 내용은 [비즈니스 리더 개요](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

이 기능은 이제 [관리자 기본 사항, 1부 학습 경로](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront One.

## 관리자를 위한 새로운 기능: 포트폴리오, 프로그램 및 회사를 그룹과 연결

Workfront 관리자는 포트폴리오, 프로그램 또는 회사를 만들거나 편집할 때 그룹에 지정할 수 있습니다. 이러한 객체에 그룹을 할당하면 그룹에 대한 책임을 쉽게 식별할 수 있습니다.

예를 들어 보고서에 조직의 모든 포트폴리오를 나열하고 그룹 열을 확인하여 그룹에서 작업 중인 포트폴리오를 확인할 수 있습니다.

자세한 내용은 문서의 &quot;그룹과 객체 연관 정보&quot; 섹션을 참조하십시오 [그룹 개요](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

이 기능은 이제 [관리자 기본 사항, 1부 학습 경로](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront One.

## 관리자용 새로운 기능: 회사에 할당된 그룹의 관리자가 회사를 관리할 수 있음

그룹 관리자가 Workfront에서 해당 그룹과 연결된 회사를 쉽게 관리할 수 있도록 했습니다. 회사를 관리할 수 있는 액세스는 연결이 이루어지면 자동으로 사용할 수 있습니다. 이는 그룹 관리자가 회사에 대한 관리 액세스 권한이 없는 경우에 특히 중요합니다.

자세한 내용은 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

회사에 대한 관리 액세스에 대한 자세한 내용은 [사용자에게 특정 영역에 대한 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

이 기능은 이제 [관리자 기본 사항, 1부 학습 경로](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront One.

## 처리 중 단추를 시작 단추로 바꾸기

작업 항목에서 실제로 작업이 시작되는 날짜와 시간을 캡처하기 위해 사용자는 처리 중 단추를 작업 항목의 상태 및 실제 시작 날짜를 자동으로 업데이트하는 시작 단추로 바꿀 수 있습니다.

9월 24일 업데이트됨: 작업 시작 또는 문제 시작을 클릭한 후 선택 사항을 되돌려 실행 취소를 클릭하여 작업 항목에서 작업을 시작할 준비가 되지 않았을 수 있음을 표시할 수 있는 옵션이 제공됩니다. 작업 항목이 신규 상태로 돌아가고 커밋 일자 및 실제 시작 일자가 삭제됩니다. 실행 취소 옵션은 매우 짧은 시간 동안 표시되며 페이지를 다른 곳으로 이동하거나 새로 고친 후에는 지워집니다.

이 옵션 구성에 대한 자세한 내용은 [처리 중 단추를 시작 단추로 바꾸기](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

이 기능은 이제 [작업자 기초 학습 경로](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) 및 [관리자 기본 사항, 1부 학습 경로](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront One.

## 대기열 주제에 대해 여러 초안 허용

요청 작업 시 보다 자유롭게 작업할 수 있도록 하기 위해 하나의 대기열 주제에 대해 저장할 수 있는 초안 수에 대한 제한이 더 이상 없습니다. 새 요청을 만들 때 동일한 대기열 주제에 대한 초안 목록에서 기존 초안을 선택하여 덮어쓴 후 새 요청으로 제출하거나 새 요청을 처음부터 만들 수 있습니다.

이 개선 이전에는 Workfront에서 요청 대기열의 각 대기열 주제에 대해 초안을 하나만 저장했습니다.

요청 제출에 대한 자세한 내용은 &quot; [Workfront 요청 만들기 및 제출](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## 팀에 그룹 할당

이제 그룹과 연결된 팀을 더 쉽게 관리하고 보고하기 위해, 편집할 수 있는 액세스 권한이 있는 팀에 모든 그룹을 할당할 수 있습니다.

그룹에 팀을 할당하면 그룹 관리자는 해당 그룹의 구성원이 되지 않고도 팀을 관리할 수 있습니다. 팀 세부 정보 페이지에서 자신이 관리하는 그룹에 할당된 팀을 볼 수 있습니다. 또한 보고서를 실행하여 특정 그룹과 연결된 모든 팀을 나열할 수 있습니다.

자세한 내용은 [팀 만들기](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

이 기능은 이제 [관리자 기본 사항, 1부 학습 경로](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront One.

## 새 필드를 사용하면 최상위 수준 그룹 및 모든 하위 그룹의 데이터에 대해 보고할 수 있습니다

최상위 그룹 및 그 하위 그룹과 관련된 데이터를 식별하는 데 도움이 되도록 그룹 개체에 대한 보고서를 만들 때 필터, 보기 및 그룹화에 사용할 수 있는 새로운 최상위 ID 필드를 추가했습니다.

이 필드는 여러 하위 그룹을 포함하는 그룹을 관리하는 그룹 관리자에게 특히 유용합니다.

예를 들어 하위 그룹 필드 마케팅 및 디지털 마케팅이 있는 마케팅 그룹을 관리한다고 가정해 보겠습니다. 다음 필터 규칙이 있는 프로젝트 영역 필터를 만들어 3개의 그룹 모두에 속하는 프로젝트를 나열할 수 있습니다.
<pre>그룹: 상위 이름 &gt; 같음 &gt; 마케팅</pre>또한 필터 또는 그룹화가 아닌 보기에서 최상위 그룹과 관련된 데이터를 식별하는 데 사용할 수 있는 새 최상위 이름 필드를 추가했습니다.

목록 및 보고서에서 필드를 사용하는 방법에 대한 자세한 내용은 [Adobe Workfront 용어 목록](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## 요청 초안을 삭제할 때 작업을 취소하는 새로운 옵션

이제 저장된 초안을 삭제할 때 초안이 삭제됨을 알리는 확인 메시지에서 취소 를 클릭할 수 있습니다. 이렇게 하면 초안을 버리려고 마음이 바뀌어도 잃어버리지 않는다.

이 기능은 새로운 Workfront 환경에서만 사용할 수 있습니다. 자세한 내용은 [Workfront 요청 만들기 및 제출](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

