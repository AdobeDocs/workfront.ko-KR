---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 의 파일 매핑 기본 정보 [!DNL Adobe Workfront Fusion]
description: 일부 모듈은 파일을 처리할 수 있습니다. 이러한 모듈은 추가 처리를 위해 전송할 출력 파일을 반환하거나 처리를 위해 파일을 해당 모듈에 전달해야 할 수 있습니다. 이러한 모듈이 함께 작동하여 파일을 처리하려면 먼저 서로 매핑해야 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# 의 파일 매핑 기본 정보 [!DNL Adobe Workfront Fusion]

일부 모듈은 파일을 처리할 수 있습니다. 이러한 모듈은 추가 처리를 위해 전송할 출력 파일을 반환하거나 처리를 위해 파일을 해당 모듈에 전달해야 할 수 있습니다. 이러한 모듈이 함께 작동하여 파일을 처리하려면 먼저 서로 매핑해야 합니다.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] 라이센스**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr>  </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 파일 매핑

파일을 사용하여 작업할 수 있는 모듈에는 두 가지 정보가 필요합니다.

* 파일 이름
* 파일 컨텐츠(데이터)

파일을 매핑할 때 시나리오에서 데이터를 가져올 모듈을 선택합니다. 그러면 파일 이름과 파일 컨텐츠가 있는 그대로 자동으로 매핑됩니다.

>[!NOTE]
>
>URL에서 파일을 처리해야 하는 경우 `HTTP > Get a File` 모듈을 사용하여 URL에서 파일을 다운로드한 다음 `HTTP > Get a File` 모듈이 없습니다.

>[!INFO]
>
>**예:** 다음 예에서는 문서를 [!DNL Adobe Workfront] to [!DNL Google Drive]. 다음 [!DNL Workfront] 트리거 [!UICONTROL 감시 레코드] 이름 및 ID를 포함하여 각 문서에 대한 자세한 정보를 반환합니다.
>
>다음 모듈이요 [!UICONTROL 문서 다운로드]를 다운로드하면 Google Drive에 업로드할 수 있도록 실제 데이터를 다운로드합니다.
>
>이 정보를 [!DNL Google Drive] 업로드할 수 있도록 정보가 매핑될 소스 파일을 지정해야 합니다. 을(를) 선택하는 경우 [!DNL Workfront] > [!UICONTROL 문서 다운로드] 소스 파일 아래의 옵션, [!DNL Workfront Fusion] 에서 문서가 [!DNL Workfront] 지정된 Google 폴더에 업로드됩니다.
>
>![](assets/wf-download-document-350x605.png)
>
>그러나 파일의 이름을 바꾸려고 하지만 데이터를 있는 그대로 유지하려면 [!UICONTROL 맵] 파일 이름과 파일 컨텐츠를 별도로 매핑하는 옵션. 확장명을 포함하여 전체 파일 이름을 입력합니다. 텍스트 형식 및 사진, 비디오, PDF 등의 이진 형식이 지원됩니다.
>
>![](assets/use-the-map-option-350x358.png)
