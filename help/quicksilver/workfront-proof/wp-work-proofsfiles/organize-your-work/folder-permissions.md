---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 의 폴더 권한 이해 [!DNL Workfront Proof]
description: 폴더에 있는 항목을 볼 수 있는 권한이 있는 사람이 폴더 자체를 볼 수도 있습니다. 그러나 이 구성 요소는 명시적으로 공유된 폴더의 항목만 볼 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 16%

---

# 의 폴더 권한 이해 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

폴더에 있는 항목을 볼 수 있는 권한이 있는 사람이 폴더 자체를 볼 수도 있습니다. 그러나 이 구성 요소는 명시적으로 공유된 폴더의 항목만 볼 수 있습니다.

## 공용 폴더

폴더가 공개 상태인 경우, 계정의 사용자(옵저버 및 라이트 사용자 제외)는 왼쪽 사이드바에서 폴더 이름을 볼 수 있습니다.

권한 프로필은 공용 폴더에 대해 갖고 있는 권한에도 영향을 줍니다.

| **프로필/작업** | **폴더의 모든 항목 보기** | **명시적으로 공유된 항목을 봅니다.** | **항목 추가** | **항목 삭제** | **하위 폴더 추가** | **하위 폴더 삭제** | **폴더 세부 사항 편집** |
|---|---|---|---|---|---|---|---|
| **작성자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **청구 관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **감독자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 아니요 | 예 | 예 | 아니요 | 예 | 아니요 | 예 |
| **관찰자** | 아니요 | 예 | 아니요 | 아니요 | 아니요 | 아니요 | 아니요 |

{style="table-layout:auto"}

관리자가 공용 폴더를 소유한 경우 루트 폴더와 하위 폴더를 삭제할 수 있습니다.

자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 개인 폴더

폴더가 개인 경우, 폴더의 폴더 또는 항목이 명시적으로 공유되었거나 감독자, 관리자 또는 청구 관리자의 프로필이 있지 않으면 동일한 계정의 다른 사용자가 왼쪽 사이드바의 폴더 이름을 볼 수 없습니다.

| **프로필/작업** | **폴더의 모든 항목 보기** | **명시적으로 공유된 항목을 봅니다.** | **항목 추가** | **항목 삭제** | **하위 폴더 추가** | **하위 폴더 삭제** | **폴더 세부 사항 편집** |
|---|---|---|---|---|---|---|---|
| **작성자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **청구 관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **감독자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 아니요 | 예 | 아니요 | 아니요 | 아니요 | 아니요 | 아니요 |
| **관찰자** | 아니요 | 예 | 아니요 | 아니요 | 아니요 | 아니요 | 아니요 |

{style="table-layout:auto"}

예를 들어, 프로젝트 관리자 및 해당 팀이 특정 폴더만 표시하도록 하려는 경우 프로젝트 관리자는 비공개 폴더를 설정한 다음 특정 사용자와 폴더를 공유할 수 있습니다.

비공개 폴더를 공유할 때 관리자가 폴더 항목을 생성, 편집 및 삭제할 수 있도록 할지 여부를 결정할 수 있습니다.

새 폴더 페이지에서 각 사용자에 대해 개별적으로 설정하고 [!UICONTROL 공유 대상] 폴더 세부 사항 페이지의 섹션을 참조하십시오. 자세한 내용은 [폴더 작성 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) 및 [폴더 및 해당 컨텐츠 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

개인 폴더가 또는 관찰자와 공유되면 폴더의 모든 항목에 대해 읽기 전용 액세스 권한이 제공됩니다. 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 및 [폴더 공유 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* 상위 폴더가 비공개 폴더인 경우 모든 하위 폴더도 비공개 폴더입니다. 비공개 상위 폴더 아래에 공용 하위 폴더가 있을 수 없습니다. 그러나 공개 상위 폴더 아래에 비공개 하위 폴더가 있을 수 있습니다.
>* 폴더의 작성자와 소유자는 항상 폴더에 액세스할 수 있으며 제거할 수 없습니다.
>* 개인 폴더의 작성자와 소유자만 폴더를 삭제할 수 있습니다.


