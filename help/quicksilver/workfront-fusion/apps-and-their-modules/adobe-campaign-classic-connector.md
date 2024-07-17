---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8 모듈
description: ' [!DNL Adobe Campaign] 모듈을 사용하면  [!DNL Adobe Campaign] 계정의 이벤트를 기반으로  [!DNL Adobe Workfront Fusion] 시나리오를 시작하고, 계약 및 기타 레코드를 만들거나 읽거나 업데이트하고, 설정한 기준을 사용하여 레코드를 검색하고, 문서를 업로드할 수 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 7decc5cbf4bb2c3d4d1802dec1f369ca061f6b48
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# [!DNL Adobe Campaign]개 모듈

[!DNL Adobe Campaign] 모듈을 사용하면 [!DNL Adobe Campaign v7/v8] 계정의 이벤트를 기반으로 [!DNL Adobe Workfront Fusion] 시나리오를 시작하고, 레코드를 만들거나, 읽거나, 업데이트하고, 설정한 기준을 사용하여 레코드를 검색하고, 사용자 지정 API 호출을 수행할 수 있습니다.

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

[!DNL Adobe Campaign]에 Fusion IP 주소를 추가해야 합니다.

* Ip 주소를 Campaign에 추가하는 방법은 Adobe Campaign 설명서에서 [IP 주소를 허용 목록에 추가하다허용 목록에 추가하다 에 추가](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list)를 참조하십시오.
* 허용 목록에 추가하다에 추가할 IP 주소 목록을 보려면 [Adobe Workfront Fusion에 액세스하기 위한 IP 주소](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md)를 참조하십시오.

## [!DNL Adobe Campaign]을(를) [!DNL Adobe Workfront Fusion]에 연결

>[!IMPORTANT]
>
>서버 간 연결을 만드는 것이 좋습니다. Adobe Campaign이 서버 간 연결만 수락하도록 API를 업데이트했습니다. Campaign 버전 8 이상에 연결하는 경우 **서버 간 연결을 만들어야**&#x200B;합니다.
>
>Campaign의 새 연결 요구 사항에 대한 자세한 내용은 Campaign 설명서에서 [Campaign 기술 연산자를 Adobe Developer Console으로 마이그레이션](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html)을 참조하십시오.

1. [!DNL Adobe Campaign] 모듈에서 [!UICONTROL 연결] 필드 옆에 있는 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.
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
            <p>기본 연결을 만드는지 아니면 서버 간 연결을 만드는지 선택합니다.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 연결 이름]</td>
          <td>
            <p>이 연결의 이름을 입력하십시오.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 기본 URL]</td>
          <td>[!DNL Adobe Campaign] 인스턴스에 연결하는 데 사용하는 기본 URL을 입력하십시오.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 사용자 이름]</td>
          <td>기본 연결을 만드는 경우 Adobe Campaign 사용자 이름을 입력합니다.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Password]</td>
          <td>기본 연결을 만드는 경우 Adobe Campaign 암호를 입력합니다.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
          <td>서버 간 연결을 만드는 경우 [!DNL Adobe] [!UICONTROL 클라이언트 ID]를 입력하십시오. 이는 [!DNL Adobe Developer Console]의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
          <td>서버 간 연결을 만드는 경우 [!DNL Adobe] [!UICONTROL 클라이언트 암호]를 입력하십시오. 이는 [!DNL Adobe Developer Console]의 [!UICONTROL 자격 증명 세부 정보] 섹션에서 찾을 수 있습니다.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 환경]</td>
          <td>프로덕션 환경에 연결되어 있는지 아니면 비프로덕션 환경에 연결되어 있는지 선택합니다.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 유형]</td>
          <td>서비스 계정에 연결할지 또는 개인 계정에 연결할지 선택합니다.
        </tr>
   </tbody>
    </table>
1. 연결을 만들고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.

## [!DNL Adobe Campaign]개 모듈 및 해당 필드

[!DNL Adobe Campaign] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Adobe Campaign] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [트리거](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### 트리거

#### [!UICONTROL 레코드 보기]

이 예약된 트리거 모듈은 레코드가 변경되면 시나리오를 시작합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>새 레코드, 업데이트된 레코드 또는 둘 다 시청할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>감시할 리소스를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">출력에 포함할 [!UICONTROL 필드]</td> 
   <td>모듈의 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">출력에 포함할 [!UICONTROL 사용자 지정 필드]</td> 
   <td>출력에 포함할 각 사용자 지정 필드에 대해 <b>[!UICONTROL 추가]</b>를 클릭하고 사용자 지정 필드의 이름을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 반환되는 최대 결과 수]</td> 
   <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>


### 액션

* [[!UICONTROL 레코드 만들기]](#create-a-record)
* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)
* [[!UICONTROL 레코드 삭제]](#delete-record)
* [[!UICONTROL 작업 수행]](#perform-an-action)
* [[!UICONTROL 레코드 읽기]](#-read-a-record)
* [[!UICONTROL 구독 또는 구독 취소]](#subscribe-or-unsubscribe)
* [[!UICONTROL 레코드 업데이트]](#update-record)

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 [!DNL Adobe Campaign]에 새 레코드를 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>만들려는 [!DNL Adobe Campaign] 레코드의 형식을 선택하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 필드] </td> 
   <td>레코드를 만들 때 값을 설정할 필드를 선택한 다음 해당 필드의 값을 채웁니다. 필드는 선택하는 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 정의 필드]</td> 
   <td> 새 레코드에 추가할 각 사용자 정의 필드에 대해 <b>[!UICONTROL 항목 추가]</b>를 클릭하고 필드의 이름과 값을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 사용자 지정 API 호출 만들기]

이 모듈은 [!DNL Adobe Campaign] API에 대한 사용자 지정 API 호출을 만듭니다.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>API 호출에서 수행할 작업을 선택합니다.</p>
      <p>[!UICONTROL 쿼리 실행]</p>
      <p>[!UICONTROL 쓰기]</p>
      <p>[!UICONTROL 더 최신인 경우 엔티티 가져오기]</p>
      <p>[!UICONTROL 모두 선택]</p>
      <p>[!UICONTROL 푸시 이벤트]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] [!UICONTROL x-security] 토큰 헤더를 자동으로 추가합니다.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>세션 요소 없이 XML에 API 호출에 대한 본문 콘텐츠를 추가합니다. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 레코드 삭제]

이 작업 모듈은 [!DNL Adobe Campaign]에서 단일 레코드를 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>삭제할 리소스 유형을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>삭제할 리소스의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 작업 수행]

이 작업 모듈은 [!DNL Adobe Campaign] API의 개체에 대해 선택한 작업을 수행합니다.

특정 작업 및 필드에 대한 자세한 내용은 [[!DNL Adobe Campaign] - API 설명서](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html)를 참조하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>객체에 대해 수행할 작업을 선택합니다.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 사용 가능한 필드는 이 문서에서 <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a>을(를) 참조하십시오. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> 사용 가능한 필드는 이 문서에서 <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a>을(를) 참조하십시오. </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> 사용 가능한 필드는 이 문서에서 <a href="#create-a-record" class="MCXref xref" >[!UICONTROL 레코드 만들기]</a>를 참조하십시오. </p></li>
   <li><p><b>[!UICONTROL 업데이트]</b></p><p> 사용 가능한 필드는 이 문서에서 <a href="#update-record" class="MCXref xref" >[!UICONTROL 레코드 업데이트]</a>를 참조하십시오. </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> 사용 가능한 필드의 경우 이 문서에서 <a href="#delete-record" class="MCXref xref" >[!UICONTROL 레코드 삭제]</a>을(를) 참조하십시오. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 [!DNL Adobe Campaign]에서 레코드를 읽습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>읽으려는 [!DNL Adobe Campaign] 레코드의 형식을 선택하십시오.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>읽으려는 레코드의 ID를 입력합니다.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">출력에 포함할 [!UICONTROL 필드] </td> 
   <td>모듈의 출력에 포함할 필드를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">출력에 포함할 [!UICONTROL 사용자 지정 필드]</td> 
   <td>출력에 포함할 각 사용자 지정 필드에 대해 <b>[!UICONTROL 추가]</b>를 클릭하고 사용자 지정 필드의 이름을 입력합니다.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 구독 또는 구독 취소]

이 작업 모듈은 사용자를 정보 서비스로 가입시키거나 가입 해제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 가입 또는 가입 해지]</td> 
   <td>정보 서비스를 구독할지 또는 구독 취소할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>구독하거나 구독을 취소할 서비스를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 수신자 이메일 주소] </td> 
   <td>정보 서비스에 가입하거나 가입을 해지하려는 사용자의 이메일 주소를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 [!DNL Adobe Campaign]의 단일 레코드를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>만들려는 [!DNL Adobe Campaign] 레코드의 형식을 선택하십시오.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>업데이트할 레코드의 ID를 매핑할 항목을 입력합니다.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL 필드] </td> 
   <td>값을 업데이트할 필드를 선택한 다음 해당 필드의 값을 채웁니다. 필드는 선택하는 레코드 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 사용자 정의 필드]</td> 
   <td> 업데이트할 각 사용자 정의 필드에 대해 <b>[!UICONTROL 항목 추가]</b>를 클릭하고 필드의 이름과 값을 입력하거나 매핑하십시오. </td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

#### [!UICONTROL 검색]

이 검색 모듈은 지정된 조건을 기반으로 레코드를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>[!DNL Adobe Campaign]에 대한 연결을 만드는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >[!DNL Adobe Campaign]</a>에 대한 연결 만들기 를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>만들려는 [!DNL Adobe Campaign] 레코드의 형식을 선택하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한] </td> 
   <td>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>
