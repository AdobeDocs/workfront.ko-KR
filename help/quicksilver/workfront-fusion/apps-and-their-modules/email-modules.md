---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 이메일 모듈
description: 다음 [!DNL Adobe Workfront Fusion] 시나리오에서 전자 메일 계정을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다. 이 기능을 사용하면 IMAP를 통해 전자 메일을 다운로드하고, SMTP를 통해 전자 메일을 보내고, 새 초안을 만들고, 한 폴더에서 다른 폴더로 전자 메일을 이동 및 복사하고, 전자 메일을 읽기 또는 읽지 않음으로 표시하고 전자 메일을 삭제할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2613'
ht-degree: 0%

---

# 이메일 모듈

다음 [!DNL Adobe Workfront Fusion] 시나리오에서 전자 메일 계정을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다. 이 기능을 사용하면 IMAP를 통해 전자 메일을 다운로드하고, SMTP를 통해 전자 메일을 보내고, 새 초안을 만들고, 한 폴더에서 다른 폴더로 전자 메일을 이동 및 복사하고, 전자 메일을 읽기 또는 읽지 않음으로 표시하고 전자 메일을 삭제할 수 있습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
  <td> <p>[!UICONTROL Pro] 이상</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Workfront Fusion에 이메일 연결 {#connect-your-email-to-workfront-fusion}

* [Google에 연결](#connect-to-google)
* [다른 이메일 서비스(SMAP)에 연결](#connect-to-other-email-services-smap)

### 연결 대상 [!DNL Google]

에 연결해야 하는 이메일 모듈을 사용하여 시나리오를 만들려면 이 옵션을 사용합니다 [!DNL Google] 계정이 필요합니다. 범위가 제한된 계정입니다.

에 대한 연결을 만들 수 있습니다 [!DNL Google] 이메일 모듈 내에서 직접 계정을 설정합니다.

1. 이메일 모듈에서 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 선택 **[!DNL Google]** 연결 유형으로 사용할 수 있습니다.
1. 연결의 이름을 입력합니다.
1. (선택 사항) 을 입력합니다 [!UICONTROL [!DNL Google] 클라이언트 ID] 및 [!UICONTROL 클라이언트 암호].
1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

### 다른 이메일 서비스(SMAP)에 연결

SMAP 연결을 통해 원격으로 사서함에 액세스하고 사서함에서 메시지를 읽거나 조작할 수 있습니다. SMAP 연결은 대부분의 이메일 모듈에서 사용됩니다.

1. 이메일 모듈에서 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 선택 **[!UICONTROL 기타(SMTP)]** 연결 유형으로 사용할 수 있습니다.
1. 을(를) 입력합니다. **[!UICONTROL 이름]** 연결할 수 없습니다.
1. 을(를) 선택합니다 **[!UICONTROL 전자 메일 공급자]** 참조하십시오. 이메일 공급자가 목록에 없으면 기타 를 선택합니다.
1. 을(를) 입력합니다. **[!UICONTROL 이메일 주소]**, **[!UICONTROL 전체 이름]**, **[!UICONTROL 사용자 이름]**, 및 **[!UICONTROL 암호]**.
1. (조건부) 공급자가 목록에 없으면 **[!UICONTROL SMTP 서버]** 및 **[!UICONTROL 포트]**, 및에 지정할 **[!UICONTROL TLS(보안 연결) 사용]**. 이 정보를 찾으려면 [!UICONTROL 도움말] 사서함의 섹션 이 정보를 사용할 수 없는 경우 이메일 서비스 공급자에게 문의하십시오.
1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!UICONTROL 이메일] 모듈 및 해당 필드

구성 시 [!UICONTROL 이메일] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 앱이나 서비스에서 액세스 수준 등의 요소에 따라 추가 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

시나리오의 다른 모듈에서 데이터를 사용했으므로 일부 이메일 필드에 이미 데이터가 포함되어 있을 수 있습니다. 전자 메일에 대한 정보가 필요한 경우 전자 메일 도움말 설명서를 참조하십시오.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>&#39;라고 하는 고유한 이메일 ID[!UICONTROL 이메일 ID(UID)]은 이메일의 식별자입니다. 이메일 ID는 각 이메일 폴더에 대해 다릅니다.

* [Triggers](#triggers)
* [액션](#actions)
* [반복기](#iterators)

### Triggers

#### [!UICONTROL 이메일 보기]

지정된 기준에 따라 처리하기 위해 새 이메일을 받으면 트리거됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>보려는 전자 메일이 포함된 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>전자 메일을 볼 기준을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 모든 이메일]</li> 
     <li>[!UICONTROL만 읽기 전자 메일]</li> 
     <li>[!UICONTROL만 읽지 않은 이메일]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>전자 메일을 볼 발신자의 전자 메일 주소를 입력합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Recipient Email Address]</td> 
   <td> <p> 전자 메일을 볼 수신자의 전자 메일 주소를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>보려는 전자 메일의 제목을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>특정 구문이 포함된 이메일만 보려면 키워드를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지를 가져올 때 읽은 상태로 표시]</td> 
   <td> <p>세부 정보를 검색한 후 읽지 않은 이메일을 읽음으로 표시하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최대 결과 수]</td> 
   <td> <p> 최대 이메일 수 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 이메일 보내기]](#send-an-email)
* [[!UICONTROL 초안 만들기]](#create-a-draft)
* [[!UICONTROL 이메일을 읽음으로 표시]](#mark-an-email-as-read)
* [[!UICONTROL 이메일을 읽지 않음으로 표시]](#mark-an-email-as-unread)
* [[!UICONTROL 이메일 이동]](#move-an-email)
* [[!UICONTROL 이메일 복사]](#copy-an-email)
* [[!UICONTROL 이메일 삭제]](#delete-an-email)
* [[!UICONTROL 이메일 가져오기]](#get-emails)
* [[!UICONTROL 전자 메일 보내기]](#send-me-an-email)

#### [!UICONTROL 이메일 보내기]

새 이메일을 보냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>이메일 계정 연결에 대한 지침 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 전송 후 메시지 저장]</td> 
   <td>전자 메일 메시지가 전송되면 사서함에 저장됩니다. 을 사용하여 보낸 이메일을 저장하려면 이 옵션을 활성화합니다 [!DNL Workfront Fusion] 변환 후 <i>[!UICONTROL 보낸 메일]</i> 사서함의 폴더 또는 다른 폴더입니다. 다음과 같은 일부 이메일 서비스 [!DNL Gmail]: 보낸 메시지를 자동으로 저장합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>이메일을 보낼 이메일 주소를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>전자 메일의 제목 줄을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>전자 메일의 [!UICONTROL content] 유형을 선택합니다.</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>[!UICONTROL 컨텐츠 유형] 필드에서 선택한 내용에 따라 HTML 태그를 사용하여 전자 메일 콘텐츠를 HTML 형식으로 입력하거나 일반 텍스트로 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 첨부 파일]</p> </td> 
   <td> <p>첨부 파일 추가:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일 이름]</strong> </p> <p>파일 이름을 입력합니다. 예: sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>첨부 파일을 업로드할 폴더 경로를 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>콘텐츠에 첨부 파일(이미지)을 삽입할 [!UICONTROL 콘텐츠 ID]를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>이 전자 메일의 사본을 보낼 하나 이상의 전자 메일 주소를 입력하거나 매핑합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy Recipient]</td> 
   <td> <p> 전자 메일 주소를 전자 메일에 표시하지 않고 이 전자 메일 사본을 보낼 전자 메일 주소를 하나 이상 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>전자 메일의 [!UICONTROL 보낸 사람] 필드에 나타나는 전자 메일 주소(및 필요한 경우 이름)를 입력하거나 매핑합니다. </p> <p>중요 사항: 올바른 구문을 사용합니다. <code>name@email.com</code> 또는 <code>"Name" name@email.com</code>.</p> <p>참고: 보통 [!DNL Workfront Fusion] 은 연결을 발신자 주소로 만들 때 입력한 이메일 주소를 사용합니다. 다른 이메일 주소를 입력하는 경우 계정에 다른 주소에서 전자 메일을 보낼 수 있는 권한이 없기 때문에 메시지를 보낼 때 오류가 발생할 수 있습니다. 예: <code>test@mail.com</code> 또는 "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>전자 메일의 [!UICONTROL 보낸 사람] 필드에 나타나는 전자 메일 주소를 입력하거나 매핑합니다.</p> <p>팁: 이 필드 또는 시작 필드를 사용할지 확실하지 않은 경우 시작 필드를 선택하는 것이 좋습니다.</p> <p>중요 사항: 올바른 구문을 사용합니다. <code>name@email.com</code> 또는 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> "보낸 사람" 주소가 아닌 다른 주소로 이 전자 메일에 대한 답장을 보내려면 이 전자 메일에 회신할 전자 메일 주소를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 특정 전자 메일에 회신하는 경우 회신할 전자 메일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 참조] </td> 
   <td> <p>스레드에 있는 모든 답장의 메시지 ID를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>이메일의 우선 순위를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>헤더 추가:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>키를 추가합니다. 예를 들어 [!UICONTROL Sender], [!UICONTROL Date], [!UICONTROL To] 등이 있습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>키의 값을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 초안 만들기]

선택한 폴더에 새 초안을 만들고 추가합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>초안 이메일을 만들 폴더를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>이메일을 보낼 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>전자 메일의 제목 줄을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>전자 메일의 콘텐츠 유형을 선택합니다.</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL 일반 텍스트]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>[!UICONTROL 컨텐츠 유형] 필드에서 선택한 내용에 따라 HTML 태그를 사용하여 전자 메일 콘텐츠를 HTML 형식으로 입력하거나 일반 텍스트로 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 첨부 파일]</p> </td> 
   <td> <p>첨부 파일 추가:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 파일 이름]</strong> </p> <p>파일 이름을 입력합니다. 예: sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>첨부 파일을 업로드할 폴더 경로를 입력합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>컨텐츠에 첨부 파일(이미지)을 삽입할 컨텐츠 ID를 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>이 전자 메일의 사본을 보낼 하나 이상의 전자 메일 주소를 입력하거나 매핑합니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy Recipient]</td> 
   <td> <p> 전자 메일 주소를 전자 메일에 표시하지 않고 이 전자 메일 사본을 보낼 전자 메일 주소를 하나 이상 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>전자 메일의 [!UICONTROL 보낸 사람] 필드에 나타나는 전자 메일 주소(및 필요한 경우 이름)를 입력하거나 매핑합니다. </p> <p>중요 사항: 올바른 구문을 사용합니다. <code>name@email.com</code> 또는 <code>"Name" name@email.com</code>.</p> <p>참고: 보통 [!DNL Workfront Fusion] 은 연결을 발신자 주소로 만들 때 입력한 이메일 주소를 사용합니다. 다른 이메일 주소를 입력하는 경우 계정에 다른 주소에서 전자 메일을 보낼 수 있는 권한이 없기 때문에 메시지를 보낼 때 오류가 발생할 수 있습니다. 예: <code>test@mail.com</code> 또는 "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>전자 메일의 [!UICONTROL 보낸 사람] 필드에 나타나는 전자 메일 주소를 입력하거나 매핑합니다.</p> <p>팁: 이 필드 또는 시작 필드를 사용할지 확실하지 않은 경우 시작 필드를 선택하는 것이 좋습니다.</p> <p>중요 사항: 올바른 구문을 사용합니다. <code>name@email.com</code> 또는 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> "[!UICONTROL from]" 주소가 아닌 다른 주소로 이 전자 메일에 대한 응답을 받으려면 이 전자 메일에 회신할 전자 메일 주소를 입력합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 특정 전자 메일에 회신하는 경우 회신할 전자 메일의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 참조] </td> 
   <td> <p>스레드에 있는 모든 답장의 메시지 ID를 입력합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>이메일의 우선 순위를 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>헤더 추가:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>키를 추가합니다. 예를 들어 보낸 사람, 날짜, 받는 사람 등이 있습니다.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>키의 값을 입력합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일을 읽음으로 표시]

선택한 폴더에 있는 전자 메일 또는 초안을 [!UICONTROL 읽기] 플래그.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>읽음으로 표시할 전자 메일 폴더를 선택합니다. 예: 기본.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 이메일 ID(UID)]</p> </td> 
   <td> <p>읽음으로 표시할 이메일의 이메일 UID를 입력합니다.</p> <p>[!UICONTROL Email] &gt;[!UICONTROL Watch Email] 모듈 또는 [!UICONTROL Search Email] 모듈을 사용하여 이메일의 UID를 가져올 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일을 읽지 않음으로 표시]

읽지 않음 플래그를 설정하여 선택한 폴더의 이메일 또는 초안을 읽지 않음으로 표시합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>읽지 않음으로 표시할 전자 메일 폴더를 선택합니다. 예: 기본.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 이메일 ID(UID)]</p> </td> 
   <td> <p>읽지 않음으로 표시할 이메일의 이메일 UID를 입력합니다.</p> <p>[!UICONTROL Email] &gt;[!UICONTROL Watch Email] 모듈 또는 [!UICONTROL Search Email] 모듈을 사용하여 이메일의 UID를 가져올 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 이동]

선택한 전자 메일 또는 초안을 선택한 폴더로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 폴더]</td> 
   <td>전자 메일을 이동할 전자 메일이 포함된 폴더를 선택합니다. 예: 기본.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 폴더]</td> 
   <td> <p> 이메일을 추가할 폴더를 선택합니다. 예: 일.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 이메일 ID(UID)]</p> </td> 
   <td> <p>대상 폴더로 이동할 이메일의 이메일 UID를 입력합니다.</p> <p>[!UICONTROL Email] &gt;[!UICONTROL Watch Email] 모듈 또는 [!UICONTROL Search Email] 모듈을 사용하여 이메일의 UID를 가져올 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 복사]

전자 메일 또는 초안을 선택한 폴더에 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 폴더]</td> 
   <td>이메일을 복사할 폴더를 선택합니다. 예: 기본.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 폴더]</td> 
   <td> <p> 이메일을 복사할 폴더를 선택합니다. 예: 일.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 이메일 ID(UID)]</p> </td> 
   <td> <p>대상 폴더에 복사할 이메일의 이메일 UID를 입력합니다.</p> <p>[!UICONTROL Email] &gt;[!UICONTROL Watch Email] 모듈 또는 [!UICONTROL Search Email] 모듈을 사용하여 이메일의 UID를 가져올 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 삭제]

선택한 폴더에서 이메일이나 초안을 제거합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>삭제할 전자 메일의 폴더를 선택합니다. 예: 기본.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 이메일 ID(UID)]</p> </td> 
   <td> <p>삭제할 이메일의 이메일 UID를 입력합니다.</p> <p>[!UICONTROL Email] &gt;[!UICONTROL Watch Email] 모듈 또는 [!UICONTROL Search Email] 모듈을 사용하여 이메일의 UID를 가져올 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>모듈에서 현재 열려 있는 사서함에서 [!UICONTROL 삭제됨]으로 플래그가 지정된 모든 메시지를 영구적으로 제거할 수 있도록 하려면 이 옵션을 활성화하십시오.</p> <p>참고: in [!DNL Gmail]로 지정하는 경우 이 동작은 [!UICONTROL 설정] &gt;[!UICONTROL Forwarding POP/IMAP in IMAP 액세스] 섹션의 설정에 의해 제어됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 이메일 가져오기]

지정된 기준과 일치하는 이메일을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>전자 메일 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 다음을 참조하십시오 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">이메일을 [!UICONTROL Workfront Fusion]에 연결</a> 참조하십시오.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>검색할 이메일이 포함된 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메시지를 가져올 때 읽은 상태로 표시] </td> 
   <td> <p>세부 사항을 검색한 후 읽지 않은 이메일을 읽음으로 표시하려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>검색할 전자 메일의 기준을 선택합니다.</p> 
    <ul> 
     <li>[!UICONTROL 모든 이메일]</li> 
     <li>[!UICONTROL만 읽기 전자 메일]</li> 
     <li>[!UICONTROL만 읽지 않은 이메일]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>이메일을 검색할 발신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Recipient Email Address]</td> 
   <td> <p> 이메일을 검색할 수신자의 이메일 주소를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 시작 날짜] </td> 
   <td> <p>지정된 날짜 이후에 처리된 이메일을 검색할 날짜를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 날짜 이전]</td> 
   <td> <p> 지정된 날짜 또는 그 이전에 처리된 이메일을 검색할 날짜를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>검색할 전자 메일의 제목을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>특정 구문을 포함하는 이메일만 검색하려면 키워드를 입력하거나 매핑하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이메일 ID(UID)]</td> 
   <td> <p> 세부 사항을 검색하려는 이메일의 이메일 ID(UID)를 입력합니다.</p> <p>을 사용하여 이메일의 UID를 가져올 수 있습니다 [!DNL Workfront Fusion]'s[!UICONTROL Watch Email] 모듈 또는 [!UICONTROL Search Email] 모듈.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 최대 결과 수]</td> 
   <td> <p> 최대 이메일 수 [!DNL Workfront Fusion] 한 시나리오 실행 주기 동안 를 반환해야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 모듈이 결과를 반환하지 않더라도 경로 실행을 계속합니다.]</td> 
   <td> <p> 반환된 결과가 없는 경우에도 모듈을 계속 실행하려면 를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 전자 메일 보내기]

이메일 주소로 새 이메일을 보냅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>전자 메일의 제목 줄을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>전자 메일 본문을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 반복기

#### [!UICONTROL 첨부 파일 반복]

받은 첨부 파일을 하나씩 반복합니다.

전자 메일 반복기 모듈을 사용하여 전자 메일 첨부 파일을 별도로 관리할 수 있습니다. 예를 들어 첨부 파일이 있는 전자 메일을 반복하고 경고를 받도록 전자 메일을 시청하도록 설정할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 모듈]</td> 
   <td> <p>반복할 첨부 파일과 함께 전자 메일을 출력하는 모듈을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

반복기에 대한 자세한 내용은 [의 반복기 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
