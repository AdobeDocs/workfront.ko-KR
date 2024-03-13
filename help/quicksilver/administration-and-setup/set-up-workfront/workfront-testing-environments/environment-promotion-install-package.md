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
source-git-commit: 690dda5bfc0ac77d396532ff7cfce38f4b61f4af
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# 환경 프로모션 패키지 설치

이 페이지는 작성 중입니다.



1. 패키지를 설치할 환경으로 이동합니다. 객체를 복사하는 환경입니다 **끝**.
1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png).
1. 선택 **시스템** 왼쪽 탐색에서 을(를) 선택합니다. **환경 프로모션**.
1. 표시된 목록에서 패키지를 선택합니다.
1. 패키지를 설치하려면 **설치** 화면 오른쪽 상단에 있습니다.
1. 패키지의 각 개체를 대상 환경의 해당 개체에 매핑합니다.

   자세한 내용은 [매핑](#mapping) 이 문서에서


## 매핑

각 객체 유형은 왼쪽 탐색 및 카드에 나열됩니다. 카드에는 해당 유형의 객체와 해당 객체가 대상 환경에 있는지 여부가 표시됩니다. 이러한 객체가 대상 환경으로 이동하는 방법을 결정할 수 있습니다.

* 새로 만들기: 개체가 대상 환경에 있습니다.
* 기존 사용: 패키지의 객체가 설치되지 않고 대상 환경에 이미 존재하는 객체가 변경되지 않습니다.
* 기존 덮어쓰기: 패키지의 객체가 대상 환경의 기존 객체를 대체합니다.
* 다음을 사용하지 마십시오.

기본값은 입니다. `Create new` 객체가 대상 환경에 없는 경우 `Use existing` 객체가 대상 환경에 있는 경우 을 클릭하여 기본 매핑으로 되돌릴 수 있습니다. **기본 매핑으로 재설정**.

사용하지 않음을 선택하면 이 선택이 다른 객체 또는 필드에 어떤 영향을 미치는지 설명하는 오류 메시지가 나타납니다.

<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.
-->

