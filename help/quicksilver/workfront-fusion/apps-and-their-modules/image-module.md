---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 이미지 모듈
description: Adobe Workfront Fusion Image 모듈을 사용하면 특정 이미지(크기, 유형 등)에 대한 정보를 얻을 수 있고, 이미지를 다른 파일 형식으로 변환한 다음 이미지 크기를 직접 변경할 수 있습니다.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# 이미지 모듈

[!DNL Adobe Workfront Fusion] [!UICONTROL 이미지] 모듈을 사용하면 특정 이미지(크기, 유형 등)에 대한 정보를 얻고, 이미지를 다른 파일 형식으로 변환한 다음, 이미지의 크기를 직접 변경할 수 있습니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 이미지] 모듈 및 해당 필드

이 모듈을 구성할 때 다음 필드가 표시됩니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

* [[!UICONTROL 크기 조정]](#resize)
* [[!UICONTROL 형식 변환]](#convert-a-format)
* [[!UICONTROL 메타데이터 추출]](#extract-metadata)

### [!UICONTROL 크기 조정]

이 변압기 모듈은 지정한 기준에 따라 이미지의 높이와 너비를 변경합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>변환할 이미지의 소스를 선택합니다. 이전 모듈에서 출력을 선택하거나 데이터 파일과 파일 이름을 매핑할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>변환할 파일을 매핑합니다. 이 필드는 [!UICONTROL Source file] 필드에서 [!UICONTROL Map]을 선택한 경우 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 이름]</td> 
   <td>변환된 파일의 이름을 입력합니다. 이 필드는 [!UICONTROL Source file] 필드에서 [!UICONTROL Map]을 선택한 경우 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 원하는 항목]</td> 
   <td>높이 너비 비율을 유지할지 아니면 치수를 지정된 높이 및 너비로 변경할지 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL에 따라]</td> 
   <td> <p>모듈에서 이미지의 새 크기를 결정할 방법을 선택합니다. 이 필드는 원하는 필드에서 높이 너비 비율을 유지하도록 선택한 경우 나타납니다. 다른 필드는 이 필드의 선택 사항에 따라 나타납니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 최대 너비]</p> <p>이미지를 지정한 너비로 줄입니다. 높이는 자동으로 계산됩니다.</p> </li> 
     <li> <p>[!UICONTROL 최대 높이]</p> <p>이미지를 지정한 높이로 줄입니다. 너비는 자동으로 계산됩니다.</p> </li> 
     <li> <p>[!UICONTROL 최대 높이 또는 너비]</p> <p>이미지의 높이와 너비가 지정한 값을 초과하지 않도록 이미지를 줄입니다. 이 옵션은 높이 너비 비율을 유지하므로 차원 중 하나가 지정된 것보다 작을 수 있습니다. 예를 들어 높이와 너비를 모두 40으로 지정하면 400x300 이미지가 40X30으로 줄어듭니다.</p> </li> 
     <li> <p>[!UICONTROL 최소 너비]</p> <p>이미지를 지정한 너비로 확대합니다. 높이는 자동으로 계산됩니다.</p> </li> 
     <li> <p>[!UICONTROL 최소 높이]</p> <p>이미지를 지정한 높이로 확대합니다. 너비는 자동으로 계산됩니다.</p> </li> 
     <li> <p>[!UICONTROL 최소 높이 또는 너비]</p> <p>이미지의 높이와 너비가 지정한 값보다 크지 않은 방식으로 이미지를 확대합니다. 이 옵션은 높이 너비 비율을 유지하므로 차원 중 하나가 지정된 것보다 클 수 있습니다. 예를 들어 높이와 너비를 모두 300으로 지정하면 40x30 이미지가 400X300으로 확장됩니다.</p> </li> 
     <li> <p>[!UICONTROL Percent]</p> <p>지정한 값에 따라 이미지 크기를 백분율로 변경합니다. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Width]</td> 
   <td>크기가 조정된 이미지의 원하는 너비를 픽셀 단위로 입력하거나 매핑합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Height]</td> 
   <td>크기가 조정된 이미지의 원하는 높이를 픽셀 단위로 입력하거나 매핑합니다.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 형식 변환]

이 변압기 모듈은 이미지 파일의 형식을 변경합니다. 이 모듈은 다음 형식과 호환됩니다.

* PNG
* JPG
* GIF
* BMP

소스 파일과 출력은 모두 이러한 형식 중 하나여야 합니다. 예: [!UICONTROL 이미지] >[!UICONTROL 형식 변환] 모듈은 PNG 파일을 BMP 파일로 변환하거나 BMP를 JPG으로 변환할 수 있습니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>변환할 이미지의 소스를 선택합니다. 이전 모듈에서 출력을 선택하거나 데이터 파일과 파일 이름을 매핑할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>변환할 파일을 매핑합니다. 이 필드는 [!UICONTROL Source file] 필드에서 [!UICONTROL Map]을 선택한 경우 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 이름]</td> 
   <td>변환된 파일의 이름을 입력합니다. 이 필드는 [!UICONTROL Source file] 필드에서 [!UICONTROL Map]을 선택한 경우 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 출력 형식]</td> 
   <td>모듈에서 소스 파일을 변환할 형식을 선택합니다. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 메타데이터 추출]

이 변압기 모듈은 모듈에 대한 기본 정보를 반환합니다.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 파일]</td> 
   <td> <p>변환할 이미지의 소스를 선택합니다. 이전 모듈에서 출력을 선택하거나 데이터 파일과 파일 이름을 매핑할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>변환할 파일을 매핑합니다. 이 필드는 [!UICONTROL 소스 파일] 필드에서 맵 을 선택한 경우 사용할 수 있습니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 파일 이름]</td> 
   <td>변환된 파일의 이름을 입력합니다. 이 필드는 [!UICONTROL 소스 파일] 필드에서 맵 을 선택한 경우 사용할 수 있습니다.</td> 
  </tr> 
 </tbody> 
</table>

## 가능한 문제

### 오류가 발생하여 작업이 종료되었습니다.

오류가 발생하여 작업을 종료할 수 있는 세 가지 경우가 있습니다.

* 받은 데이터가 JPG/GIF/PNG/BMP 형식이 아닙니다
* 이미지 차원을 변경하는 동안 최대 너비/높이 제한을 초과했습니다. 이미지 크기는 3840px 너비와 2160px 높이를 초과할 수 없습니다
* 이미지의 차원이나 형식을 변경하는 동안 허용되는 최대 크기를 초과했습니다.
