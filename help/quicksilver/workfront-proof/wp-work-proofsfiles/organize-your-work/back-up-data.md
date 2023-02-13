---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 백업 [!DNL Workfront Proof] 데이터
description: 에서 모든 데이터의 백업을 요청할 수 있습니다 [!DNL Workfront Proof] 백업 기능을 사용합니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 0%

---

# 백업 [!DNL Workfront Proof] 데이터

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

## 백업 소개

에서 모든 데이터의 백업을 요청할 수 있습니다 [!DNL Workfront Proof] 백업 기능을 사용합니다.

백업은 .zip 파일로 전달됩니다. 여기에는 모든 데이터의 XML 내보내기(모든 증명 버전에 대한 설명 및 응답 포함)가 포함됩니다. 그러나 증명으로 업로드한 원본 파일은 포함되지 않습니다.

다운로드하도록 작성된 각 백업 .zip 파일에는 다음과 같은 고유한 파일 이름이 있습니다.

9789_05_05_2011_61703.zip

이 예제의 파일 이름은 다음 정보를 제공합니다.

* 9789는 [!DNL Workfront Proof] 계정 식별자
* 05_05_2011은 2011년 5월 5일 만든 날짜입니다
* 61703은 시스템에서 할당한 번호입니다

이러한 명명 규칙을 사용하면 모든 백업 .zip 파일을 컴퓨터의 단일 위치에 저장하고 각 백업이 사용자에 대해 만들어진 시점을 정확하게 파악할 수 있습니다.

다음 [!UICONTROL 백업] 함수를 사용하면 리소스를 사용하는 방법을 결정할 수 있습니다.

* 액티브 또는 아카이브 증명을 유실하지 않고 스토리지 공간을 확보할 수 있습니다. 백업을 요청하거나 증명을 삭제한 다음 [휴지통 복원 및 비우기 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* 원래 업로드한 파일에 액세스할 수 있습니다 [!DNL Workfront] 증명. 을 사용하여 다운로드할 수 있습니다. [!UICONTROL 원본 파일 다운로드] 함수 위에 있어야 합니다.

>[!NOTE]
>
>백업을 사용할 때는 다음 사항을 고려하십시오.
>
>* 백업은 엔터프라이즈 및 무제한 계획에서 사용할 수 있습니다. 다음 주소로 문의하십시오 [영업 팀](mailto:sales@proofhq.com) 인용을 참조하십시오.
>* 데이터 인코딩 유형은 기본적으로 UTF-8로 설정되며 이 설정을 사용하는 것이 좋습니다. 인터넷 응용 프로그램에서 가장 일반적으로 사용되는 인코딩 유형입니다.
>* 하나만 요청할 수 있습니다 [!DNL backup] 한번에 백업 .zip 파일이 처리되는 경우 백업 탭의 새 백업 요청 링크가 표시되지 않고 표시된 메시지는 변경되지 않은 상태로 유지됩니다. 백업 요청에 대한 내용은 [에서 새 데이터 백업 요청 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>




## 데이터 백업

1. 클릭 **[!UICONTROL 계정 설정]** 오른쪽 위 모서리에서 [!DNL Workfront Proof] 인터페이스. (1)
1. 을(를) 클릭합니다. **[!UICONTROL 백업]** 탭. (2)
1. 을(를) 클릭합니다. **[!UICONTROL 새 백업 요청]** 링크(3)

백업이 준비되면 다음 작업이 수행됩니다.

* 보낸 사람 이메일 받기 [!DNL Workfront Proof] 이 사실을 알려드립니다. [!DNL Workfront Proof] 백업 준비 완료&quot;) 전자 메일에는 백업 데이터에 대한 다운로드 링크가 포함되어 있습니다.
* 다음 [계정 설정](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) 백업 탭에는 백업 데이터에 대한 다운로드 링크가 표시됩니다.
* 새 백업 요청 링크(3)가 백업 탭에 다시 나타납니다

데이터를 zip 파일로 다운로드할 수 있습니다. 알림 전자 메일 또는 [!UICONTROL 계정 설정]다음 섹션에 설명된 대로 작성할 수 있습니다.

* [이메일 알림에서 백업 .zip 파일 다운로드](#downloading-your-backup-zip-file-from-your-email-notification)
* [계정 설정에서 백업 .zip 파일 다운로드](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## 이메일 알림에서 백업 .zip 파일 다운로드 {#downloading-your-backup-zip-file-from-your-email-notification}

백업 .zip 파일을 다운로드할 준비가 되면 [!DNL Workfront Proof] 제목 줄 &#39;Your [!DNL Workfront Proof] 백업이 준비되었습니다.&#39;

이메일에서 백업 .zip 파일을 다운로드하려면

1. 이메일에서 다운로드 링크를 클릭합니다.\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   현재 로그인하지 않은 경우 [!DNL Workfront Proof]새 브라우저 창이 열리고 로그인 페이지가 표시됩니다.

## 계정 설정에서 백업 .zip 파일 다운로드 {#downloading-your-backup-zip-file-from-the-account-settings}

백업 .zip 파일을 다운로드할 준비가 되면 [!UICONTROL 백업] 탭은 다운로드 링크를 표시하여 나타냅니다. 또한 [!UICONTROL 새 백업 요청] 링크가 다시 나타납니다.

1. 클릭 **[!UICONTROL 계정 설정]** 오른쪽 위 모서리에서 [!DNL Workfront Proof] 인터페이스. (1)
1. 을(를) 클릭합니다. **[!UICONTROL 백업]** 탭. (2)\
   계정에 있는 사용자가 백업을 요청하지 않은 경우 [!UICONTROL 백업] 탭에는 백업이 없음을 나타냅니다. 사용자가 백업을 요청한 경우 마지막 백업에 대한 작성 날짜와 다운로드 링크가 탭에 표시됩니다.

1. 을(를) 클릭합니다. **[!UICONTROL 백업 다운로드]** 링크를 클릭합니다. (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) 다운로드 파일을 열지 또는 저장할지 묻는 파일 다운로드 화면이 나타납니다.

1. 클릭 **[!UICONTROL 저장]**&#x200B;그런 다음 백업 .zip 파일을 저장할 컴퓨터의 위치를 선택합니다.\
   가장 최근 백업 날짜를 식별하는 메시지가 [!UICONTROL 백업] 다음에 백업을 요청할 때까지의 페이지입니다. 백업 다운로드 링크는 마지막 백업에 적용됩니다. 항상 [!UICONTROL 새 백업 요청] 링크가 표시되면 링크를 클릭하여 다른 백업을 요청할 수 있습니다.

## 백업 .zip 파일의 파일 이해

백업 .zip 파일에는 데이터를 백업할 때까지 활성 및 보관된 증명의 정보를 포함하는 7개의 CSV(쉼표로 구분된 값 또는 쉼표로 구분된) 파일이 포함되어 있습니다.

* comments.csv - 증명에 대한 댓글 포함
* comment_replies.csv - 증명 organization.csv에 대한 댓글에 대한 응답 포함 - 숫자 식별자 및 조직 이름(계정) 포함
* contact.csv - 각 연락처의 숫자 식별자, 이름 및 조직을 포함합니다.
* files.csv - 증명 세부 사항 페이지 또는 파일에 업로드된 증명 또는 파일에 대한 파일 세부 정보 페이지의 정보를 포함합니다 [!DNL Workfront Proof]
* recipients.csv - 검토를 위해 증명을 업로드할 때 검토자, 검토자 및 승인자 등으로 지정된 각 사람의 숫자 식별자, 역할 및 결정을 포함합니다 [!DNL Workfront Proof]
* users.csv - 숫자 식별자 및 계정에 있는 모든 사용자의 이름을 포함합니다.

사용하는 zip 유틸리티를 사용하여 백업 .zip 파일에서 이러한 파일을 추출한 다음 컴퓨터에서 원하는 위치에 저장할 수 있습니다. zip 파일을 저장하고 개별 CSV 파일을 추출하면 내부 레코드 유지에 대해 원하는 대로 정보를 조작할 수 있습니다.

요청에 작성된 각 백업 .zip 파일의 이름은 백업 작성 날짜를 포함하는 고유한 이름을 가지지만, 각 백업 .zip 파일에 포함된 CSV 파일의 이름은 항상 동일합니다. 다음 방법 중 하나를 사용하여 백업 파일이 서로 구분되도록 할 수 있습니다.

* 각 백업 .zip 파일과 해당 파일에서 추출하는 CSV 파일에 대한 새 폴더를 만듭니다.
* zip 파일에서 백업 날짜를 추출하려면 각 개별 CSV 파일의 이름을 바꾸십시오.

>[!NOTE]
>
>If [!DNL Microsoft Excel] 이 컴퓨터에 설치되어 있으면 추출 유틸리티에서 개별 CSV 파일의 파일 유형을 [!DNL Microsoft Office Excel] 쉼표로 구분된 값 파일입니다. 를 사용하여 추출된 CSV 파일을 열 수 있습니다 [!DNL Excel] 파일을 [!DNL Excel] 통합 문서 (&#42;.xlsx) 또는 기타 파일 형식을 사용할 수 있습니다.
