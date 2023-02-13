---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP 모듈
description: FTP 모듈을 사용하여 선택한 폴더의 파일 변경을 모니터링하고, 새 파일을 원하는 폴더로 업로드하고, 폴더에 이미 있는 기존 파일을 수정하거나 삭제할 수 있습니다.
author: Becky
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1295'
ht-degree: 0%

---

# FTP 모듈

FTP 모듈을 사용하여 선택한 폴더의 파일 변경을 모니터링하고, 새 파일을 원하는 폴더로 업로드하고, 폴더에 이미 있는 기존 파일을 수정하거나 삭제할 수 있습니다.

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

를 사용하려면 [Fusion 앱] with [!DNL Workfront Fusion]에는 FTP 계정이 있어야 합니다.

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
   <td>[!UICONTROL Host] </td> 
   <td> <p>FTP 서버 호스트 이름을 입력합니다. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Port] </td> 
   <td> <p>FTP 서버 포트 번호를 입력합니다. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User name] </td> 
   <td> <p>FTP 계정 사용자 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Password] </td> 
   <td> <p>FTP 계정 암호를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>TLS(보안 연결) 사용</p> </td> 
   <td> <p>보안 연결을 사용할지 여부를 선택합니다.</p> <p style="font-weight: bold;">[!UICONTROL No]</p> <p>연결이 보안되지 않았습니다.</p> <p style="font-weight: bold;">[!UICONTROL 명시적 암호화 또는 암시적 암호화]</p> <p>연결은 SSL을 사용하여 보호됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 권한 없는 인증서 거부]</p> </td> 
   <td> <p>이 옵션을 활성화하여 FTP 서버 인증서를 확인합니다. 확인이 실패하면 연결이 만들어지지 않습니다. 확인을 전달하려면 인증서가 다음 기준 중 하나를 충족해야 합니다.</p> 
    <ul> 
     <li>루트에 의해 서명됨 <a href="https://en.wikipedia.org/wiki/Certificate_authority">인증 기관</a></li> 
     <li>중간 인증 기관에서 서명합니다(예: <a href="https://knowledge.digicert.com/solution/SO16297.html">인증서 체인 작동 방식</a> 자세한 설명). 이 경우 모든 중간 인증서는 FTP 서버에 설치해야 합니다.</li> 
     <li>[!UICONTROL 자체 서명 인증서] 필드에서 제공하는 자체 서명 인증서여야 합니다(아래 참조).</li> </ul>

이 옵션을 비활성화하면 FTP 서버 인증서가 확인되지 않습니다. 연결을 불안정하게 하고 심각한 보안 위험을 야기하므로 이 옵션을 비활성화하지 않는 것이 좋습니다.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL 자체 서명 인증서]</p> </td> 
   <td> <p>을(를) 클릭합니다. <b>[!UICONTROL Extract]</b> 단추를 클릭하여 업로드 대화 상자를 엽니다.</p> <p>자체 서명된 인증서와 함께 TLS를 사용하도록 인증서를 업로드합니다. [!DNL Workfront Fusion] 는 파일 및 암호와 같이 제공한 데이터를 유지하거나 저장하지 않습니다. 파일 및 암호는 인증서를 추출하는 데만 사용됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP 모듈 및 해당 필드

* [Triggers](#triggers)
* [액션](#actions)

### Triggers

#### [!UICONTROL 감시 파일]

[!UICONTROL 감시 파일] 는 FTP에 대한 유일한 트리거 모듈입니다. 선택한 폴더의 파일 내용을 모니터링합니다. 지정된 폴더에 새 파일을 삽입하면 트리거가 실행됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#create-a-connection" class="MCXref xref">FTP 모듈에서 [!UICONTROL 연결 만들기]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>보려는 폴더를 선택합니다.</p> <p><b>참고:</b> 시나리오당 하나의 폴더만 허용됩니다. 하위 폴더는 무시됩니다.</p> <p><b>팁:</b> 여러 폴더를 추적하려면 각 폴더에 대해 독립적인 시나리오를 만드십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 파일 수] </td> 
   <td> <p>최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 번의 사이클로 작동합니다. 이 값을 너무 높게 설정하면 지정된 타사 서비스(시간 초과)의 측에서 연결이 중단될 수 있습니다. [!DNL Workfront Fusion] 는 이 작업에 영향을 주지 않습니다. 더 낮은 값을 설정하고 최대 주기 수에 대해 더 높은 값을 정의하거나 시나리오를 더 자주 실행하는 것이 좋습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 권한 변경]](#change-permissions)
* [[!UICONTROL 폴더 만들기]](#create-a-folder)
* [[!UICONTROL 파일 삭제]](#delete-a-file)
* [[!UICONTROL 폴더 삭제]](#delete-a-folder)
* [[!UICONTROL 파일 가져오기]](#get-a-file)
* [[!UICONTROL 폴더의 파일 목록]](#list-of-files-in-a-folder)
* [[!UICONTROL 파일 또는 폴더 이동]](#move-a-file-or-folder)
* [[!UICONTROL 업로드] 파일](#upload-a-file)

#### [!UICONTROL 권한 변경]

이 작업 모듈은 파일 또는 폴더의 권한 설정을 변경합니다.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#Create" class="MCXref xref" >FTP 모듈에서 [!UICONTROL 연결 만들기]</a> 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL 권한 설정 변경]</td>
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
               <p>원하는 파일 또는 폴더 권한을 설정합니다. chmod 매개 변수를 사용합니다. 예: <code>777 </code>또는 <code>-rwxrwxrwx</code>.</p>
               <p>사용 권한은 패턴과 일치해야 합니다 <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
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
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#Create" class="MCXref xref" >FTP 모듈에서 [!UICONTROL 연결 만들기]</a> 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL 폴더 경로]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">파일 경로를 새 폴더에 입력하거나 매핑합니다.</td>
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
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#Create" class="MCXref xref" >FTP 모듈에서 [!UICONTROL 연결 만들기]</a> 참조하십시오.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>파일을 삭제할 FTP 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 이름]</td> 
   <td> <p> 파일 이름 확장명을 포함하여 파일 이름을 입력합니다. 예: <code>[!DNL image].png</code></p> </td> 
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
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#Create" class="MCXref xref" >FTP 모듈에서 [!UICONTROL 연결 만들기]</a> 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Folder]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>파일을 삭제할 FTP 폴더를 선택합니다.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 파일 가져오기]

FTP 서버에서 파일을 검색하여 추가 처리할 수 있습니다(예: [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 연결 만들기</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 경로]</td> 
   <td> <p> 가져올 파일의 경로를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더의 파일 목록]

파일 및/또는 폴더 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 연결 만들기</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>검색할 FTP 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>파일 또는 폴더에 대한 정보를 검색할지 또는 둘 다 검색할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>검색어를 입력합니다. 검색어를 입력하지 않으면 지정된 폴더의 모든 파일과 폴더가 검색됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 파일 수]</td> 
   <td> <p> 이 모듈에서 검색한 파일의 최대 수를 설정합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 또는 폴더 이동]

이 작업 모듈은 파일이나 폴더를 다른 위치로 이동합니다.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#Create" class="MCXref xref" >FTP 모듈에서 [!UICONTROL 연결 만들기]</a> 참조하십시오.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL 이전 파일 경로]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>파일을 이동할 경로를 입력합니다. 예: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL 새 파일 경로]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>파일을 이동할 경로를 입력합니다. 예: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL 파일 업로드]

파일을 FTP 서버에 업로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>FTP 계정에 대한 연결 설정에 대한 지침은 <a href="#creating-the-ftp-connection" class="MCXref xref">FTP 연결 만들기</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>파일을 업로드할 FTP 폴더를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소스 파일] </td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기존 파일에 추가]</td> 
   <td> <p>이 옵션이 활성화되어 있고 파일이 FTP 서버에 이미 있으면 파일의 내용이 기존 파일에 추가됩니다. 이 옵션을 활성화하지 않으면 파일의 내용을 덮어씁니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더가 없는 경우 폴더 만들기] </td> 
   <td> <p>이 옵션이 활성화되어 있고 폴더 필드에 입력한 폴더가 FTP 서버에 없으면 모듈이 폴더를 만듭니다</p> </td> 
  </tr> 
 </tbody> 
</table>

## 문제 해결 {#troubleshooting}

연결을 만드는 동안 또는 모듈의 작업 중에 FTP 앱에 문제가 발생하는 경우 많이 사용되는 FTP 클라이언트 중 하나를 사용하고 동일한 작업을 수행합니다(예: 폴더에 연결 또는 목록 파일 만들기). 사용. FTP 클라이언트에도 동일한 문제가 발생하는 경우 FTP 서버의 구성이 잘못되었을 수 있습니다.
