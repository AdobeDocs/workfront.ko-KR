---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets 모듈
description: 사용 [!DNL Adobe Experience Manager Assets] 커넥터 [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] 계정, 자산 만들기, 업로드 및 업데이트, 폴더 및 자산 복사 또는 이동.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] 모듈

사용 [!DNL Adobe Experience Manager Assets] 커넥터 [!DNL Adobe Workfront Fusion]를 설정하는 경우, [!DNL Adobe Experience Manager Assets] 계정, 자산 만들기, 업로드 및 업데이트, 폴더 및 자산 복사 또는 이동.

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

* 다음을 수행해야 합니다. [!DNL Adobe Experience Manager Assets] 이러한 모듈을 사용할 계정입니다.
* 다음을 설정해야 합니다. [!UICONTROL 서버 간] 의 흐름 [!DNL Adobe Developer console].

   설정에 대한 지침 [!UICONTROL 서버 간] 의 흐름 [!DNL Adobe Developer console]를 참조하십시오. [서버 측 API에 대한 액세스 토큰 생성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

에 대한 연결을 만들려면 [!DNL Adobe Experience Manager Assets] 모듈:

1. 클릭 [!UICONTROL 추가] 다음 [!UICONTROL 연결] 상자.

2. 생성 중인 연결 유형을 선택합니다.

   * **[!DNL AEM Assets as a Cloud Service]**

      이 구성에는 [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]**

      이 구성에는 사용자 이름과 암호가 필요합니다.

3. 만들려는 연결 유형에 대한 필드를 채웁니다.

   대상 [!DNL AEM Assets as a Cloud Service]를 참조하십시오. [연결 구성 [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   대상 [!UICONTROL AEM Assets Basic]를 참조하십시오. [연결 구성 [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. 클릭 **[!UICONTROL 계속]** 연결을 저장하고 모듈로 돌아가려면 를 클릭합니다.


### 연결 구성 [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>이러한 필드에 대한 정보는 설정의 일부로 생성됩니다 [!UICONTROL 서버 간] 흐름 [!DNL Adobe Developer Console]. 이러한 값은 해당 설정의 일부로 생성된 서비스 자격 증명 JSON 파일에서 찾을 수 있습니다.
>
>설정에 대한 지침 [!UICONTROL 서버 간] 흐름 [!UICONTROL Adobe Developer 콘솔]를 참조하십시오. [서버 측 API에 대한 액세스 토큰 생성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL 연결 이름]</td>
                  <td>
                      <p>이 연결의 이름을 입력하십시오.</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 인스턴스 URL(후행 슬래시 없음)</td>
                  <td>의 URL을 입력합니다 [!DNL Adobe Experience Manager] 인스턴스. 슬래시 포함 안 함 <code>/</code> 를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client ID]</td>
                  <td>[!UICONTROL Server-to-Server] 설정에서 생성된 클라이언트 ID를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>[!UICONTROL Server-to-Server] 설정에서 생성된 클라이언트 암호를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 기술 계정 ID]</td>
                  <td>기술 계정의 ID를 입력합니다. 클라이언트 자격 증명 JSON 파일의 "[!UICONTROL id]" 필드입니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 조직 ID]</td>
                  <td class="">조직의 ID를 입력합니다. 클라이언트 자격 증명 JSON 파일의 "[!UICONTROL org]" 필드입니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 메타 범위]</td>
                  <td>[!UICONTROL Server-to-Server] 설정에서 생성된 메타 범위를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 개인 키]</td>
                  <td>[!UICONTROL Server-to-Server] 설정에서 생성된 개인 키를 입력합니다. 개인 키를 추출하려면 [!UICONTROL 추출]을 클릭한 다음 추출할 파일과 파일의 암호를 입력합니다.</td>
              </tr>
          </tbody>
      </table>


### 연결 구성 [!DNL AEM Assets Basic]

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL 연결 이름]</td>
                <td>
                    <p>이 연결의 이름을 입력하십시오.</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL 인스턴스 URL(후행 슬래시 없음)</td>
                <td>의 URL을 입력합니다 [!DNL Adobe Experience Manager] 인스턴스. 슬래시 포함 안 함 <code>/</code> 를 입력합니다.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>사용자 이름을 입력합니다. [!DNL AEM Assets] 이 연결에서 사용하는 계정입니다.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>암호를 입력합니다. [!DNL AEM Assets] 이 연결에서 사용하는 계정입니다.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] 모듈 및 해당 필드

구성 시 [!DNL Adobe Experience Manager Essentials] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Experience Manager Essentials] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL 폴더 또는 자산 복사]

이 작업 모듈은 폴더 또는 자산을 Adobe Experience Manager Assets 계정의 다른 위치로 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>폴더를 복사할지 또는 자산을 복사할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset Selection]</td> 
   <td>복사할 폴더 또는 자산을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 경로]</td> 
   <td>경로를 선택하거나 새 폴더 또는 자산의 위치에 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 복사된 폴더의 이름] / [!UICONTROL asset]</td> 
   <td>새 폴더 또는 자산의 이름을 입력합니다. 에 표시되는 폴더 이름 [!DNL Adobe Experience Manager Assets] 은 원래 이름과 동일합니다. 여기에 입력한 이름이 새 폴더 또는 자산의 URL에 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 하위 항목 복사]</td> 
   <td>폴더 내에서 하위 폴더나 자산을 복사하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>복사되는 폴더 또는 자산과 이름이 같은 대상 위치의 폴더 또는 자산을 덮어쓰려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 만들기]

이 작업 모듈은 폴더 또는 자산 설명을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체 유형]</td> 
   <td> <p>폴더를 만들지 자산에 주석을 사용할지 여부를 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>폴더 이름을 입력합니다. 이 이름은 파일 경로에 표시되므로 공백이나 다른 문자를 포함하지 않아야 합니다. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>이름 대신 표시할 수 있는 폴더의 제목을 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset 주석]</p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p>[!UICONTROL 자산 선택]</p> <p>주석을 추가할 자산의 ID를 선택하거나 매핑합니다.</p> </li> 
       <li> <p>[!UICONTROL Comment]</p> <p>설명 텍스트를 입력합니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 삭제]

이 작업 모듈은 폴더, 자산 또는 표현물을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>폴더, 자산 또는 표현물을 삭제할 것인지 여부를 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>경로에 있는 폴더를 선택하여 삭제할 폴더를 선택합니다.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>경로에 있는 폴더를 선택한 다음 삭제할 자산을 선택하여 자산을 선택합니다.</p> </li> 
     <li> <p>[!UICONTROL Rendition]</p> <p>해당 경로에서 폴더를 선택하여 변환을 선택합니다.</p> <p>표현물의 이름을 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 폴더 목록 가져오기]

이 작업 모듈은 기존 폴더 및 해당 하위 엔티티(폴더 또는 자산)의 표현을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>검색할 폴더를 선택하거나 매핑합니다. 경로에 하위 폴더를 추가하려면 더하기 아이콘을 클릭하고 하위 폴더를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 사용자 지정 API 호출 만들기]

이 작업 모듈은 [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>을 기준으로 경로를 입력합니다 [!DNL Adobe Experience Manager] 기본 URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열] </td> 
   <td> <p>요청 쿼리 문자열을 입력합니다. 각 키/값 쌍에 대해 <b>[!UICONTROL 항목 추가]</b> [!UICONTROL Key] 및 [!UICONTROL Value]를 입력합니다.</p> </td> 
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

### [!UICONTROL 폴더 또는 자산 이동]

이 작업 모듈은 지정된 경로의 자산 또는 폴더를 새 위치로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>폴더를 이동할지 또는 자산을 이동할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset]</td> 
   <td>이동할 폴더 또는 자산을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 경로]</td> 
   <td>폴더 또는 자산을 이동할 위치에 경로를 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이동된 폴더의 이름] / [!UICONTROL asset]</td> 
   <td>이동한 폴더 또는 자산의 새 이름을 입력합니다. 에 표시되는 폴더 이름 [!DNL Adobe Experience Manager Assets] 은 원래 이름과 동일합니다. 여기에 입력한 이름이 이동한 폴더 또는 자산의 URL에 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>복사되는 폴더 또는 자산과 이름이 같은 대상 위치의 폴더 또는 자산을 덮어쓰려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 기존 레코드를 업데이트합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>자산 메타데이터 또는 자산 표현물을 삭제할지 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL Asset 메타데이터]</p> 
      <ul> 
       <li> <p>메타데이터를 업데이트할 자산을 선택합니다.</p> </li> 
       <li> <p>자산의 새 제목을 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset Rendition]</p> 
      <ul> 
       <li> <p>변환을 업데이트할 자산을 선택합니다.</p> </li> 
       <li> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 자산 업로드]

이 작업 모듈은 자산을 [!DNL Adobe Experience Manager Assets] 계정이 필요합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Adobe Experience Manager Assets] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상]</td> 
   <td> <p>자산을 업로드할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td>소스 파일의 이름과 데이터를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>
