---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: 을 사용하여 계정 간에 사용자 이동 [!DNL Workfront Proof]
description: 만약 [!DNL Workfront Proof] 관리자 및 주 계정에 연결된 하나 이상의 위성 계정이 있는 경우 이러한 모든 계정 간에 사용자를 이동할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# 을 사용하여 계정 간에 사용자 이동 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

만약 [!DNL Workfront] 증명 관리자 및 주 계정에 연결된 하나 이상의 위성 계정이 있는 경우 이러한 모든 계정 간에 사용자를 이동할 수 있습니다.

## 연결된 계정 간에 사용자 이동

1. 클릭 **[!UICONTROL 설정]** > **[!UICONTROL 계정 설정]**.

1. 를 엽니다. **[!UICONTROL 사용자]** 탭.
1. 을(를) 클릭합니다. **[!UICONTROL 사용자 이동]** 아이콘(1) ![Move_user2.png](assets/move-user2-350x95.png)

1. 표시되는 사용자 이동 상자에서 이동할 사용자(1)를 확인합니다.
1. 연결된 계정 목록(2)에서 대상 계정을 선택합니다.
1. 이 사용자에게 새 계정에 대해 가져야 하는 프로필 권한(3)을 할당합니다.
1. 이동하지 않을 항목의 소유권을 가져올 사용자(4)를 선택합니다.
여기에는 이전 계정에서 떠나기로 결정한 항목과 이동할 수 없는 항목이 포함됩니다(참조) [이동할 수 없는 항목](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) 아래에 표시됩니다.

1. 사용자와 함께 증명(5) 및 파일(6)을 이동하려면 확인란을 선택합니다.
1. 이동된 모든 항목이 새 계정에 배치되는 폴더(7)의 이름을 만듭니다.
1. 클릭 **[!UICONTROL 사용자 이동]** (8) 프로세스를 시작합니다.
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

증명 및 파일 없이 사용자를 이동하도록 선택하면 바로 이 작업이 수행됩니다. 교정용 및 파일과 함께 사용자를 이동하도록 선택하면 사용자의 프로필을 바로 재할당하지만 이 작업을 수행하려면 데이터를 전송하는 시간이 필요하므로 증명 및 파일이 대상 계정에 점진적으로 표시됩니다.

파일 및 증명 이동 프로세스에 따라 몇 분에서 몇 시간까지 걸릴 수 있습니다.

>[!NOTE]
>
>프로세스가 예상보다 오래 걸리거나 이동한 증명 및/또는 파일이 새 계정에 표시되지 않을 경우 지원 팀에 문의하십시오.

## 이동할 수 없는 항목

### 이동된 사용자가 생성 또는 소유한 폴더

폴더 및 해당 컨텐츠에 적용되는 다양한 권한의 특성(예: 다른 사용자 및 계정과 공유될 수 있음)으로 인해 Adobe에서는 사용자와 폴더 구조를 이동할 수 없습니다.

이동된 사용자가 폴더를 소유한 경우 &quot;사용자 이동&quot; 팝업에서 선택한 사용자(4)에게 소유권이 이전됩니다.

>[!NOTE]
>
>이동된 사용자가 폴더를 만든 경우 해당 폴더는 해당 작성자가 되므로 소유자만 이전됩니다. 폴더는 새 계정의 사이드바에서 이동한 사용자에게 계속 표시됩니다. 이동된 사용자는 이러한 폴더 내에 배치된 항목에 대해 &quot;읽기 전용&quot; 액세스를 계속 갖습니다.

이동된 사용자가 이러한 권한을 유지하지 못하게 하거나 이동된 사용자가 이전 및 계정에서 이전 폴더를 보지 않게 하려면 여기에서 해결 방법은 다음과 같이 폴더를 삭제하는 것입니다.

1. 이전 계정에 새 폴더를 만듭니다.
1. 이동한 사용자의 폴더에서 새로 만든 폴더로 모든 항목을 이동합니다.
1. 이동된 사용자가 남긴 모든 폴더를 삭제합니다.

### 다른 소유자가 있는 버전 세트

증명에 버전이 몇 개 있고 각 버전이 다른 사용자가 소유한 경우 이동된 사용자가 소유한 버전은 이동되지 않습니다. 이러한 버전의 소유권은 사용자 이동 상자에서 선택한 대로 다른 사용자에게 전달됩니다(4). (자세한 내용은 를 참조하십시오.)

>[!NOTE]
>
>이동한 사용자는 증명을 이동할 수 있도록 세트에 있는 모든 증명 버전을 소유해야 합니다.

### 그룹

이동된 사용자가 새 계정에서 그룹을 다시 만들어야 합니다. 자세한 내용은 [다음 방법으로 교정 그룹 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### 사용자 정의 보기

개인 사용자 지정 보기는 이동된 사용자가 새 계정에서 다시 만들어야 합니다. 자세한 내용은 [에서 사용자 지정 보기 만들기 및 관리 [!DNL Workfront Proof] 증명](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### 사용자 정의 필드

사용자 지정 필드는 이동할 수 없으며 사용자 지정 필드의 데이터는 손실되므로, 이동하기 전에 필수 항목에 대한 보고서를 생성했는지 확인하십시오.

### 자동화된 워크플로우 템플릿

자동화된 워크플로우 템플릿은 새 계정에서 다시 만들어야 하지만, 템플릿은 템플릿으로 만든 이동된 증명에서 유지됩니다.

### 댓글에 대한 작업

주석에 대한 작업은 증명에 남아 있지만 더 이상 주석에 의해 필터링할 수 없습니다. 해결 방법은 새 계정에 일치하는 작업을 만들고 필요한 경우 새 작업으로 주석을 다시 플래그를 지정하는 것입니다.
