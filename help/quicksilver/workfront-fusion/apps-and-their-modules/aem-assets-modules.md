---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets 모듈
description: ' [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] 계정의  [!DNL Adobe Experience Manager Assets] 커넥터를 사용하여 자산을 만들고, 업로드하고, 업데이트하고, 폴더 및 자산을 복사하거나 이동합니다.'
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets]개 모듈

[!DNL Adobe Workfront Fusion]에 대한 [!DNL Adobe Experience Manager Assets] 커넥터를 사용하면 [!DNL Adobe Experience Manager Assets] 계정의 이벤트를 기반으로 시나리오를 시작하고, 자산을 만들고, 업로드하고, 업데이트하며, 폴더 및 자산을 복사하거나 이동할 수 있습니다.

Adobe Experience Manager Assets 커넥터에 대한 소개는 다음을 참조하십시오.

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

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

* 이 모듈을 사용하려면 [!DNL Adobe Experience Manager Assets] 계정이 있어야 합니다.
* [!DNL Adobe Developer console]에서 [!UICONTROL 서버 간] 흐름을 설정해야 합니다.

  [!DNL Adobe Developer console]에서 [!UICONTROL 서버 간] 흐름을 설정하는 방법에 대한 지침은 [서버측 API에 대한 액세스 토큰 생성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow)을 참조하십시오.
* Adobe Experience Manager 기술 계정에 쓰기 권한이 있어야 합니다.

  Adobe Experience Manager 기술 계정에 쓰기 권한을 추가하는 방법에 대한 지침은 Adobe Experience Manager 설명서에서 [서비스 자격 증명](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)을 참조하십시오.

## Adobe Experience Manager Assets API 정보

Adobe Experience Manager Assets 커넥터는 다음을 사용합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API 태그</td> 
   <td>v1.8.61</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]에 연결 {#connect-adobe-experience-manager-assets-to-workfront-fusion}

[!DNL Adobe Experience Manager Assets] 모듈에 대한 연결을 만들려면:

1. [!UICONTROL 연결] 상자 옆에 있는 [!UICONTROL 추가]를 클릭합니다.

2. 생성 중인 연결 유형을 선택합니다.

   * **[!DNL AEM Assets as a Cloud Service]**

     이 구성에는 [!DNL Adobe Admin Console]의 정보가 필요합니다.

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     이 구성에는 사용자 이름과 암호가 필요합니다.

3. 생성 중인 연결 유형의 필드를 채웁니다.

   [!DNL AEM Assets as a Cloud Service]에 대해서는 [연결 구성 [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service)을 참조하십시오.

   [!UICONTROL AEM Assets Basic]([!DNL Adobe Managed Services])에 대해서는 [[!UICONTROL AEM Assets Basic에 대한 연결 구성]](#configure-the-connection-for-aem-assets-basic)을 참조하십시오.

4. 연결을 저장하고 모듈로 돌아가려면 **[!UICONTROL 계속]**&#x200B;을 클릭하세요.


### [!DNL AEM Assets as a Cloud Service]에 대한 연결 구성

>[!NOTE]
>
>* 이 필드에 대한 정보는 [!DNL Adobe Developer Console]에서 [!UICONTROL 서버 간] 흐름을 설정하는 과정에서 생성됩니다. 해당 설정의 일부로 생성된 서비스 자격 증명 JSON 파일에서 이러한 값을 찾을 수 있습니다.
>
>   [!UICONTROL Adobe Developer Console]에서 [!UICONTROL 서버 간] 흐름을 설정하는 방법에 대한 지침은 [Server Side API에 대한 액세스 토큰 생성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow)을 참조하십시오.
>
>* Adobe Experience Manager 기술 계정에 쓰기 권한이 있어야 합니다.
>
>   Adobe Experience Manager 기술 계정에 쓰기 권한을 추가하는 방법에 대한 지침은 Adobe Experience Manager 설명서에서 [서비스 자격 증명](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)을 참조하십시오.


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL 연결 이름]</td>
                  <td>
                      <p>이 연결의 이름 입력</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">뒤쪽 슬래시가 없는 [!UICONTROL 인스턴스 URL]</td>
                  <td>[!DNL Adobe Experience Manager] 인스턴스의 URL을 입력하십시오. URL 끝에 슬래시 <code>/</code>을(를) 포함하지 마십시오.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 계정 세부 사항 채우기 옵션]</td>
                  <td>계정 세부 정보를 설명하는 JSON을 제공할지 또는 세부 정보를 수동으로 입력할지 선택합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL JSON 형식의 기술 계정 세부 정보]</td>
                  <td>JSON을 제공하는 경우 계정 세부 사항을 설명하는 JSON을 입력하거나 붙여 넣습니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
                  <td>세부 정보를 수동으로 입력하는 경우 [!UICONTROL 서버 간] 설정에서 생성된 클라이언트 ID를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
                  <td>세부 정보를 수동으로 입력하는 경우 [!UICONTROL 서버 간] 설정에서 생성된 클라이언트 암호를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 기술 계정 ID]</td>
                  <td>세부 정보를 수동으로 입력하는 경우 기술 계정의 ID를 입력합니다. 클라이언트 자격 증명 JSON 파일의 "[!UICONTROL ID]" 필드입니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 조직 ID]</td>
                  <td class="">상세내역을 수동으로 입력하는 경우 조직의 ID를 입력합니다. 클라이언트 자격 증명 JSON 파일의 "[!UICONTROL org]" 필드입니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 메타 범위]</td>
                  <td>[!UICONTROL 서버 간] 설정에서 생성된 메타 범위를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 개인 키]</td>
                  <td>[!UICONTROL Server-to-Server] 설정에서 생성된 개인 키를 입력합니다. 개인 키를 추출하려면 [!UICONTROL Extract]를 클릭한 다음 추출할 파일과 해당 파일의 암호를 입력합니다.</td>
              </tr>
          </tbody>
      </table>


### [!DNL AEM Assets Basic]([!DNL Adobe Managed Services])에 대한 연결 구성

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL 연결 이름]</td>
                <td>
                    <p>이 연결의 이름 입력</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">뒤쪽 슬래시가 없는 [!UICONTROL 인스턴스 URL]</td>
                <td>[!DNL Adobe Experience Manager] 인스턴스의 URL을 입력하십시오. URL 끝에 슬래시 <code>/</code>을(를) 포함하지 마십시오.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL 사용자 이름]</td>
                <td>이 연결에서 사용하는 [!DNL AEM Assets] 계정의 사용자 이름을 입력하십시오.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>이 연결에서 사용하는 [!DNL AEM Assets] 계정의 암호를 입력하십시오.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets]개 모듈 및 해당 필드

[!DNL Adobe Experience Manager Essentials] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 [!DNL Adobe Experience Manager Essentials] 필드가 추가로 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [폴더 또는 자산 복사](#copy-a-folder-or-asset)
* [레코드 만들기](#create-a-record)
* [폴더, 에셋 또는 렌디션 삭제](#delete-a-folder-asset-or-rendition)
* [폴더 목록 가져오기](#get-a-folder-listing)
* [사용자 지정 API 호출 만들기](#make-a-custom-api-call)
* [폴더 또는 자산 이동](#move-a-folder-or-asset)
* [레코드 업데이트](#update-a-record)
* [에셋 업로드](#upload-an-asset)

### [!UICONTROL 폴더 또는 자산 복사]

이 작업 모듈은 폴더 또는 에셋을 Adobe Experience Manager Assets 계정의 다른 위치에 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>폴더를 복사할지 자산을 복사할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset selection]</td> 
   <td>복사할 폴더 또는 자산을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 경로]</td> 
   <td>경로를 선택하거나 새 폴더 또는 에셋의 위치에 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 복사된 폴더 이름] / [!UICONTROL 자산]</td> 
   <td>새 폴더 또는 에셋의 이름을 입력합니다. [!DNL Adobe Experience Manager Assets]에 표시되는 폴더 이름이 원래 이름과 같습니다. 여기에 입력한 이름은 새 폴더 또는 에셋의 URL에 나타납니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 하위 항목 복사]</td> 
   <td>폴더 내의 하위 폴더 또는 에셋을 복사하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 덮어쓰기]</td> 
   <td>대상 위치의 폴더 또는 에셋 중 복사할 폴더 또는 에셋과 같은 이름을 가진 폴더 또는 에셋을 덮어쓰려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 만들기]

이 작업 모듈은 폴더 또는 에셋 주석을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 개체 유형]</td> 
   <td> <p>에셋에 대해 폴더 또는 댓글을 작성할지 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 폴더]</p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p>[!UICONTROL 이름]</p> <p>폴더 이름을 입력합니다. 이 이름은 파일 경로에 나타나므로 공백이나 다른 문자를 포함해서는 안 됩니다. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>이름 대신 표시할 수 있는 폴더의 제목을 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL 자산 주석]</p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p>[!UICONTROL 자산 선택]</p> <p>댓글을 추가할 에셋의 ID를 선택하거나 매핑합니다.</p> </li> 
       <li> <p>[!UICONTROL Comment]</p> <p>주석의 텍스트를 입력합니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 폴더, 에셋 또는 렌디션 삭제]

이 작업 모듈은 폴더, 에셋 또는 렌디션을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>폴더, 에셋 또는 렌디션을 삭제할 것인지 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 폴더]</p> <p>경로에서 폴더를 선택하여 삭제할 폴더를 선택합니다.</p> </li> 
     <li> <p>[!UICONTROL 자산] </p> <p>경로에 있는 폴더를 선택한 다음 삭제할 자산을 선택하여 자산을 선택합니다.</p> </li> 
     <li> <p>[!UICONTROL 렌디션]</p> <p>해당 경로의 폴더를 선택하여 렌디션을 선택합니다.</p> <p>렌디션의 이름을 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 폴더 목록 가져오기]

이 작업 모듈은 기존 폴더 및 그 하위 엔티티(폴더 또는 에셋)의 표현을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더]</td> 
   <td>검색할 폴더를 선택하거나 매핑합니다. 경로에 하위 폴더를 추가하려면 더하기 아이콘을 클릭하고 하위 폴더를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 사용자 지정 API 호출 만들기]

이 작업 모듈은 [!DNL Adobe Experience Manager Assets] API에 대한 사용자 지정 API 호출을 만듭니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>[!DNL Adobe Experience Manager] 기본 URL에 상대적인 경로를 입력하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 [!DNL Adobe Workfront Fusion]</a>에서 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP 요청 메서드를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열] </td> 
   <td> <p>요청 쿼리 문자열을 입력합니다. 각 키/값 쌍에 대해 <b>[!UICONTROL 항목 추가]</b>를 클릭하고 [!UICONTROL 키] 및 [!UICONTROL 값]을 입력합니다.</p> </td> 
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

### [!UICONTROL 폴더 또는 자산 이동]

이 작업 모듈은 지정된 경로의 에셋 또는 폴더를 새 위치로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>폴더를 이동할지 자산을 이동할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더] / [!UICONTROL 자산]</td> 
   <td>이동할 폴더 또는 자산을 선택하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상 경로]</td> 
   <td>폴더 또는 자산을 이동할 위치를 선택하거나 경로를 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 이동한 폴더의 이름] / [!UICONTROL 자산]</td> 
   <td>이동한 폴더 또는 에셋의 새 이름을 입력합니다. [!DNL Adobe Experience Manager Assets]에 표시되는 폴더 이름이 원래 이름과 같습니다. 여기에 입력한 이름은 이동한 폴더 또는 에셋의 URL에 표시됩니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 덮어쓰기]</td> 
   <td>대상 위치의 폴더 또는 에셋 중 복사할 폴더 또는 에셋과 같은 이름을 가진 폴더 또는 에셋을 덮어쓰려면 이 옵션을 활성화합니다.</td> 
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
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>에셋 메타데이터 또는 에셋 렌디션을 삭제할지 선택합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 자산 메타데이터]</p> 
      <ul> 
       <li> <p>메타데이터를 업데이트할 자산을 선택합니다.</p> </li> 
       <li> <p>에셋의 새 제목을 입력합니다.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL 자산 렌디션]</p> 
      <ul> 
       <li> <p>렌디션을 업데이트할 에셋을 선택합니다.</p> </li> 
       <li> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 자산 업로드]

이 작업 모듈은 자산을 [!DNL Adobe Experience Manager Assets] 계정에 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Adobe Experience Manager Assets] 계정을 [!DNL Workfront Fusion]에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">[!DNL Adobe Experience Manager Assets]을(를) [!DNL Workfront Fusion]</a>에 연결 을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상]</td> 
   <td> <p>에셋을 업로드할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source 파일]</td> 
   <td>소스 파일의 이름과 데이터를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>
