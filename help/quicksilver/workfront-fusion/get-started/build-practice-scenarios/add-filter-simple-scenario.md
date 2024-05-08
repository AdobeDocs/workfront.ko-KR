---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 기본 시나리오에 필터 추가
description: 필터를 사용하면 특정 조건이 충족되는 경우에만 시나리오가 진행되도록 할 수 있습니다.
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# 의 기본 시나리오에 필터 추가 [!DNL Adobe Workfront Fusion]

필터를 사용하면 특정 조건이 충족되는 경우에만 시나리오가 진행되도록 할 수 있습니다.

이 예제에서는 요청이 특정 요청 대기열에 제출된 경우에만 요청에서 새 프로젝트를 만들 수 있도록 하는 필터를 시나리오에 추가합니다.

이 예는에서 생성된 시나리오를 수정합니다. [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront 트리거 모듈에는 특정 조건이 충족되는 경우에만 시나리오를 시작할 수 있도록 하는 필터가 포함됩니다. 그러나 모듈간 필터는 트리거가 아닌 모든 및 Workfront이 아닌 사용 사례에 사용되므로 모듈 간에 필터를 사용하는 방법을 알아보는 것이 중요합니다. 이 예제에서는 모듈 내 필터에서 충족할 수 있는 기능을 위해 모듈 간 필터를 사용합니다.

## 전제 조건

에 설명된 시나리오를 만들어야 합니다. [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) 이 절차를 수행하기 전에.

## 필터 추가

### 필터 추가 준비

1. 첫 번째 시나리오를 엽니다.
1. 다음에서 **출력** 영역, 선택 `Project`.
이제 다음을 수행해야 합니다. `ID`, `Name`, 및 `Project` 선택됨.
1. 확인 을 클릭하여 모듈 설정을 저장합니다.
1. Workfront을 엽니다.
1. Workfront에서 Fusion 시나리오가 작동할 요청 대기열을 나타내는 프로젝트를 찾습니다.

   이 프로젝트는 Fusion 연결이 설정된 Workfront 계정과 동일한 계정에 있어야 합니다.

1. URL에 프로젝트 ID를 기록합니다.

   예: https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### 필터 추가 및 구성

1. 시나리오 편집기에서 시나리오를 엽니다.
1. 렌치 아이콘 클릭 ![렌치 아이콘](assets/wrench-icon.png) 첫 번째 모듈과 두 번째 모듈 사이에서 **필터 설정**.
1. 레이블 필드에 &quot;요청 대기열에 대한 필터&quot;와 같은 이 필터의 레이블을 입력합니다.
1. 다음에서 **조건** 영역, 맨 위 필드에서 `projectID` 첫 번째 모듈에서

   ![프로젝트 ID 매핑](assets/map-proj-id.png)
1. 나가기 **조건** 같음 연산자입니다.
1. 의 맨 아래 필드에서 **조건** 영역, 의 프로젝트 URL에서 기록한 프로젝트 ID에 붙여 넣습니다. [필터 추가 준비](#prepare-to-add-the-filter).
1. 클릭 **확인** 필터 설정을 저장합니다.

### 테스트 및 활성화

1. Fusion이 연결 중인 Workfront 환경으로 이동하여 필터에 지정한 프로젝트에 문제를 추가합니다. 다른 프로젝트에 다른 문제를 추가합니다.
1. 클릭 **[!UICONTROL 한 번 실행]** (시나리오 편집기의 왼쪽 아래 모서리)를 참조하십시오.
1. 출력을 검사하여 시나리오가 예상대로 실행되었는지 확인합니다.

   두 문제는 모두 첫 번째 시나리오의 출력에 표시되어야 하지만 지정된 프로젝트의 문제만 두 번째 시나리오의 입력으로 표시되어야 합니다.
1. 시나리오가 예상대로 작동하는 경우 **예약** 화면 왼쪽 하단에서 전환 **날짜**.

   이렇게 하면 시나리오가 활성화됩니다.
1. 위치 [!DNL Workfront Fusion], 클릭 **[!UICONTROL 저장]** 왼쪽 아래 모서리 근처에 있습니다.

   >[!IMPORTANT]
   >
   >원하는 만큼 자주 저장하고 시나리오를 테스트합니다.

## 리소스

* 필터에 대한 자세한 내용은 [시나리오에 필터 추가](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

