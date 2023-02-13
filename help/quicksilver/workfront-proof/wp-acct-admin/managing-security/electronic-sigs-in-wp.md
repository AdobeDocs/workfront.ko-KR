---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: 의 전자 서명 이해 [!DNL Workfront Proof]
description: 전자 서명을 사용하면 증명 보안을 강화하고 ISO와 같은 업계 표준을 준수할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 의 전자 서명 이해 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

전자 서명을 사용하면 증명 보안을 강화하고 ISO와 같은 업계 표준을 준수할 수 있습니다.

이 설정은 계정 수준에서 필수 또는 비필수로 설정할 수 있습니다. 기본적으로 필수로 설정되어 있는 경우, 계정에서 만든 모든 증명에서 활성화되며 증명 수준에서 비활성화할 수 없습니다. 이 설정이 기본적으로 필수가 아닌 경우 증명 수준에서 활성화/비활성화할 수 있습니다.

자세한 내용은 를 참조하십시오.

증명의 전자 서명 설정이 활성화되면 전자 서명 상자는 증명의 결정을 내리는 검토자에게 전자 메일 및 암호를 제공하라는 메시지를 표시합니다.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## 전자 서명 [!UICONTROL 증명 세부 사항] 페이지

검토자가 [!UICONTROL 증명 세부 사항] 페이지(1) 및 [!UICONTROL 전자 서명] 팝업 상자가 표시되어 세부 정보(2)를 입력하고 결정(3)을 확인하라는 메시지를 표시합니다.

팝업에는 기본 메시지 세트(있는 경우)가 표시되며 검토자는 이메일과 암호를 입력해야 합니다.

다음 [!UICONTROL 전자 서명] 팝업이 언어 교정 뷰어에 표시되며 [!UICONTROL 증명 세부 사항] 검토자가 해당 수준에서 결정을 내리기로 결정하는 경우 페이지입니다.

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

만약 [!UICONTROL 단일 사인온] 증명 시 옵션이 활성화되어 있으면 전자 메일 및 암호 세부 사항이 [!UICONTROL 전자 서명] 결정을 내릴 때 갑자기 나타난다.

대신, [!UICONTROL 확인] (4) 이 팝업에서 검토자가 [!UICONTROL 단일 사인온] 페이지.

SSO 자격 증명을 입력하면 검토자가 자동으로 다시 [!UICONTROL 증명 세부 사항] 페이지(또는 [!UICONTROL 증명 뷰어] 여기서 결정하면)

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> 만약 그 결정이 전자적으로 서명된다면, **[!UICONTROL 서명 아이콘]** (5)이 페이지의 [!UICONTROL 워크플로우] 섹션에 [!UICONTROL 증명 세부 사항] 페이지. 검토자가 아니라 증명의 편집 권한이 있는 다른 사람이 결정을 변경한 경우 해당 사람이 전자 서명을 하도록 요청되지 않으며 결정(6) 옆에는 서명 아이콘이 없습니다.

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)단일 사인온에 대한 자세한 내용은 [Workfront에서 단일 사인온 증명](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

증명 세부 사항 페이지에 대한 자세한 내용은 [의 증명 세부 정보 관리 [!DNL Workfront] 증명](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
