---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: ' [!DNL Workfront Proof]의 전자 서명 이해'
description: 전자 서명을 사용하면 증명에 대한 보안을 강화하고 ISO와 같은 업계 표준을 준수할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# [!DNL Workfront Proof]의 전자 서명 이해

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

전자 서명을 사용하면 증명에 대한 보안을 강화하고 ISO와 같은 업계 표준을 준수할 수 있습니다.

이 설정은 계정 수준에서 필수 또는 비필수로 지정할 수 있습니다. 기본적으로 필수인 경우, 계정에서 만든 모든 증명에서 활성화되며 증명 수준에서 비활성화될 수 없습니다. 이 설정이 기본적으로 필수가 아닌 경우 증명 수준에서 활성화/비활성화할 수 있습니다.

자세한 내용은 를 참조하십시오.

증명에서 전자 서명 설정이 활성화되면 증명을 결정하는 모든 검토자에게 전자 메일 및 암호를 입력하라는 전자 서명 상자가 표시됩니다.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## [!UICONTROL 증명 세부 정보] 페이지의 전자 서명

검토자가 [!UICONTROL 증명 세부 정보] 페이지에서 결정을 선택하면(1) [!UICONTROL 전자 서명] 팝업 상자가 표시되어 세부 정보를 입력하고(2) 결정을 확인합니다(3).

팝업에 기본 메시지 집합(있는 경우)이 표시되며, 검토자는 전자 메일과 암호를 입력해야 합니다.

검토자가 해당 수준에서 결정하기로 결정하면 증명 뷰어와 [!UICONTROL 증명 세부 정보] 페이지에 [!UICONTROL 전자 서명] 팝업이 표시됩니다.

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

증명에서 [!UICONTROL SSO(Single Sign-On)] 옵션을 사용하도록 설정한 경우 결정 시 전자 메일 및 암호 세부 정보가 [!UICONTROL 전자 서명] 팝업에 표시되지 않습니다.

대신 이 팝업에서 [!UICONTROL 확인] (4) 단추를 클릭하면 검토자가 [!UICONTROL Single Sign-On] 페이지로 리디렉션됩니다.

SSO 자격 증명을 입력하면 검토자가 자동으로 [!UICONTROL 증명 세부 정보] 페이지로 다시 리디렉션됩니다(또는 해당 페이지에서 결정이 내려지는 경우 [!UICONTROL 증명 뷰어] (으)로 다시 리디렉션됨).

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> 결정에 전자 서명이 있으면 [!UICONTROL 증명 세부 정보] 페이지의 [!UICONTROL 워크플로] 섹션에서 결정 옆에 **[!UICONTROL 서명 아이콘]**(5)이 나타납니다. 심사자가 아니라 증명에 대한 편집 권한이 있는 다른 사람이 결정을 변경하면 해당 사람에게 결정에 전자적으로 서명하도록 요청하지 않으며 결정 옆에 서명 아이콘이 없습니다(6).

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Single Sign-On에 대한 자세한 내용은 [Workfront Proof의 Single Sign-On](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md)을 참조하세요.

증명 세부 정보 페이지에 대한 자세한 내용은 [Proof에서 증명 세부 정보 관리 [!DNL Workfront] Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)를 참조하십시오.
