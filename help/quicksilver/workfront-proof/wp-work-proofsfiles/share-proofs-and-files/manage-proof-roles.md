---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: 의 증명 역할 관리 [!DNL Workfront Proof]
description: 증명 역할을 사용하면 사용자 프로필에 구성된 권한 프로필로 제한된 사용자에게 권한을 부여할 수 있습니다. (권한 프로필에 대한 자세한 내용은 [!DNL Workfront Proof])
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 1%

---

# 의 증명 역할 관리 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

증명 역할을 사용하면 사용자 프로필에 구성된 권한 프로필로 제한된 사용자에게 권한을 부여할 수 있습니다. 권한 프로필에 대한 자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md))

증명 역할은 계정 프로필과 다릅니다. 계정 프로필은 계정에 있는 전체 권한 수준과 관련이 있으며 사용자와 명시적으로 공유되지 않은 계정에서도 모든 증명을 가지고 있는 권한에 영향을 줍니다.

자세한 내용은 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 증명 역할 정보

증명을 검토하도록 사용자에게 초대될 때 개별 증명에 대한 다음 증명 역할이 사용자에게 부여됩니다.

* [읽기 전용](#read-only)
* [검토자](#reviewer)
* [승인자](#approver)
* [검토자 및 승인자](#reviewer-approver)
* [작성자](#author)
* [중재자](#moderator)

증명 역할은 검토자가 특정 증명과 관련하여 수행할 수 있는 작업을 정의합니다.

예를 들어 검토자인 경우, 마크업과 주석을 추가하여 증명을 검토하라는 메시지가 표시됩니다. 검토자 및 승인자인 경우, 검토를 요청받고 증명에 대한 결정을 내려야 합니다.

특정 증명 역할은 검토자가 증명에 대한 편집 권한을 부여하고(계정 프로필이 승인되지 않은 경우에도), 주석에 대한 작업 추가, 새 버전 만들기, 증명에 더 많은 검토자 추가와 같은 일부 추가 기능을 사용할 수 있도록 해줍니다.

자세한 내용은 다음 문서를 참조하십시오.

* [증명 주석에 작업 사용](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [증명 공유 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### 읽기 전용

{#read-only}

![cleaner.png](assets/cleaner.png) 증명을 볼 수 있습니다.

![no.png](assets/no.png) 마크업을 추가할 수 없습니다.

![no.png](assets/no.png) 주석을 추가할 수 없습니다.

![no.png](assets/no.png) 결정을 내릴 수 없음

![no.png](assets/no.png) 다른 사람이 작성한 주석을 삭제할 수 없습니다.

![no.png](assets/no.png) 증명에 대한 편집 권한이 없습니다.

>[!NOTE]
>
>폴더를 [!DNL Workfront Proof]로 설정되면 폴더에 있는 모든 기존 및 이후에 추가된 항목에 대해 읽기 전용 권한이 자동으로 부여됩니다.

자세한 내용은 [폴더 공유 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### 검토자 {#reviewer}

![cleaner.png](assets/cleaner.png) 증명을 볼 수 있습니다.

![cleaner.png](assets/cleaner.png) 마크업을 추가할 수 있습니다

![cleaner.png](assets/cleaner.png) 댓글 추가 가능

![[!DNL cleaner].png](assets/cleaner.png) 응답이 없는 경우 댓글을 편집할 수 있습니다

![no.png](assets/no.png) 결정을 내릴 수 없음

![no.png](assets/no.png) 다른 사람이 작성한 주석을 편집하거나 삭제할 수 없습니다.

![no.png](assets/no.png) 증명에 대한 편집 권한이 없습니다.

### 승인자 {#approver}

![cleaner.png](assets/cleaner.png) 증명을 볼 수 있습니다.

![cleaner.png](assets/cleaner.png) 결정을 내릴 수 있음

![no.png](assets/no.png) 마크업을 추가할 수 없습니다.

![no.png](assets/no.png) 주석을 추가할 수 없습니다.

![no.png](assets/no.png) 다른 사람이 작성한 주석을 편집하거나 삭제할 수 없습니다.

![no.png](assets/no.png) 증명에 대한 편집 권한이 없습니다.

### 검토자 및 승인자 {#reviewer-approver}

![cleaner.png](assets/cleaner.png) 증명을 볼 수 있습니다.

![cleaner.png](assets/cleaner.png) 마크업을 추가할 수 있습니다

![cleaner.png](assets/cleaner.png) 댓글 추가 가능

![[!DNL cleaner].png](assets/cleaner.png) 응답이 없는 경우 댓글을 편집할 수 있습니다

![cleaner.png](assets/cleaner.png) 결정을 내릴 수 있음

![no.png](assets/no.png) 다른 사람이 작성한 주석을 편집하거나 삭제할 수 없습니다.

![no.png](assets/no.png) 증명에 대한 편집 권한이 없습니다.

### 작성자 {#author}

![cleaner.png](assets/cleaner.png) 마크업을 추가할 수 있습니다

![cleaner.png](assets/cleaner.png) 댓글 추가 가능

![[!DNL cleaner].png](assets/cleaner.png) 응답이 없는 경우 댓글을 편집할 수 있습니다

![cleaner.png](assets/cleaner.png) 결정을 내릴 수 있음

![cleaner.png](assets/cleaner.png) 새 버전을 제출할 수 있음

![cleaner.png](assets/cleaner.png) 증명 사본을 만들 수 있습니다.

![cleaner.png](assets/cleaner.png) 다른 사람과 증명 공유 가능

![cleaner.png](assets/cleaner.png) 주석에 작업을 적용할 수 있습니다

![cleaner.png](assets/cleaner.png) 댓글 해결 가능

![no.png](assets/no.png) 다른 사람이 작성한 주석을 편집하거나 삭제할 수 없습니다.

>[!NOTE]
>
>이 역할은 [!DNL Workfront Proof]

### 중재자 {#moderator}

![cleaner.png](assets/cleaner.png) 마크업을 추가할 수 있습니다

![cleaner.png](assets/cleaner.png) 댓글 추가 가능

![[!DNL cleaner].png](assets/cleaner.png) 응답이 없는 경우 댓글을 편집할 수 있습니다

![cleaner.png](assets/cleaner.png) 결정을 내릴 수 있음

![cleaner.png](assets/cleaner.png) 새 버전을 제출할 수 있음

![cleaner.png](assets/cleaner.png) 새 검토자를 추가할 수 있습니다.

![cleaner.png](assets/cleaner.png) 주석에 작업을 적용할 수 있습니다

![cleaner.png](assets/cleaner.png) 댓글 해결 가능

![cleaner.png](assets/cleaner.png) 본인 또는 다른 사람이 만든 증명의 댓글과 답글을 삭제할 수 있습니다.

* 주석 스레드에서 첫 번째 주석을 삭제하면 전체 스레드가 삭제됩니다
* 댓글 스레드에서 응답을 삭제하면 해당 응답만 삭제됩니다

![no.png](assets/no.png) 다른 사람이 작성한 주석을 편집할 수 없습니다.

이 역할을 통해 사용자는 증명 댓글을 관리 및 중재하여 증명의 관련 댓글만 유지하고 관련 없는 댓글을 제거할 수 있는 기회를 제공합니다.

>[!NOTE]
>
>이 역할은 [!DNL Workfront Proof].

## 증명 역할 할당

새 증명을 만들거나, 새 버전의 기존 증명을 만들거나, 기존 증명에서 증명 역할을 지정할 수 있습니다.

* [새 증명](#new-proofs)
* [새 버전](#new-versions)
* [기존 증명](#existing-proofs)

### 새 증명 {#new-proofs}

에서 검토자에게 증명 역할을 할당할 수 있습니다 [!UICONTROL 새로운 증명] 페이지를 만듭니다(1).

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### 새 버전 {#new-versions}

증명의 새 버전을 만들 때 이전 버전의 검토자가 자동으로 표시됩니다(이전 버전과 동일한 역할).

새 버전(1)을 만들 때 검토자에게 적용된 증명 역할을 편집할 수 있습니다.

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### 기존 증명 {#existing-proofs}

기존 증명의 개인 역할을 변경하려면 [!UICONTROL 증명 세부 사항] 워크플로우 섹션(1)에서 해당 역할을 편집할 때 인라인 페이지로 이동:

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## 증명 뷰어에서 역할 확인

증명 뷰어(1)에서 직접 검토자의 역할을 확인하고 필요한 경우 (2)를 편집할 수 있습니다.

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## 기본 증명 역할

에서 기본 증명 역할을 설정할 수 있습니다 [!DNL Proofing Defaults] 페이지를 개인 설정으로 지정합니다. 즉, 증명에 추가되면 기본 증명 역할이 자동으로 채워집니다. 증명의 편집 권한이 있는 사용자가 증명 수준에서 이 역할을 변경할 수 있습니다.

>[!NOTE]
>
>관리자 또는 청구 관리자 프로필이 있는 사용자만 계정의 다른 사용자에 대한 교재 기본값을 변경할 수 있습니다.

자세한 내용은 [의 개인 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## 작성자 및 소유자

작성자 및 소유자는 증명의 전체 편집 권한을 갖습니다.

* [작성자](#creators)
* [소유자](#owners)

### 작성자 {#creators}

증명 작성자는 첫 번째 인스턴스에서 증명을 업로드하는 사용자입니다. 증명 작성자는 증명(기본 역할)을 위한 사람 목록에 자동으로 표시됩니다.

설정 [!UICONTROL 새로운 증명] 페이지를 증명 작성자에게(기본 역할 제외) 다른 증명 역할을 지정할 수 있습니다.

증명 작성자는 증상에서 변경하거나 제거할 수 없습니다.

### 소유자 {#owners}

기본적으로 작성자는 증명의 소유자입니다. 그러나 작성자는 처음에 증명을 만들 때( [!UICONTROL 새로운 증명] 페이지).

새 증명 페이지에서 소유자를 변경하려면

1. 작성자의 이름 옆에 표시되는 변경 링크를 클릭합니다.
1. 드롭다운 메뉴에서 새 소유자를 선택합니다. (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

증명이 만들어지면 소유자를 변경할 수 있습니다. 증명에 대한 편집 권한이 있는 모든 사용자는 [!UICONTROL 증명 세부 사항] 페이지(아래 참조).

증명의 소유자를 변경하는 기능은 특히 워크플로우 관리 측면에서 유용합니다. 이를 통해 프로젝트에 대한 책임이 있는 사람이 증명 소유권을 승계하여 증명을 편집할 수 있는 권한과 증명을 에서 볼 수 있는 기능을 제공할 수 있습니다 [!UICONTROL 내 증명] 보기.

를 통해 증명의 소유자를 변경하려면 [!UICONTROL 증명 세부 사항] 페이지:

* 소유자를 만들 사람의 이름 옆에 있는 작업 메뉴를 클릭합니다
* 선택 [!UICONTROL 소유자 만들기] 를 클릭합니다.
* 또는 을 클릭하여 [!UICONTROL 소유자] 증명 이미지 옆의 필드를 선택하고 표시되는 드롭다운에서 새 소유자 를 선택합니다.

이 작업이 완료되면 해당 사용자의 이름 옆에 &quot;소유자&quot;라는 단어가 표시됩니다.

>[!NOTE]
>
>동일한 계정 또는 파트너 계정의 사용자만 증명 소유자로 만들 수 있습니다. 파트너 계정의 사용자는 다음과 같은 경우에만 증명 소유자가 될 수 있습니다.
>
>* 계정 간에 설정된 기존 파트너 관계가 있습니다. 자세한 내용은 [의 파트너 계정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* 에는 사용자 지정 필드가 없습니다 [!UICONTROL 새로운 증명] 페이지.
>* 증명을 폴더에 할당하지 않았습니다.
>* 증명에 태그가 적용되지 않았습니다.
>




내에서 증명 소유권을 일시적으로 위임하려면 [!DNL Workfront Proof]를 참조하십시오. [에서 임시 증명 소유자 지정 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
