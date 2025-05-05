---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: ' [!DNL Workfront Proof]을(를) 사용하여 사용자 정보 구성'
description: ' [!DNL Workfront Proof]을(를) 사용하여 사용자 정보 구성'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# [!DNL Workfront Proof]을(를) 사용하여 사용자 정보 구성

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

1. [다음을 사용하여 사용자 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md)에 설명된 대로 사용자를 만들거나 편집하십시오.
1. 다음 정보를 지정합니다.

   * **[!UICONTROL 개인 정보]** 섹션에서:

      * **이메일 주소:** 사용자의 이메일 주소입니다.
      * **이름:** 사용자의 이름입니다.
      * **성:** 사용자의 성입니다.
      * **위치:** 회사에서 사용자의 위치입니다.
      * **권한 프로필:** 증명 계정에 대한 사용자의 권한입니다.
      * **언어:** 사용자의 기본 언어입니다.
      * **표준 시간대:** 사용자의 표준 시간대를 선택합니다.
      * **날짜 형식:** 사용자의 기본 날짜 형식을 선택합니다.
      * **옵트인 - 제품 및 마케팅 이메일:** 제품 및 마케팅 이메일에 대해 사용자를 옵트인할지 여부를 선택합니다.
      * **API만:** 사용자가 API를 통해서만 로그인할 수 있도록 허용합니다.

   * **[!UICONTROL 사용자 세부 정보]** 섹션에서 주소 및 전화 번호와 같은 사용자 연락처 정보를 입력하십시오.
   * **[!UICONTROL 기본 증명 설정]** 섹션에서 사용자가 증명을 만들거나 작업하는 방식에 영향을 주는 설정을 구성합니다.

      * **기본 증명 역할:** 사용자에 대한 기본 증명 역할을 선택합니다. 역할 옵션은 **[!UICONTROL 읽기 전용]**, **[!UICONTROL 검토자]**, **[!UICONTROL 승인자]**, **[!UICONTROL 검토자 및 승인자]**, **[!UICONTROL 작성자]** 또는 **[!UICONTROL 중재자]**&#x200B;입니다.

        증명 역할에 대한 자세한 내용은 [증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.

      * **모든 결정을 내릴 때 증명 잠금:** 증명에 대한 모든 결정이 내려진 후 추가 변경으로부터 증명을 자동으로 잠급니다.
      * **로그인이 필요합니다. 증명을 다른 사용자와만 공유할 수 있습니다.** [!DNL Workfront Proof] 로그인 자격 증명을 가진 사용자만 증명을 사용할 수 있습니다.
      * **하나의 결정만 필요합니다.** 증명에 하나의 결정만 필요합니다.
      * **원본 파일 다운로드:** 사용자가 증명을 위한 원본 파일을 다운로드할 수 있습니다. 이 옵션은 기본적으로 활성화되어 있습니다.

        원본 파일 다운로드에 대한 자세한 내용은 [저장된 파일 다운로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md)를 참조하십시오.

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **구독. 공개 URL 또는 포함 코드를 통해 증명에 등록할 수 있습니다.** 조직 외부의 검토자가 공개 URL 또는 포함 코드를 통해 증명에 등록할 수 있습니다.

        이 옵션을 선택하면 **구독자가 증명에 액세스하려면 전자 메일의 링크를 클릭해야 합니다**&#x200B;도 사용할 수 있습니다. 외부 검토자가 증명에 액세스하기 위해 이메일 내의 링크를 클릭하도록 하려면 이 옵션을 선택합니다.
이 옵션은 **공개 공유** 옵션을 선택한 경우 기본적으로 활성화됩니다.

      * **새 게스트 검토자의 기본 역할:** 게스트 검토자의 기본 증명 역할을 선택하십시오. 옵션은 **기본 증명 역할**&#x200B;의 옵션과 동일하지만 중재자와 작성자는 예외입니다.

   * **[!UICONTROL 기본 전자 메일 경고 설정]** 섹션에서:

      * **기본 전자 메일 경고:** 사용자가 전자 메일 업데이트를 받는 빈도를 선택합니다. **모든 활동, 내 댓글에 답글 달기, 결정, 최종 결정, 시간별 요약, 일별 요약,** 또는 **사용 안 함**&#x200B;을 선택합니다.

        기본 전자 메일 경고 옵션에 대한 자세한 내용은 [전자 메일 알림 설정 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)을 참조하세요.

      * **새 게스트 검토자에 대한 기본 전자 메일 알림:** 게스트 검토자가 전자 메일 업데이트를 받는 빈도를 선택하십시오. 옵션은 **기본 전자 메일 경고에 대한 옵션과 동일합니다.**

      * **증명이 준비되면 확인 이메일을 보냅니다.** 증명이 준비되면 확인 이메일을 사용자에게 자동으로 보내려면 선택합니다.
      * **이 사용자에게 보낸 전자 메일 형식:** 사용자에게 보낸 전자 메일의 기본 형식으로 **[!UICONTROL HTML]** 또는 **[!UICONTROL 일반 텍스트]**&#x200B;를 선택합니다.

   * **[!UICONTROL 사용자 지정 메시지 설정]** 섹션: 증명 템플릿에 대한 설정을 만듭니다.

     템플릿에 대한 자세한 내용은 다음을 참조하십시오.

      * **증명 제목 템플릿:** 증명 제목용 템플릿을 만듭니다.
      * **증명 메시지 템플릿:** 증명 메시지 및 해당 형식에 대한 템플릿을 만듭니다.
