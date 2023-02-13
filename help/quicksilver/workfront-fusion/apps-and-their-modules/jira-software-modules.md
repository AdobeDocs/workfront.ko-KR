---
title: Jira 소프트웨어 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Jira] 소프트웨어, 그리고 여러 타사 애플리케이션 및 서비스에 연결합니다.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2039'
ht-degree: 1%

---

# [!DNL Jira Software] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Jira Software]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>작업 자동화 및 통합을 위한 [!UICONTROL Workfront Fusion] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 전제 조건

를 사용하려면 [!DNL Jira] 모듈을 사용해야 합니다. [!DNL Jira] 계정이 필요합니다.

## Connect [!DNL Jira Software] to [!DNL Workfront Fusion]

연결 방법은 [!DNL Jira Cloud] 또는 [!DNL Jira Server].

* [Connect [!DNL Jira Cloud] Workfront Fusion으로](#connect-jira-cloud-to-workfront-fusion)
* [Connect [!DNL Jira Server] to [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connect [!DNL Jira Cloud] to [!DNL Workfront Fusion]

Connect [!DNL Jira Cloud] to [!DNL Workfront Fusion]

연결하려면 [!DNL Jira Software] to [!DNL Workfront Fusion]를 지정하는 경우 API 토큰을 만들고, 서비스 URL 및 사용자 이름과 함께 를 [!UICONTROL 연결 만들기] 필드 [!DNL Workfront Fusion].

#### 에서 API 토큰 만들기 [!DNL Jira]

1. 이동 [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) 로그인하고
1. 클릭 **[!UICONTROL API 토큰 만들기]**.
1. 토큰의 이름(예: )을 입력합니다 *Workfront Fusion*.
1. 를 사용하여 토큰 복사 **[!UICONTROL 클립보드에 복사]** 버튼을 클릭합니다.

   >[!IMPORTANT]
   >
   >이 대화 상자를 닫은 후에는 토큰을 다시 볼 수 없습니다.
1. 생성된 토큰을 안전한 위치에 저장합니다.
1. 계속 [구성 [!DNL Jira] 의 API 토큰 [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### 구성 [!DNL Jira] 의 API 토큰 [!DNL Workfront Fusion]

1. in [!DNL Workfront Fusion], 추가 [!DNL Jira] 모듈을 모듈로 확장하여 **[!UICONTROL 연결 만들기]** 상자.
1. 다음 정보를 지정합니다.

   * **[!UICONTROL 서비스 URL]**
   * **[!UICONTROL 사용자 이름]**
   * **[!UICONTROL API 토큰]:** 이 토큰은 [에서 API 토큰 만들기 [!DNL Jira]](#create-an-api-token-in-jira) 섹션 을 참조하십시오.

1. 클릭 [!UICONTROL 계속] 연결을 만들고 모듈로 돌아가려면 를 클릭합니다.

### Connect [!DNL Jira Server] to [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

다음 사이의 연결을 승인하려면 [!DNL Workfront Fusion] 및 [!DNL Jira Server], 소비자 키, 개인 키 및 서비스 URL이 필요합니다. 귀하의 [!DNL Jira] 관리자 를 참조하십시오.

* [사용자의 공용 및 개인 키 생성 [!DNL Jira] 연결](#generate-public-and-private-keys-for-your-jira-connection)
* [에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [연결 만들기 [!DNL Jira] 의 서버 또는 Jira 데이터 센터 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 사용자의 공용 및 개인 키 생성 [!DNL Jira] 연결

개인 키를 획득하려면 [!DNL Workfront Fusion Jira] 연결 시 공개 및 개인 키를 생성해야 합니다.

1. 터미널에서 다음을 실행합니다 `openssl` 명령.

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
      >1. 터미널 출력을 복사합니다(포함) `-------BEGIN PUBLIC KEY--------` 및 `-------END PUBLIC KEY--------`
      >   
      >1. 터미널 출력을 라는 파일에 붙여 넣습니다. `jira_publickey.pem`.



1. 계속 [에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### 에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]

1. 에 로그인합니다. [!DNL Jira] 인스턴스.
1. 왼쪽 탐색 패널에서 **[!UICONTROL [!DNL Jira]설정]** ![](assets/jira-settings-icon.png) > **[!UICONTROL 애플리케이션]**> **[!UICONTROL 애플리케이션 링크]**.
1. 에서 **[!UICONTROL 연결할 응용 프로그램의 URL을 입력합니다]** 필드, 입력

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. 클릭 **[!UICONTROL 새 링크 만들기]**. &quot;입력한 URL에서 응답을 받지 않았습니다.&quot; 오류 메시지를 무시합니다.
1. 에서 **[!UICONTROL 애플리케이션 연결]** 창의 값을 **[!UICONTROL 소비자 키]** 및 **[!UICONTROL 공유 암호]** 필드.

   이러한 필드의 값을 선택할 수 있습니다.

1. 의 값을 복사합니다. **[!UICONTROL 소비자 키]** 및 **[!UICONTROL 공유 암호]** 필드를 보안 위치에 추가합니다.

   나중에 구성 프로세스에서 이러한 값이 필요합니다.

1. 다음과 같이 URL 필드를 입력합니다.

   | 필드 | 설명 |
   |---|---|
   | [!UICONTROL 요청 토큰 URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 인증 URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL 액세스 토큰 URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. 을(를) 선택합니다 **[!UICONTROL 들어오는 링크 만들기]** 확인란을 선택합니다.
1. 클릭 **[!UICONTROL 계속]**.
1. 에서 **[!UICONTROL 애플리케이션 연결]** 창에서 다음 필드를 입력합니다.

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> 보안 위치에 복사한 소비자 키에 붙여넣습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Name]</td> 
      <td>원하는 이름을 입력합니다. 이 이름은 직접 참조할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 공개 키]</td> 
      <td>에서 공개 키에 붙여넣습니다. <code>[!DNL jira_publickey.pem]</code> 파일.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]**.
1. 계속 [연결 만들기 [!DNL Jira Server] 또는 [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 연결 만들기 [!DNL Jira Server] 또는 [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>를 사용하십시오 [!DNL Jira Server] 연결할 앱 [!DNL Jira Server] 또는 [!DNL Jira Data Center].
1. 어떤 경우에서도 [!DNL Jira Server] 모듈 [!DNL Workfront Fusion]를 클릭합니다. **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 에서 [!UICONTROL 연결 만들기] 패널에서 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 연결 이름]</p> </td> 
      <td> <p>연결의 이름을 입력합니다</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>의 보안 위치에 복사한 소비자 키에 붙여넣습니다. <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">에서 클라이언트 앱을 소비자로 구성 [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>의 개인 키에 붙여넣습니다. <code>[!DNL jira_privatekey.pcks8]</code> 만든 파일 <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">사용자의 공용 및 개인 키 생성 [!DNL Jira] 연결</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>을(를) 입력합니다. [!DNL Jira] 인스턴스 URL. </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!DNL Jira Software] 모듈 및 해당 필드

구성 시 [!DNL Jira Software] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Jira Software] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### Triggers

#### [!UICONTROL 레코드 감시]

이 트리거 모듈은 레코드가 추가, 업데이트 또는 삭제될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>레코드를 확인하는 데 사용할 웹 후크를 선택합니다. </p> <p>새 웹 후크를 추가하려면 다음을 수행합니다.</p> 
    <ol> 
     <li value="1">클릭 <strong>[!UICONTROL Add]</strong></li> 
     <li value="2">웹 후크의 이름을 입력합니다.</li> 
     <li value="3"> <p>웹 후크에 사용할 연결을 선택합니다. </p> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </li> 
     <li value="4"> <p>소프트웨어에서 확인할 레코드 유형을 선택합니다.</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL 문제]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 스프린트에 문제 추가]](#add-issue-to-sprint)
* [[!UICONTROL 사용자 지정 API 호출]](#custom-api-call)
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
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>문제를 추가할 스프린트의 스프린트 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 문제 ID 또는 키]</td> 
   <td>스프린트에 추가할 각 문제에 대해 문제 ID 또는 키를 추가합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 Jira에 새 레코드를 만듭니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈을 만들 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL Jira Software] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Jira Software] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
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
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 특정 레코드를 삭제합니다.

레코드의 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈을 삭제할 레코드 유형을 선택합니다. </p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 또는 Key]</td> 
   <td>삭제할 레코드의 ID 또는 키를 입력하거나 매핑합니다.</td> 
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
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>다운로드할 첨부 파일의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 [!DNL Jira Software].

레코드의 ID를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>유형 선택 [!DNL Jira] 모듈을 읽을 것을 기록합니다.</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>받을 출력을 선택합니다. 출력 옵션은 "[!UICONTROL 레코드 유형]" 필드에서 선택한 레코드 유형에 따라 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>고유 번호를 입력하거나 매핑합니다 [!DNL Jira Software] 모듈을 읽을 레코드의 ID입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 문제 또는 프로젝트와 같은 기존 레코드를 업데이트합니다.

레코드의 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈을 업데이트할 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL 전환 문제]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 또는 Key]</td> 
   <td>업데이트할 레코드의 ID 또는 키를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 레코드 나열]](#list-records)
* [[!UICONTROL 레코드 검색]](#search-for-records)

#### [!UICONTROL 레코드 나열]

이 검색 모듈은 검색 쿼리와 일치하는 특정 유형의 모든 항목을 검색합니다

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈을 나열할 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL 문제]</li> 
     <li>[!UICONTROL Project]</li> 
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

이 검색 모듈은 [!DNL Jira Software] 지정한 검색 쿼리와 일치합니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Jira Software] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈이 검색할 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Language)] </p> <p>JQL에 대한 자세한 내용은 <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> at.js 참조. </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Project by issue]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
