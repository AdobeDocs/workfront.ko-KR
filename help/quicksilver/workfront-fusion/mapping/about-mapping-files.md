---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe Workfront Fusion]의 매핑 파일 정보'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion]의 매핑 파일 정보

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [모듈 간에 파일 매핑](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

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
  </tr>  </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 파일 매핑

파일 작업 기능이 있는 모듈에는 두 가지 정보가 필요합니다.

* 파일 이름
* 파일 콘텐츠(데이터)

파일을 매핑할 때 데이터를 가져올 시나리오의 모듈을 선택합니다. 그러면 파일 이름과 파일 콘텐츠가 있는 그대로 자동으로 매핑됩니다.

>[!NOTE]
>
>URL에서 파일을 처리해야 하는 경우 `HTTP > Get a File` 모듈을 사용하여 URL에서 파일을 다운로드한 다음 `HTTP > Get a File` 모듈에서 파일을 시나리오에서 원하는 모듈의 필드에 매핑하는 것이 좋습니다.

>[!INFO]
>
>**예제:** 이 예제는 [!DNL Adobe Workfront]에서 [!DNL Google Drive](으)로 문서를 다운로드하는 방법을 보여 줍니다. [!DNL Workfront] 트리거 [!UICONTROL 레코드 보기]는 이름과 ID를 포함하여 각 문서에 대한 자세한 정보를 반환합니다.
>
>다음 모듈인 [!UICONTROL 문서 다운로드]에서는 실제 데이터를 다운로드하여 Google 드라이브에 업로드할 수 있습니다.
>
>이 정보를 [!DNL Google Drive]에 매핑하여 업로드하려면 정보를 매핑할 원본 파일을 지정해야 합니다. 소스 파일에서 [!DNL Workfront] > [!UICONTROL 문서 다운로드] 옵션을 선택하면 [!DNL Workfront Fusion]이(가) 파일 이름과 파일 콘텐츠를 매핑하여 [!DNL Workfront]의 문서가 지정된 Google 폴더로 업로드됩니다.
>
>![](assets/wf-download-document-350x605.png)
>
>그러나 파일의 이름을 바꾸고 데이터를 그대로 유지하려는 경우 [!UICONTROL 맵] 옵션을 사용하여 파일 이름과 파일 내용을 별도로 매핑할 수 있습니다. 확장자를 포함하여 전체 파일 이름을 입력합니다. 사진, 비디오 및 PDF과 같은 텍스트 형식 및 바이너리 형식이 지원됩니다.
>
>![](assets/use-the-map-option-350x358.png)
