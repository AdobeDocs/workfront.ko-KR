---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Authenticator 모듈
description: Adobe Authenticator 모듈을 사용하면 단일 연결을 사용하여 API를 통해 모든 Adobe 제품에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
source-git-commit: 07443d85e160004c273fc977629dd9f588cc23b2
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 1%

---

# Adobe Authenticator 모듈

Adobe Authenticator 모듈을 사용하면 단일 연결을 사용하여 모든 Adobe API에 연결할 수 있습니다. 이렇게 하면 아직 전용 Fusion 커넥터가 없는 Adobe 제품에 보다 쉽게 연결할 수 있습니다.

HTTP 모듈에 대한 이점은 전용 앱에서와 같이 연결을 만들 수 있다는 것입니다.

사용 가능한 Adobe API 목록을 보려면 X를 참조하십시오. 할당된 API만 사용할 수 있습니다.

## 액세스 요구 사항

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 플랜</td>
      <td>
        <p>새로 만들기: 모두</p><p>또는</p><p>현재: [!UICONTROL Pro] 이상</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td>
      <td>
        <p>새로운 기능: 표준</p><p>또는</p><p>현재: [!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스</td>
      <td>
   <p>현재 Fusion 라이센스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 Fusion 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">제품</td>
      <td>
   <p>새 Workfront 플랜: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>현재 Workfront 플랜: 조직에서 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td>
    </tr>
  </tbody>
</table>

## 전제 조건

* 모듈을 연결할 Adobe 제품에 대한 액세스 권한이 있어야 합니다.
* Adobe Developer 콘솔에 액세스할 수 있어야 합니다.
* 모듈을 연결할 API가 포함된 프로젝트가 Adobe Developer 콘솔에 있어야 합니다. 다음을 수행할 수 있습니다.

   * API를 사용하여 새 프로젝트를 만듭니다.

     또는
   * 기존 프로젝트에 API를 추가합니다.

  Adobe Developer 콘솔에서 API를 만들거나 프로젝트에 추가하는 방법에 대한 자세한 내용은 을 참조하십시오. [프로젝트 만들기](https://developer.adobe.com/dep/guides/dev-console/create-project/) Adobe 설명서에서 확인할 수 있습니다.

## 연결 만들기

Adobe Authenticator 연결은 Adobe Developer 콘솔의 단일 프로젝트에 연결합니다. 두 개 이상의 Adobe API에 대해 동일한 연결을 사용하려면 동일한 프로젝트에 API를 추가하고 해당 프로젝트에 대한 연결을 만듭니다.

별도의 프로젝트에 대해 별도의 연결을 만들 수 있지만 연결을 사용하여 해당 연결에 지정된 프로젝트에 없는 API에 액세스할 수는 없습니다.

>[!IMPORTANT]
>
>Adobe Authenticator 커넥터를 사용하면 OAuth 서버 간 연결과 서비스 계정(JWT) 연결 중 하나를 선택할 수 있습니다. Adobe에 더 이상 사용되지 않는 JWT 자격 증명이 있으며, 2025년 1월 1일 이후 작동을 중지합니다. **따라서 OAuth 연결을 만드는 것이 좋습니다.**
>
>이러한 연결 유형에 대한 자세한 내용은 [서버 간 인증](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) Adobe 설명서에서

연결을 만들려면 다음 작업을 수행하십시오.

1. Adobe Authenticator 모듈에서 **추가** 연결 필드 옆에 있습니다.
1. 다음 필드를 채웁니다.

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL 연결 유형]</td>
        <td>
          <p>OAuth 서버 간 연결을 만들지 서비스 계정(JWT) 연결을 만들지 선택합니다.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 연결 이름]</td>
        <td>
          <p>이 연결의 이름을 입력하십시오.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] 클라이언트 ID. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] 클라이언트 암호. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 범위]</td>
        <td>OAuth 연결을 선택한 경우 이 연결에 필요한 범위를 입력하십시오.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 기술 계정 ID]</td>
        <td>다음을 입력하십시오. [!DNL Adobe] 기술 계정 ID. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 조직 ID]</td>
        <td>JWT 연결을 선택한 경우 [!DNL Adobe] 조직 ID. 이 정보는 의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다. [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 메타 범위]</td>
        <td>JWT 연결을 선택한 경우 이 연결에 필요한 메타 범위를 입력합니다. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 개인 키]</td>
        <td>
          <p>JWT 연결을 선택한 경우에서 자격 증명을 생성할 때 생성된 개인 키를 입력합니다 [!DNL Adobe Developer Console]. </p>
          <p>개인 키 또는 인증서를 추출하려면 다음을 수행하십시오.</p>
          <ol>
            <li value="1">
              <p>클릭 <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>추출 중인 파일 유형을 선택합니다.</p>
            </li>
            <li value="3">
              <p>개인 키 또는 인증서가 포함된 파일을 선택합니다.</p>
            </li>
            <li value="4">
              <p>파일의 암호를 입력합니다.</p>
            </li>
            <li value="5">
              <p>클릭 <b>[!UICONTROL 저장]</b> 를 클릭하여 파일을 추출하고 연결 설정으로 돌아갑니다.</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 환경]</td>
        <td>프로덕션 환경에 연결할지 아니면 비프로덕션 환경에 연결할지 선택합니다.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL 유형]</td>
        <td>서비스 계정에 연결할지 또는 개인 계정에 연결할지 선택합니다.</td>
      </tr>
    </tbody>
    </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 저장하고 모듈로 돌아갑니다.

## 모듈

### 사용자 지정 API 호출 만들기

이 작업 모듈에서는 모든 Adobe API를 호출할 수 있습니다.

>[!TIP]
>
>연결할 API의 전체 URL을 입력해야 합니다. 이 모듈은 상대 URL을 허용하지 않습니다.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Adobe Authenticator 모듈에 대한 연결 만들기에 대한 지침은 <a href="#create-a-connection" class="MCXref xref" >연결 만들기</a> 이 문서에서.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>연결하려는 API 포인트의 전체 URL을 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 메서드]</p>
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion은 인증 헤더를 자동으로 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 쿼리 문자열]  </td>
      <td>
        <p>요청 쿼리 문자열을 입력합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용할 때 <code>if</code> json에서 따옴표를 조건문 외부에 넣습니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 제한]  </td>
      <td>
        <p>한 실행 주기에서 모듈이 반환할 최대 결과 수를 입력합니다.</p>
      </td>
    </tr>
  </tbody>
</table>

