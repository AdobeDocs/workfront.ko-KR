---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: ' [!DNL Workfront Proof]의 폴더 권한 이해'
description: 폴더에 있는 항목을 볼 수 있는 권한이 있는 사람은 폴더 자체도 볼 수 있습니다. 하지만 이 사용자는 명시적으로 공유된 폴더의 항목만 볼 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 15%

---

# [!DNL Workfront Proof]의 폴더 권한 이해

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

폴더에 있는 항목을 볼 수 있는 권한이 있는 사람은 폴더 자체도 볼 수 있습니다. 하지만 이 사용자는 명시적으로 공유된 폴더의 항목만 볼 수 있습니다.

## 공용 폴더

폴더가 공개이면 계정의 사용자(관찰자 및 라이트 사용자 제외)는 왼쪽 사이드바에서 폴더 이름을 볼 수 있습니다.

사용 권한 프로필은 공용 폴더에 대한 권한에도 영향을 줍니다.

| **프로필/작업** | **폴더의 모든 항목 보기** | **명시적으로 공유된 항목 보기** | **항목 추가** | **항목 삭제** | **하위 폴더 추가** | **하위 폴더 삭제** | **폴더 세부 정보 편집** |
|---|---|---|---|---|---|---|---|
| **작성자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **청구 관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **감독자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 아니요 | 예 | 예 | 아니요 | 예 | 아니요 | 예 |
| **관찰자** | 아니요 | 예 | 아니요 | 아니요 | 아니요 | 아니요 | 아니요 |

{style="table-layout:auto"}

관리자가 공용 폴더를 소유한 경우 루트 폴더와 하위 폴더를 삭제할 수 있습니다.

자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)을 참조하세요.

## 비공개 폴더

폴더가 비공개인 경우 폴더의 폴더 또는 항목이 사용자와 명시적으로 공유되었거나 감독자, 관리자 또는 청구 관리자의 프로필이 없으면 동일한 계정의 다른 사용자가 왼쪽 사이드바에서 폴더 이름을 볼 수 없습니다.

| **프로필/작업** | **폴더의 모든 항목 보기** | **명시적으로 공유된 항목 보기** | **항목 추가** | **항목 삭제** | **하위 폴더 추가** | **하위 폴더 삭제** | **폴더 세부 정보 편집** |
|---|---|---|---|---|---|---|---|
| **작성자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **청구 관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **감독자** | 예 | 예 | 예 | 예 | 예 | 예 | 예 |
| **관리자** | 아니요 | 예 | 아니요 | 아니요 | 아니요 | 아니요 | 아니요 |
| **관찰자** | 아니요 | 예 | 아니요 | 아니요 | 아니요 | 아니요 | 아니요 |

{style="table-layout:auto"}

예를 들어 프로젝트 관리자와 해당 팀이 특정 폴더만 볼 수 있도록 하려는 경우 프로젝트 관리자는 개인 폴더를 설정한 다음 해당 폴더를 특정 사용자와 공유할 수 있습니다.

개인 폴더를 공유할 때 관리자가 폴더 항목을 생성, 편집 및 삭제할 수 있도록 할지 여부를 결정할 수 있습니다.

새 폴더 페이지에서 각 사용자에 대해 개별적으로 설정하고 폴더 세부 정보 페이지의 [!UICONTROL 다음 사용자와 공유] 섹션에서 변경할 수 있습니다. 자세한 내용은 [폴더 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) 및 [폴더 및 해당 컨텐츠 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md)를 참조하십시오.

비공개 폴더를 또는 관찰자와 공유하는 경우 폴더의 모든 항목에 대해 읽기 전용 액세스 권한을 갖게 됩니다. 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 및 [폴더 공유 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md)를 참조하십시오.

>[!NOTE]
>
>* 상위 폴더가 비공개이면 모든 하위 폴더도 비공개가 됩니다. 비공개 상위 폴더 아래에 공개 하위 폴더를 둘 수 없습니다. 그러나 공개 상위 폴더 아래에 개인 하위 폴더를 가질 수 있습니다.
>* 폴더의 작성자 및 소유자는 항상 폴더에 액세스할 수 있으며 제거할 수 없습니다.
>* 비공개 폴더의 작성자 및 소유자만 폴더를 삭제할 수 있습니다.

