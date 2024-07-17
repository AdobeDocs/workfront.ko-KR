---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 모듈 보관
description: ' [!DNL Adobe Workfront Fusion] 시나리오에서는 압축 파일과 같은 아카이브를 여러 타사 응용 프로그램 및 서비스에 연결할 수 있습니다. 예를 들어 다음과 같은 시나리오를 구성할 수 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL 보관] 모듈

[!DNL Adobe Workfront Fusion] 시나리오에서는 압축된 파일과 같은 아카이브를 사용하여 자동화 또는 통합에 사용할 수 있습니다.

시나리오를 만드는 방법에 대한 지침이 필요하면 [시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)를 참조하십시오. 모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)을 참조하세요.

## [!UICONTROL 보관] 모듈 및 해당 필드

[!UICONTROL 보관] 모듈을 구성할 때 [!DNL Workfront Fusion]에 아래 나열된 필드가 표시됩니다. 앱 또는 서비스의 액세스 수준과 같은 요소에 따라 이러한 필드와 함께 추가 [!UICONTROL 보관] 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [한 모듈에서 다른 모듈로 정보를 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 보관 추출]](#extract-an-archive)
* [[!UICONTROL 보관 만들기]](#create-an-archive)
* [[!UICONTROL 부풀리기]](#inflate)
* [[!UICONTROL 수축]](#deflate)

## [!UICONTROL 보관 추출]

이 작업 모듈은 아카이브에서 사용자가 식별하는 파일을 추출합니다.

모듈은 파일의 ID와 연결된 필드, 그리고 연결이 액세스하는 모든 사용자 지정 필드 및 값을 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source 파일]</td> 
   <td> <p> 추출할 파일을 선택합니다. 이 파일은 이전 모듈([!DNL Workfront] &gt;[!UICONTROL 문서 다운로드] 모듈 등)에서 매핑할 수 있습니다.</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** 정의된 [!DNL Dropbox] 폴더(예: 보관 파일)에서 ZIP 파일을 가져온 다음 [!UICONTROL 보관] 모듈을 사용하여 압축을 풀고 [!UICONTROL 전자 메일] 또는 [!DNL Gmail] 모듈을 통해 추출된 파일을 원하는 전자 메일 주소에 첨부 파일로 보냅니다.
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL 보관 만들기]

이 집계 모듈은 [!UICONTROL ZIP] 또는 [!UICONTROL TAR] 보관 파일에 원하는 파일을 추가합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source 모듈]</td> 
   <td> <p> 파일을 검색할 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 유형] </td> 
   <td> <p>파일을 [!UICONTROL ZIP] 아카이브에 추가할지 [!UICONTROL TAR] 아카이브에 추가할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>아카이브에 추가할 설명을 입력합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>집계된 출력을 그룹화할 표현식을 정의합니다. 이 표현식은 하나 이상의 매핑된 항목을 포함할 수 있습니다. 그런 다음 이 표현식의 값을 사용하여 집계된 데이터가 그룹으로 분리됩니다. 각 그룹은 키(평가된 표현식)와 값(집계된 텍스트)을 사용하여 별도의 번들로 출력합니다. 키는 후속 모듈에서 필터로 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 빈 집계 후 처리 중지]</td> 
   <td>결과가 없을 때 시나리오를 중지하려면 이 옵션을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archive name]</td> 
   <td> <p> 생성된 아카이브의 이름을 입력합니다. 확장을 추가하지 마십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source 파일]</td> 
   <td> <p>이전 모듈에서 소스 파일을 선택하거나 소스 파일의 이름과 데이터를 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** [!DNL Gmail] >[!UICONTROL 전자 메일 보기] 모듈을 사용하여 수신 전자 메일을 봅니다. 전자 메일을 받으면 해당 첨부 파일이 개별 번들로 반복된 다음 [!DNL ZIP] 파일에 보관되고 정의된 Dropbox 폴더에 저장됩니다.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL 부풀리기]

이 변환기 모듈은 인플레이션 알고리즘을 이용하여 이진 데이터를 압축 해제한다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>inflate 함수를 사용하여 압축을 풀 데이터를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL 수축]

이 변압기 모듈은 디플레이션 알고리즘을 사용하여 이진 데이터를 압축한다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>수축 함수를 사용하여 압축할 데이터를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
