---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion]에서 잠긴 시나리오 관리'
description: ' [!DNL Adobe Workfront Fusion]에서 잠긴 시나리오 관리'
author: Becky
feature: Workfront Fusion
exl-id: 5fccf336-d904-43fe-ad4a-c3ce76dbcad0
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 잠긴 시나리오 관리

경우에 따라 시나리오가 [!DNL Workfront Fusion]에서 일시적으로 잠길 수 있습니다. 잠긴 실행은 2~4시간 내에 자동으로 잠금 해제됩니다. 시나리오를 수동으로 잠금 해제할 수도 있습니다.

>[!IMPORTANT]
>
>시나리오를 수동으로 잠금 해제하면 시나리오 실행에 오류가 발생할 수 있습니다.

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
  <td> <p>작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p><p>작업 자동화용 [!UICONTROL [!DNL Workfront Fusion]] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구입해야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 잠긴 시나리오 이해

여러 가지 이유로 인해 시나리오가 잠길 수 있습니다.

Workfront Fusion은 예약된 시나리오의 병렬 처리를 지원하지 않습니다. 이러한 시나리오는 시나리오 실행 시작 시 잠기고 완료되면 잠금 해제됩니다. 실행이 중단되면 시나리오가 잠금 해제되지 않을 수 있습니다. 사용자가 시나리오를 수동으로 중지하거나 시스템 문제가 있을 때 이러한 문제가 발생할 수 있습니다.

또한 성능 또는 기타 문제를 일으키므로 Workfront Fusion 엔지니어링 팀이 시나리오를 잠글 수 있습니다.

잠긴 시나리오의 원인에 관계없이 시나리오는 잠긴 후 2~4시간 후에 자동으로 잠금 해제됩니다.

## 잠긴 시나리오 잠금 해제

잠긴 시나리오는 잠긴 시간으로부터 2~4시간 후에 잠금 해제됩니다. 시나리오를 자동으로 잠금 해제하도록 예약하기 전에 수동으로 잠금 해제할 수 있습니다.

시나리오를 수동으로 잠금 해제하면 시나리오 실행에 오류가 발생할 수 있습니다. 시나리오 설계의 일부로 실행 실행 및 중지로 인해 시나리오가 잠긴 경우에만 시나리오를 수동으로 잠금 해제하는 것이 좋습니다. 다른 상황에서는 시나리오가 자동으로 잠금 해제될 때까지 기다리는 것이 좋습니다.

>[!IMPORTANT]
>
>시나리오를 수동으로 잠금 해제하면 시나리오 실행에 오류가 발생할 수 있습니다.

1. 잠긴 시나리오의 시나리오 세부 정보 페이지로 이동합니다.
1. 화면 오른쪽 상단의 **[!UICONTROL 옵션]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 실행 잠금 해제]**&#x200B;를 선택하십시오.
1. **[!UICONTROL 잠금 해제]**&#x200B;를 클릭합니다.
