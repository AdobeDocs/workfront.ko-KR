---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: cURL을 사용하여 HTTP 모듈 추가
description: cURL 요청을 시나리오에 붙여 넣을 수 있으며, Fusion은 cURL 요청에서 구성된 HTTP 모듈을 만듭니다.
author: Becky
feature: Workfront Fusion
source-git-commit: 4cc881f4f5a28bd105e6898ad7ffb57c1dafb563
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# cURL을 사용하여 HTTP 모듈 추가

cURL 요청을 시나리오에 붙여 넣을 수 있으며, Fusion은 cURL 요청에서 구성된 HTTP 모듈을 만듭니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront 플랜</td>  
      <td>임의</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront 라이선스</td>  
      <td>
        새로운 기능: 표준<br>
        또는<br>
        현재: 작업 시간 이상
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion 라이선스</td>  
      <td> 
        현재: Workfront Fusion 라이센스 요구 사항이 없습니다.<br>
        또는<br>
        레거시: 모두
      </td>  
    </tr>  
    <tr>  
      <td>제품</td>  
      <td> 
        새로운 기능: Select 또는 Prime Workfront 플랜: 조직에서 Adobe Workfront Fusion을 구매해야 합니다.<br>
        Ultimate Workfront 플랜: Workfront Fusion이 포함됩니다.<br>
        또는<br>
        현재: 조직은 Adobe Workfront Fusion을 구매해야 합니다.
      </td>  
    </tr> 
  </tbody>  
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

+++

## cURL 요청에서 HTTP 모듈 만들기


cURL을 사용하여 HTTP 모듈을 만들려면 다음을 수행하십시오.

1. 텍스트 편집기에서와 같이 Fusion 외부에 cURL 요청 텍스트를 만듭니다.

   >[!IMPORTANT]
   >
   >Windows 시스템에서 Fusion을 사용하는 경우 cURL 요청에 줄 바꿈이 포함되지 않아야 합니다.
1. cURL 요청을 클립보드에 복사합니다.
1. 왼쪽 패널의 **[!UICONTROL 시나리오]** 탭을 클릭합니다.
1. 모듈을 만들 시나리오를 선택합니다.
1. 시나리오의 아무 곳이나 클릭하여 시나리오 편집기를 입력합니다.
1. 시나리오 편집기에서 공백을 마우스 오른쪽 단추로 클릭하고 **붙여넣기**&#x200B;를 선택합니다.

   또는

   Ctrl + V (Windows) 또는 Cmd + V (Mac)를 누릅니다.


   HTML 모듈이 만들어집니다.
1. 모듈을 드래그하여 시나리오에 연결합니다.

## 문제 해결

cURL을 시나리오에 붙여 넣을 수 없는 경우 다음을 확인하십시오.

* 브라우저 설정을 확인하여 클립보드에서 붙여넣기가 활성화되어 있는지 확인합니다.
* Windows를 실행하는 경우 cURL 요청에 줄 바꿈이 포함되어 있지 않은지 확인하십시오.



