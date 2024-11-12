---
title: Workfront Planning 레코드 자동화를 사용하여 Workfront 객체 생성
description: 활성화되면 Workfront에서 개체를 만들도록 Workfront Planning에서 자동화를 구성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: bac3ed2a169e070b541192ab312d4fc1a1b467d1
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# Workfront Planning 레코드 자동화를 사용하여 Workfront 객체 생성

활성화되면 Workfront에서 개체를 만들도록 Workfront Planning에서 자동화를 구성할 수 있습니다.

레코드에서 자동화를 활성화합니다. Workfront의 개체는 자동화를 활성화한 Planning 레코드에 연결됩니다.

예를 들어, Workfront Planning 캠페인을 가져와 Workfront에서 프로젝트를 생성하여 해당 캠페인의 진행 상황을 추적하는 자동화를 만들 수 있습니다. 이 프로젝트는 Workfront 계획 캠페인에 연결됩니다.

연결된 레코드에 대한 자세한 내용은 [연결된 레코드 개요](/help/quicksilver/planning/records/connected-records-overview.md)를 참조하십시오.


## Workfront Planning에서 자동화 구성

자동화를 사용하여 Workfront 개체를 만들려면 먼저 Workfront Planning에서 자동화를 구성해야 합니다.

1. **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭하고 **자동화**&#x200B;를 선택합니다.

   사용 가능한 자동화 목록이 열립니다.

1. 화면 오른쪽 상단의 **새 자동화 만들기**&#x200B;를 클릭합니다.
1. **단추 텍스트** 필드에 단추에 표시할 텍스트를 입력합니다. 자동화를 사용하여 Workfront 개체를 만들 때 이 단추를 클릭합니다.
1. (선택 사항) 버튼에 아이콘을 추가하려면 사용 가능한 옵션에서 아이콘을 선택합니다.
1. **형식 만들기** 필드에서 자동화를 만들 개체를 선택합니다.

   사용 가능한 객체는 다음과 같습니다.

   * 프로젝트
   * Portfolio
   * 프로그램
   * 그룹

1. **프로젝트 이름에 사용할 필드 선택** 필드에서 레코드 필드를 선택합니다. Workfront의 새 프로젝트 이름에는 이 필드의 내용이 포함됩니다.
1. **생성된 프로젝트를 다시 연결할 필드 선택** 필드에서 레코드 필드를 선택합니다. Workfront Planning에서 레코드를 볼 때 Workfront의 새 프로젝트가 이 필드에 나타납니다.
1. 생성 중인 객체 유형에 사용할 수 있는 다른 옵션을 선택합니다.
1. **만들기** 클릭

자동화는 자동화 목록에 표시되며 레코드에서 사용할 수 있습니다.

## Workfront Planning 자동화를 사용하여 Workfront 개체 만들기

1. Workfront Planning에서 Workfront 객체를 생성하는 데 사용할 레코드가 포함된 레코드 유형 페이지를 엽니다.
1. 하나 이상의 레코드를 선택합니다.
1. 화면 오른쪽 아래 모서리에 있는 자동화 버튼을 클릭합니다.

   이 예에서는 프로젝트 만들기 버튼입니다.

   ![자동화 단추](assets/automation-custom-button.png)

>[!NOTE]
>
>개체가 예상대로 만들어지고 연결되었는지 확인하는 것이 좋습니다.
