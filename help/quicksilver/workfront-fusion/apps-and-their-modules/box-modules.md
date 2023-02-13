---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 상자 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오 Box를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다. 지정된 폴더를 모니터링하여 파일 변경 내용을 확인하거나 기존 파일을 수정 및 삭제하거나 새 파일을 폴더에 업로드합니다.
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# 상자 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL Box]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다. 지정된 폴더를 모니터링하여 파일 변경 내용을 확인하거나 기존 파일을 수정 및 삭제하거나 새 파일을 폴더에 업로드합니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

를 사용하려면 [!DNL Box] 모듈이면 반드시 [!DNL Box] 계정이 필요합니다.

## [!DNL Box] 모듈 및 해당 필드

구성 시 [!DNL Box] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL Box] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

* [[!UICONTROL 새 이벤트]](#new-event)
* [[!UICONTROL 감시 파일]](#watch-files)

#### [!UICONTROL 새 이벤트]

이 인스턴트 트리거 모듈은 파일이 추가, 이동, 복사, 삭제, 잠금 또는 잠금 해제될 때 시나리오를 시작합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>보내는 메시지를 보는 데 사용할 웹 후크를 선택합니다. 웹 후크를 추가하려면 <strong>[!UICONTROL Add]</strong> 웹 후크의 이름과 연결을 입력합니다.</p> <p> [!UICONTROL Box] 계정을 [!UICONTROL Workfront Fusion]에 연결하는 방법은 를 참조하십시오 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">모듈의 앱 또는 웹 서비스를 [!UICONTROL Workfront Fusion]에 연결</a> 기사 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]에서 시나리오 만들기</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 반환된 최대 이벤트 수]</p> </td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 이벤트 수를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 감시 파일]

이 트리거 모듈은 새 파일이 추가되거나 감시 중인 폴더에서 기존 파일이 업데이트될 때 시나리오를 시작합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Box] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  <tr> 
   <td role="rowheader">보기</td> 
   <td> <p>보려는 파일 유형을 선택합니다.</p> 
    <ul> 
     <li> <p><strong>새 파일만</strong> </p> <p>새 파일이 추가되면 시나리오가 시작됩니다.</p> </li> 
     <li> <p><strong>새 파일 및 모든 변경 사항</strong> </p> <p>시나리오는 파일이 추가되거나 파일 컨텐츠나 파일 속성(예: 이름)이 수정될 때 시작됩니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>다운로드한 최대 파일 수</p> </td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 파일 수를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 업로드] 파일](#upload-a-file)
* [[!UICONTROL 파일 업데이트]](#update-a-file)
* [[!UICONTROL 파일 삭제]](#delete-a-file)
* [[!UICONTROL 파일 가져오기]](#get-a-file)

#### [!UICONTROL 파일 업로드]

이 작업 모듈은 파일을 업로드합니다.

파일을 지정합니다. 파일에 새 파일 이름을 제공할 수도 있습니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 파일 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Box] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>이 모듈이 실패하면 다음 사항을 고려하십시오.
>
>* 파일 크기가 최대 파일 크기 제한을 초과할 수 있습니다 [!DNL Box] 계획을 세우거나 [!DNL Box] 계정의 저장소 할당량입니다. 저장 공간을 더 확보하려면 기존 파일을 [!DNL Box] 또는 업그레이드 [!DNL Box] 계정이 필요합니다.
>* [!DNL Box] 에서는 이름이 같은 두 개 이상의 파일을 단일 폴더에 업로드하지 않습니다. 대상 폴더에 업로드 중인 파일과 이름이 같은 파일이 포함되어 있으면 시나리오 실행이 오류 때문에 종료됩니다. 이를 방지하려면 파일의 이름을 변경합니다. 파일을 업데이트하려면 **[!UICONTROL 파일 업데이트]** 모듈.


#### [!UICONTROL 파일 업데이트]

이 작업 모듈은 파일을 업데이트합니다.

파일의 ID를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 파일 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Box] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID]</td> 
   <td>모듈을 업데이트할 파일의 고유 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 삭제]

이 작업 모듈은 파일을 삭제합니다.

파일의 ID를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 파일 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Box] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID]</td> 
   <td>모듈을 업데이트할 파일의 고유 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 파일 가져오기]

이 작업 모듈은 파일을 다운로드합니다.

파일의 ID를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 파일 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

>[!NOTE]
>
>이 모듈은 후속 모듈에 파일을 제공하는 데 유용합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>연결 방법에 대한 지침은 [!DNL Box] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">연결 만들기 [!DNL Adobe Workfront Fusion] - 기본 지침</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 ID]</td> 
   <td>모듈을 업데이트할 파일의 고유 ID를 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
