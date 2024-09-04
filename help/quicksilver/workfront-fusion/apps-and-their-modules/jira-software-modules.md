---
title: Jira 소프트웨어 모듈
description: ' [!DNL Adobe Workfront Fusion] 시나리오에서는  [!DNL Jira] 소프트웨어를 사용하는 워크플로를 자동화할 수 있을 뿐만 아니라 여러 타사 응용 프로그램 및 서비스에 연결할 수도 있습니다.'
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: ed7ea1d3409c39caea5fe8b107b7b2907dc87d76
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 1%

---

# [!DNL Jira Software]개 모듈

[!DNL Adobe Workfront Fusion] 시나리오에서는 [!DNL Jira Software]을(를) 사용하는 워크플로를 자동화하고 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요하면 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오.

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)을 참조하세요.

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 전제 조건

[!DNL Jira] 모듈을 사용하려면 [!DNL Jira] 계정이 있어야 합니다.

## [!DNL Jira Software]을(를) [!DNL Workfront Fusion]에 연결

연결 메서드는 [!DNL Jira Cloud]을(를) 사용하는지 [!DNL Jira Server]을(를) 사용하는지 여부를 기준으로 합니다.

* [Workfront Fusion에  [!DNL Jira Cloud] 연결](#connect-jira-cloud-to-workfront-fusion)
* [ [!DNL Jira Server] to [!DNL Workfront Fusion] 연결](#connect-jira-server-to-workfront-fusion)

### [!DNL Jira Cloud]을(를) [!DNL Workfront Fusion]에 연결

[!DNL Jira Cloud]을(를) [!DNL Workfront Fusion]에 연결

[!DNL Jira Software]을(를) [!DNL Workfront Fusion]에 연결하려면 API 토큰을 만들고 서비스 URL 및 사용자 이름과 함께 [!DNL Workfront Fusion]의 [!UICONTROL 연결 만들기] 필드에 삽입해야 합니다.

#### [!DNL Jira]에서 API 토큰 만들기

1. [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens)(으)로 이동하여 로그인합니다.
1. **[!UICONTROL API 토큰 만들기]**&#x200B;를 클릭합니다.
1. 토큰 이름을 입력하십시오(예: *Workfront Fusion*).
1. **[!UICONTROL 클립보드에 복사]** 단추를 사용하여 토큰을 복사합니다.

   >[!IMPORTANT]
   >
   >이 대화 상자를 닫은 후에는 토큰을 다시 볼 수 없습니다.
1. 생성된 토큰을 안전한 장소에 저장합니다.
1. [다음 위치에서  [!DNL Jira] API 토큰 구성 [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion)을(를) 계속합니다.

#### [!DNL Workfront Fusion]에서 [!DNL Jira] API 토큰 구성

1. [!DNL Workfront Fusion]에서 시나리오에 [!DNL Jira] 모듈을 추가하여 **[!UICONTROL 연결 만들기]** 상자를 엽니다.
1. 다음 정보를 지정합니다.

   * **[!UICONTROL 서비스 URL]**
   * **[!UICONTROL 사용자 이름]**
   * **[!UICONTROL API 토큰]:** 이 문서의 [API 토큰 만들기 [!DNL Jira]](#create-an-api-token-in-jira) 섹션에서 만든 API 토큰입니다.

1. 연결을 만들고 모듈로 돌아가려면 [!UICONTROL 계속]을 클릭하세요.

### [!DNL Jira Server]을(를) [!DNL Workfront Fusion]에 연결

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

[!DNL Workfront Fusion]과(와) [!DNL Jira Server] 간의 연결을 승인하려면 소비자 키, 개인 키 및 서비스 URL이 필요합니다. 이 정보를 보려면 [!DNL Jira] 관리자에게 문의해야 할 수 있습니다.

* [ [!DNL Jira] 연결에 대한 공개 및 개인 키 생성](#generate-public-and-private-keys-for-your-jira-connection)
* [ [!DNL Jira]에서 클라이언트 앱을 소비자로 구성](#configure-the-client-app-as-a-consumer-in-jira)
* [ [!DNL Workfront Fusion]에서  [!DNL Jira] 서버 또는 Jira 데이터 센터에 연결 만들기](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### [!DNL Jira] 연결에 대한 공개 및 개인 키 생성

[!DNL Workfront Fusion Jira] 연결에 대한 개인 키를 얻으려면 공개 및 개인 키를 생성해야 합니다.

1. 터미널에서 다음 `openssl` 명령을 실행합니다.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     이 명령은 1024비트 개인 키를 생성합니다.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     이 명령은 X509 인증서를 만듭니다.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     이 명령은 개인 키(PKCS8 형식)를 `jira_privatekey.pcks8`에 추출합니다.
파일.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     이 명령은 인증서에서 `jira_publickey.pem` 파일로 공개 키를 추출합니다.

     >[!NOTE]
     >
     >Windows를 사용하는 경우 공개 키를 `jira_publickey.pem` 파일에 수동으로 저장해야 할 수 있습니다.
     >
     >1. 터미널에서 다음 명령을 실행합니다.
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. 터미널 출력 복사(`-------BEGIN PUBLIC KEY--------` 및 `-------END PUBLIC KEY--------` 포함)
     >   
     >1. 터미널 출력을 `jira_publickey.pem` 파일에 붙여 넣습니다.


1. [클라이언트 앱을 소비자로 구성 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)을 계속합니다.

#### [!DNL Jira]에서 클라이언트 앱을 소비자로 구성

1. [!DNL Jira] 인스턴스에 로그인합니다.
1. 왼쪽 탐색 패널에서 **[!UICONTROL [!DNL Jira]설정]** ![](assets/jira-settings-icon.png) > **[!UICONTROL 응용 프로그램]**> **[!UICONTROL 응용 프로그램 링크]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 연결할 응용 프로그램의 URL을 입력하십시오]** 필드에 다음을 입력하십시오.

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. **[!UICONTROL 새 링크 만들기]**&#x200B;를 클릭합니다. &quot;입력한 URL에서 응답을 받지 못했습니다.&quot; 오류 메시지는 무시합니다.
1. **[!UICONTROL 응용 프로그램 연결]** 창에서 **[!UICONTROL 소비자 키]** 및 **[!UICONTROL 공유 암호]** 필드에 값을 입력하십시오.

   이러한 필드의 값을 선택할 수 있습니다.

1. **[!UICONTROL 소비자 키]** 및 **[!UICONTROL 공유 암호]** 필드의 값을 안전한 위치에 복사합니다.

   이러한 값은 나중에 구성 프로세스에서 필요합니다.

1. 다음과 같이 URL 필드를 채웁니다.

   | 필드 | 설명 |
   |---|---|
   | [!UICONTROL 요청 토큰 URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 인증 URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL 액세스 토큰 URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. **[!UICONTROL 수신 링크 만들기]** 확인란을 선택하십시오.
1. **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 응용 프로그램 연결]** 창에서 다음 필드를 입력하십시오.

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
      <td><code>[!DNL jira_publickey.pem]</code> 파일의 공개 키에 붙여넣습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
1. [계속  [!DNL Jira Server] 또는 [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)에 연결 만들기

#### [!DNL Workfront Fusion]에서 [!DNL Jira Server] 또는 [!DNL Jira Data Center]에 연결 만들기

>[!NOTE]
>
>[!DNL Jira Server] 앱을 사용하여 [!DNL Jira Server] 또는 [!DNL Jira Data Center]에 연결합니다.
1. [!DNL Workfront Fusion]의 [!DNL Jira Server] 모듈에서 [!UICONTROL 연결] 필드 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.
1. [!UICONTROL 연결 만들기] 패널에서 다음 필드를 채웁니다.

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
      <td><a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">의 보안 위치에 복사한 소비자 키에 붙여 넣기 [!DNL Jira]</a>에서 클라이언트 앱을 소비자로 구성합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td><a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">[!DNL Jira] 연결에 대한 공개 및 개인 키 생성</a>에서 만든 <code>[!DNL jira_privatekey.pcks8]</code> 파일의 개인 키에 붙여 넣으십시오.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>[!DNL Jira] 인스턴스 URL을 입력하십시오. </td> 
     </tr> 
    </tbody> 
   </table>

1. 연결을 만들고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.

## [!DNL Jira Software]개 모듈 및 해당 필드

[!DNL Jira Software] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Jira Software] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### 트리거

#### [!UICONTROL 레코드 보기]

이 트리거 모듈은 레코드가 추가, 업데이트 또는 삭제될 때 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>레코드를 감시하는 데 사용할 웹후크를 선택합니다. </p> <p>새 Webhook를 추가하려면</p> 
    <ol> 
     <li value="1"><strong>[!UICONTROL 추가]</strong>를 클릭합니다.</li> 
     <li value="2">Webhook의 이름을 입력합니다.</li> 
     <li value="3"> <p>Webhook에 사용할 연결을 선택합니다. </p> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </li> 
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
* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 사용자 지정 API 호출]](#custom-api-call)
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
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
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
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
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

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL Jira Software] API에 대해 사용자 지정 인증된 호출을 수행할 수 있습니다. 이렇게 하면 다른 [!DNL Jira Software] 모듈에서 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>상대 경로 입력<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   td&gt; <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP 요청 메서드를 참조하십시오.</p> </td> 
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
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
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
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
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
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>다운로드하려는 첨부 파일의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 [!DNL Jira Software]의 단일 레코드에서 데이터를 읽습니다.

레코드의 ID를 지정합니다.

모듈은 연결에서 액세스하는 모든 사용자 지정 필드 및 값과 함께 레코드와 연결된 모든 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈에서 읽을 [!DNL Jira] 레코드의 형식을 선택하십시오.</p> 
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
   <td> <p>모듈에서 읽을 레코드의 고유 [!DNL Jira Software] ID를 입력하거나 매핑합니다.</p> </td> 
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
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
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

* [[!UICONTROL 레코드 나열]](#list-records)
* [[!UICONTROL 레코드 검색]](#search-for-records)

#### [!UICONTROL 레코드 나열]

이 검색 모듈은 검색 쿼리와 일치하는 특정 유형의 모든 항목을 검색합니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
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

이 검색 모듈은 지정한 검색 쿼리와 일치하는 [!DNL Jira Software]의 개체에서 레코드를 찾습니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>모듈에서 검색할 레코드 유형을 선택합니다. 레코드 유형을 선택하면 해당 레코드 유형과 관련된 다른 필드가 모듈에 나타납니다.</p> 
    <ul> 
     <li>[!UICONTROL 문제]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira 쿼리 언어)] </p> <p>JQL에 대한 자세한 내용은 Atlassian 도움말 사이트에서 <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a>을(를) 참조하십시오. </p> </li> 
     <li>[!UICONTROL 프로젝트]</li> 
     <li>[!UICONTROL Project by issue]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
