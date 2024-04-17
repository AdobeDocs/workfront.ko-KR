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
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 환경 프로모션 패키지 설치

>[!NOTE]
>
>패키지를 설치하려면 패키지를 설치할 환경에 로그인해야 합니다. 이 환경은 개체를 복사하는 환경입니다 **끝**.

1. 패키지를 설치할 환경으로 이동합니다.
1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png).
1. 선택 **시스템** 왼쪽 탐색에서 을(를) 선택합니다. **환경 프로모션**.
1. 표시된 목록에서 패키지를 선택합니다.
1. 충돌이 있는 각 개체에 대해 충돌 해결 방법을 선택합니다.

   충돌을 해결하려면 객체 유형 옆의 드롭다운 화살표를 클릭하고 수행할 작업을 선택합니다.

   자세한 내용은 [충돌](#collisions) 이 문서에서
1. 패키지를 새 환경에 배포하려면 **배포** 화면 오른쪽 상단에 있습니다.

## 충돌

설치 패키지의 일부인 객체가 대상 환경에 이미 있을 때 충돌이 발생합니다. 이 경우 충돌 해결 방법을 선택할 수 있습니다. 충돌은 객체 레벨에서 해결됩니다.

각 객체 유형 옆에 있는 드롭다운을 클릭하여 충돌을 볼 수 있습니다. 충돌은 충돌(Collision) 열에 표시됩니다.

충돌을 해결하려면 배포 작업 열에서 작업을 선택하거나 이미 표시된 기본 작업을 사용합니다.

* **새 이름으로 만들기**: 대상 환경에서 새 개체를 만듭니다. 객체가 대상 환경에 존재하면 새 이름으로 새 객체를 작성할 수 있습니다. 대상 환경에 없는 경우 새 이름으로 개체를 만들거나 개체가 패키지에 있는 이름으로 개체를 만들 수 있습니다.
* **기존 항목 사용**: 패키지의 개체가 설치되지 않았으며 대상 환경에 이미 있던 개체가 변경되지 않았습니다.
* **덮어쓰기**: 패키지의 개체가 대상 환경의 기존 개체를 대체합니다.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

기본값은 입니다. `Create new` 객체가 대상 환경에 없는 경우 `Use existing` 객체가 대상 환경에 있는 경우 을 클릭하여 기본 매핑으로 되돌릴 수 있습니다. **기본 매핑으로 재설정**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
