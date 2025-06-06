---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Outlook용  [!DNL Workfront] 의 사용 권한 수준
description: ' [!DNL Workfront for Outlook] 추가 기능을 사용하려면 읽기/쓰기 사서함 액세스가 필요합니다.  [!DNL Workfront for Outlook] 통합은 사용자가 첨부 파일이 있는 전자 메일에서 요청을 제출할 때 Outlook exchange 서버에서 전자 메일 첨부 파일을 다운로드하여  [!DNL Workfront]에 업로드할 수 있으므로 최상위 수준의 권한이 필요합니다.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# [!DNL Workfront for Outlook]에 대한 권한 수준

>[!IMPORTANT]
>
>[Microsoft에서 기존 Exchange 온라인 토큰에 대한 지원을 사용하지 않도록 설정하는 중입니다](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens). 이 토큰은 현재 인증을 위해 Workfront Outlook 추가 기능에서 사용됩니다. Microsoft의 이러한 변경 사항은 이미 고객에게 영향을 주기 시작했으며 2025년 10월까지 단계적으로 계속 적용될 예정입니다.
>
>* **Microsoft에서 이 토큰을 완전히 비활성화하면 Microsoft Outlook용 Workfront 통합이 더 이상 작동하지 않습니다.**
>
>이 변경의 일부로 Microsoft은 토큰이 다시 활성화되는 방식을 변경하기로 결정했습니다. **2025년 6월 30일** 이후에는 관리자가 더 이상 토큰을 직접 다시 활성화할 수 없습니다. Microsoft 지원에서만 예외를 허용할 수 있습니다. **2025년 10월 1일부터 모든 테넌트에 대해 레거시 토큰이 꺼집니다. 예외가 부여되지 않습니다.**

[!DNL Workfront for Outlook]에는 [!DNL Outlook] 추가 기능에서 허용되는 네 가지 권한 수준 중 가장 높은 수준이 필요합니다.

[!DNL Outlook] 추가 기능의 사용 권한에 대한 자세한 내용은 [!DNL Microsoft] 설명서의 [추가 기능에 대한 개인 정보, 사용 권한 및 보안 [!DNL Outlook] 을 참조하십시오.](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security)

[!DNL Workfront for Outlook] 추가 기능을 사용하려면 가장 높은 권한 범위인 읽기/쓰기 사서함 액세스(`ReadWriteMailbox`)가 필요합니다.
[!DNL Workfront for Outlook] 통합은 사용자가 첨부 파일이 있는 전자 메일에서 요청을 제출할 때 [!DNL Outlook] exchange 서버에서 전자 메일 첨부 파일을 다운로드하여 [!DNL Workfront]에 업로드할 수 있으므로 최상위 수준의 권한이 필요합니다. 이 기능을 사용하려면 [!DNL Workfront for Outlook]이(가) [!DNL Office] 추가 기능 JavaScript API의 `mailbox.getCallbackTokenAsync()` 함수를 사용하여 토큰을 얻고 이를 사용하여 Exchange Server에서 전자 메일 첨부 파일을 다운로드합니다. 해당 함수를 사용할 수 있는 유일한 권한은 `ReadWriteMailbox`입니다. 자세한 내용은 Microsoft 설명서에서 [Outlook 추가 기능에 대한 개인 정보, 권한 및 보안](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security)을 참조하세요.

[!DNL Workfront for Outlook] 추가 기능에는 전자 메일 본문을 읽고 전자 메일 메타데이터를 읽기/업데이트하는 데 사용되는 `ReadWriteItem` 권한(`ReadWriteMailbox`에 포함됨)도 필요합니다.

* 이메일 본문 읽기:

  [!DNL Workfront for Outlook]은(는) 사용자가 요청을 제출하거나 [!DNL Adobe Workfront] 개체에 대한 업데이트로 전자 메일 본문을 보낼 때 전자 메일 본문을 읽습니다.
* 이메일 메타데이터 읽기/업데이트:

  [!DNL Workfront for Outlook]은(는) 사용자가 전자 메일에서 요청을 제출하면 전자 메일 헤더를 업데이트합니다. 이 작업은 제출된 [!DNL Adobe Workfront] 개체에 대한 정보를 저장하기 위해 수행되므로 사용자가 다음에 동일한 전자 메일에 대한 추가 기능을 열면 해당 전자 메일을 사용한 이전 작업에 대한 정보가 표시됩니다.

[!DNL Workfront for Outlook]은(는) 사용자가 추가 기능 내에서 작업을 수행할 때만 사용자의 사서함에 액세스합니다. 여기에는 백그라운드 기능이 없습니다. Outlook용 Workfront은 다음 시나리오에서만 사용자 사서함에 액세스합니다.

* 사용자가 [!DNL Workfront for Outlook]에서 업데이트로 요청을 제출하거나 작업을 만들거나 전자 메일을 보내려고 합니다(추가 기능을 열고 작업 선택)
   * [!DNL Workfront for Outlook]이(가) 전자 메일 본문을 읽고 추가 기능 내의 양식에 채웁니다.
   * [!DNL Workfront for Outlook]은(는) 전자 메일 메타데이터를 읽어서 추가 기능에서 동일한 전자 메일을 사용하여 수행한 이전 작업에 대한 추가 기능에 대한 정보를 표시합니다.
* 사용자가 [!DNL Workfront for Outlook]에서 업데이트로 요청을 제출하거나 작업을 만들거나 이메일을 보낼 때(추가 기능에서 [!UICONTROL 제출] 단추 클릭):
   * [!DNL Workfront for Outlook]이(가) 전자 메일 본문을 읽어 Workfront에 요청 설명 또는 댓글로 보냅니다.
   * [!DNL Workfront for Outlook]은(는) 전자 메일 메타데이터를 업데이트하여 제출된 요청 또는 업데이트된 개체에 대한 정보를 저장합니다.
   * [!DNL Workfront for Outlook]은(는) exchange 서버에서 전자 메일 첨부 파일을 다운로드하여 제출된 요청, 생성된 작업 또는 업데이트된 개체에 업로드합니다.
