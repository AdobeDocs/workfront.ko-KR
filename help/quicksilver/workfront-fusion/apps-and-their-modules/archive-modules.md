---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 아카이브 모듈
description: 다음 [!DNL Adobe Workfront Fusion] 시나리오에서는 압축된 파일과 같은 아카이브를 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다. 예를 들어
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL 아카이브] 모듈

다음 [!DNL Adobe Workfront Fusion] 시나리오에서 압축 파일과 같은 아카이브를 사용하여 자동 또는 통합에서 사용할 수 있습니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL 아카이브] 모듈 및 해당 필드

구성 시 [!UICONTROL 아카이브] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!UICONTROL 아카이브] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 아카이브 추출]](#extract-an-archive)
* [[!UICONTROL 아카이브 만들기]](#create-an-archive)
* [[!UICONTROL 부풀림]](#inflate)
* [[!UICONTROL 디플레이트]](#deflate)

## [!UICONTROL 아카이브 추출]

이 작업 모듈은 아카이브에서 식별하는 파일을 추출합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 파일 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 소스 파일]</td> 
   <td> <p> 추출할 파일을 선택합니다. 이 파일은 이전 모듈(예: [!DNL Workfront] &gt;[!UICONTROL 문서 다운로드] 모듈).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** 정의된 [!DNL Dropbox] 폴더(예: 아카이브)를 사용하여 추출합니다 [!UICONTROL 아카이브] 모듈을 사용하여 추출된 파일을 원하는 전자 메일 주소로 첨부 파일로 보냅니다. [!UICONTROL 이메일] 또는 [!DNL Gmail] 모듈.
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL 아카이브 만들기]

이 누적 모듈은 원하는 파일을 [!UICONTROL ZIP] 또는 [!UICONTROL TAR] 보관.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 소스 모듈]</td> 
   <td> <p> 파일을 검색할 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>파일을 [!UICONTROL ZIP] 보관 위치에 추가할지 또는 [!UICONTROL TAR] 보관 위치에 추가할지를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>아카이브에 추가할 설명을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>집계된 출력을 그룹화할 표현식을 정의합니다. 이 표현식은 하나 이상의 매핑된 항목을 포함할 수 있습니다. 그런 다음 집계된 데이터는 이 표현식의 값을 사용하여 그룹으로 분리됩니다. 각 그룹은 키(평가된 표현식)와 값(집계된 텍스트)으로 별도의 번들로 출력됩니다. 키를 후속 모듈에서 필터로 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 빈 집계 후 처리 중지]</td> 
   <td>결과가 없는 경우 시나리오를 중지하려면 이 옵션을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archive name]</td> 
   <td> <p> 생성된 아카이브의 이름을 입력합니다. 확장을 추가하지 마십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 소스 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** 을(를) 사용하여 수신 전자 메일 보기 [!DNL Gmail] >[!UICONTROL 이메일 보기] 모듈. 이메일이 수신되면 해당 첨부 파일이 개별 번들로 반복된 다음 [!DNL ZIP] 파일을 생성하여 정의된 Dropbox 폴더에 저장합니다.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL 부풀림]

이 변압기 모듈은 인플레이션 알고리즘을 사용하여 이진 데이터를 압축 해제합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>inflate 함수를 사용하여 압축을 해제할 데이터를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL 디플레이트]

이 변압기 모듈은 디플레이션 알고리즘을 사용하여 이진 데이터를 압축합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>deflate 함수를 사용하여 압축할 데이터를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
