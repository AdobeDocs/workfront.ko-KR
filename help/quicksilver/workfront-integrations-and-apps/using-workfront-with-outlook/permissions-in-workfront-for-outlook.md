---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 에 대한 권한 수준 [!DNL Workfront] Outlook용
description: '다음 [!DNL Workfront for Outlook] 추가 기능을 사용하려면 읽기/쓰기 사서함 액세스 권한이 필요합니다. 다음 [!DNL Workfront for Outlook] 통합에는 Outlook exchange 서버에서 전자 메일 첨부 파일을 다운로드하여 업로드하는 기능이 있으므로 가장 높은 수준의 권한이 필요합니다 [!DNL Workfront]: 사용자가 첨부 파일이 있는 이메일에서 요청을 제출할 때.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# 에 대한 권한 수준 [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] 에는 허용되는 네 가지 권한 수준 중 가장 높은 수준의 권한이 필요합니다. [!DNL Outlook] 추가 기능.

의 권한에 대한 자세한 내용은 [!DNL Outlook] 추가 기능은 [에 대한 개인 정보, 권한 및 보안 [!DNL Outlook] 추가 기능](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) 에서 [!DNL Microsoft] 설명서.

다음 [!DNL Workfront for Outlook] 추가 기능을 사용하려면 읽기/쓰기 사서함 액세스(`ReadWriteMailbox`). 가장 높은 권한 범위입니다.
다음 [!DNL Workfront for Outlook] 통합에는 [!DNL Outlook] exchange server에서 업로드하여 [!DNL Workfront]: 사용자가 첨부 파일이 있는 이메일에서 요청을 제출할 때. 이 기능을 사용하려면 [!DNL Workfront for Outlook] 함수 사용 `mailbox.getCallbackTokenAsync()` 변환 전: [!DNL Office] 토큰을 가져오고 이를 사용하여 Exchange 서버에서 전자 메일 첨부 파일을 다운로드할 수 있는 추가 JavaScript API입니다. 해당 함수를 사용할 수 있는 유일한 권한은 입니다 `ReadWriteMailbox`. 자세한 내용은 [Outlook 추가 기능에 대한 개인 정보, 권한 및 보안](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) ( Microsoft 설명서)를 참조하십시오.

다음 [!DNL Workfront for Outlook] 추가 기능도 필요합니다 `ReadWriteItem` 권한(포함) `ReadWriteMailbox`). 전자 메일 본문을 읽고 전자 메일 메타데이터를 읽기/업데이트하는 데 사용됩니다.

* 전자 메일 본문 읽기:

   [!DNL Workfront for Outlook] 사용자가 요청을 제출하거나 이메일 본문을 업데이트로 보낼 때 이메일 본문을 읽습니다 [!DNL Adobe Workfront] 개체.
* 전자 메일 메타데이터 읽기/업데이트:

   [!DNL Workfront for Outlook] 사용자가 이메일에서 요청을 제출할 때 이메일 헤더를 업데이트합니다. 이 작업은 제출된 정보에 대한 정보를 저장하는 데 수행됩니다 [!DNL Adobe Workfront] 개체이므로 다음번에 사용자가 동일한 전자 메일에 대한 추가 기능을 열 때에는 해당 전자 메일이 있는 이전 작업에 대한 정보가 표시됩니다.

[!DNL Workfront for Outlook] 사용자가 추가 기능 내에서 작업을 수행할 때만 사용자의 사서함에 액세스합니다. 배경 기능이 없습니다. Workfront for Outlook은 다음 시나리오에서만 사용자의 사서함에 액세스합니다.

* 사용자는 요청 제출, 작업 만들기 또는 전자 메일을 업데이트로 보내려고 합니다. [!DNL Workfront for Outlook] (추가 기능 열기 및 작업 선택)
   * [!DNL Workfront for Outlook] 는 추가 기능 내의 양식에 채울 이메일 본문을 읽습니다.
   * [!DNL Workfront for Outlook] 전자 메일 메타데이터를 읽어 추가 기능에서 동일한 전자 메일을 사용하여 수행한 이전 작업에 대한 추가 기능에 대한 정보를 표시합니다.
* 사용자가 요청을 제출하거나 작업을 만들거나 업데이트로 이메일을 보냅니다. [!DNL Workfront for Outlook] ( [!UICONTROL 제출] 추가 기능 버튼):
   * [!DNL Workfront for Outlook] 요청 설명 또는 주석으로 Workfront에 보낼 이메일 본문을 읽습니다.
   * [!DNL Workfront for Outlook] 전자 메일 메타데이터를 업데이트하여 제출된 요청 또는 업데이트된 개체에 대한 정보를 저장합니다.
   * [!DNL Workfront for Outlook] exchange 서버에서 전자 메일 첨부 파일을 다운로드하여 제출된 요청, 생성된 작업 또는 업데이트된 개체에 업로드합니다.
