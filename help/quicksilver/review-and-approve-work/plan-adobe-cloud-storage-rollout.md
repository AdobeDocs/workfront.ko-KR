---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Adobe 클라우드 스토리지 롤아웃 계획
description: Adobe 클라우드 스토리지가 사용자에게 표시되는 방식을 선택하고, 단일 그룹으로 테스트하고, 검토자, 승인자 및 프로젝트 소유자에게 놀라운 일이 없도록 작업 순서를 지정합니다.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# Adobe 클라우드 스토리지 롤아웃 계획

Adobe 클라우드 스토리지가 사용자에게 도달하는 방법과 시기를 결정합니다. Workfront 관리자가 Adobe 클라우드 스토리지를 설정 영역의 기본 스토리지 옵션으로 설정할 때까지 아무것도 변경되지 않으므로 누구나 작업하기 전에 경험을 테스트하고 팀을 준비할 시간이 있습니다.

이 문서에서는 선택할 수 있는 롤아웃 구성, 단일 그룹으로 테스트하는 방법 및 제안된 작업 순서를 다룹니다.

## Adobe 클라우드 스토리지 롤아웃 방법 선택

구성은 두 가지가 있으며, 하나를 조직 전체 또는 특정 Workfront 그룹에 적용할 수 있습니다. Adobe 클라우드 스토리지에서 생성된 모든 프로젝트는 기본적으로 통합 승인 및 Frame.io 뷰어를 사용합니다.

단계별 지침은 [조직에 Adobe 클라우드 저장소 사용](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)을 참조하십시오.

### 구성 옵션

* **Adobe 클라우드 저장소만**: 새 프로젝트는 기본적으로 Adobe 클라우드 저장소를 사용합니다. 사용자가 레거시 프로젝트를 만들 수 없습니다.
* **Adobe 클라우드 저장소 및 레거시 Workfront 저장소**: 사용자가 프로젝트를 만들 때 Adobe 클라우드 저장소(&quot;새 프로젝트&quot;로 표시)와 레거시 Workfront 저장소(&quot;레거시 저장소&quot;로 표시) 중에서 선택합니다. 이 옵션은 설정 영역에서 **사용자가 저장소 공급자를 선택할 수 있도록 허용** 확인란을 선택하여 사용할 수 있습니다.

>[!TIP]
>
>먼저 Adobe 클라우드 스토리지를 더 작은 팀 앞에 배치하려면 단일 Workfront 그룹에 구성 중 하나를 적용하십시오. 이렇게 하면 더 광범위하게 롤아웃하기 전에 타깃팅된 파일럿을 실행할 수 있습니다. 제어된 게재 간격에 대한 그룹 수준 롤아웃으로 시작한 다음 파일럿 그룹이 경험의 유효성을 검사하면 전체 조직으로 확장하는 것이 좋습니다.

기존 객체는 생성된 스토리지 모델을 유지합니다. 기본 저장소 기본 설정을 변경해도 기존 개체는 변경되지 않습니다.

![설정의 저장소 환경 설정](assets/storage-preference-groups.png)

## 롤아웃 계획

모든 Workfront 환경은 다릅니다. Adobe 클라우드 스토리지를 사용자의 기본값으로 설정하기 전에 시간을 내어 조직에 성공적인 롤아웃이 어떻게 표시되는지 계획하십시오. 아래의 제안은 정확한 체크리스트가 아니라, 자신의 플랜에 대한 시작점이다.

### 파일럿 그룹 선택

그룹 범위 롤아웃을 사용하면 Adobe 클라우드 스토리지를 더 작은 팀 앞에 먼저 배치하고 피드백을 수집한 다음 더 넓은 롤아웃 전에 조정할 수 있습니다. 초기에 알고 싶은 문제를 표시할 수 있을 만큼 작업 패턴이 대표적인 그룹을 선택하십시오.

<!--
>[!IMPORTANT]
>
>Only members of the pilot group can convert an Adobe cloud storage object, such as a request or a task, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."
-->

### 시작하기 전에 테스트

Adobe 클라우드 스토리지는 Workfront 샌드박스 환경에서 사용할 수 있으므로 프로덕션 전에 많은 경험을 확인할 수 있습니다. Frame.io 뷰어는 샌드박스에서 사용할 수 없으므로 파일럿 그룹을 사용하여 프로덕션에서 전체 검토 및 승인 환경을 확인합니다. 자세한 내용은 [조직에 Adobe 클라우드 저장소 사용](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)을 참조하세요.

### 최종 사용자에게 변경 사항 전달

검토자, 승인자 및 프로젝트 소유자에게 표시되는 가장 큰 변경 사항은 Adobe 클라우드 스토리지 프로젝트에 대한 검토 및 승인을 지원하는 새 문서 영역 및 Frame.io 뷰어입니다. 사용자가 첫 번째 Adobe 클라우드 스토리지 프로젝트를 접했을 때 예상되는 결과를 알 수 있도록 이러한 사항을 도입하는 방법을 계획합니다. [통합 검토 및 승인 시작](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) 문서는 최종 사용자 대면 자료에 유용한 시작점입니다.

### 권한 및 거버넌스 검토

Adobe 클라우드 스토리지 프로젝트에서 [관리] 및 [기여]는 모두 외부 공유를 포함하는 Frame.io의 [편집 및 공유]에 매핑됩니다. 팀을 Adobe 클라우드 스토리지로 가져오기 전에 공유 패턴을 검토하고 거버넌스 모델에 적합한지 여부를 결정하십시오. 자세한 내용은 [Adobe 클라우드 스토리지의 차이점](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping)을 참조하세요.

### 감사 템플릿 및 이름 지정

Adobe 클라우드 스토리지는 엄격한 이름 지정 규칙을 적용하고 Workfront은 충돌하는 객체의 이름을 자동으로 바꿉니다. 템플릿으로 프로젝트를 만드는 경우 생성되는 이름과 구조가 규칙에 맞도록 이러한 템플릿을 검토하십시오. 자세한 내용은 [Adobe 클라우드 스토리지의 차이점](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules)을 참조하세요.

### Workfront Fusion 관련 플랜

기존 증명 기반 Fusion 시나리오는 기존 프로젝트에서 계속 작동하지만, Adobe 클라우드 스토리지 프로젝트에 대해 자동으로 작동하지 않습니다. 이러한 시나리오에 의존하는 팀을 Adobe 클라우드 스토리지로 가져오기 전에 각 시나리오를 편집, 다시 빌드 또는 폐기로 분류하십시오. 자세한 내용은 [통합 검토 및 승인을 위해 Workfront Fusion 시나리오 업데이트](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)를 참조하십시오.

### 변경 사항 보고 계획

통합 승인 작업 과정 데이터 및 보고가 캔버스 대시보드에 표시됩니다. 기존 승인 보고서는 자동으로 이전되지 않으므로 파일럿 팀이 사용하기 전에 대체 대시보드를 설정하십시오. 자세한 내용은 [검토 및 승인을 위한 보고서 대시보드 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)를 참조하세요.

## 제안된 시퀀스

이 순서를 사용자 환경에 맞게 조정하여 템플릿으로 사용합니다.

1. 샌드박스와 프로덕션의 파일럿 그룹으로 경험을 테스트합니다.
2. Fusion 시나리오를 분류 및 업데이트하고 캔버스 대시보드 보고를 빌드합니다.
3. 템플릿을 감사하고 권한 및 공유 모델을 검토하십시오.
4. 변경 내용을 사용할 검토자, 승인자 및 프로젝트 소유자에게 전달합니다.
5. Adobe 클라우드 스토리지를 파일럿 그룹의 기본값으로 설정한 다음 파일럿이 경험을 검증하면 더 많은 그룹 또는 전체 조직으로 확장합니다.
