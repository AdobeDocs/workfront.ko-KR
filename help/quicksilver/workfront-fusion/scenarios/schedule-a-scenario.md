---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion에서 시나리오 예약
description: 기본적으로 시나리오는 15분마다 실행됩니다. 활성화된 시나리오가 실행되는 시기와 빈도를 정의하여 이를 변경할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 시나리오 예약

기본적으로 시나리오는 15분마다 실행됩니다. 활성화된 시나리오가 실행되는 시기와 빈도를 정의하여 이를 변경할 수 있습니다. Fusion 시나리오는 5분마다 실행되도록 예약할 수 있습니다.

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
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime] [!DNL Adobe Workfront] 플랜이 있는 경우 조직에서 이 문서에 설명된 기능을 사용하려면 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다. [!DNL Workfront Fusion]이(가) [!UICONTROL Ultimate] [!DNL Workfront] 계획에 포함되어 있습니다.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 이 문서에 설명된 기능을 사용하려면 조직에서 [!DNL Adobe Workfront Fusion]과(와) [!DNL Adobe Workfront]을(를) 구매해야 합니다.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

## 시나리오 예약

1. 시나리오 세부 정보 페이지의 오른쪽 상단 모서리에서 **[!UICONTROL 옵션]** > **[!UICONTROL 예약]**&#x200B;을 클릭합니다.

   또는

   시나리오의 트리거 모듈에서 **[!UICONTROL 예약]** 아이콘(시계)을 클릭합니다.

1. 다음 필드에 정보를 입력합니다.

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 실행 시나리오]</td> 
      <td> <p>시나리오를 실행할 빈도를 선택한 다음 간격을 선택합니다.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL At regular interval]</strong> </p> <p>실행 간격(분)을 입력합니다. 기본값은 15분입니다.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>시나리오를 실행할 날짜 및 시간을 입력합니다. <code>MM/DD/YYYY h:mm A</code> 형식을 사용합니다. 예: <code>06/25/2019 11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Every day]</strong> </p> <p>시나리오를 실행할 시간을 입력합니다. <code>h:mm A</code> 형식을 사용합니다. 예: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 요일]</strong> </p> <p>일: 시나리오를 실행할 요일을 선택합니다. 하나 이상의 요일을 선택할 수 있습니다.</p> <p>시간: 선택한 일자에 시나리오를 실행할 시간을 입력합니다. <code>h:mm A</code> 형식을 사용합니다. 예: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 해당 월의 일]</strong> </p> <p>일: 시나리오를 실행할 월을 선택합니다. 하나 이상의 요일을 선택할 수 있습니다.</p> <p>시간: 선택한 일자에 시나리오를 실행할 시간을 입력합니다. <code>h:mm A</code> 형식을 사용합니다. 예: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 지정 날짜]</strong> </p> <p>월: 시나리오를 실행할 월을 선택합니다. 하나 이상의 월을 선택할 수 있습니다.</p> <p>일: 시나리오를 실행할 월을 선택합니다. 하나 이상의 요일을 선택할 수 있습니다.</p> <p>시간: 선택한 일자에 시나리오를 실행할 시간을 입력합니다. <code>h:mm A</code> 형식을 사용합니다. 예: <code>11:00 PM</code></p> </li> 
       </ul> <p>주: 시나리오가 해당 일자에 실행되려면 일자가 있어야 합니다. 예를 들어, 해당 달에는 31번째 날이 없으므로 해당 달의 31일에만 예약된 시나리오는 2월, 4월, 6월, 9월 또는 11월에 실행되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 고급 예약]</td> 
      <td>시나리오를 실행할 특정 시간 간격을 정의할 수 있습니다. 주중 또는 월 단위 시간 간격을 지정할 수 있습니다. 각 간격에 대해 <strong>[!UICONTROL 추가]</strong>를 클릭하고 [!UICONTROL 실행 시나리오] 필드에 설명된 대로 필드를 채웁니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시작]</td> 
      <td>시나리오를 실행할 날짜 및 시간을 입력합니다. <code>MM/DD/YYYY h:mm A</code> 형식을 사용합니다. 예: <code>06/25/2019 11:00 PM</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>시나리오를 실행할 날짜 및 시간을 입력합니다. <code>MM/DD/YYYY h:mm A</code> 형식을 사용합니다. 예: <code>06/25/2019 11:00 PM</code></td> 
     </tr> 
    </tbody> 
   </table>

1. 예약 설정을 저장하고 시나리오로 돌아가려면 **[!UICONTROL 확인]**&#x200B;을 클릭하세요.
