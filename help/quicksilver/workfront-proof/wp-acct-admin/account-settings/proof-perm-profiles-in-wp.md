---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Workfront Proof의 증명 권한 프로필
description: Workfront 관리자 또는 Workfront Proof 관리자는 사용자에게 증명 권한 프로필을 할당하여 시스템의 모든 증명에 대해 사용자가 보유할 증명 기능을 지정할 수 있습니다. 사용자의 증명 권한 프로필 구성에 대한 자세한 내용은 Workfront Proof에서 사용자의 증명 권한 프로필 구성 을 참조하십시오.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 0%

---

# [!DNL Workfront Proof]의 증명 권한 프로필

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

[!DNL Workfront] 관리자 또는 [!DNL Workfront Proof] 관리자는 사용자에게 증명 권한 프로필을 할당하여 시스템의 모든 증명에 대해 사용자가 보유할 증명 기능을 지정할 수 있습니다. 사용자의 증명 권한 프로필 구성에 대한 자세한 내용은 [사용자의 증명 권한 프로필 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md)을 참조하십시오.

>[!NOTE]
>
>다음을 수행할 수도 있습니다.
>
>* 개별 증명에 대한 특정 역할을 사용자에게 부여합니다. 증명 역할에 대한 자세한 내용은 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.
>* 조직의 사용자를 위한 사용자 지정 프로필을 만듭니다. 자세한 내용은 [사용자 지정 프로필 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md)을 참조하십시오.
>

다음 표에는 각 증명 권한 프로필에서 사용할 수 있는 권한이 표시됩니다.

| **고유 항목** |  |  |  |  | **다른 사용자의 항목** |  |  | **관리자** | **청구** |
|---|---|---|---|---|---|---|---|---|---|
|   | **추가** | **보기** | **편집** | **삭제** | **보기** | **편집** | **삭제** | **편집 및 삭제** | **편집** |
| 청구 관리자 | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) |
| 관리자 | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) |   |
| 감독자 | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) |   |   |
| 관리자 | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) | ![확인 표시](assets/cleaner2.png) |   |   |   |   |   |
| 관찰자 |   | ![확인 표시](assets/cleaner2.png) |   |   |   |   |   |   |   |
| 방문자 |   | ![확인 표시](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

역할 및 권한에 대해 다음 사항을 고려하십시오.

* 할당된 프로필 권한은 사용자 계정의 사용자 및 항목에만 관련됩니다. 기본(허브) 계정의 관리자 및 청구 관리자가 허브 계정 수준에서 해당 계정의 계정 설정 및 청구에 액세스하고 관리할 수 있는 위성 계정의 경우는 예외입니다.
* 청구 관리자 및 관리자는 사용자를 삭제할 수 있습니다. 이 작업은 계정 설정에서만 수행할 수 있습니다.
* 청구 관리자 및 관리자는 자신의 계정에서 다른 사용자가 소유한 증명을 볼 때 검토자 역할로 볼 수 있습니다.
* 청구 관리자 및 관리자는 읽기 전용 역할을 사용하여 사용자와 공유된 폴더 또는 자신이 생성한 폴더에서 증명에 액세스할 수 있습니다.

다음 섹션에서는 표준 [!DNL Workfront Proof] 설정에서 각 프로필 및 프로필과 연결된 권한에 대해 설명합니다.

* [청구 관리자](#billing-administrator)
* [관리자](#administrator)
* [감독자](#supervisor)
* [관리자](#manager)
* [관찰자](#observer)
* [방문자](#visitor)
* [게스트](#guest)

## 청구 관리자 {#billing-administrator}

청구 관리자는  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)의 [계정 설정에 액세스할 수 있으며 다음 권한이 있습니다.

![확인 표시](assets/cleaner2.png)증명을 생성하고, 파일을 업로드하고, 폴더를 만들 수 있습니다. 자세한 내용은 [증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 콘텐츠 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) 및 [폴더 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)자신이 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)다른 사용자의 공용 폴더를 삭제할 수 있습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

![확인 표시](assets/cleaner2.png)계정에서 만든 모든 증명에 대한 편집 권한이 있습니다.

![확인 표시](assets/cleaner2.png)드롭 영역 소유자로 설정할 수 있습니다. 자세한 내용은 [드롭 영역 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)을 참조하세요.

![확인 표시](assets/cleaner2.png)청구 페이지에 액세스하여 청구 세부 정보를 편집할 수 있습니다. 자세한 내용은 [청구 페이지 [!DNL Workfront Proof] 2}를 참조하세요.](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)

![확인 표시](assets/cleaner2.png)계정 설정 페이지에 액세스하여 계정 세부 정보를 편집할 수 있습니다. 자세한 내용은 [계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)을 참조하세요.

![확인 표시](assets/cleaner2.png)휴지통을 비울 수 있습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)사용자를 추가, 편집 및 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![확인 표시](assets/cleaner2.png)연락처를 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)답글이 없으면 증명을 편집할 수 있습니다.

![빨간색 X](assets/no2.png)증명 회신을 편집할 수 없습니다.

![빨간색 X](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

계정 설정에 대한 자세한 내용은  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)의 [계정 설정을 참조하십시오.

청구에 대한 자세한 내용은 [청구 페이지 [!DNL Workfront Proof] 2}를 참조하세요.](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)

### 관리자 {#administrator}

관리자는 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)에 액세스할 수 있으며 다음 권한이 있습니다.

![확인 표시](assets/cleaner2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 있습니다. 자세한 내용은 [증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 콘텐츠 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) 및 [폴더 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)증명과 만들어진 파일을 보고 편집하고 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)다른 사용자의 공용 폴더를 삭제할 수 있습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

![확인 표시](assets/cleaner2.png)계정에서 만든 모든 증명에 대한 편집 권한이 있습니다.

![확인 표시](assets/cleaner2.png)드롭 영역 소유자로 설정할 수 있습니다. 자세한 내용은 [드롭 영역 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)을 참조하세요.

![확인 표시](assets/cleaner2.png)계정 설정 페이지에 액세스하여 계정 세부 정보를 편집할 수 있습니다. 자세한 내용은 [계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)을 참조하세요.

![확인 표시](assets/cleaner2.png)휴지통을 비울 수 있습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)사용자를 추가, 편집 및 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![확인 표시](assets/cleaner2.png)연락처를 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)답글이 없으면 증명을 편집할 수 있습니다.

![빨간색 X](assets/no2.png)증명 회신을 편집할 수 없습니다.

![빨간색 X](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

![빨간색 X](assets/no2.png)청구 페이지에 액세스하거나 청구 세부 정보를 편집할 수 없습니다. 자세한 내용은 [청구 페이지 [!DNL Workfront Proof] 2}를 참조하세요.](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)

### 감독자 {#supervisor}

감독자는 다음과 같은 권한을 가집니다.

![확인 표시](assets/cleaner2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 있습니다. 자세한 내용은 [증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 콘텐츠 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) 및 [폴더 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)자신이 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)다른 사용자의 공용 폴더를 삭제할 수 있습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

![확인 표시](assets/cleaner2.png)계정에서 만든 모든 증명에 대한 편집 권한이 있습니다.

![확인 표시](assets/cleaner2.png)드롭 영역 소유자로 설정할 수 있습니다. 자세한 내용은 [드롭 영역 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)을 참조하세요.

![확인 표시](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![확인 표시](assets/cleaner2.png)연락처를 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)답글이 없으면 증명을 편집할 수 있습니다.

![빨간색 X](assets/no2.png)증명 회신을 편집할 수 없습니다.

![빨간색 X](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md)를 참조하세요.

![빨간색 X](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)을 참조하세요. [!DNL Workfront Proof] 

![빨간색 X](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)휴지통을 비울 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)를 참조하십시오.

### 관리자 {#manager}

관리자는 다음 권한을 가집니다.

![확인 표시](assets/cleaner2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 있습니다. 자세한 내용은 [증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 콘텐츠 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) 및 [폴더 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)자신이 만들거나 소유한 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![확인 표시](assets/cleaner2.png)다른 사용자와 명시적으로 공유된 증명(공유 폴더의 모든 항목에 대한 읽기 전용 권한)을 보고, 검토하고, 승인할 수 있습니다. 자세한 내용은 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![빨간색 X](assets/no2.png)조직의 다른 사용자가 만든 증명 및 파일을 보거나 편집하거나 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)증명 또는 답글을 편집할 수 없습니다.

![빨간색 X](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

![빨간색 X](assets/no2.png)다른 사용자의 공용 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

![빨간색 X](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)을 참조하세요. [!DNL Workfront Proof] 

![빨간색 X](assets/no2.png)드롭 영역 소유자로 설정할 수 없습니다. 자세한 내용은 [드롭 영역 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)을 참조하세요.

![빨간색 X](assets/no2.png)휴지통을 비울 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)를 참조하십시오.

![빨간색 X](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)연락처를 삭제할 수 없습니다.

### 관찰자 {#observer}

관찰자는 다음 권한을 갖습니다.

![확인 표시](assets/cleaner2.png)다른 사용자와 명시적으로 공유된 다른 사용자의 증명을 보고 검토하고 승인할 수 있습니다(공유 폴더의 모든 항목에 대한 읽기 전용 권한). 자세한 내용은 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)명시적으로 공유된 파일을 볼 수 있습니다.

![확인 표시](assets/cleaner2.png) 연락처 및 그룹을 볼 수 있음

![빨간색 X](assets/no2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 없습니다. 자세한 내용은 [파일 및 웹 콘텐츠 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)를 참조하십시오.

![빨간색 X](assets/no2.png)조직의 다른 사용자가 만든 증명 및 파일을 보거나 편집하거나 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)증명 또는 답글을 편집할 수 없습니다.

![빨간색 X](assets/no2.png)조직에서 만든 항목을 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)을 참조하세요. [!DNL Workfront Proof] 

![빨간색 X](assets/no2.png)드롭 영역 소유자로 설정할 수 없습니다. 자세한 내용은 [드롭 영역 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)을 참조하세요.

![빨간색 X](assets/no2.png)휴지통을 비울 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)를 참조하십시오.

![빨간색 X](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)그룹을 만들거나 새 연락처를 추가할 수 없습니다.

![빨간색 X](assets/no2.png)연락처를 삭제할 수 없습니다.

>[!NOTE]
>
>관찰자가 사용할 수 있는 메뉴 및 기능은 제한됩니다.
>
>* 관찰자는 대시보드에 헤더 메뉴 또는 녹색 새로 만들기 메뉴를 표시하지 않습니다
>* 관찰자는 자신의 설정에 계정 설정, 청구 링크가 표시되지 않습니다.
>

### 방문자 {#visitor}

방문자는 다음 권한을 갖습니다.

![확인 표시](assets/cleaner2.png)다른 사용자와 명시적으로 공유된 증명(공유 폴더의 모든 항목에 대한 읽기 전용 권한)을 보고, 검토하고, 승인할 수 있습니다. 자세한 내용은 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.

![확인 표시](assets/cleaner2.png)명시적으로 공유된 파일을 볼 수 있습니다.

![빨간색 X](assets/no2.png) 연락처 및 그룹을 볼 수 없음

![빨간색 X](assets/no2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 없습니다. 자세한 내용은 [파일 및 웹 콘텐츠 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)를 참조하십시오.

![빨간색 X](assets/no2.png)조직의 다른 사용자가 만든 증명 및 파일을 보거나 편집하거나 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)증명 또는 답글을 편집할 수 없습니다.

![빨간색 X](assets/no2.png)조직에서 만든 항목을 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)을 참조하세요. [!DNL Workfront Proof] 

![빨간색 X](assets/no2.png)드롭 영역 소유자로 설정할 수 없습니다. 자세한 내용은 [드롭 영역 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)을 참조하세요.

![빨간색 X](assets/no2.png)휴지통을 비울 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)를 참조하십시오.

![빨간색 X](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![빨간색 X](assets/no2.png)그룹을 만들거나 새 연락처를 추가할 수 없습니다.

![빨간색 X](assets/no2.png)연락처를 삭제할 수 없습니다.

>[!NOTE]
>
>방문자가 사용할 수 있는 메뉴 및 기능은 제한됩니다.
>
>* 방문자의 대시보드에 헤더 메뉴 또는 녹색 새로 만들기 메뉴가 표시되지 않음
>* 방문자의 설정에 계정 설정, 청구 링크가 표시되지 않습니다.
>

### 게스트 {#guest}

게스트 프로필은 자체 Workfront Proof 계정이 없는 검토자의 증명에 대한 액세스 권한을 제공하는 데 사용됩니다. 개인 이메일 알림을 통해 직접 공유된 증명에 액세스할 수 있습니다.

![확인 표시](assets/cleaner2.png)명시적으로 공유된 증명을 보고 검토하고 승인할 수 있습니다.

![확인 표시](assets/cleaner2.png)명시적으로 공유된 파일을 볼 수 있습니다.

![빨간색 X](assets/no2.png)대시보드에 액세스할 수 없습니다.

![빨간색 X](assets/no2.png)폴더를 공유할 수 없습니다. 자세한 내용은 [폴더 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하세요.

![빨간색 X](assets/no2.png)증명에 작성자 또는 중재자로 추가할 수 없습니다. 자세한 내용은 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.

>[!NOTE]
>
>게스트는 Workfront Proof 사용자가 아니므로 자신의 대시보드에서 게스트와 공유된 모든 증명을 볼 수 없습니다.

## 사용자의 증명 권한 프로필 편집

관리자 및 청구 관리자는 계정의 모든 사용자에 대한 권한 프로필을 편집할 수 있습니다.

1. 편집할 사용자를 찾으려면 다음 중 하나를 수행합니다.

   * **[!UICONTROL 계정 설정]**(으)로 이동한 다음 **[!UICONTROL 사용자]** 탭을 클릭합니다.

   * **[!UICONTROL 연락처]** 페이지로 이동합니다.

1. 권한을 편집할 사용자의 이름을 클릭합니다. ![사용자 선택](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. **[!UICONTROL 권한 프로필]** 드롭다운 메뉴를 클릭하고 새 권한 프로필을 선택합니다. :

   ![권한 프로필](assets/screenshot-2018-03-30-14-18-03a.png)

   권한 프로필은 관리자, 감독자, 관리자 및 관찰자입니다.

1. 메뉴 바깥쪽을 클릭하여 저장합니다.

>[!NOTE]
>
>관리자는 청구 관리자 프로필을 할당할 수 없습니다. 다음 로그에서 프로필 변경 사항 목록을 찾을 수 있습니다.
>
>* 계정 활동 로그
>* 사용자 프로필 로그(해당 사용자만 액세스할 수 있음)
>

활동 로그에 대한 자세한 내용은 [활동 감사 추적 이해 [!DNL Workfront Proof] 2}를 참조하십시오.](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md)
