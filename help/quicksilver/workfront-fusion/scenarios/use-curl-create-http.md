---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: cURL을 사용하여 HTTP 모듈 추가
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# cURL을 사용하여 HTTP 모듈 추가

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [cURL을 사용하여 HTTP 모듈 추가](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/use-curl-create-http.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

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

cURL을 시나리오에 붙여 넣을 수 없는 경우 브라우저 설정을 확인하여 클립보드에서 붙여 넣기가 활성화되어 있는지 확인하십시오.


