---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: AWS S3 모듈
description: 다음 [!DNL Adobe Workfront Fusion AWS] S3 모듈을 사용하면 S3 버킷에 대한 작업을 수행할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 0%

---

# AWS S3 모듈

다음 [!DNL Adobe Workfront Fusion AWS] S3 모듈을 사용하면 S3 버킷에 대한 작업을 수행할 수 있습니다.

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

## 전제 조건

를 사용하려면 [!UICONTROL AWS S3] 모듈이면 반드시 [!DNL Amazon Web Service] 계정이 필요합니다.

## Connect [!DNL AWS] to [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

연결하려면 [!DNL AWS S3] to [!DNL Workfront Fusion] 연결 [!DNL AWS] 계정 대상 [!DNL Workfront Fusion]. 이를 수행하려면 먼저 API 사용자를 [!DNL AWS] [!UICONTROL IAM].

1. 사용자 [!DNL AWS] [!UICONTROL IAM] 계정이 필요합니다.
1. 다음으로 이동 **[!UICONTROL ID 및 액세스 관리]** > **[!UICONTROL 액세스 관리]** > **[!UICONTROL 사용자]**.

1. 클릭 **[!UICONTROL 사용자 추가]**.
1. 새 사용자의 이름을 입력하고 **[!UICONTROL 프로그래밍 방식 액세스]** 옵션 [!UICONTROL 액세스 유형] 섹션을 참조하십시오.
1. 클릭 **[!UICONTROL 기존 정책을 직접 연결]**, 을 검색하여 **[!UICONTROL AmazonS3FullAccess]** 를 클릭합니다. 나타날 때 클릭한 다음 **[!UICONTROL 다음]**.

1. 다른 대화 상자를 계속 진행했다가 **[!UICONTROL 사용자 만들기]**.
1. 제공된 을 복사합니다. **[!UICONTROL 액세스 키 ID]** 및 **[!UICONTROL 비밀 액세스 키]**.

1. 이동 [!DNL Workfront Fusion] 그리고 [!DNL AWS S3] 모듈 **[!UICONTROL 연결 만들기]** 대화 상자.
1. 을(를) 입력합니다. [!UICONTROL 액세스 키 ID] 및 [!UICONTROL 비밀 액세스 키] 7단계에서 각 필드로 이동하고 **[!UICONTROL 계속]** 연결을 설정하려면 다음을 수행하십시오.

연결이 설정되었습니다. 모듈 설정을 계속 진행할 수 있습니다.

## [!DNL AWS S3] 모듈 및 해당 필드

구성 시 [!DNL AWS S3] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL AWS S3] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [액션](#actions)
* [검색 결과](#searches)

### 액션

* [[!UICONTROL 버킷 만들기]](#create-bucket)
* [[!UICONTROL 파일 가져오기]](#get-file)
* [[!UICONTROL 파일 업로드]](#upload-file)
* [[!UICONTROL API 호출 만들기]](#make-an-api-call)

#### [!UICONTROL 버킷 만들기]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL AWS] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>새 버킷의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 엔드포인트</a> ( AWS 설명서)를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

버킷에서 파일을 다운로드합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL AWS] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 엔드포인트</a> 에서 [!DNL AWS] 설명서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>파일을 다운로드할 버킷을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>파일의 경로를 입력합니다. 예: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업로드]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL AWS] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 엔드포인트</a> 에서 [!DNL AWS] 설명서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder](선택 사항) </p> </td> 
   <td> <p>파일을 업로드할 대상 폴더를 지정합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers](선택 사항)</p> </td> 
   <td> <p> 요청 헤더를 삽입합니다. 사용 가능한 헤더는 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] 설명서 - [!UICONTROL PUT] 개체</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 호출 만들기]

자세한 내용은 [!DNL Amazon S3] API입니다. 자세한 내용은 [[!DNL Amazon S3] [!UICONTROL REST] API 소개](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL AWS] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 엔드포인트</a> 에서 [!DNL AWS] 설명서.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL 호스트 URL을 입력합니다. 경로는 을 기준으로 해야 합니다<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 [!UICONTROL HTTP] 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 [!UICONTROL HTTP] 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>요청 헤더를 추가합니다. 다음과 같은 일반적인 요청 헤더를 사용할 수 있습니다. 추가 요청 헤더에 대해서는 다음을 참조하십시오 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API 설명서</a>.</p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>헤더 이름</th> 
       <th> <p> 설명</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>RFC 2616에 따른 메시지 길이(헤더 없음)입니다. 이 헤더는 로깅 및 ACL과 같이 XML을 로드하는 [!UICONTROL PUT] 및 작업에 필요합니다.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>요청 컨텐츠가 본문에 있는 경우 리소스의 컨텐츠 유형입니다. 예: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>RFC 1864에 따라 메시지의 base64로 인코딩된 128비트 MD5 다이제스트(헤더 없음)입니다. 이 헤더를 메시지 무결성 확인으로 사용하여 데이터가 원래 전송된 데이터와 같은지 확인할 수 있습니다. 선택 사항이지만 [!UICONTROL Content-MD5] 메커니즘을 종단 간 무결성 검사로 사용하는 것이 좋습니다. [!UICONTROL REST] 요청 인증에 대한 자세한 내용을 보려면 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] 인증</a> 에서 <i>[!DNL Amazon] Simple Storage Service Developer Guide</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL 날짜]</p> </td> 
       <td> <p>요청자에 따른 현재 날짜 및 시간입니다. 예: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 을 지정하는 경우 <code>Authorization </code>header 를 지정하는 경우 <code>x-amz-date</code> 또는 <code>Date </code>헤더.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>응용 프로그램에서 [!UICONTROL 100-continue]를 사용하는 경우 승인을 받을 때까지 요청 본문을 전송하지 않습니다. 헤더를 기반으로 메시지가 거부되면 메시지 본문이 전송되지 않습니다. 이 헤더는 본문을 보내는 경우에만 사용할 수 있습니다.</p> <p>유효한 값: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>경로 스타일 요청의 경우 값은 다음과 같습니다. <code>s3.amazonaws.com</code>. 가상 스타일 요청의 경우 값은 다음과 같습니다. <code>BucketName.s3.amazonaws.com</code>. 자세한 내용은 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">가상 호스팅</a> 에서 <i>[!DNL Amazon] Simple Storage Service Developer Guide</i>.</p> <p>이 헤더는 HTTP 1.1에 필요합니다(대부분의 도구 키트는 이 헤더를 자동으로 추가). HTTP/1.0 요청에 선택 사항입니다.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>서명 버전 4를 사용하여 요청을 인증할 때 이 헤더에서는 요청 페이로드의 해시를 제공합니다. 개체를 청크로 업로드할 때 값을 로 설정합니다. <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> 는 시그니처가 헤더만 덮으며 페이로드가 없음을 나타냅니다. 자세한 내용은 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">인증 헤더에 대한 서명 계산: 여러 청크로 페이로드 전송(청크 업로드) ([!DNL AWS] 서명 버전 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>요청자에 따른 현재 날짜 및 시간입니다. 예: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 을 지정하는 경우 <code>Authorization </code>header 를 지정하는 경우 <code>x-amz-date</code> 또는 <code>Date </code>헤더. 둘 다 지정하는 경우, <code>x-amz-date</code> 헤더가 우선합니다.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>이 헤더는 다음 시나리오에서 사용할 수 있습니다.</p> 
        <ul> 
         <li>에 보안 토큰 제공 [!DNL Amazon DevPay] 작업. 를 사용하는 각 요청 [!DNL Amazon DevPay] 2개 <code>x-amz-security-token</code> 헤더: 제품 토큰용 하나와 사용자 토큰용 하나. When [!DNL Amazon S3] 인증된 요청을 받으면 계산된 서명을 제공된 서명과 비교합니다. 서명을 계산하는 데 사용되는 잘못된 형식의 다중 값 헤더가 있으면 인증 문제가 발생할 수 있습니다.</li> 
         <li>임시 보안 자격 증명을 사용할 때 보안 토큰을 제공하십시오. IAM에서 얻은 임시 보안 자격 증명을 사용하여 요청을 할 때는 이 헤더를 사용하여 보안 토큰을 제공해야 합니다. 임시 보안 자격 증명에 대한 자세한 내용을 보려면 요청 만들기로 이동하십시오.</li> 
        </ul> <p>이 헤더는 를 사용하는 요청에 필요합니다. [!DNL Amazon DevPay] 및 임시 보안 자격 증명을 사용하여 서명된 요청.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>매개 변수 또는 양식 필드와 같은 원하는 쿼리 문자열을 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:   <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 파일 나열]](#list-files)
* [[!UICONTROL 폴더 나열]](#list-folders)

#### [!UICONTROL 파일 나열]

지정된 위치에서 파일 목록을 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL AWS] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 엔드포인트</a> 에서 [!DNL AWS] 설명서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>을(를) 선택합니다 [!DNL Amazon S3] 파일을 검색할 버킷입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix](선택 사항)</p> </td> 
   <td> <p> 파일 조회 폴더 경로(예: <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 나열]

지정된 위치에서 폴더 목록을 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL AWS] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Connect [!DNL AWS] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 엔드포인트</a> ( AWS 설명서)를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>을(를) 선택합니다 [!DNL Amazon S3] 폴더를 검색할 버킷입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix](선택 사항)</p> </td> 
   <td> <p> 폴더 경로(예: <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
