---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: ' [!DNL Workfront Proof] 데이터 백업'
description: 백업 기능을 사용하여  [!DNL Workfront Proof] 에서 모든 데이터의 백업을 요청할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# [!DNL Workfront Proof] 데이터 백업

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

## 백업 소개

백업 기능을 사용하여 [!DNL Workfront Proof]에 있는 모든 데이터의 백업을 요청할 수 있습니다.

백업은 .zip 파일로 전달됩니다. 여기에는 모든 데이터(모든 증명 버전의 주석 및 응답 포함)의 XML 내보내기가 포함되지만 증명으로 업로드한 원본 파일은 포함되지 않습니다.

다운로드할 수 있도록 작성된 각 백업 .zip 파일에는 다음과 같은 고유한 파일 이름이 있습니다.

9789_05_05_2011_61703.zip

이 예제의 파일 이름은 다음 정보를 제공합니다.

* 9789는 [!DNL Workfront Proof] 계정 식별자입니다.
* 05_05_2011은 작성 날짜이며 2011년 5월 5일입니다
* 61703은 임의의 시스템 지정 번호입니다.

이 이름 지정 규칙을 사용하면 모든 백업 .zip 파일을 컴퓨터의 단일 위치에 쉽게 저장하고 각 백업이 언제 생성되었는지 정확하게 알 수 있습니다.

[!UICONTROL Backup] 함수를 사용하면 리소스를 사용하는 방법을 결정할 수 있습니다.

* 활성 또는 보관된 증명을 손실하지 않고 저장소 공간을 확보할 수 있습니다. 백업을 요청하고 증명을 삭제한 다음 [휴지통 복원 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)을(를) 비울 수 있습니다.
* 원래 [!DNL Workfront] 증명에 업로드한 모든 파일에 액세스할 수 있습니다. 증명을 삭제하기 전에 [!UICONTROL 원본 파일 다운로드] 기능을 사용하여 다운로드할 수 있습니다.

>[!NOTE]
>
>백업을 사용할 때는 다음 사항을 고려하십시오.
>
>* Enterprise 및 Unlimited 플랜에서 백업을 사용할 수 있습니다. 견적은 [영업팀](mailto:sales@proofhq.com)에 문의하십시오.
>* 데이터 인코딩 유형은 기본적으로 UTF-8로 설정되며 이 설정을 사용하는 것이 좋습니다. 이는 인터넷 애플리케이션에서 가장 일반적으로 사용되는 인코딩 유형입니다.
>* 한 번에 한 개의 [!DNL backup]만 요청할 수 있습니다. 백업 .zip 파일이 처리 중일 때 백업 탭에 새 백업 요청 링크가 나타나지 않고 표시되는 메시지가 변경되지 않습니다. 백업 요청에 대한 자세한 내용은 [새 데이터 백업 요청 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md)을 참조하십시오.
>



## 데이터 백업

1. [!DNL Workfront Proof] 인터페이스의 오른쪽 위 모서리에서 **[!UICONTROL 계정 설정]**&#x200B;을 클릭합니다. (1)
1. **[!UICONTROL 백업]** 탭을 클릭합니다. (2)
1. **[!UICONTROL 새 백업 요청]** 링크를 클릭합니다(3).

백업이 준비되면 다음 상황이 발생합니다.

* [!DNL Workfront Proof](으)로부터 이를 알리는 이메일을 받습니다(&quot;[!DNL Workfront Proof] 백업이 준비되었습니다&quot;). 이메일에는 백업 데이터에 대한 다운로드 링크가 포함되어 있습니다.
* [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 백업 탭에 백업 데이터에 대한 다운로드 링크가 표시됩니다.
* 백업 탭에 새 백업 요청 링크(3)가 다시 나타납니다

데이터를 zip 파일로 다운로드할 수 있습니다. 다음 섹션에 설명된 대로 알림 전자 메일 또는 [!UICONTROL 계정 설정]에서 백업 .zip 파일을 다운로드할 수 있습니다.

* [이메일 알림에서 백업 .zip 파일 다운로드](#downloading-your-backup-zip-file-from-your-email-notification)
* [계정 설정에서 백업 .zip 파일 다운로드](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## 이메일 알림에서 백업 .zip 파일 다운로드 {#downloading-your-backup-zip-file-from-your-email-notification}

백업 .zip 파일을 다운로드할 준비가 되면 제목 줄 &#39;내 [!DNL Workfront Proof] 백업이 준비되었습니다&#39;가 포함된 이메일을 [!DNL Workfront Proof]에서 받게 됩니다.

이메일에서 백업 .zip 파일을 다운로드하려면:

1. 이메일에서 다운로드 링크를 클릭합니다.\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   현재 [!DNL Workfront Proof]에 로그인하지 않은 경우 새 브라우저 창이 열리고 로그인 페이지가 표시됩니다.

## 계정 설정에서 백업 .zip 파일 다운로드 {#downloading-your-backup-zip-file-from-the-account-settings}

백업 .zip 파일을 다운로드할 준비가 되면 [!UICONTROL 백업] 탭에 다운로드 링크가 표시되어 이를 나타냅니다. 또한 [!UICONTROL 새 백업 요청] 링크가 다시 나타납니다.

1. [!DNL Workfront Proof] 인터페이스의 오른쪽 위 모서리에서 **[!UICONTROL 계정 설정]**&#x200B;을 클릭합니다. (1)
1. **[!UICONTROL 백업]** 탭을 클릭합니다. (2)\
   계정의 사용자가 백업을 요청하지 않은 경우 [!UICONTROL 백업] 탭은 백업이 없음을 나타냅니다. 사용자가 백업을 요청한 경우 탭에 마지막 백업에 대한 작성 날짜 및 다운로드 링크가 표시됩니다.

1. **[!UICONTROL 백업 다운로드]** 링크를 클릭합니다. (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) 다운로드 파일을 열거나 저장할지 묻는 파일 다운로드 화면이 나타납니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭한 다음 컴퓨터에서 백업 .zip 파일을 저장할 위치를 선택하십시오.\
   가장 최근 백업 날짜를 식별하는 메시지는 다음 번에 백업을 요청할 때까지 [!UICONTROL 백업] 페이지 하단에 계속 표시됩니다. 백업 다운로드 링크는 마지막 백업에 적용됩니다. [!UICONTROL 새 백업 요청] 링크가 표시될 때마다 해당 링크를 클릭하여 다른 백업을 요청할 수 있습니다.

## 백업 .zip 파일의 파일 이해

백업 .zip 파일에는 활성 증명과 아카이브된 증명의 정보를 포함하여 데이터가 백업될 때까지의 정보가 포함된 7개의 CSV(쉼표로 구분된 값 또는 쉼표로 구분된) 파일이 포함되어 있습니다.

* comments.csv - 증명에 대한 댓글이 포함됩니다.
* comment_replies.csv - proofs organization.csv에 대한 댓글에 대한 응답을 포함합니다. - 숫자 식별자와 조직(계정)의 이름을 포함합니다.
* contacts.csv - 각 연락처의 숫자 식별자, 이름 및 조직이 포함됩니다.
* files.csv - 증명 세부 정보 페이지 또는 [!DNL Workfront Proof]에 업로드된 증명 또는 파일에 대한 파일 세부 정보 페이지의 정보를 포함합니다.
* recipients.csv - [!DNL Workfront Proof]에 검토를 위해 증명을 업로드할 때 검토자, 검토자 및 승인자 등으로 지정된 각 개인의 숫자 식별자, 역할 및 결정을 포함합니다.
* users.csv - 계정에 있는 모든 사용자의 숫자 식별자 및 이름을 포함합니다.

사용하는 zip 유틸리티로 백업 .zip 파일에서 이러한 파일을 추출한 다음 컴퓨터에서 선택한 위치에 저장할 수 있습니다. zip 파일을 저장하고 개별 CSV 파일을 추출한 후 내부 레코드 보관에 필요한 정보를 조작할 수 있습니다.

요청 시 작성된 각 백업 .zip 파일에는 백업 생성 날짜가 포함된 고유한 이름이 있지만 각 백업 .zip 파일에 포함된 CSV 파일의 이름은 항상 동일합니다. 다음 방법 중 하나를 사용하여 백업 파일이 서로 구분되도록 할 수 있습니다.

* 각 백업 .zip 파일 및 이 파일에서 추출하는 CSV 파일에 대해 새 폴더를 만듭니다.
* zip 파일에서 추출할 때 백업 날짜를 포함하도록 각 개별 CSV 파일의 이름을 변경합니다.

>[!NOTE]
>
>[!DNL Microsoft Excel]이(가) 컴퓨터에 설치되어 있으면 추출 유틸리티에서 개별 CSV 파일의 파일 형식을 [!DNL Microsoft Office Excel] 쉼표로 구분된 값 파일로 나열할 수 있습니다. [!DNL Excel]을(를) 사용하여 추출한 CSV 파일을 열고 [!DNL Excel] 통합 문서(&#42;.xlsx) 또는 다른 파일 형식으로 저장할 수 있습니다.
