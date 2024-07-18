---
title: AI Assistant를 사용하여 계산된 필드 공식 개정
content-type: reference
description: AI Assistant를 사용하여 계산된 필드에서 잘못된 사용자 정의 표현식의 오류를 해결할 수 있습니다.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# AI Assistant를 사용하여 계산된 필드 공식 개정

AI Assistant를 사용하여 계산된 필드에서 잘못된 사용자 정의 표현식의 오류를 해결할 수 있습니다.

사용자 정의 양식 빌더에서 계산된 필드를 만들 때 공식이 잘못된 경우 필드 아래에 오류 메시지가 표시됩니다.

![잘못된 식 오류](assets/invalid-expression.png)

AI 도우미는 공식을 유효한 계산된 필드 표현식으로 수정하는 데 도움이 될 수 있습니다.

## 계산된 필드 표현식 수정

잘못된 계산된 필드 표현식을 수정하려면 다음을 수행합니다.

1. 화면 오른쪽 상단 근처에 있는 **AI Assistant** 아이콘 ![AI Assistant 아이콘](assets/ai-assistant-icon.png)을 클릭합니다.
1. ai Assistant 패널 하단 근처에 있는 프롬프트 영역에서 다음과 같은 프롬프트를 입력합니다.
   `Rewrite this formula to remove the invalid expression error`
1. 사용자 정의 양식 빌더에서 잘못된 표현식을 복사하여 프롬프트 영역에 붙여넣습니다.
1. **Enter**&#x200B;를 누릅니다.

   공식의 크기나 복잡성에 따라 AI 도우미가 수정된 공식을 생성하는 데 약간의 시간이 걸릴 수 있습니다.
1. AI 지원 패널에서 수정된 공식을 확인합니다.
1. (선택 사항) AI 지원 패널에서 수정된 공식을 복사하여 사용자 정의 양식 빌더의 계산된 필드에 붙여넣습니다.

>[!NOTE]
>
>예상 결과를 검색하는지 확인하려면 계산된 필드를 테스트하는 것이 좋습니다.

Workfront의 계산된 필드에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.
