---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP 모듈
description: 다음 [!DNL Adobe Workfront Fusion SFTP] 모듈을 사용하면 선택한 폴더/하위 폴더에 있는 파일 변경을 모니터링하거나, 새 파일을 원하는 폴더에 업로드하거나, 폴더에 이미 있는 기존 파일을 수정 또는 삭제하거나, 파일 권한을 변경할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# SFTP 모듈

다음 [!DNL Adobe Workfront Fusion] SFTP 모듈을 사용하면 선택한 폴더/하위 폴더에 있는 파일 변경 사항을 모니터링하거나, 새 파일을 원하는 폴더에 업로드하거나, 폴더에 이미 있는 기존 파일을 수정 또는 삭제하거나, 파일 권한을 변경할 수 있습니다.

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

와 함께 SFTP를 사용하기 위해 [!DNL Workfront Fusion]를 설정하는 경우 SFTP 계정이 있어야 합니다(예: [!DNL GoDaddy] 웹 호스팅).

## SFTP를에 연결 [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

SFTP 계정을 [!DNL Workfront Fusion] 대상 호스트 및 모듈의 SFTP 자격 증명(사용자 이름 및 암호 또는 사용자 이름 및 키)을 입력해야 합니다 [!UICONTROL 연결 만들기] 대화 상자.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 연결 이름]</td> 
   <td> <p> SFTP 연결의 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>연결할 SFTP 서버의 호스트 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>SFTP 서버 포트를 입력합니다. 예를 들어 22입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 인증 유형]</p> </td> 
   <td> <p>SFTP 서버에 연결하는 데 사용할 인증 방법을 선택합니다.</p> 
    <ul> 
     <li><strong>[!UICONTROL 사용자 이름 및 암호]</strong>: 자격 증명을 입력합니다.</li> 
     <li> <p><strong>[!UICONTROL 사용자 이름 및 키]</strong>: 사용자 이름과 개인 키/인증서를 입력합니다</p> <p>자체 서명된 인증서를 사용하여 TLS를 사용하려면 클라이언트 측 인증을 사용하거나 인증서(P12 또는 PFX 파일)를 업로드하려면 개인 키를 업로드하십시오. 클라이언트측 인증서 인증을 사용하는 경우 여기에 CA 인증서를 입력할 수 있습니다.</p> <p>[!DNL Workfront Fusion] 는 여기에 제공한 데이터(파일, 암호)를 유지하거나 저장하지 않습니다. 파일 및 암호는 개인 키/인증서를 추출하는 데만 사용됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

연결 정보를 입력한 후 **[!UICONTROL 계속]** 연결을 설정하려면 다음을 수행하십시오.

## [!UICONTROL SFTP] 모듈 및 해당 필드

구성 시 [!UICONTROL SFTP] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!UICONTROL SFTP] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL 폴더에서 파일 보기]

지정된 폴더에서 파일을 만들거나 변경할 때 세부 사항이 있는 파일을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>보려는 폴더를 입력하거나 매핑합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>버퍼 크기 [B]</td> 
   <td> <p> 버퍼 크기를 바이트 단위로 입력합니다. 값은 서버에서 전송된 청크의 크기를 정의합니다. 값이 너무 높으면 일부 서버에서 문제가 발생하거나 파일이 손상될 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 파일 수]</td> 
   <td> <p> 최대 파일 수 설정 [!DNL Workfront Fusion] 한 번의 사이클로 작동함</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더에서 하위 폴더 보기]

지정된 폴더에서 폴더를 만들거나 변경할 때 세부 정보가 있는 폴더를 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>보려는 폴더를 입력하거나 매핑합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 파일 수]</td> 
   <td> <p> 최대 폴더 수 설정 [!DNL Workfront Fusion] 은 한 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

#### [!UICONTROL 폴더 컨텐츠 나열]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>파일, 폴더 또는 둘 다 검색할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>나열할 파일 또는 폴더가 포함된 폴더를 입력하거나 매핑합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>검색어를 입력하거나 매핑합니다. 예를 들어 파일 확장명이 .txt인 파일을 검색하려면 을 입력합니다. <code>.txt</code>검색할 파일의 이름을 입력하거나 매핑할 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 정렬 기준]</td> 
   <td> <p> 파일 이름, 크기, 마지막 액세스 날짜 또는 마지막 수정 날짜별로 결과를 정렬할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 정렬 순서] </td> 
   <td> <p>결과를 오름차순으로 반환할지 또는 내림차순으로 반환할지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 모듈이 결과를 반환하지 않더라도 경로 실행을 계속합니다.]</p> </td> 
   <td>결과를 반환하지 않는 경우 이 모듈에서 시나리오를 중지하지 않도록 하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 결과 수]</td> 
   <td> <p> 최대 결과 수 설정 [!DNL Workfront Fusion] 은 한 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

이 모듈은 지정된 폴더의 파일을 나열합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 버퍼 크기 [B]]</td> 
   <td> <p> 버퍼 크기를 바이트 단위로 입력합니다. 값은 서버에서 전송된 청크의 크기를 정의합니다. 값이 너무 높으면 일부 서버에서 문제가 발생하거나 파일이 손상될 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>나열할 파일 또는 폴더가 포함된 폴더를 입력하거나 매핑합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>검색어를 입력하거나 매핑합니다. 예를 들어 파일 확장명이 .txt인 파일을 검색하려면 을 입력합니다. <code>.txt</code>검색할 파일의 이름을 입력하거나 매핑할 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 정렬 기준]</td> 
   <td> <p> 파일 이름, 크기, 마지막 액세스 날짜 또는 마지막 수정 날짜별로 결과를 정렬할지 여부를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 정렬 순서]</td> 
   <td> <p> 결과를 오름차순으로 반환할지 또는 내림차순으로 반환할지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 모듈이 결과를 반환하지 않더라도 경로 실행을 계속합니다.]</p> </td> 
   <td>결과를 반환하지 않는 경우 이 모듈에서 시나리오를 중지하지 않도록 하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 반환된 최대 결과 수]</td> 
   <td> <p> 최대 파일 수 설정 [!DNL Workfront Fusion] 은 한 주기 동안 반환됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

이 모듈은 파일의 데이터를 포함하여 파일 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 버퍼 크기 [B]]</td> 
   <td> <p> 버퍼 크기를 바이트 단위로 입력합니다. 값은 서버에서 전송된 청크의 크기를 정의합니다. 값이 너무 높으면 일부 서버에서 문제가 발생하거나 파일이 손상될 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 경로] </td> 
   <td> <p>파일의 경로를 입력합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/file.txt</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 업로드]

이 모듈에서 파일을 SFTP 서버에 업로드할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>기존 폴더를 파일의 저장 위치로 지정합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소스 파일]</td> 
   <td> <p> [!UICONTROL Dropbox] &gt; [!UICONTROL 파일 가져오기]와 같은 이전 모듈의 소스 파일을 매핑합니다. 파일 이름과 파일 데이터를 입력하거나 매핑할 수도 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 권한]</p> </td> 
   <td> <p>파일 또는 폴더에 대해 원하는 권한을 설정합니다. chmod 매개 변수를 사용합니다. 예: <code>777 </code>또는 <code>-rwxrwxrwx</code>.</p> <p>chmod에 대한 자세한 내용은 <a href="https://ss64.com/bash/chmod.html">chmod 설명서</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 이름 바꾸기]

파일 이름을 변경합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 경로]</td> 
   <td> <p> 이름을 바꿀 파일의 경로를 입력합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/file.txt</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 파일 이름]</td> 
   <td> <p> 파일 확장명을 포함하여 파일의 새 이름을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 이동]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 경로]</td> 
   <td> <p> 이동할 파일의 경로를 입력합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/file.txt</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 새 폴더]</td> 
   <td> <p> 파일의 새 위치에 대한 경로를 입력합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 삭제]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 경로]</td> 
   <td> <p> 삭제할 파일의 경로를 입력합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/file.txt</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 권한 업데이트]

파일의 권한을 변경할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 파일 경로]</td> 
   <td> <p> 이동할 파일의 경로를 입력합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/file.txt</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 권한]</p> </td> 
   <td> <p>원하는 파일 권한을 설정합니다. chmod 매개 변수를 사용합니다. 예, <code>777 </code>또는 <code>-rwxrwxrwx</code>.</p> <p>패턴과 일치해야 함 <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>chmod에 대한 자세한 내용은 <a href="https://ss64.com/bash/chmod.html">chmod 설명서</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 만들기]

지정된 위치에 새 폴더를 만듭니다.

>[!NOTE]
>
>폴더가 이미 있으면 모듈에 오류가 발생합니다. 플로우를 중단되지 않고 계속하려면 오류 처리기 경로를 모듈에 연결하여 오류를 포착하고 [!UICONTROL 다시 시작] 흐름을 계속하기 위한 지시입니다. 오류 처리기 경로 연결에 대한 자세한 내용은 [에서 오류 처리 중 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). 오류 처리기 경로에 대한 자세한 내용은 [에서 오류 처리를 위한 지시어 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>기존 폴더를 새 폴더의 저장소 위치로 지정합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/file.txt</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 폴더 이름]</td> 
   <td> <p> 폴더 이름을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 권한]</p> </td> 
   <td> <p>원하는 폴더 권한을 설정합니다. chmod 매개 변수를 사용합니다. 예, <code>777 </code>또는 <code>-rwxrwxrwx</code>.</p> <p>패턴과 일치해야 함 <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>chmod에 대한 자세한 내용은 <a href="https://ss64.com/bash/chmod.html">chmod Man 페이지</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 폴더 삭제]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>SFTP 계정을 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP를에 연결 [!DNL Workfront Fusion]</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> 삭제할 폴더의 경로를 지정합니다. 다음과 같은 절대 경로를 지정할 수 있습니다. <code>/home/user/</code>. 또는 로그인된 사용자의 특정 폴더를 가리키는 상대 경로를 지정할 수 있습니다(예: ) <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
