---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: 에서 승인 결정 옵션을 구성합니다. [!DNL Workfront Proof]
description: 로서의 [!DNL Workfront Proof] 관리자는 Select 또는 Premium 편집 계획을 사용하여 만든 모든 증명에 대해 다음과 같은 방법으로 승인 결정 옵션을 구성할 수 있습니다 [!DNL Workfront Proof] 조직의 사용자 - 나를 편집합니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# 에서 승인 결정 옵션을 구성합니다. [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

로서의 [!DNL Workfront Proof] 관리자는 Select 또는 Premium 편집 계획을 사용하여 만든 모든 증명에 대해 다음과 같은 방법으로 승인 결정 옵션을 구성할 수 있습니다 [!DNL Workfront Proof] 조직의 사용자:

* 결정 이름 변경
* 언어 교정 뷰어에 표시되는 결정 순서를 변경합니다
* 표시할 결정을 결정합니다

이 문서에서는 다음 사항에 대해 설명합니다.

## 결정 설정 구성

1. 클릭 **[!UICONTROL 계정 설정]**.
1. 를 엽니다. **[!UICONTROL 결정]** 탭.
1. 다음 중 하나를 변경합니다.

   * 결정을 숨기려면 **[!UICONTROL 숨기기]** 당신이 필요하지 않은 결정권에.
   * 결정 이름을 변경하려면 결정 이름을 클릭하고 편집한 다음 상자 외부를 클릭하거나 Enter 키를 누릅니다. [!DNL Workfront Proof] 시스템의 모든 기존 증명에 대한 결정 이름을 업데이트합니다.

      >[!IMPORTANT]
      >
      >이름을 바꿀 때 결정에 대한 논리를 유지합니다. 예를 들어 기본 결정 &quot;거부됨&quot;을 &quot;새 버전 필요&quot;로 변경할 수 있지만 &quot;프린터로 보내기&quot;로 변경해서는 안 됩니다.

      다시 로 돌아가려면 [!DNL Workfront Proof] 기본값을 사용하여 기본 결정 복원을 클릭할 수 있습니다.

>[!NOTE]
>
>* 결정 뒤의 로직은 다양한 수준에 대한 여러 결정이 있는 경우 증명 워크플로우의 전체 상태를 계산하는 데 사용됩니다.
>* 결정 &quot;승인됨&quot; 및 &quot;변경 내용으로 승인됨&quot;은 자동 워크플로우에서 다음 단계를 트리거합니다.
>* 의사 결정 이름을 변경하고 논리를 확인하려면 **[!UICONTROL 활동]** 왼쪽 탐색 패널에서 원래 의사 결정이 대괄호로 표시되는 활동 로그를 선택합니다.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## 결정 사유 생성

의사 결정 이유는 증명에 대한 추가 의사 결정 정보를 캡처하는 좋은 방법입니다.

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**.

1. 를 엽니다. **[!UICONTROL 결정]** 탭.
기본적으로, 증명을 통해 모든 의사 결정권자가 이유를 사용할 수 있지만, 주요 의사 결정권자만 제한할 수 있습니다.
요구 사항에 따라 여러 이유를 선택하거나 단일 선택 목록으로 만들 수 있습니다. 권장 사항을 만들 수도 있습니다. 이는 검토자가 증명에 대한 결정을 저장하기 전에 이유를 선택해야 함을 의미합니다.
   ![Reasons_setup.png](assets/reasons-setup-350x121.png)

1. 에서 **[!UICONTROL 이유]** 섹션을 클릭합니다. **[!UICONTROL 새로운 이유]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. 아래에 표시되는 상자에 이유 섹션의 제목을 입력합니다 **[!UICONTROL 이유]**.
1. 텍스트 상자를 포함하려면 **[!UICONTROL 텍스트 상자 포함]**.
1. **[!UICONTROL 저장]**을 클릭합니다.
   ![re이유_setup_2.png](assets/reasons-setup-2-350x146.png)
가장 중요한 단계는 사유를 표시해야 하는 결정을 선택하는 것입니다. 여러분이 그것을 하는 것을 잊는다면, 그 이유는 여러분의 증명에 표시되지 않을 것입니다.

1. 에서 상자를 선택합니다. **[!UICONTROL 표시 이유]** 열(열)을 클릭하여 제품에서 사용할 수 있습니다. 사용자의 이유로 하나 이상의 결정을 선택할 수 있습니다.
   ![이유_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## 게시물 결정 메시지 만들기

검토자가 증명에 결정을 저장한 후에 표시할 게시물 결정 메시지를 만들 수 있습니다.

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**.

1. 를 엽니다. **[!UICONTROL 결정]** 탭.
1. 에서 **[!UICONTROL 의사 결정 메시지 게시]** 섹션을 클릭합니다. **[!UICONTROL 편집]** 의 끝 **[!UICONTROL 메시지]** 행을 클릭합니다.
또한 메시지를 모든 의사 결정권자에게 표시할지 또는 기본 의사 결정자로 제한할지 여부를 결정할 수 있습니다.
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. 에서 **[!UICONTROL 메시지 표시]** 열에서 이 메시지가 표시되어야 하는 결정을 지정합니다.
결정을 선택하지 않으면 증명에 메시지가 표시되지 않습니다. 이 열에 있는 하나 이상의 상자를 선택해야 합니다.
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
