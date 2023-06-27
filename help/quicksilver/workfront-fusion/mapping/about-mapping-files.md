---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 의 매핑 파일 정보 [!DNL Adobe Workfront Fusion]
description: 일부 모듈에는 파일을 처리하는 기능이 있습니다. 이러한 모듈은 추가 처리를 위해 전송할 출력 파일을 반환하거나 처리를 위해 파일을 해당 모듈에 전달해야 합니다. 이러한 모듈을 함께 사용하여 파일을 처리하려면 먼저 모듈을 서로 매핑해야 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 의 매핑 파일 정보 [!DNL Adobe Workfront Fusion]

일부 모듈에는 파일을 처리하는 기능이 있습니다. 이러한 모듈은 추가 처리를 위해 전송할 출력 파일을 반환하거나 처리를 위해 파일을 해당 모듈에 전달해야 합니다. 이러한 모듈을 함께 사용하여 파일을 처리하려면 먼저 모듈을 서로 매핑해야 합니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>[!DNL Pro] 이상</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이선스**</td> 
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
  </tr>  </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 파일 매핑

파일 작업 기능이 있는 모듈에는 두 가지 정보가 필요합니다.

* 파일 이름
* 파일 콘텐츠(데이터)

파일을 매핑할 때 데이터를 가져올 시나리오의 모듈을 선택합니다. 그러면 파일 이름과 파일 콘텐츠가 있는 그대로 자동으로 매핑됩니다.

>[!NOTE]
>
>URL에서 파일을 처리해야 하는 경우 `HTTP > Get a File` url에서 파일을 다운로드한 다음 `HTTP > Get a File` 를 시나리오에서 원하는 모듈의 필드로 이동합니다.

>[!INFO]
>
>**예:** 다음 예에서는 에서 문서를 다운로드하는 방법을 보여 줍니다. [!DNL Adobe Workfront] 끝 [!DNL Google Drive]. 다음 [!DNL Workfront] 트리거 [!UICONTROL 녹화 시청] 는 이름과 ID를 포함하여 각 문서에 대한 자세한 정보를 반환합니다.
>
>다음 모듈, [!UICONTROL 문서 다운로드]는 Google 드라이브에 업로드할 수 있도록 실제 데이터를 다운로드합니다.
>
>이 정보를 다음에 매핑하려면 [!DNL Google Drive] 업로드할 수 있도록 정보를 매핑할 소스 파일을 지정해야 합니다. 을(를) 선택하는 경우 [!DNL Workfront] > [!UICONTROL 문서 다운로드] 소스 파일 아래에 있는 옵션 [!DNL Workfront Fusion] 파일 이름과 파일 컨텐트를 매핑하여 문서 출처 [!DNL Workfront] 은(는) 지정된 Google 폴더에 업로드됩니다.
>
>![](assets/wf-download-document-350x605.png)
>
>그러나 파일의 이름을 바꾸고 데이터를 그대로 유지하려는 경우 [!UICONTROL 맵] 옵션을 사용하여 파일 이름과 파일 내용을 개별적으로 매핑할 수 있습니다. 확장자를 포함하여 전체 파일 이름을 입력합니다. 사진, 비디오 및 PDF과 같은 텍스트 형식 및 바이너리 형식이 지원됩니다.
>
>![](assets/use-the-map-option-350x358.png)
