---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 기본 시나리오에 트리거 모듈 추가
description: 시나리오가 정기적으로 새 요청을 검색하고 프로젝트로 변환할 수 있도록 트리거 모듈을 추가하는 방법을 알아봅니다.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# 함수를 사용하여 의 간단한 시나리오로 프로젝트 업데이트 [!DNL Adobe Workfront Fusion]

Workfront 작업 항목 업데이트는 Workfront Fusion의 일반적인 사용 사례입니다. 이 예제에서는 함수를 사용하여 프로젝트 이름을 대문자로 변경합니다.

Fusion에는 데이터에 대해 조건부 논리를 변환하고 수행할 수 있는 다양한 유형의 함수가 포함되어 있습니다. 함수 사용에 대한 자세한 내용은 [Adobe Workfront Fusion의 한 모듈에서 다른 모듈로 정보 매핑](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

이 예는에서 생성된 시나리오를 수정합니다. [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 전제 조건

에 설명된 시나리오를 만들어야 합니다. [기본 시나리오 만들기](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) 이 절차를 수행하기 전에.

## 함수를 사용하여 프로젝트 업데이트

### 시나리오에 레코드 업데이트 모듈 추가

1. 시나리오 편집기에서 시나리오를 엽니다.
1. 모듈 오른쪽에 있는 부분 원을 마우스로 가리킨 다음 을 클릭합니다 **[!UICONTROL 다른 모듈 추가]**.
1. 선택 [!DNL Adobe Workfront] 응용 프로그램 목록에서 모듈을 선택합니다 **[!UICONTROL 레코드 업데이트]**.
1. id 필드에서 Convert 개체 모듈 아래에 있는 ID 블록을 선택합니다. 해당 모듈에서 출력된 프로젝트의 ID입니다.

   ![Convert 개체의 ID](assets/id-convert-object.png)

1. 업데이트할 개체가 프로젝트이므로 레코드 유형 필드에서 프로젝트를 선택합니다.
1. 매핑할 필드 선택 영역에서 이름을 선택합니다.

   이름 필드가 열립니다.

### 이름 업데이트를 위한 함수 매핑

이 시나리오가 요청을 프로젝트로 변환할 때 프로젝트의 이름이 요청과 동일합니다. 여기서 함수는 해당 이름을 사용하고 그 안에 있는 모든 문자를 대문자로 바꿉니다.

1. 다음을 클릭합니다. **이름** 필드.

   매핑 패널이 열립니다.
1. 매핑 패널에서 **텍스트 및 이진 함수** 아이콘. ![텍스트 함수 아이콘](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. 함수 선택 **upper**.

   이 함수는 기대하는 입력에 대한 형식을 포함하여 이름 필드에 나타납니다.

   이 예제의 입력은 프로젝트가 전환된 문제의 이름입니다.

1. 입력이 진행될 위치이므로 커서를 괄호 사이로 이동합니다.
1. 매핑 패널에서 **모듈 출력** 아이콘. ![모듈 출력 아이콘](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. 첫 번째 모듈에서 출력한 이름 블록을 선택합니다.

   이름 블록이 함수에 나타납니다.

   ![함수의 이름 블록](assets/map-name.png)

1. 확인 을 클릭하여 모듈 설정을 저장합니다.

### 테스트 및 활성화

1. 다음을 클릭하여 시나리오 테스트 **한 번 실행** 화면의 왼쪽 아래에 있습니다.
1. 출력을 검사하여 시나리오가 예상대로 실행되었는지 확인합니다.
1. 시나리오가 예상대로 작동하는 경우 **예약** 화면 왼쪽 하단에서 전환 **날짜**.

   이렇게 하면 시나리오가 활성화됩니다. 활성 시나리오는 트리거 모듈에 설정된 일정에 따라 실행됩니다.
1. 위치 [!DNL Workfront Fusion], 클릭 **[!UICONTROL 저장]** 왼쪽 아래 모서리 근처에 있습니다.

   >[!IMPORTANT]
   >
   >원하는 만큼 자주 저장하고 시나리오를 테스트합니다.

## 리소스:

* [에서 함수를 사용하여 항목 매핑 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
