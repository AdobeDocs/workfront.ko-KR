---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: 다음을 사용하여 사용자 정보 구성 [!DNL Workfront Proof]
description: 다음을 사용하여 사용자 정보 구성 [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# 다음을 사용하여 사용자 정보 구성 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품의 기능에 대해 설명합니다 [!DNL Workfront Proof]. 내부 교정에 대한 정보 [!DNL Adobe Workfront], 참조 [증명](../../../review-and-approve-work/proofing/proofing.md).

1. 에 설명된 대로 사용자 만들기 또는 편집 시작 [다음을 사용하여 사용자 만들기 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. 다음 정보를 지정합니다.

   * 다음에서 **[!UICONTROL 개인 세부 정보]** 섹션:

      * **이메일 주소:** 사용자의 이메일 주소입니다.
      * **이름:** 사용자의 이름입니다.
      * **성:** 사용자의 성입니다.
      * **위치:** 회사에서 사용자의 위치입니다.
      * **권한 프로필:** 증명 계정에 대한 사용자의 권한입니다.
      * **언어:** 사용자의 기본 언어입니다.
      * **시간대:** 사용자의 시간대를 선택합니다.
      * **날짜 형식:** 사용자의 선호 날짜 형식을 선택합니다.
      * **옵트인 - 제품 및 마케팅 이메일:** 제품 및 마케팅 이메일에 대해 사용자를 옵트인할지 여부를 선택합니다.
      * **API 전용:** 사용자가 API를 통해서만 로그인할 수 있습니다.

   * 다음에서 **[!UICONTROL 사용자 세부 정보]** 섹션에는 사용자의 주소 및 전화 번호와 같은 연락처 정보를 입력합니다.
   * 다음에서 **[!UICONTROL 기본 증명 설정]** 섹션에서 사용자가 증명을 만들거나 작업하는 방식에 영향을 주는 설정을 구성합니다.

      * **기본 증명 역할:** 사용자의 기본 증명 역할을 선택하십시오. 역할 옵션은 다음과 같습니다 **[!UICONTROL 읽기 전용]**, **[!UICONTROL 검토자]**, **[!UICONTROL 승인자]**, **[!UICONTROL 검토자 및 승인자]**, **[!UICONTROL 작성자]**, 또는 **[!UICONTROL 중재자]**.

        증명 역할에 대한 자세한 내용은 [에서 증명 역할 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **모든 결정이 내려지면 증명 잠금:** 증명에 대한 모든 결정이 내려진 후 추가 변경으로부터 증명을 자동으로 잠급니다.
      * **로그인 필요. 증명은 다른 사용자와만 공유할 수 있습니다.** 다음 사용자가 증명을 사용할 수 있도록 함: [!DNL Workfront Proof] 로그인 자격 증명입니다.
      * **필요한 결정은 단 하나입니다.** 증명에 대해 하나의 결정만 필요합니다.
      * **원본 파일 다운로드:** 사용자가 증명을 위한 원본 파일을 다운로드할 수 있습니다. 이 옵션은 기본적으로 활성화되어 있습니다.

        원본 파일 다운로드에 대한 자세한 내용은 [저장된 파일 다운로드 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **구독. 사용자는 공개 URL 또는 포함 코드를 통해 증명에 등록할 수 있습니다.** 조직 외부의 검토자가 공개 URL 또는 포함 코드를 통해 증명에 등록할 수 있도록 허용합니다.

        이 옵션을 선택하면 **구독자가 증명에 액세스하려면 이메일의 링크를 클릭해야 합니다.** 을 사용할 수도 있습니다. 외부 검토자가 증명에 액세스하기 위해 이메일 내의 링크를 클릭하도록 하려면 이 옵션을 선택합니다.
이 옵션은 다음과 같은 경우에 기본적으로 활성화됩니다. **공개 공유** 옵션이 선택되어 있습니다.

      * **새 게스트 검토자에 대한 기본 역할:** 게스트 검토자에 대한 기본 증명 역할을 선택하십시오. 옵션은 의 옵션과 동일합니다 **기본 증명 역할**, 중재자 및 작성자 제외

   * 다음에서 **[!UICONTROL 기본 이메일 경고 설정]** 섹션:

      * **기본 이메일 경고:** 사용자가 이메일 업데이트를 받는 빈도를 선택합니다. 선택 **모든 활동, 내 의견에 응답, 결정, 최종 결정, 시간별 요약, 일별 요약,** 또는 **비활성화됨**.

        기본 이메일 경고 옵션에 대한 자세한 내용은 [에서 이메일 알림 설정 구성 [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **새 게스트 검토자에 대한 기본 이메일 경고:** 게스트 검토자가 이메일 업데이트를 받는 빈도를 선택하십시오. 옵션은 의 옵션과 동일합니다 **기본 이메일 경고.**

      * **증명이 준비되면 이메일 확인 보내기:** 증명이 준비되면 사용자에게 확인 이메일을 자동으로 보내려면 선택합니다.
      * **이 사용자에게 보낸 전자 메일 형식:** 선택 **[!UICONTROL HTML]** 또는 **[!UICONTROL 일반 텍스트]** 을(를) 사용자에게 보내는 이메일의 기본 형식으로 사용하십시오.

   * 다음에서 **[!UICONTROL 사용자 정의 메시지 설정]** 섹션: 증명 템플릿 설정 만들기

     템플릿에 대한 자세한 내용은 다음을 참조하십시오.

      * **증명 제목 템플릿:** 증명 제목용 템플릿을 만듭니다.
      * **증명 메시지 템플릿:** 증명 메시지용 템플릿과 해당 형식을 만듭니다.
