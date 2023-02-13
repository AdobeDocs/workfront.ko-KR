---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Workfront 증명의 증명 권한 프로필
description: Workfront 관리자나 Workfront 증명 관리자는 사용자에게 증명 권한 프로필을 할당하여 시스템에서 모든 증명을 위한 사용자 교정 기능을 지정할 수 있습니다. 사용자의 증명 권한 프로필 구성에 대한 자세한 내용은 Workfront 증명의 사용자 증명 권한 프로필 구성 을 참조하십시오.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 1%

---

# 증명 권한 프로필 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

로서의 [!DNL Workfront] 관리자 또는 [!DNL Workfront Proof] 관리자는 사용자에게 증명 권한 프로파일을 할당하여 시스템에서 모든 증명을 위한 교정 기능을 지정할 수 있습니다. 사용자의 증명 권한 프로필 구성에 대한 내용은 [에서 사용자의 증명 권한 프로필 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>다음을 수행할 수도 있습니다.
>
>* 개별 증명에 대한 특정 역할을 사용자에게 부여합니다. 증명 역할에 대한 자세한 내용은 [의 증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* 조직의 사용자를 위한 사용자 지정 프로필을 만듭니다. 자세한 내용은 [에서 사용자 지정 프로필 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>


다음 표에는 각 증명 권한 프로필에서 사용할 수 있는 권한이 표시됩니다.

| **고유 항목** |  |  |  |  | **기타 사용자 항목** |  |  | **관리자** | **과금** |
|---|---|---|---|---|---|---|---|---|---|
|  | **추가** | **** 보기 | **편집** | **삭제** | **** 보기 | **편집** | **삭제** | **편집 및 삭제** | **편집** |
| 청구 관리자 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| 관리자 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| 감독자 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| 관리자 | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| 관찰자 |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| 방문자 |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

역할 및 권한에 대해 다음 사항을 고려하십시오.

* 할당된 프로필 권한은 자신의 계정에 있는 사용자 및 항목만 연관시킵니다. 단, 주(허브) 계정에 대한 관리자 및 과금 관리자가 허브 계정 수준에서 해당 계정의 계정 설정과 과금을 액세스 및 관리할 수 있는 위성 계정의 경우에는 예외입니다.
* 청구 관리자 및 관리자는 사용자를 삭제할 수 있습니다. 이 작업은 계정 설정에서만 수행할 수 있습니다.
* 청구 관리자 및 관리자가 자신의 계정에 있는 다른 사용자가 소유한 증명을 볼 때 검토자의 역할을 사용하여 증명을 봅니다.
* 청구 관리자 및 관리자는 읽기 전용 역할을 사용하여 자신과 공유되는 폴더나 자신이 만든 폴더에서 증명을 액세스할 수 있습니다.

다음 섹션에서는 각 프로필과 프로필과 연관된 권한을 표준에서 설명합니다 [!DNL Workfront Proof] 설정:

* [청구 관리자](#billing-administrator)
* [관리자](#administrator)
* [감독자](#supervisor)
* [관리자](#manager)
* [관찰자](#observer)
* [방문자](#visitor)
* [게스트](#guest)

## 청구 관리자 {#billing-administrator}

청구 관리자는 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md), 및에 다음 권한이 있습니다.

![](assets/cleaner2.png)증명을 생성하고 파일을 업로드하고 폴더를 만들 수 있습니다. 자세한 내용은 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 컨텐츠를에 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), 및 [폴더 작성 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)사용자가 직접 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![](assets/cleaner2.png)조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![](assets/cleaner2.png)다른 사용자의 공용 폴더를 삭제할 수 있습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)계정에서 만든 모든 증명에 대한 편집 권한이 있습니다.

![](assets/cleaner2.png)Dropzone 소유자로 설정할 수 있습니다. 자세한 내용은 [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)청구 페이지에 액세스하여 청구 세부 정보를 편집할 수 있습니다. 자세한 내용은 [다음 [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)계정 설정 페이지에 액세스하여 계정 세부 사항을 편집할 수 있습니다. 자세한 내용은 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)휴지통을 비울 수 있습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)사용자를 추가, 편집 및 삭제할 수 있습니다.

![](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![](assets/cleaner2.png)연락처를 삭제할 수 있습니다.

![](assets/cleaner2.png)답장이 없는 경우 증명을 편집할 수 있습니다.

![](assets/no2.png)증명 응답을 편집할 수 없습니다.

![](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

계정 설정에 대한 자세한 내용은 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

청구에 대한 자세한 내용은 [다음 [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### 관리자 {#administrator}

관리자는 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)및에 다음 권한이 있습니다.

![](assets/cleaner2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 있습니다. 자세한 내용은 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 컨텐츠를에 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), 및 [폴더 작성 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![](assets/cleaner2.png)조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![](assets/cleaner2.png)다른 사용자의 공용 폴더를 삭제할 수 있습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)계정에서 만든 모든 증명에 대한 편집 권한이 있습니다.

![](assets/cleaner2.png)Dropzone 소유자로 설정할 수 있습니다. 자세한 내용은 [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)계정 설정 페이지에 액세스하여 계정 세부 사항을 편집할 수 있습니다. 자세한 내용은 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)휴지통을 비울 수 있습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)사용자를 추가, 편집 및 삭제할 수 있습니다.

![](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![](assets/cleaner2.png)연락처를 삭제할 수 있습니다.

![](assets/cleaner2.png)답장이 없는 경우 증명을 편집할 수 있습니다.

![](assets/no2.png)증명 응답을 편집할 수 없습니다.

![](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)청구 페이지에 액세스하거나 청구 세부 정보를 편집할 수 없습니다. 자세한 내용은 [다음 [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### 감독자 {#supervisor}

감독자에게는 다음 권한이 있습니다.

![](assets/cleaner2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 있습니다. 자세한 내용은 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 컨텐츠를에 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), 및 [폴더 작성 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)자신이 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![](assets/cleaner2.png)조직의 모든 사용자가 만든 증명 및 파일을 보고 편집하고 삭제할 수 있습니다.

![](assets/cleaner2.png)다른 사용자의 공용 폴더를 삭제할 수 있습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)계정에서 만든 모든 증명에 대한 편집 권한이 있습니다.

![](assets/cleaner2.png)Dropzone 소유자로 설정할 수 있습니다. 자세한 내용은 [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![](assets/cleaner2.png)연락처를 삭제할 수 있습니다.

![](assets/cleaner2.png)답장이 없는 경우 증명을 편집할 수 있습니다.

![](assets/no2.png)증명 응답을 편집할 수 없습니다.

![](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [다음 [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![](assets/no2.png)휴지통으로 이동할 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### 관리자 {#manager}

관리자는 다음 권한을 가집니다.

![](assets/cleaner2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 있습니다. 자세한 내용은 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [파일 및 웹 컨텐츠를에 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md), 및 [폴더 작성 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)자신이 만들거나 소유한 증명 및 파일을 보고, 편집하고, 삭제할 수 있습니다.

![](assets/cleaner2.png)사용자와 명시적으로 공유되는 다른 사용자의 증명을 보고, 검토하고, 승인할 수 있습니다(공유 폴더의 모든 항목에 대한 읽기 전용 권한). 자세한 내용은 [의 증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)그룹을 만들고 새 연락처를 추가할 수 있습니다.

![](assets/no2.png)조직의 다른 사용자가 만든 증명 및 파일을 보거나, 편집하거나, 삭제할 수 없습니다.

![](assets/no2.png)증명 또는 답글을 편집할 수 없습니다.

![](assets/no2.png)다른 사용자의 개인 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)다른 사용자의 공용 폴더를 삭제할 수 없습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [다음 [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Dropzone 소유자로 설정할 수 없습니다. 자세한 내용은 [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)휴지통으로 이동할 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![](assets/no2.png)연락처를 삭제할 수 없습니다.

### 관찰자 {#observer}

옵저버에는 다음 권한이 있습니다.

![](assets/cleaner2.png)사용자와 명시적으로 공유되는 다른 사용자의 증명을 보고, 검토하고, 승인할 수 있습니다(공유 폴더의 모든 항목에 대한 읽기 전용 권한). 자세한 내용은 [의 증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)명시적으로 공유된 파일을 볼 수 있습니다.

![](assets/cleaner2.png) 연락처 및 그룹을 볼 수 있습니다.

![](assets/no2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 없습니다. 자세한 내용은 [파일 및 웹 컨텐츠를에 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)조직의 다른 사용자가 만든 증명 및 파일을 보거나, 편집하거나, 삭제할 수 없습니다.

![](assets/no2.png)증명 또는 답글을 편집할 수 없습니다.

![](assets/no2.png)조직에서 만든 항목을 삭제할 수 없습니다.

![](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [다음 [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Dropzone 소유자로 설정할 수 없습니다. 자세한 내용은 [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)휴지통으로 이동할 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![](assets/no2.png)그룹을 만들거나 새 연락처를 추가할 수 없습니다.

![](assets/no2.png)연락처를 삭제할 수 없습니다.

>[!NOTE]
>
>옵저버에서 사용할 수 있는 메뉴와 기능은 제한됩니다.
>
>* 옵저버는 대시보드에 머리글 메뉴 또는 녹색 새로 만들기 메뉴가 표시되지 않습니다
>* 옵저버는 해당 설정에서 다음 링크를 볼 수 없습니다. 계정 설정, 청구
>


### 방문자 {#visitor}

방문자에게는 다음 권한이 있습니다.

![](assets/cleaner2.png)사용자와 명시적으로 공유되는 다른 사용자의 증명을 보고, 검토하고, 승인할 수 있습니다(공유 폴더의 모든 항목에 대한 읽기 전용 권한). 자세한 내용은 [의 증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)명시적으로 공유된 파일을 볼 수 있습니다.

![](assets/no2.png) 연락처 및 그룹을 볼 수 없습니다.

![](assets/no2.png)증명을 만들고, 파일을 업로드하고, 폴더를 만들 수 없습니다. 자세한 내용은 [파일 및 웹 컨텐츠를에 업로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)조직의 다른 사용자가 만든 증명 및 파일을 보거나, 편집하거나, 삭제할 수 없습니다.

![](assets/no2.png)증명 또는 답글을 편집할 수 없습니다.

![](assets/no2.png)조직에서 만든 항목을 삭제할 수 없습니다.

![](assets/no2.png)청구 페이지 또는 계정 설정에 액세스할 수 없습니다. 자세한 내용은 [다음 [!DNL Workfront Proof] 청구 페이지](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) 및 [의 계정 설정 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Dropzone 소유자로 설정할 수 없습니다. 자세한 내용은 [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)휴지통으로 이동할 수 없습니다. 자세한 내용은 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)사용자를 추가, 편집 또는 삭제할 수 없습니다.

![](assets/no2.png)그룹을 만들거나 새 연락처를 추가할 수 없습니다.

![](assets/no2.png)연락처를 삭제할 수 없습니다.

>[!NOTE]
>
>방문자가 사용할 수 있는 메뉴와 기능은 제한됩니다.
>
>* 방문자는 대시보드에 헤더 메뉴나 녹색 새 메뉴가 표시되지 않습니다
>* 방문자의 설정에 다음 링크가 표시되지 않습니다. 계정 설정, 청구
>


### 게스트 {#guest}

게스트 프로필은 자체 Workfront 증명 계정이 없는 검토자를 위해 증명을 액세스하는 데 사용됩니다. 게스트는 개인 이메일 알림을 통해 직접 사용자와 공유한 증명에 액세스할 수 있습니다.

![](assets/cleaner2.png)명시적으로 공유되는 증명을 보고, 검토하고, 승인할 수 있습니다.

![](assets/cleaner2.png)명시적으로 공유된 파일을 볼 수 있습니다.

![](assets/no2.png)대시보드에 액세스할 수 없습니다.

![](assets/no2.png)폴더와 공유할 수 없습니다. 자세한 내용은 [폴더 관리 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)증명에 작성자 또는 중재자로 추가할 수 없습니다. 자세한 내용은 [의 증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>게스트는 Workfront 증명 사용자가 아니므로 자체 대시보드에서 사용자와 공유된 모든 증명을 볼 수 없습니다.

## 사용자의 증명 권한 프로필 편집

관리자 및 청구 관리자는 계정에 있는 모든 사용자의 권한 프로필을 편집할 수 있습니다.

1. 편집할 사용자를 찾으려면 다음 중 하나를 수행합니다.

   * 다음으로 이동 **[!UICONTROL 계정 설정]**&#x200B;를 클릭한 다음 **[!UICONTROL 사용자]** 탭.

   * 로 이동합니다. **[!UICONTROL 연락처]** 페이지.

1. 편집할 사용자 이름을 클릭합니다. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. 을(를) 클릭합니다. **[!UICONTROL 권한 프로필]** 드롭다운 메뉴에서 새 권한 프로필을 선택합니다. :

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   권한 프로필은 관리자, 감독자, 관리자 및 관찰자입니다.

1. 저장할 메뉴 외부의 아무 곳이나 클릭합니다.

>[!NOTE]
>
>관리자는 청구 관리자 프로필을 할당할 수 없습니다. 다음 로그에서 프로필 변경 사항 목록을 찾을 수 있습니다.
>
>* 계정 활동 로그
>* 사용자의 프로필 로그(해당 사용자만 액세스할 수 있음)
>


활동 로그에 대한 자세한 내용은 [이해 [!DNL Workfront Proof] 활동 감사 추적](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
