---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: Dropzone
description: 엔터프라이즈 플랜이 있는 경우 Dropzone을 사용하여 계정에 로그인하지 않고도 새로운 증명 및 새로운 버전의 증명을 계정에 제출할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Dropzone

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

엔터프라이즈 플랜이 있는 경우 Dropzone을 사용하여 계정에 로그인하지 않고도 새로운 증명 및 새로운 버전의 증명을 계정에 제출할 수 있습니다.

Dropzone을 통해 증명을 제출하면 Dropzone 페이지의 [!DNL Workfront Proof] 계정이 필요합니다. 여기에서 워크플로우로 라우팅할 수 있습니다.

## Dropzone URL을 통해 새 증명 제출

1. 브라우저에 설명된 대로 고유한 Dropzone URL로 이동합니다. [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. 이메일 주소 입력.
1. 클릭 **[!UICONTROL 파일 선택]** 또는 **[!UICONTROL 웹 페이지 캡처]** 업로드할 파일 또는 웹 페이지를 선택합니다.

1. 보안 코드를 입력한 다음 **[!UICONTROL 다음]**.\
   진행 표시줄에는 업로드의 진행 상태가 표시됩니다.\
   다음 화면에서 증명 세부 사항을 추가할 수 있습니다.\
   이 섹션은 Dropzone 설정에서 활성화되었을 경우에만 나타납니다.

1. 세부 사항을 입력한 후 **[!UICONTROL 다음]**.
1. 증명에 추가된 모든 검토자는 증명을 활성화한 경우에만 알림 이메일을 받게 됩니다(아래 참조).
1. 증명은 Dropzone에 제출한 후 다음 상태를 따릅니다.

   * 파일을 Dropzone에 처음 업로드하면 증명에 초안으로 표시됩니다.
   * 제출을 완료하면 Dropzone에 증명이 제출됨으로 표시됩니다.
   * 증명의 활성화 및 잠금이 해제되면 Dropzone에 활성 상태로 표시됩니다.
   * 증명이 잠긴 경우 Dropzone에 잠긴 것으로 표시됩니다.

## Dropzone URL을 통해 기존 증명의 새 버전 제출

1. 브라우저에 설명된 대로 고유한 Dropzone URL로 이동합니다. [에서 드롭존을 구성합니다. [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. 이메일 주소 입력.
1. 확인란을 선택하여 기존 증명의 새 버전을 업로드하고 있음을 나타냅니다.\
   증명의 새 버전을 만드는 방법에 대한 자세한 내용은 를 참조하십시오.
1. 클릭 **[!UICONTROL 파일 선택]** 또는 **[!UICONTROL 웹 페이지 캡처]** 업로드할 파일 또는 웹 페이지를 선택합니다.

1. 보안 코드를 입력한 다음 **[!UICONTROL 다음]**.\
   진행 표시줄에는 업로드의 진행 상태가 표시됩니다.\
   Workfront 증명 은 유효성 검사 이메일을 보냅니다.

1. 이메일의 링크를 클릭합니다.\
   이메일이 브라우저에서 Dropzone 창을 엽니다. 이메일 알림의 링크는 24시간 동안 유효합니다.
1. 이전 버전의 증명을 선택합니다(만들거나 제출한 증명만 표시됩니다.).\
   다음 화면에서 증명 세부 사항을 추가할 수 있습니다.\
   이 섹션은 Dropzone 설정에서 활성화되었을 경우에만 나타납니다.

1. 세부 정보를 입력하고 **[!UICONTROL 다음]**.

   >[!NOTE]
   >
   >증명에 추가된 모든 검토자는 증명을 활성화한 경우에만 알림 이메일을 받게 됩니다(아래 참조).

   증명은 Dropzone에 제출한 후 다음 상태를 따릅니다.

   * 파일을 Dropzone에 처음 업로드하면 증명에 초안으로 표시됩니다.
   * 제출을 완료하면 Dropzone에 증명이 제출됨으로 표시됩니다.
   * 증명의 활성화 및 잠금이 해제되면 Dropzone에 활성 상태로 표시됩니다.
   * 증명이 잠긴 경우 Dropzone에 잠긴 것으로 표시됩니다.

## Dropzone에 증명 전자 메일 보내기

>[!NOTE]
>
>드롭존에 증명을 이메일로 보낼 수 없습니다.


## 제출 완료

Workfront에서 전송 완료 이메일을 보내 파일이 새 증명인지 새 버전인지 확인하는 메시지를 보냅니다. 이메일 알림의 링크는 24시간 동안 유효합니다.

1. 링크를 클릭하고 새 증표인지 기존 증명의 새 버전인지에 따라 위의 단계를 수행합니다.

## 증명 활성화

Dropzone 소유자는 Dropzone에 새 증명을 제출했음을 알리는 알림 이메일을 수신합니다.

* 증명은 계정의 Dropzone 페이지에 나타납니다(Dropzone 페이지에 액세스하려면 왼쪽 탐색 사이드바의 링크를 클릭하십시오.).
* 증명은 Dropzone 소유자(또는 수퍼바이저 프로필이 적어도 있는 사용자)가 액세스할 수 있습니다. 소유자는 Dropzone 설정 내에서 변경할 수 있습니다(청구 관리자 또는 관리자만 이 작업을 수행할 수 있음).
* 증명의 작업을 수행하려면 먼저 Dropzone 소유자(감독자 프로파일이 있는 사용자도 이 작업을 수행할 수 있음)가 증명의 활성화/잠금 해제해야 합니다. 증명의 상태는 활성화되거나 잠금 해제될 때까지 제출됨으로 표시됩니다.

증명을 활성화하려면

1. 증명 오른쪽에 있는 드롭다운 메뉴로 이동한 다음 를 클릭합니다. **[!UICONTROL 활성화]**.
1. 증명을 활성화/잠금 해제하면:

   * 증명 상태가 활성으로 변경됩니다.
   * 증명에 추가된 모든 사람은 검토할 새로운 증명이 있음을 알리는 알림 이메일을 받게 됩니다. (증명을 활성화/잠금 해제할 때까지 이메일이 전송되지 않습니다.)
   * 그 증명은 정상적으로 적용될 수 있다
   * 제출자가 또한 자신을 증표에 명시적으로 추가하는 경우 새로운 증명 이메일을 받지 않습니다. 자세한 내용은 [새로운 증명 이메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## Dropzone 관리

Dropzone 페이지를 사용하면 Dropzone에 대한 제출을 손쉽게 관리할 수 있습니다. Dropzone 페이지에는 다음 옵션 및 기능이 포함되어 있습니다.

* 페이지 레이아웃(1)
* 보기(2)에서 보관된 증명을 포함하거나 제외하도록 선택합니다
* 작업 단추(3)
* 정렬(4)
* 필터(5)
* 증명 작업 메뉴(6)
* 증명 보관 해제(7)
* 증명 요약 확장/축소(8)
* 증명 선택(9)

페이지 레이아웃, 정렬 및 필터링 옵션은 [!DNL Views] 목록. 자세한 내용은 [의 보기 페이지에서 항목 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 추가 정보.

![New_Dropzone_design__Feb_2013_.jpg](assets/new-dropzone-design--feb-2013--350x224.jpg)
