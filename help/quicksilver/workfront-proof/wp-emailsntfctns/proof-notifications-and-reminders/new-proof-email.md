---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: 새 증명 이메일
description: 이 문서가 PiW에 더 잘 작동하도록 합니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 1030d4110fd5dabb3b5751387585cc66968c2326
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 새 증명 이메일

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

새 증명 또는 증명의 새 버전을 만들거나, 증명에 새 사용자를 추가하거나, 증명에 워크플로를 추가할 때 다음 문서에 설명된 대로 검토자에게 이메일을 전송할지 여부를 결정할 수 있습니다.

* [자동화된 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [ [!DNL Workfront Proof]에서 증명 생성](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

받는 사람이 받는 전자 메일을 [!UICONTROL 새 증명] 전자 메일이라고 합니다. 증명 생성자 및 증명에 검토자를 추가할 권한이 있는 사용자만 이 이메일을 제어할 수 있습니다. 수신자는 비활성화할 수 없습니다.

새 증명 이메일에는 다음이 포함되어 있습니다.

* 개인 메시지(포함을 선택한 경우)
* 항상 동일한 사용자 지정 메시지를 검토자에게 보내는 경우 [!UICONTROL 증명 기본값] 탭 아래의 [!UICONTROL 개인 설정]에 저장하는 것이 좋습니다. 자세한 내용은 를 참조하십시오.
* 증명에 대한 개인 링크
* 연결된 [!DNL Workfront] 개체(예: 프로젝트, 작업 또는 문제)로 이동하는 **[!UICONTROL 세부 정보 보기]** 링크
* 증명 이미지의 썸네일
* 다음 증명 세부 정보:

   * 교정쇄 이름
   * 버전 번호
   * 검토자 목록 및 증명 진행 상황
   * 다른 사용자와 증명을 공유할 수 있는 링크

     이를 통해 원본 파일에 대한 증명 URL 및/또는 다운로드 링크를 공유할 수 있습니다. 이 경우 증명에 검토자를 명시적으로 추가할 수 없으며 공개 증명 URL만 공유하게 되고 수신자는 증명에 대한 읽기 전용 액세스 권한을 받게 됩니다.

     자세한 내용은 [증명 공유 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)를 참조하십시오.

     이 링크가 받는 사람의 전자 메일에 표시되지 않도록 하려면 증명에서 [!UICONTROL 공개 공유] 설정을 사용하지 않도록 설정할 수 있습니다.

     원본 파일 및 공개 URL 다운로드). 자세한 내용은 [증명 세부 정보 관리 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)를 참조하십시오.

## 활동 로그

검토자에게 [!UICONTROL 새 증명] 전자 메일을 보내는 것은 [!UICONTROL 증명 세부 정보] 페이지의 [!UICONTROL 활동] 섹션에 기록됩니다. 자세한 내용은  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)의 [관리[!UICONTROL  증명 세부 정보]를 참조하십시오. 증명을 만들 때 [!UICONTROL 새 증명] 전자 메일이 활성화되었는지 확인할 수 있습니다.

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* 증명 작성자 또는 소유자의 개인 설정에서 기본적으로 [!UICONTROL 증명 작성]이(가) 비활성화된 이메일이 있는 경우 새 증명 페이지에서 [!UICONTROL 이메일로 사람들에게 알림] 상자를 선택하더라도 [!UICONTROL 증명 작성] 또는 [!UICONTROL 새 증명]이(가) 수신되지 않습니다. 자세한 내용은 를 참조하십시오.
>* [!UICONTROL 계정 설정]에서 이메일 알림을 기본값으로 사용하지 않도록 설정한 경우, 증명 작성자/소유자는 개인 설정에서 [!UICONTROL 증명 작성] 또는 [!UICONTROL 새 증명]을 사용하도록 설정하고 새 증명 페이지에서 [!UICONTROL 메일로 사람들에게 알림]을 확인란이 선택되어 있더라도 이메일을 받지 못합니다. 자세한 내용은 [증명 [!UICONTROL 확인] 메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)을 참조하세요.
>



## [!UICONTROL 새 증명] 전자 메일을 사용하도록 설정하고 사용자 지정 메시지 포함

증명을 만들 때 또는 증명에 사용자를 추가할 때 검토자에게 이메일 경고를 보낼지 여부를 지정할 수 있습니다.

* [증명 생성 시](#when-you-create-a-proof)
* [증명에 검토자를 추가할 때](#when-you-add-a-reviewer-to-a-proof)

### 증명 생성 시 {#when-you-create-a-proof}

[!UICONTROL 새 증명] 페이지의 **[!UICONTROL 공유]** 섹션 아래에서 새 증명을 만들 때 전자 메일 경고를 보낼지 여부를 선택할 수 있습니다.

* 여기에서 [!UICONTROL 사람들에게 이메일로 알림](1)을 원하는지 결정할 수 있습니다. 이 옵션을 선택 취소하면 검토자 중 아무도 증명을 검토할 준비가 되었음을 알리는 이메일을 받지 못합니다.
* 이메일 알림(2)에 사용자 지정 메시지를 포함할 수도 있습니다.
* 사용자 정의 메시지를 추가하기로 결정하는 경우 사용자 정의 제목 줄(3)과 메시지를 이메일 본문(4)에 넣을 수 있습니다.
* 사용자 지정 메시지를 취소하려면 링크(5)를 클릭하면 됩니다.

  >[!NOTE]
  >
  >항상 동일한 사용자 지정 메시지를 검토자에게 보내는 경우 [!UICONTROL 증명 기본값] 탭 아래의 개인 설정에 저장하는 것이 좋습니다. 자세한 내용은 를 참조하십시오.

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### 증명에 검토자를 추가할 때 {#when-you-add-a-reviewer-to-a-proof}

기존 증명에 추가된 새 검토자에게 증명을 알릴지 여부를 선택할 수 있습니다(위와 유사).

* 먼저 **[!UICONTROL 증명 세부 정보]** 페이지(1)에서 **[!UICONTROL 이 버전 공유]** 단추를 클릭하여 새 검토자를 추가하십시오.

![Proof_Details_page_1.png](assets/proof-details-page-1-350x118.png)

* 새 검토자를 추가할 수 있는 상자가 나타납니다. 그런 다음 (2) 전자 메일로 알림을 받을지 결정하고 전자 메일에 사용자 지정 메시지를 추가하도록 선택할 수 있습니다 (3).

![Proof_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* 사용자 지정 메시지를 추가하도록 선택하면 상자가 확장되고 이메일 본문에 사용자 지정 제목 줄(4)과 사용자 지정 텍스트(5)를 넣을 수 있습니다. 링크 (6)을 클릭하여 사용자 지정 메시지를 삭제할 수도 있습니다.

![Proof_Details_page_3.png](assets/proof-details-page-3-350x258.png)
