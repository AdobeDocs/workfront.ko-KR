---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP 모듈
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 0%

---

# FTP 모듈

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [FTP 모듈](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/ftp-modules.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

FTP 모듈을 사용하면 선택한 폴더의 파일 변경 사항을 모니터링하고, 새 파일을 원하는 폴더에 업로드하고, 폴더에 이미 있는 기존 파일을 수정하거나 삭제할 수 있습니다.

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

[!DNL Workfront Fusion]에서 [Fusion 앱]을 사용하려면 FTP 계정이 있어야 합니다.

## FTP 모듈에서 연결 만들기 {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 연결 이름]</td> 
   <td> <p> FTP 연결의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 호스트] </td> 
   <td> <p>FTP 서버 호스트 이름을 입력합니다. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 포트] </td> 
   <td> <p>FTP 서버 포트 번호를 입력합니다. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 사용자 이름] </td> 
   <td> <p>FTP 계정 사용자 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Password] </td> 
   <td> <p>FTP 계정 암호를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>TLS(보안 연결) 사용</p> </td> 
   <td> <p>보안 연결을 사용할지 여부를 선택합니다.</p> <p style="font-weight: bold;">[!UICONTROL No]</p> <p>연결이 보호되지 않습니다.</p> <p style="font-weight: bold;">[!UICONTROL 명시적 암호화 또는 암시적 암호화]</p> <p>연결은 SSL을 사용하여 보호됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 승인되지 않은 인증서 거부]</p> </td> 
   <td> <p>FTP 서버 인증서를 확인하려면 이 옵션을 활성화하십시오. 확인에 실패하면 연결이 만들어지지 않습니다. 인증을 통과하려면 인증서가 다음 기준 중 하나를 충족해야 합니다.</p> 
    <ul> 
     <li>루트 <a href="https://en.wikipedia.org/wiki/Certificate_authority">인증 기관</a>에서 서명합니다.</li> 
     <li>중간 인증 기관에서 서명합니다(예: <a href="https://knowledge.digicert.com/solution/SO16297.html">인증서 체인이 작동하는 방법</a> 참조). 이 경우 모든 중간 인증서를 FTP 서버에 설치해야 합니다.</li> 
     <li>[!UICONTROL 자체 서명된 인증서] 필드에 제공된 자체 서명된 인증서여야 합니다(아래 참조)</li> </ul>

이 옵션이 비활성화되어 있으면 FTP 서버 인증서가 확인되지 않습니다. 연결을 안전하지 않게 만들고 심각한 보안 위험을 초래하므로 옵션을 비활성화하지 않는 것이 좋습니다.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL 자체 서명된 인증서]</p> </td> 
   <td> <p>업로드 대화 상자를 열려면 <b>[!UICONTROL 추출]</b> 단추를 클릭하십시오.</p> <p>자체 서명된 인증서와 함께 TLS를 사용하려면 인증서를 업로드하십시오. [!DNL Workfront Fusion]은(는) 파일 및 암호와 같이 사용자가 제공한 데이터를 유지하거나 저장하지 않습니다. 파일 및 암호는 인증서를 추출하는 데만 사용됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP 모듈 및 해당 필드

* [트리거](#triggers)
* [액션](#actions)

### 트리거

#### [!UICONTROL 파일 보기]

[!UICONTROL 파일 보기]가 FTP용 유일한 트리거 모듈입니다. 선택한 폴더의 파일 컨텐츠를 모니터링합니다. 트리거는 새 파일이 지정된 폴더에 삽입되면 실행됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>FTP 계정에 연결하는 방법에 대한 지침은 이 문서의 FTP 모듈</a>에서 <a href="#create-a-connection" class="MCXref xref">[!UICONTROL 연결 만들기]를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 폴더]</p> </td> 
   <td> <p>감시할 폴더를 선택합니다.</p> <p><b>참고:</b> 시나리오당 하나의 폴더만 허용됩니다. 하위 폴더는 무시됩니다.</p> <p><b>팁:</b> 여러 폴더를 추적하려면 각 폴더에 대해 독립적인 시나리오를 만드십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환되는 최대 파일 수] </td> 
   <td> <p>한 주기 동안 [!DNL Workfront Fusion]에서 사용할 최대 결과 수를 설정하십시오. 값이 너무 높게 설정되면 지정된 타사 서비스 측에서 연결이 중단될 수 있습니다(시간 초과). [!DNL Workfront Fusion]은(는) 이 작업에 영향을 주지 않습니다. 낮은 값을 설정하고 최대 주기 횟수에 대해 높은 값을 정의하거나 시나리오를 더 자주 실행하는 것이 좋습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 권한 변경]](#change-permissions)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 파일 삭제]](#delete-a-file)
* [[!UICONTROL 폴더 삭제]](#delete-a-folder)
* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 폴더에 있는 파일 목록]](#list-of-files-in-a-folder)
* [[!UICONTROL 파일 또는 폴더 이동]](#move-a-file-or-folder)
* [파일 [!UICONTROL 업로드]](#upload-a-file)

#### [!UICONTROL 권한 변경]

이 작업 모듈은 파일 또는 폴더의 권한 설정을 변경합니다.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP 계정에 연결하는 방법에 대한 지침은 이 문서의 FTP 모듈</a>에서 <a href="#Create" class="MCXref xref" >[!UICONTROL 연결 만들기]를 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL 의 권한 설정 변경]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>파일 또는 폴더의 설정을 변경할지 여부를 선택합니다.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL 파일 경로]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">폴더 또는 파일에 파일 경로를 입력하거나 매핑합니다.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL 권한]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>원하는 파일 또는 폴더 권한을 설정합니다. chmod 매개 변수를 사용합니다. 예: <code>777 </code> 또는 <code>-rwxrwxrwx</code>.</p>
               <p>사용 권한은 <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code> 패턴과 일치해야 합니다.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 폴더 만들기]

이 작업 모듈은 새 폴더를 만듭니다.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP 계정에 연결하는 방법에 대한 지침은 이 문서의 FTP 모듈</a>에서 <a href="#Create" class="MCXref xref" >[!UICONTROL 연결 만들기]를 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL 폴더 경로]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">파일 경로를 입력하거나 새 폴더에 매핑합니다.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL 새 폴더 이름]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>새 폴더의 이름을 입력하거나 매핑합니다.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 파일 삭제]

지정된 폴더에서 파일을 삭제합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP 계정에 연결하는 방법에 대한 지침은 이 문서의 FTP 모듈</a>에서 <a href="#Create" class="MCXref xref" >[!UICONTROL 연결 만들기]를 참조하십시오.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>파일을 삭제할 FTP 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 이름]</td> 
   <td> <p> 파일 이름 확장자를 포함하여 파일 이름을 입력합니다. 예: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 삭제]

이 작업 모듈은 지정된 폴더를 영구적으로 삭제합니다.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">FTP 계정에 연결하는 방법에 대한 지침은 이 문서의 FTP 모듈</a>에서 <a href="#Create" class="MCXref xref" >[!UICONTROL 연결 만들기]를 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL 폴더]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>파일을 삭제할 FTP 폴더를 선택합니다.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 파일 가져오기]

추가 처리(예: [!DNL Dropbox](으)로 업로드)할 수 있는 FTP 서버에서 파일을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>FTP 계정에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 연결 만들기</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 경로]</td> 
   <td> <p> 가져올 파일의 경로를 입력하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더에 있는 파일 목록]

파일 및/또는 폴더 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>FTP 계정에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 연결 만들기</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>검색할 FTP 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 표시] </td> 
   <td> <p>파일 또는 폴더에 대한 정보를 검색할지 또는 둘 다에 대한 정보를 검색할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>검색어를 입력합니다. 검색어를 입력하지 않으면 지정된 폴더의 모든 파일과 폴더가 검색됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환되는 최대 파일 수]</td> 
   <td> <p> 이 모듈에서 검색된 최대 파일 수를 설정합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 또는 폴더 이동]

이 작업 모듈은 파일 또는 폴더를 다른 위치로 이동합니다.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">FTP 계정에 연결하는 방법에 대한 지침은 이 문서의 FTP 모듈</a>에서 <a href="#Create" class="MCXref xref" >[!UICONTROL 연결 만들기]를 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL 이전 파일 경로]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>파일을 이동할 경로를 입력합니다. 예: <code>/folder1/document.txt</code></p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL 새 파일 경로]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>파일을 이동할 경로를 입력합니다. 예: <code>/folder2/document.txt</code></p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL 파일 업로드]

FTP 서버에 파일을 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>FTP 계정에 연결하는 방법에 대한 지침은 이 문서에서 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 연결 만들기</a>를 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더] </td> 
   <td> <p>파일을 업로드할 FTP 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source 파일] </td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기존 파일에 추가]</td> 
   <td> <p>이 옵션을 활성화하고 파일이 FTP 서버에 이미 있으면 파일의 내용이 기존 파일에 추가됩니다. 이 옵션을 활성화하지 않으면 파일의 내용을 덮어씁니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 존재하지 않는 경우 폴더 만들기] </td> 
   <td> <p>이 옵션을 활성화하고 폴더 필드에 입력한 폴더가 FTP 서버에 없는 경우 모듈이 폴더를 만듭니다</p> </td> 
  </tr> 
 </tbody> 
</table>

## 문제 해결 {#troubleshooting}

연결 생성 중이나 모듈 작업 중에 FTP 앱에 문제가 발생하는 경우 자주 사용하는 FTP 클라이언트 중 하나를 사용하고 동일한 작업(예: 연결을 만들거나 폴더에 파일을 나열)을 수행해 보십시오. FTP 클라이언트 사용. FTP 클라이언트에서도 동일한 문제가 발생하는 경우 FTP 서버의 구성이 잘못되었을 수 있습니다.
