---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: ' [!DNL Workfront] 증명 청구 페이지'
description: '[!UICONTROL 청구] 페이지에 액세스하려면 화면 오른쪽 상단에서 설정 메뉴를 열고 드롭다운 메뉴에서 청구를 선택합니다.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# [!DNL Workfront Proof] 청구 페이지

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

## 과금 페이지

[!UICONTROL 청구] 페이지에 액세스하려면 화면 오른쪽 상단의 **[!UICONTROL 설정]** 메뉴를 열고 드롭다운 메뉴에서 **[!UICONTROL 청구]**&#x200B;를 선택하십시오.

[!UICONTROL 청구] 페이지에는 다음이 포함되어 있습니다.

* 계정 이름 (1)
* 계정 목록(예: 위성 계정이 있는 경우)(2)
* 변경 계획 (3)
* 결제 세부 사항 변경(4)
* 새 위성 계정(5)
* 계정 닫기(6)
* 현재 플랜 정보 (7)
* 청구 담당자 및 주소 (8)
* 사용량 통계 (9)
* 청구 내역(10)
* 청구 활동(11)

  ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL 현재 계획]

이 섹션(7)은 다음을 포함하여 현재 플랜의 세부 사항을 보여 줍니다.

* 플랜의 이름
* 현재 결제 방법
* 현재 계획 시작 및 완료 일자
* 다음 플랜 유형
* 다음 플랜 결제 방법

  자세한 내용은 [결제 방법 선택 [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md)을 참조하세요.

## [!UICONTROL 청구 연락처 및 주소]

이 섹션 (8)에는 계정에 대한 기본 청구 연락처 및 주소 세부 정보가 표시됩니다.

청구 담당자는 계정에서 청구 관리자로 설정된 사용자만 선택할 수 있습니다. 위성 계정의 경우 이 필드에는 기본 계정의 청구 관리자만 설정할 수 있습니다.

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> 계정에 여러 명의 청구 관리자가 있을 수 있지만 [!UICONTROL 청구 연락처] 필드에서 선택한 청구 관리자 중 한 명만 모든 청구 알림 및 계정 사용 알림을 받게 됩니다.

여기에는 다음과 같은 알림 이메일이 포함됩니다.

* 증명 사용
* 인보이스
* 다운그레이드
* 지연 지급/계정 일시 중단 경고
* 신용 카드 오류

  ![Billin_CC.png](assets/billin-cc-350x103.png)

[!UICONTROL 청구 CC] 필드에서는 모든 청구 관련 전자 메일에 복사할 전자 메일 주소를 추가할 수도 있습니다. 필드를 클릭하여 인라인 편집을 활성화하고 선택한 이메일 주소를 입력합니다(기존 사용자의 이메일 주소도 될 수 있음).

## [!UICONTROL 청구 주소]

이 섹션에서는 인라인 편집을 사용하므로 필드를 클릭하여 텍스트를 입력/편집하면 됩니다.

>[!NOTE]
>
> 이 주소는 구독 청구서에 포함되므로 이 데이터가 항상 최신 상태인지 확인하십시오.

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL 사용량 통계]

이 섹션에서는 다음을 포함하여 현재 청구 기간 내의 계정에 대한 사용 통계를 보여 줍니다.

* 사용된 스토리지
* 사용된 증명
* 사용된 사용자 제한

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL 사용 경고]

계정에 대한 청구 담당자(1)로 설정된 [[!UICONTROL 증명 권한 프로필] in [!DNL Workfront] 증명](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)은(는) 계정이 다음 항목에 도달하면 전자 메일을 통해 알림을 받게 됩니다.

* 스토리지 용량의 75%, 98%
* 증명 한도의 75% 및 100%

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

증명 또는 저장소 제한에 도달하면 [!UICONTROL 청구] 페이지 상단에 알림도 표시됩니다.

* 증명 한도에 도달함

  ![Proofs_limit_reached.png](assets/proofs-limit-reached-350x65.png)

* 스토리지 한도 도달

![Storage_limit_reached.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>증명 수는 계정에서 증명을 만들 때 모두 사용되며 증명을 제거하여 복원할 수 없습니다.

증명 및 파일을 삭제하고 나중에 [!UICONTROL 휴지통]을(를) 비우면 저장소 공간을 확보할 수 있습니다.

더 많은 증명, 스토리지 또는 사용자가 필요한 경우 언제든지 계정을 업그레이드할 수 있습니다. 그러면 즉시 적용됩니다.

## [!UICONTROL 청구 기록]

이 섹션에는 최근 청구 기간에 대한 활동이 표시됩니다. 이 섹션에서 청구서를 다운로드할 수도 있습니다.

자세한 내용은 &quot;[청구서 다운로드 [!DNL Workfront Proof] 2&rbrace;&quot;를 참조하십시오.](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md)

## [!UICONTROL 청구 활동]

이 섹션에서는 [!DNL Workfront Proof] 플랜의 구독, 업그레이드, 다운그레이드 및 갱신 등 청구 설정에 대한 최근 변경 사항을 보여줍니다.

플랜을 더 낮은 사용자 제한(1)이 있는 플랜으로 변경하면 새로운 제한을 초과하는 사용자는 새로운 플랜이 시작될 때 자동으로 비활성화됩니다. 이 활동은 계정 로그(2)에도 캡처됩니다.

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
