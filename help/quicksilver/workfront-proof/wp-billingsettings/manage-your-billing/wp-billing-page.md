---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: 다음 [!DNL Workfront] 증명 청구 페이지
description: 에 액세스하려면 [!UICONTROL 과금] 페이지의 오른쪽 상단에 있는 설정 메뉴를 열고 드롭다운 메뉴에서 과금을 선택합니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 다음 [!DNL Workfront Proof] 청구 페이지

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

## 청구 페이지

에 액세스하려면 [!UICONTROL 과금] 페이지를 열고 **[!UICONTROL 설정]** 화면 오른쪽 상단의 메뉴를 선택하고 **[!UICONTROL 과금]** 를 클릭합니다.

다음 [!UICONTROL 과금] 페이지에는 다음 내용이 포함되어 있습니다.

* 계정 이름(1)
* 계정 목록(예: 위성 계정이 있는 경우)(2)
* 계획 변경(3)
* 지급 상세내역 변경(4)
* 새 위성 계정(5)
* 계정 닫기(6)
* 현재 계획 정보(7)
* 청구 연락처 및 주소(8)
* 사용 통계(9)
* 청구 내역(10)
* 청구 활동(11)

   ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL 현재 계획]

이 섹션(7)에는 다음을 포함하여 현재 계획의 세부 사항이 표시됩니다.

* 계획의 이름
* 현재 결제 방법
* 현재 계획 시작 및 완료 날짜
* 다음 계획 유형
* 다음 계획 결제 방법

   자세한 내용은 [에서 결제 방법 선택 [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL 청구 연락처 및 주소]

이 섹션(8)에는 계정에 대한 주 청구 담당자 및 주소 세부 정보가 표시됩니다.

청구 담당자는 계정의 청구 관리자로 설정된 사용자만 선택할 수 있습니다. 위성 계정에서는 기본 계정의 청구 관리자만 이 필드에 설정할 수 있습니다.

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> 계정에 여러 청구 관리자를 사용할 수 있지만 이 중 하나만 [!UICONTROL 청구 담당자] 필드에서는 모든 청구 알림 및 계정 사용 경고를 수신하게 됩니다.

여기에는 다음 알림 이메일이 포함됩니다.

* 증명 사용
* 송장
* 다운그레이드
* 지연 지급/계정 일시 중단 경고
* 신용 카드 실패

   ![Bilin_CC.png](assets/billin-cc-350x103.png)

다음 [!UICONTROL 청구 CC] 또한, 모든 청구 관련 이메일에 복사할 이메일 주소를 추가할 수 있습니다. 필드를 클릭하여 포함 편집을 활성화하고 선택한 이메일 주소를 입력합니다(기존 사용자의 이메일 주소일 수도 있음).

## [!UICONTROL 청구 주소]

이 섹션에서는 인라인 편집을 사용하여 필드를 클릭하여 텍스트를 입력/편집하면 됩니다.

>[!NOTE]
>
> 구독 송장에 이 주소를 포함하므로 이 데이터가 항상 최신 상태인지 확인합니다.

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL 사용 통계]

이 섹션에서는 다음을 포함하여 현재 청구 기간 내의 계정에 대한 사용 통계를 보여줍니다.

* 사용된 스토리지
* 사용된 증명
* 사용된 사용자 제한

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL 사용 경고]

다음 [[!UICONTROL 증명 권한 프로필] in [!DNL Workfront] 증명](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 계정에 대한 청구 담당자 (1)로 설정하면 계정이 다음과 같이 되면 이메일을 통해 통지됩니다.

* 스토리지 용량의 75% 및 98%
* 75%와 100%의 증명 제한

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

증명 또는 저장소 제한에 도달하면 맨 위에 경고가 표시됩니다 [!UICONTROL 과금] 페이지:

* 증명 제한에 도달했습니다.

   ![Prop_limit_reach.png](assets/proofs-limit-reached-350x65.png)

* 스토리지 제한에 도달했습니다.

![Storage_limit_reach.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>증명 수는 계정에 증명을 만들 때 사용되며 증명을 제거하여 복원할 수 없습니다.

증명 및 파일을 삭제하고 비우고 저장 공간을 확보할 수 있습니다 [!UICONTROL 휴지통] 나중에

증명, 스토리지 또는 사용자가 더 필요한 경우 언제든지 계정을 업그레이드할 수 있습니다. 그리고 그것은 즉시 영향을 받습니다.

## [!UICONTROL 청구 내역]

이 섹션에서는 최근 청구 기간에 대한 활동을 보여줍니다. 또한 이 섹션에서 송장을 다운로드할 수 있습니다.

자세한 내용은 &quot; [다운로드 [!DNL Workfront Proof] 송장](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).&quot;

## [!UICONTROL 청구 활동]

이 섹션에서는 청구 설정(예: 구독, 업그레이드, 다운그레이드 및 갱신)에 대한 최근 변경 사항을 보여줍니다 [!DNL Workfront Proof] 계획.

계획을 사용자 제한(1)이 낮은 사용자 제한으로 변경하면 새 계획이 시작될 때 새 제한을 초과하는 사용자는 자동으로 비활성화됩니다. 이 활동은 계정 로그(2)에도 캡처됩니다.

![Billing_Downgrade_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
