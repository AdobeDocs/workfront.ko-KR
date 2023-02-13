---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Azure DevOps 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Azure DevOps]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1749'
ht-degree: 0%

---

# [!DNL Azure DevOps] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Azure DevOps]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

를 사용하려면 [!DNL Azure DevOps] 모듈이면 반드시 [!DNL Azure] DevOps 계정.

## Connect [!DNL Azure DevOps] to [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. 추가 [!DNL Azure DevOps] 모듈에 대해 고려합니다.
1. 클릭 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 에서 [!UICONTROL 연결 유형] 필드, 선택 **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >다음 [!UICONTROL [!DNL Azure DevOps] (모든 범위 요청)] 연결 유형은 가까운 미래에 더 이상 사용되지 않습니다. 따라서 사용하지 않는 것이 좋습니다.

1. 다음 필드를 채웁니다.

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL 연결 이름]</td>
            <td>생성 중인 연결의 이름을 입력합니다.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>생성된 조직의 이름을 입력합니다 [!DNL Azure DevOps] 응용 프로그램.</td>
        </tr>
    </table>

1. 클릭 **[!UICONTROL 계속]** 연결 설정을 완료하고 시나리오 만들기를 계속 수행하려면 다음을 수행하십시오.

## [!UICONTROL Azure DevOps] 모듈 및 해당 필드

구성 시 [!DNL Azure DevOps] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Azure DevOps] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [액션](#actions)
* [검색 결과](#searches)

### Triggers

#### [!UICONTROL 작업 항목 보기]

이 인스턴트 트리거 모듈은 레코드가 추가, 업데이트 또는 삭제될 때 시나리오를 실행합니다 [!UICONTROL Azure DevOps].

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>모듈의 웹 후크를 선택하거나 추가합니다.</p> <p>트리거 모듈의 웹 후크에 대한 자세한 내용은 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">의 즉각적인 트리거(웹 후크) [!DNL Adobe Workfront Fusion]</a>.</p> <p>웹 후크를 만드는 방법에 대한 자세한 내용은 <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [사용자 지정 API 호출](#custom-api-call)
* [레코드 읽기](#read-record)
* [레코드 만들기](#create-a-record)
* [작업 항목 업데이트](#update-a-work-item)
* [[!UICONTROL 첨부 파일 업로드]](#upload-an-attachment)
* [첨부 파일 다운로드](#download-an-attachment)
* [작업 항목 연결]([!UICONTROL #link-work-items])

#### [!UICONTROL 사용자 지정 API 호출]

이 작업 모듈을 사용하면 [!DNL Azure DevOps] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Azure DevOps] 모듈.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기본 URL]</td> 
   <td> <p>연결하는 데 사용하는 기본 URL을 선택하거나 매핑합니다 [!DNL Azure DevOps] account</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 상대 URL]</td> 
   <td> <p>이 API 호출에 연결할 상대 URL을 입력합니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API 버전]</td> 
   <td>버전 선택 또는 매핑 [!DNL Azure DevOps] 이 API 호출에 대해 연결할 API입니다. 선택한 버전이 없으면 [!DNL Workfront Fusion] 연결 대상 [!DNL Azure DevOps] API 버전 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 메서드]</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 쿼리 문자열]</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 쿼리를 추가합니다.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL 레코드 읽기]

이 작업 모듈은 [!DNL Azure DevOps].

레코드의 ID를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>프로젝트를 읽을지 작업 항목을 읽을지 선택합니다</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>: 읽을 프로젝트를 선택합니다.</p> </li> 
     <li> <p><strong>[!UICONTROL 작업 항목]</strong>: 읽을 작업 항목이 포함된 프로젝트를 선택한 다음 작업 항목 유형을 선택합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>이 모듈의 출력 번들에 포함할 정보를 선택합니다. 사용 가능한 필드는 작업 항목 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>읽을 레코드의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 레코드 만들기]

이 작업 모듈은 새 프로젝트 또는 작업 항목을 만듭니다.

이 모듈은 새로 생성된 작업 항목에 대한 객체 ID 또는 새로 생성된 프로젝트의 URL 및 상태 코드를 출력합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>작업 항목을 만들지 프로젝트를 만들지 여부를 선택합니다.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>: 새 프로젝트의 이름을 입력하거나 매핑합니다.</p> </li> 
       <li> <p><strong>[!UICONTROL Description]</strong>: 새 프로젝트에 대한 설명을 입력하거나 매핑합니다. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>: 프로젝트를 공개 또는 비공개로 할지 선택합니다. 사용자는 조직에 로그인해야 하며 비공개 프로젝트와 상호 작용하기 위해 프로젝트에 대한 액세스 권한이 부여되어야 합니다. 공용 프로젝트는 조직에 로그인하지 않은 사용자가 볼 수 있습니다.</p> </li> 
       <li> <p><strong>[!UICONTROL 버전 제어]</strong>: 프로젝트를 사용할지 여부를 선택합니다 [!DNL Git] 또는 [!UICONTROL Team Foundation Version Control (TFCV)]을 버전 제어에 사용할 수 있습니다.</p> </li> 
       <li> <p><strong>[!UICONTROL 작업 항목 프로세스]</strong>: 프로젝트에 사용할 작업 프로세스를 선택합니다. 옵션은 [!UICONTROL Basic], [!UICONTROL Screm], [!UICONTROL Capability Maturity Model Integration (CMMI)] 및 [!UICONTROL Agile]입니다.</p> <p>자세한 내용은 [!DNL Azure DevOps] 프로세스 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">프로세스 선택</a> 에서 [!DNL Azure DevOps] 설명서.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL 작업 항목]</strong> </p> <p>다음 필드를 채웁니다.</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>: 작업 항목을 만들 프로젝트를 선택합니다.</p> </li> 
       <li> <p><strong>[!UICONTROL 작업 항목 유형]</strong>: 만들려는 작업 항목의 유형을 선택합니다.</p> </li> 
       <li> <p><strong>[!UICONTROL 기타 필드]</strong>: 이러한 필드에 지정된 속성에 대해 작업 항목이 가질 값을 입력합니다. 사용 가능한 필드는 작업 항목 유형에 따라 다릅니다.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 작업 항목 업데이트]

이 작업 모듈은 ID를 사용하여 기존 작업 항목을 업데이트합니다.

이 모듈은 업데이트된 작업 항목의 ID를 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>업데이트할 작업 항목이 포함된 프로젝트를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 항목 유형]</td> 
   <td> <p>업데이트할 작업 항목 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 기타 필드]</td> 
   <td>이러한 각 필드에 지정된 속성에 대해 작업 항목이 가질 값을 입력합니다. 사용 가능한 필드는 작업 항목 유형에 따라 다릅니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 항목 ID]</td> 
   <td>업데이트할 작업 항목의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 첨부 파일 업로드]

이 작업 모듈은 파일을 업로드하고 작업 항목에 첨부합니다.

이 모듈은 첨부 파일의 첨부 파일 ID와 다운로드 URL을 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>첨부 파일을 업로드할 프로젝트를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 항목 ID]</td> 
   <td> <p>첨부 파일을 업로드할 작업 항목의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>업로드된 첨부 파일에 추가할 주석의 텍스트를 입력합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일] </td> 
   <td>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 컨텐츠를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 첨부 파일 다운로드]

이 작업 모듈은 첨부 파일을 다운로드합니다.

모듈은 첨부 파일의 파일 컨텐츠를 반환합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 첨부 파일 URL]</td> 
   <td> <p>다운로드할 첨부 파일의 URL을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 작업 항목 연결]

이 작업 모듈은 두 작업 항목을 링크하고 그 사이의 관계를 정의합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 기본 작업 항목 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 항목 ID]</td> 
   <td>다른 작업 항목을 연결할 주 작업 항목 항목의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 연결된 작업 항목 ID]</td> 
   <td>주 작업 항목에 연결할 작업 항목의 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 링크 유형]</td> 
   <td> <p>연결할 작업 항목 간의 관계를 정의합니다.</p> <p>자세한 내용은 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">링크 유형 참조</a> ( [!UICONTROL Azure DevOps] 설명서).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>댓글 텍스트를 입력하거나 매핑합니다. 이 방법은 링크의 추론이나 의도를 설명하는 데 유용합니다.</td> 
  </tr> 
 </tbody> 
</table>

### 검색 결과

#### [!UICONTROL 작업 항목 나열]

이 작업 모듈은 [!DNL Azure DevOps] 프로젝트.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 기본 작업 항목 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Azure DevOps] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] [!UICONTROL Workfront Fusion] 변환</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>작업 항목을 검색할 프로젝트를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 작업 항목 유형]</td> 
   <td> <p>검색할 작업 항목의 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력]</td> 
   <td>모듈의 출력에 표시할 속성을 선택합니다. 사용 가능한 필드는 검색할 작업 항목의 유형에 따라 다릅니다. 속성을 하나 이상 선택해야 합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td>최대 작업 항목 수를 입력하거나 매핑합니다 [!DNL Workfront Fusion] 한 실행 주기 동안 를 반환합니다.</td> 
  </tr> 
 </tbody> 
</table>
