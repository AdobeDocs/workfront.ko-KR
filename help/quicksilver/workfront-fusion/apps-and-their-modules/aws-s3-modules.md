---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: AWS S3 모듈
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1455'
ht-degree: 0%

---

# AWS S3 모듈

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [AWS S3 모듈](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/aws-s3-modules.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

[!DNL Adobe Workfront Fusion AWS] S3 모듈을 사용하면 S3 버킷에서 작업을 수행할 수 있습니다.

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

[!UICONTROL AWS S3] 모듈을 사용하려면 [!DNL Amazon Web Service] 계정이 있어야 합니다.

## AWS S3 API 정보

AWS S3 커넥터는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">기본 URL</td> 
   <td>https://s3입니다.{{parameters.region}}.amazonaws.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td>v1.5.21</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL AWS]을(를) [!DNL Workfront Fusion]에 연결 {#connect-aws-to-workfront-fusion}

[!DNL AWS S3]을(를) [!DNL Workfront Fusion]에 연결하려면 [!DNL AWS] 계정을 [!DNL Workfront Fusion]에 연결해야 합니다. 이렇게 하려면 먼저 [!DNL AWS] [!UICONTROL IAM]에서 API 사용자를 만들어야 합니다.

1. [!DNL AWS] [!UICONTROL IAM] 계정에 로그인합니다.
1. **[!UICONTROL ID 및 액세스 관리]** > **[!UICONTROL 액세스 관리]** > **[!UICONTROL 사용자]**(으)로 이동합니다.

1. **[!UICONTROL 사용자 추가]**&#x200B;를 클릭합니다.
1. 새 사용자의 이름을 입력하고 [!UICONTROL 액세스 형식] 섹션에서 **[!UICONTROL 프로그래밍 방식 액세스]** 옵션을 선택합니다.
1. **[!UICONTROL 기존 정책을 직접 첨부]**&#x200B;를 클릭한 다음 검색 창에서 **[!UICONTROL AmazonS3FullAccess]**&#x200B;를 검색합니다. 나타나면 클릭한 다음 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.

1. 다른 대화 상자 화면을 계속 진행하고 **[!UICONTROL 사용자 만들기]**&#x200B;를 클릭합니다.
1. 제공된 **[!UICONTROL 액세스 키 ID]** 및 **[!UICONTROL 비밀 액세스 키]**&#x200B;를 복사합니다.

1. [!DNL Workfront Fusion](으)로 이동하여 [!DNL AWS S3] 모듈의 **[!UICONTROL 연결 만들기]** 대화 상자를 엽니다.
1. 7단계의 각 필드에 [!UICONTROL 액세스 키 ID] 및 [!UICONTROL 비밀 액세스 키]를 입력하고 **[!UICONTROL 계속]**&#x200B;을 클릭하여 연결을 설정하십시오.

연결이 설정되었습니다. 모듈 설정을 진행할 수 있습니다.

## [!DNL AWS S3]개 모듈 및 해당 필드

[!DNL AWS S3] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL AWS S3] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

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
   <td> <p>[!DNL AWS] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이름] </td> 
   <td> <p>새 버킷의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 영역] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 AWS 설명서에서 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 끝점</a>에 대한 설명을 참조하십시오.</p> </td> 
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
   <td> <p>[!DNL AWS] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 영역] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 [!DNL AWS] 설명서에서 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 끝점</a>에 대한 설명을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 버킷] </td> 
   <td> <p>파일을 다운로드할 버킷을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 경로]</p> </td> 
   <td> <p>파일 경로를 입력합니다. 예: <code>/photos/2019/February/image023.jpg</code></p> </td> 
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
   <td> <p>[!DNL AWS] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 영역] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 [!DNL AWS] 설명서에서 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 끝점</a>에 대한 설명을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder] (선택 사항) </p> </td> 
   <td> <p>파일을 업로드할 대상 폴더를 지정합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers] (선택 사항)</p> </td> 
   <td> <p> 요청 헤더를 삽입합니다. 사용 가능한 헤더는 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] 설명서([!UICONTROL PUT] 개체</a>)에서 찾을 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 호출 만들기]

[!DNL Amazon S3] API에 대한 자세한 내용은 [[!DNL Amazon S3] [!UICONTROL REST] API 소개](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html)를 참조하십시오.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 영역] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 [!DNL AWS] 설명서에서 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 끝점</a>에 대한 설명을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL 호스트 URL을 입력합니다. 경로는 <code> https://s3.&lt;selected-region>.amazonaws.com/</code>에 상대적이어야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 [!UICONTROL HTTP] 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] 요청 메서드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>요청 헤더를 추가합니다. 다음과 같은 일반적인 요청 헤더를 사용할 수 있습니다. 추가 요청 헤더는 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API 설명서</a>를 참조하십시오.</p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> 
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
       <td> <p>RFC 2616에 따른 메시지 길이(헤더 없음). 이 헤더는 로깅 및 ACL과 같이 XML을 로드하는 작업 및 [!UICONTROL PUT]에 필요합니다.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>요청 콘텐츠가 본문에 있는 경우 리소스의 콘텐츠 유형입니다. 예: <code>text/plain</code></p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Base64는 RFC 1864에 따라 메시지의 128비트 MD5 다이제스트(헤더 없음)를 인코딩했습니다. 이 헤더를 메시지 무결성 검사로 사용하여 데이터가 원래 전송된 데이터와 동일한지 확인할 수 있습니다. 선택 사항이지만 [!UICONTROL Content-MD5] 메커니즘을 엔드 투 엔드 무결성 검사로 사용하는 것이 좋습니다. [!UICONTROL REST] 요청 인증에 대한 자세한 내용을 보려면 <i>[!DNL Amazon] Simple Storage Service Developer Guide</i>의 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] Authentication</a>(으)로 이동하십시오.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL 날짜]</p> </td> 
       <td> <p>요청자에 따른 현재 날짜 및 시간입니다. 예: <code>Wed, 01 Mar 2006 12:00:00 GMT</code> <code>Authorization </code>헤더를 지정할 때는 <code>x-amz-date</code> 또는 <code>Date </code>헤더를 지정해야 합니다.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>애플리케이션이 [!UICONTROL 100-continue]를 사용하는 경우 승인을 받을 때까지 요청 본문을 전송하지 않습니다. 헤더를 기반으로 메시지가 거부되면 메시지 본문이 전송되지 않습니다. 본문을 보내는 경우에만 이 헤더를 사용할 수 있습니다.</p> <p>유효한 값: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL 호스트]</p> </td> 
       <td> <p>경로 스타일 요청의 경우 값은 <code>s3.amazonaws.com</code>입니다. 가상 스타일 요청의 경우 값은 <code>BucketName.s3.amazonaws.com</code>입니다. 자세한 내용은 <i>[!DNL Amazon] Simple Storage Service 개발자 안내서</i>의 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">가상 호스팅</a>을 참조하세요.</p> <p>이 헤더는 HTTP 1.1에 필요합니다(대부분의 도구 키트에서 이 헤더를 자동으로 추가). HTTP/1.0 요청에는 선택 사항입니다.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>서명 버전 4를 사용하여 요청을 인증할 때 이 헤더는 요청 페이로드의 해시를 제공합니다. 개체를 청크로 업로드할 때 서명에서 헤더만 다루고 페이로드가 없음을 나타내려면 값을 <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code>(으)로 설정하십시오. 자세한 내용은 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">인증 헤더에 대한 서명 계산: 페이로드를 여러 청크(청크 업로드)로 전송 중([!DNL AWS] 서명 버전 4)</a>을 참조하십시오.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>요청자에 따른 현재 날짜 및 시간입니다. 예: <code>Wed, 01 Mar 2006 12:00:00 GMT</code> <code>Authorization </code>헤더를 지정할 때는 <code>x-amz-date</code> 또는 <code>Date </code>헤더를 지정해야 합니다. 둘 다 지정하면 <code>x-amz-date</code> 헤더에 지정된 값이 우선합니다.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>이 헤더는 다음 시나리오에서 사용할 수 있습니다.</p> 
        <ul> 
         <li>[!DNL Amazon DevPay] 작업에 대한 보안 토큰을 제공합니다. [!DNL Amazon DevPay]을(를) 사용하는 각 요청에는 두 개의 <code>x-amz-security-token</code> 헤더가 필요합니다. 하나는 제품 토큰에 사용되고 다른 하나는 사용자 토큰에 사용됩니다. [!DNL Amazon S3]이(가) 인증된 요청을 받으면 계산된 서명을 제공된 서명과 비교합니다. 서명을 계산하는 데 사용되는 형식이 올바르지 않은 다중 값 헤더로 인해 인증 문제가 발생할 수 있습니다.</li> 
         <li>임시 보안 자격 증명을 사용할 때 보안 토큰을 제공합니다. IAM에서 가져온 임시 보안 자격 증명을 사용하여 요청할 때 이 헤더를 사용하여 보안 토큰을 제공해야 합니다. 임시 보안 자격 증명에 대한 자세한 내용을 보려면 요청 만들기를 참조하십시오.</li> 
        </ul> <p>이 헤더는 [!DNL Amazon DevPay]을(를) 사용하는 요청과 임시 보안 자격 증명을 사용하여 서명된 요청에 필요합니다.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>매개 변수 또는 양식 필드 등 원하는 쿼리 문자열을 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>표준 JSON 개체의 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:   <p>JSON에서 <code>if</code>과(와) 같은 조건문을 사용할 때 따옴표를 조건문 외부에 넣으십시오.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

* [[!UICONTROL 목록 파일]](#list-files)
* [[!UICONTROL 폴더 나열]](#list-folders)

#### [!UICONTROL 목록 파일]

지정된 위치의 파일 목록을 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 영역] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 [!DNL AWS] 설명서에서 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 끝점</a>에 대한 설명을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 버킷] </td> 
   <td> <p>파일을 검색할 [!DNL Amazon S3] 버킷을 선택하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (선택 사항)</p> </td> 
   <td> <p> 파일을 조회할 폴더 경로(예: ). <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 나열]

지정된 위치의 폴더 목록을 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 영역] </td> 
   <td> <p>지역 끝점을 선택합니다. 자세한 내용은 AWS 설명서에서 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">지역 끝점</a>에 대한 설명을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 버킷] </td> 
   <td> <p>폴더를 검색할 [!DNL Amazon S3] 버킷을 선택하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix] (선택 사항)</p> </td> 
   <td> <p> 폴더를 조회할 폴더 경로(예: ) <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
