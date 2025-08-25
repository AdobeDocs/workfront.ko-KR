---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 환경 프로모션 FAQ
description: Workfront 환경 프로모션과 관련하여 자주 묻는 질문을 살펴보십시오.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 2%

---

# 환경 프로모션 FAQ

다음은 환경 프로모션과 관련하여 자주 묻는 질문입니다.

## 도메인 간 승격이 지원됩니까?

### 답변

도메인 간 환경 프로모션은 현재 지원되지 않습니다. 동일한 도메인에 있는 환경 간에 프로모션해야 합니다.—>

<!--DELETE THIS SECTION MARCH 2026-->

<!--## Is the Adobe Business Platform / IMS a prerequisite for environment promotion?

### Answer

No. Environment Promotion is available for both IMS-enabled and non-IMS Workfront instances.-->

## Workfront 인스턴스가 Prime 또는 Ultimate 라이선스에 있는지 어떻게 확인할 수 있습니까?

### 답변

* Workfront 관리자는 조직의 라이선스를 찾을 수 있습니다.

   1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
   1. 왼쪽 패널에서 **시스템** 클릭
   1. Workfront 플랜을 보려면 **라이선스**&#x200B;를 선택하세요.
플랜이 페이지의 오른쪽 상단 근처에 표시됩니다.
      ![계획 찾기](assets/locate-plan.png)

  또는
* Workfront 계정 담당자에게 문의하십시오.

## 환경 프로모션이 양방향입니까?

### 답변

예. 예를 들어 Sandox에서 프로덕션으로 승격하거나 프로덕션에서 샌드박스로 승격할 수 있습니다.

## 공유가 지원됩니까?

### 답변

아니요. 현재 공유가 지원되지 않습니다.

## 패키지 롤백을 사용할 수 있습니까?

### 답변

패키지 롤백은 패키지 설치 후 24시간 이내에 최신 패키지에 대해 사용할 수 있습니다.

## 개별 구성 요소의 프로모션을 건너뛸 수 있는 옵션이 있습니까? `Use Existing`, `Overwrite` 및 `Save with a new Name`&quot; 옵션이 있는 경우 개별 매개 변수의 프로모션을 건너뛸 수 있도록 `Skip`을(를) 추가할 수 있습니까?

### 답변

* &quot;기존 사용&quot;은 대상 환경의 기존 오브젝트에 매핑되고 변경을 수행하지 않으므로 &quot;건너뛰기&quot; 또는 배포를 무시하는 것과 동일합니다.
* 오브젝트를 건너뛰려면 프로모션 패키지나 소스 환경에서 직접 설치하지 않으려는 오브젝트를 제거하는 것이 좋습니다. 개체를 제거한 후 패키지를 다시 어셈블합니다.
