---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets 모듈
description: 포함 [!DNL Adobe Experience Manager Assets] 커넥터 [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] 에셋을 계정, 생성, 업로드 및 업데이트하고 폴더 및 에셋을 복사하거나 이동합니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1544'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] 모듈

포함 [!DNL Adobe Experience Manager Assets] 커넥터 [!DNL Adobe Workfront Fusion], 의 이벤트를 기반으로 시나리오를 시작할 수 있습니다. [!DNL Adobe Experience Manager Assets] 에셋을 계정, 생성, 업로드 및 업데이트하고 폴더 및 에셋을 복사하거나 이동합니다.

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

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

* 다음 항목이 있어야 합니다. [!DNL Adobe Experience Manager Assets] 계정 을 클릭하여 이러한 모듈을 사용합니다.
* 다음을 설정해야 합니다. [!UICONTROL 서버 간] 흐름 [!DNL Adobe Developer console].

  설정에 대한 지침 [!UICONTROL 서버 간] 흐름 [!DNL Adobe Developer console], 참조 [서버측 API용 액세스 토큰 생성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## 연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

에 대한 연결을 만들려면 [!DNL Adobe Experience Manager Assets] 모듈:

1. 클릭 [!UICONTROL 추가] 다음 옆에 [!UICONTROL 연결] 상자.

2. 생성 중인 연결 유형을 선택합니다.

   * **[!DNL AEM Assets as a Cloud Service]**

     이 구성을 사용하려면 다음 위치의 정보가 필요합니다. [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     이 구성에는 사용자 이름과 암호가 필요합니다.

3. 생성 중인 연결 유형의 필드를 채웁니다.

   대상 [!DNL AEM Assets as a Cloud Service], 참조 [다음에 대한 연결 구성 [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   대상 [!UICONTROL AEM Assets 기본] ([!DNL Adobe Managed Services]), 다음을 참조하십시오. [다음에 대한 연결 구성 [!UICONTROL AEM Assets 기본]](#configure-the-connection-for-aem-assets-basic).

4. 클릭 **[!UICONTROL 계속]** 연결을 저장하고 모듈로 돌아갑니다.


### 다음에 대한 연결 구성 [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>이러한 필드에 대한 정보는 설정의 일부로 생성됩니다 [!UICONTROL 서버 간] 플로우 [!DNL Adobe Developer Console]. 해당 설정의 일부로 생성된 서비스 자격 증명 JSON 파일에서 이러한 값을 찾을 수 있습니다.
>
>설정에 대한 지침 [!UICONTROL 서버 간] 플로우 [!UICONTROL Adobe Developer 콘솔], 참조 [서버측 API용 액세스 토큰 생성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


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
                  <td>에 대한 URL을 입력합니다. [!DNL Adobe Experience Manager] 인스턴스. 슬래시를 포함하지 않음 <code>/</code> URL의 끝 부분에 있어야 합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 클라이언트 ID]</td>
                  <td>[!UICONTROL Server-to-Server] 설정에서 생성된 클라이언트 ID를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 클라이언트 암호]</td>
                  <td>[!UICONTROL Server-to-Server] 설정에서 생성된 클라이언트 암호를 입력합니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 기술 계정 ID]</td>
                  <td>기술 계정의 ID를 입력합니다. 클라이언트 자격 증명 JSON 파일의 "[!UICONTROL ID]" 필드입니다.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL 조직 ID]</td>
                  <td class="">조직의 ID를 입력합니다. 클라이언트 자격 증명 JSON 파일의 "[!UICONTROL org]" 필드입니다.</td>
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


### 다음에 대한 연결 구성 [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

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
                <td>에 대한 URL을 입력합니다. [!DNL Adobe Experience Manager] 인스턴스. 슬래시를 포함하지 않음 <code>/</code> URL의 끝 부분에 있어야 합니다.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL 사용자 이름]</td>
                <td>에 대한 사용자 이름 입력 [!DNL AEM Assets] 이 연결이 사용하는 계정입니다.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>다음에 대한 암호 입력 [!DNL AEM Assets] 이 연결이 사용하는 계정입니다.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] 모듈 및 해당 필드

를 구성할 때 [!DNL Adobe Experience Manager Essentials] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Adobe Experience Manager Essentials] 앱이나 서비스의 액세스 수준 등에 따라 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL 폴더 또는 자산 복사]

이 작업 모듈은 폴더 또는 에셋을 Adobe Experience Manager 에셋 계정의 다른 위치에 복사합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
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
   <td>새 폴더 또는 에셋의 이름을 입력합니다. 에 표시되는 폴더 이름 [!DNL Adobe Experience Manager Assets] 은 원래 이름과 동일합니다. 여기에 입력한 이름은 새 폴더 또는 에셋의 URL에 나타납니다.</td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
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

### [!UICONTROL 레코드 삭제]

이 작업 모듈은 폴더, 에셋 또는 렌디션을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 폴더]</td> 
   <td>검색할 폴더를 선택하거나 매핑합니다. 경로에 하위 폴더를 추가하려면 더하기 아이콘을 클릭하고 하위 폴더를 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 사용자 지정 API 호출 만들기]

이 작업 모듈은에 대한 사용자 지정 API 호출을 만듭니다. [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>에 상대적인 경로 입력 [!DNL Adobe Experience Manager] 기본 URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 메서드]</p> </td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>표준 JSON 개체 형태로 요청의 헤더를 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 인증 헤더를 자동으로 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열] </td> 
   <td> <p>요청 쿼리 문자열을 입력합니다. 각 키/값 쌍에 대해 <b>[!UICONTROL 항목 추가]</b> [!UICONTROL 키] 및 [!UICONTROL 값]을 입력합니다.</p> </td> 
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

### [!UICONTROL 폴더 또는 자산 이동]

이 작업 모듈은 지정된 경로의 에셋 또는 폴더를 새 위치로 이동합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
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
   <td>이동한 폴더 또는 에셋의 새 이름을 입력합니다. 에 표시되는 폴더 이름 [!DNL Adobe Experience Manager Assets] 은 원래 이름과 동일합니다. 여기에 입력한 이름은 이동한 폴더 또는 에셋의 URL에 표시됩니다.</td> 
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
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
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

### [!UICONTROL 에셋 업로드]

이 작업 모듈은 에셋을 [!DNL Adobe Experience Manager Assets] 계정입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결에 대한 자세한 내용 [!DNL Adobe Experience Manager Assets] 계정 위치: [!DNL Workfront Fusion], 참조 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">연결 [!DNL Adobe Experience Manager Assets] 끝 [!DNL Workfront Fusion]</a> 이 문서에서.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 대상]</td> 
   <td> <p>에셋을 업로드할 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td>소스 파일의 이름과 데이터를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>
