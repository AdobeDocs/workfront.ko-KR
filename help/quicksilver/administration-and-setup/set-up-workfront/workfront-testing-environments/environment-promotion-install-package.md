---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 환경 프로모션 패키지 설치
description: 환경 프로모션 기능은 구성 관련 객체를 한 환경에서 다른 환경으로 이동할 수 있는 기능을 제공하기 위한 것입니다. 대상 환경에 환경 프로모션 패키지를 설치하는 방법을 알아봅니다.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 6497bfa1bf8236baaf4beee38078426b754e1241
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# 환경 프로모션 패키지 설치

패키지를 만든 후에는 다른 환경에 설치할 수 있습니다.

## 전제 조건

패키지를 설치하려면 먼저 패키지를 생성해야 합니다.

자세한 내용은 [환경 프로모션 패키지 만들기 또는 편집](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

>[!NOTE]
>
>패키지를 설치하려면 패키지를 설치할 환경에 로그인해야 합니다. 객체를 복사하는 환경입니다 **끝**.

1. 패키지를 설치할 환경으로 이동합니다.
1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png).
1. 선택 **시스템** 왼쪽 탐색에서 을(를) 선택합니다. **환경 프로모션**.
1. 표시된 목록에서 패키지를 선택합니다.
1. 충돌이 있는 각 개체에 대해 충돌 해결 방법을 선택합니다.

   충돌을 해결하려면 객체 유형 옆에 있는 드롭다운 화살표를 클릭하고 수행할 작업을 선택합니다.

   자세한 내용은 [충돌](#collisions) 이 문서에서
1. 패키지를 새 환경에 배포하려면 **배포** 화면 오른쪽 상단에 있습니다.

## 충돌

충돌은 설치 패키지의 일부인 객체가 대상 환경에 이미 존재하는 객체와 동일한 이름을 가질 때 발생합니다. 이 경우 충돌 해결 방법을 선택할 수 있습니다. 충돌은 객체 레벨에서 해결됩니다.

각 객체 유형 옆에 있는 드롭다운을 클릭하여 충돌을 볼 수 있습니다. 충돌은 충돌(Collision) 열에 표시됩니다.

충돌을 해결하려면 배포 작업 열에서 작업을 선택하거나 이미 표시된 기본 작업을 사용합니다.

* **새 이름으로 만들기**: 대상 환경에서 새 개체를 만듭니다. 객체가 대상 환경에 존재하면 새 이름으로 새 객체를 작성할 수 있습니다. 대상 환경에 없는 경우 새 이름으로 개체를 만들거나 개체가 패키지에 있는 이름으로 개체를 만들 수 있습니다.
* **기존 항목 사용**: 패키지의 개체가 설치되지 않았으며 대상 환경에 이미 있던 개체가 변경되지 않았습니다.
* **덮어쓰기**: 패키지의 개체가 대상 환경의 기존 개체를 대체합니다.

  충돌이 감지되지 않더라도 덮어쓸 오브젝트를 선택할 수도 있습니다.

  덮어쓰기가 상위 및 하위 객체에 미치는 영향에 대한 자세한 내용은 [상위 및 하위 개체 덮어쓰기](#overwriting-parent-and-child-objects) 이 문서에서.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

기본값은 입니다. `Create new` 객체가 대상 환경에 없는 경우 `Use existing` 객체가 대상 환경에 있는 경우 을 클릭하여 기본 매핑으로 되돌릴 수 있습니다. **기본 매핑으로 재설정**.

## 상위 및 하위 개체 덮어쓰기

프로모션 패키지의 일부 오브젝트에 하위 오브젝트가 포함될 수 있습니다. 예를 들어 프로젝트(상위)에는 작업(하위)이 있습니다. 상위 객체를 덮어쓸 때 하위 객체는 다음과 같이 처리됩니다.

* 패키지와 대상 모두에 있는 하위 개체는 패키지와 일치하도록 대상에서 업데이트됩니다.
* 패키지에 있지만 대상이 아닌 하위 개체가 만들어집니다.
* 대상에 존재하지만 패키지가 아닌 하위 개체는 변경되지 않습니다.

이 기능은 다음 상위 및 하위 객체에 영향을 줍니다.

| 상위 오브젝트 | 하위 개체 |
|---|---|
| 프로젝트 | 작업<br>QueueDef(대기열 정의)<br>라우팅 규칙 |
| 템플릿 | TemplateTask<br>QueueDef(대기열 정의)<br>라우팅 규칙 |
| 매개 변수(사용자 정의 양식 필드) | ParameterOption(사용자 정의 양식 필드 옵션) |
| 캘린더 정보 | CalendarSection |
| QueueDef(대기열 정의) | 대기열 주제 그룹<br>대기열 주제 |

