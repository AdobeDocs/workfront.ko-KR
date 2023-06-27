---
title: Jira 소프트웨어 모듈
description: 다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Jira] 소프트웨어를 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 1%

---

# [!DNL Jira Software] 모듈

다음에서 [!DNL Adobe Workfront Fusion] 시나리오에서는 다음을 사용하는 워크플로를 자동화할 수 있습니다 [!DNL Jira Software]을 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 전제 조건

사용 [!DNL Jira] 모듈 이 있어야 합니다. [!DNL Jira] 계정입니다.

## 연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]

연결 방법은 사용 여부를 기반으로 합니다 [!DNL Jira Cloud] 또는 [!DNL Jira Server].

* [연결 [!DNL Jira Cloud] Workfront Fusion으로](#connect-jira-cloud-to-workfront-fusion)
* [연결 [!DNL Jira Server] 끝 [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### 연결 [!DNL Jira Cloud] 끝 [!DNL Workfront Fusion]

연결 [!DNL Jira Cloud] 끝 [!DNL Workfront Fusion]

연결하려면 [!DNL Jira Software] 끝 [!DNL Workfront Fusion], API 토큰을 만들고 서비스 URL 및 사용자 이름과 함께 [!UICONTROL 연결 만들기] 의 필드 [!DNL Workfront Fusion].

#### 에서 API 토큰 만들기 [!DNL Jira]

1. 다음으로 이동 [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) 로그인합니다.
1. 클릭 **[!UICONTROL API 토큰 만들기]**.
1. 토큰 이름 입력(예: *Workfront Fusion*.
1. 다음을 사용하여 토큰 복사 **[!UICONTROL 클립보드에 복사]** 단추를 클릭합니다.

   >[!IMPORTANT]
   >
   >이 대화 상자를 닫은 후에는 토큰을 다시 볼 수 없습니다.
1. 생성된 토큰을 안전한 장소에 저장합니다.
1. 계속 [구성 [!DNL Jira] 의 API 토큰 [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### 구성 [!DNL Jira] 의 API 토큰 [!DNL Workfront Fusion]

1. 위치 [!DNL Workfront Fusion], 추가 [!DNL Jira] 을(를) 시나리오에 연결하여 **[!UICONTROL 연결 만들기]** 상자.
1. 다음 정보를 지정합니다.

   * **[!UICONTROL 서비스 URL]**
   * **[!UICONTROL 사용자 이름]**
   * **[!UICONTROL API 토큰]:** 에서 만든 API 토큰입니다. [에서 API 토큰 만들기 [!DNL Jira]](#create-an-api-token-in-jira) 이 문서의 섹션.

1. 클릭 [!UICONTROL 계속] 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

### 연결 [!DNL Jira Server] 끝 [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

간 연결을 승인하려면 [!DNL Workfront Fusion] 및 [!DNL Jira Server], 소비자 키, 개인 키 및 서비스 URL이 필요합니다. 다음으로 문의해야 할 수도 있습니다. [!DNL Jira] 관리자 를 참조하십시오.

* [에 대한 공개 및 비공개 키 생성 [!DNL Jira] 연결](#generate-public-and-private-keys-for-your-jira-connection)
* [에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [에 대한 연결 만들기 [!DNL Jira] 의 서버 또는 Jira 데이터 센터 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 에 대한 공개 및 비공개 키 생성 [!DNL Jira] 연결

의 개인 키를 획득하려면 [!DNL Workfront Fusion Jira] 연결에서는 공개 및 개인 키를 생성해야 합니다.

1. 터미널에서 다음을 실행합니다 `openssl` 명령입니다.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     이 명령은 1024비트 개인 키를 생성합니다.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     이 명령은 X509 인증서를 만듭니다.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     이 명령은 개인 키(PKCS8 형식)를 `jira_privatekey.pcks8`
파일.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     이 명령은 인증서에서 로 공개 키를 추출합니다 `jira_publickey.pem` 파일.

     >[!NOTE]
     >
     >Windows를 사용하는 경우 공개 키를 `jira_publickey.pem` 수동으로 파일:
     >
     >1. 터미널에서 다음 명령을 실행합니다.
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. 터미널 출력 복사(포함) `-------BEGIN PUBLIC KEY--------` 및 `-------END PUBLIC KEY--------`
     >   
     >1. 터미널 출력을 다음 파일에 붙여넣기 `jira_publickey.pem`.


1. 계속 [에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### 에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]

1. 에 로그인 [!DNL Jira] 인스턴스.
1. 왼쪽 탐색 패널에서 을 클릭합니다. **[!UICONTROL [!DNL Jira]설정]** ![](assets/jira-settings-icon.png) > **[!UICONTROL 애플리케이션]**> **[!UICONTROL 애플리케이션 링크]**.
1. 다음에서 **[!UICONTROL 연결할 응용 프로그램의 URL을 입력하십시오.]** 필드, 입력

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. 클릭 **[!UICONTROL 새 링크 만들기]**. &quot;입력한 URL에서 응답을 받지 못했습니다.&quot; 오류 메시지는 무시합니다.
1. 다음에서 **[!UICONTROL 애플리케이션 연결]** 창에 값을 입력합니다 **[!UICONTROL 소비자 키]** 및 **[!UICONTROL 공유 암호]** 필드.

   이러한 필드의 값을 선택할 수 있습니다.

1. 의 값을 복사합니다. **[!UICONTROL 소비자 키]** 및 **[!UICONTROL 공유 암호]** 필드를 보안 위치에 추가합니다.

   이러한 값은 나중에 구성 프로세스에서 필요합니다.

1. 다음과 같이 URL 필드를 채웁니다.

   | 필드 | 설명 |
   |---|---|
   | [!UICONTROL 요청 토큰 URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 인증 URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL 토큰 URL 액세스] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. 다음 항목 선택 **[!UICONTROL 수신 링크 만들기]** 확인란.
1. 클릭 **[!UICONTROL 계속]**.
1. 다음에서 **[!UICONTROL 애플리케이션 연결]** 창에서 다음 필드를 입력합니다.

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 소비자 키]</p> </td> 
      <td> 보안 위치에 복사한 소비자 키에 붙여넣습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer name]</td> 
      <td>선택한 이름을 입력합니다. 이 이름은 참조용입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 공개 키]</td> 
      <td>에서 공개 키에 붙여넣기 <code>[!DNL jira_publickey.pem]</code> 파일.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]**.
1. 계속 [에 대한 연결 만들기 [!DNL Jira Server] 또는 [!DNL Jira Data Center] 위치: [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 에 대한 연결 만들기 [!DNL Jira Server] 또는 [!DNL Jira Data Center] 위치: [!DNL Workfront Fusion]

>[!NOTE]
>
>사용 [!DNL Jira Server] 연결할 앱 [!DNL Jira Server] 또는 [!DNL Jira Data Center].
1. 다음 중 하나 [!DNL Jira Server] 의 모듈 [!DNL Workfront Fusion], 클릭 **[!UICONTROL 추가]** 다음 옆에 [!UICONTROL 연결] 필드.
1. 다음에서 [!UICONTROL 연결 만들기] 패널, 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 연결 이름]</p> </td> 
      <td> <p>연결 이름 입력</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 소비자 키]</td> 
      <td>의 보안 위치에 복사한 소비자 키에 붙여넣습니다. <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>의 개인 키에 붙여넣기 <code>[!DNL jira_privatekey.pcks8]</code> 에서 생성한 파일 <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">에 대한 공개 및 비공개 키 생성 [!DNL Jira] 연결</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>다음을 입력하십시오. [!DNL Jira] 인스턴스 URL. </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Jira Software] 모듈 및 해당 필드

를 구성할 때 [!DNL Jira Software] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Jira Software] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### 트리거

#### [!UICONTROL 레코드 시청]

이 트리거 모듈은 레코드가 추가, 업데이트 또는 삭제될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>레코드를 감시하는 데 사용할 웹후크를 선택합니다. </p> <p>새 Webhook를 추가하려면</p> 
    <ol> 
     <li value="1">클릭 <strong>[!UICONTROL 추가]</strong></li> 
     <li value="2">Webhook의 이름을 입력합니다.</li> 
     <li value="3"> <p>Webhook에 사용할 연결을 선택합니다. </p> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </li> 
     <li value="4"> <p>소프트웨어에서 감시할 레코드 유형을 선택합니다.</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL 문제]</li> 
       <li>[!UICONTROL 프로젝트] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 스프린트에 문제 추가]](#add-issue-to-sprint)
* [[!UICONTROL 사용자 정의 API 호출]](#custom-api-call)
* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 레코드 삭제]](#delete-a-record)
* [[!UICONTROL 첨부 파일 다운로드]](#download-an-attachment)
* [[!UICONTROL 레코드 읽기]](#read-a-record)
* [[!UICONTROL 레코드 업데이트]](#update-a-record)

#### [!UICONTROL 스프린트에 문제 추가]

이 작업 모듈은 스프린트에 하나 이상의 문제를 추가합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>문제를 추가하려는 스프린트의 스프린트 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제 ID 또는 키]</td> 
   <td>스프린트에 추가하려는 각 문제에 대한 문제 ID 또는 키를 추가합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 Jira에 새 레코드를 만듭니다.

모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈에서 만들 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL 첨부 파일]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사용자 정의 API 호출]

이 작업 모듈에서는 다음을 위한 사용자 지정 인증 호출을 만들 수 있습니다. [!DNL Jira Software] API. 이렇게 하면 다른 사용자가 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Jira Software] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형식으로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 특정 레코드를 삭제합니다.

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈에서 삭제할 레코드 유형을 선택합니다. </p> 
    <ul> 
     <li>[!UICONTROL 첨부 파일]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 또는 키]</td> 
   <td>삭제하려는 레코드의 ID 또는 키를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 첨부 파일 다운로드]

이 작업 모듈은 특정 첨부 파일을 다운로드합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>다운로드하려는 첨부 파일의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 의 단일 레코드에서 데이터를 읽습니다. [!DNL Jira Software].

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>유형 선택 [!DNL Jira] 모듈에서 읽을 레코드를 기록합니다.</p> 
    <ul> 
     <li>[!UICONTROL 첨부 파일]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>수신하려는 출력을 선택합니다. 출력 옵션은 "[!UICONTROL 레코드 유형]" 필드에서 선택한 레코드 유형에 따라 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>고유 항목 입력 또는 매핑 [!DNL Jira Software] 모듈에서 읽을 레코드의 ID입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 문제 또는 프로젝트 등의 기존 레코드를 업데이트합니다.

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈을 업데이트할 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL 전환 문제]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 또는 키]</td> 
   <td>업데이트하려는 레코드의 ID 또는 키를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 목록 레코드]](#list-records)
* [[!UICONTROL 레코드 검색]](#search-for-records)

#### [!UICONTROL 목록 레코드]

이 검색 모듈은 검색 쿼리와 일치하는 특정 유형의 모든 항목을 검색합니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈에 나열할 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL Sprint 문제]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 최대 결과]</p> </td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 검색할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 검색]

이 검색 모듈은 의 개체에서 레코드를 찾습니다. [!DNL Jira Software] 지정한 검색 쿼리와 일치하는 쿼리입니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Jira Software] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">연결 [!DNL Jira Software] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈에서 검색할 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL 문제]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira 쿼리 언어)] </p> <p>JQL에 대한 자세한 내용은 <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> Atlassian 도움말 사이트에서요. </p> </li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL Project by issue]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
