---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion에서 시나리오 예약
description: 기본적으로 시나리오는 15분마다 실행됩니다. 활성화된 시나리오가 실행되는 시기와 빈도를 정의하여 이를 변경할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 1%

---

# 시나리오 예약 위치 [!DNL Adobe Workfront Fusion]

기본적으로 시나리오는 15분마다 실행됩니다. 활성화된 시나리오가 실행되는 시기와 빈도를 정의하여 이를 변경할 수 있습니다.

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
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>현재 제품 요구 사항: [!UICONTROL Select] 또는 [!UICONTROL Prime]이 있는 경우 [!DNL Adobe Workfront] 플랜, 조직은 다음을 구매해야 합니다. [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오. [!DNL Workfront Fusion] [!UICONTROL Ultimate]에 포함되어 있습니다. [!DNL Workfront] 계획.</p>
   <p>또는</p>
   <p>레거시 제품 요구 사항: 조직에서 구매해야 함 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 이 문서에 설명된 기능을 사용하십시오.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

다음에 대한 정보: [!DNL Adobe Workfront Fusion] 라이센스, 참조 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 시나리오 예약

1. 시나리오 세부 정보 페이지의 오른쪽 상단 모서리에서 **[!UICONTROL 옵션]** > **[!UICONTROL 예약]**

   또는

   다음을 클릭합니다. **[!UICONTROL 예약]** 시나리오의 트리거 모듈에 있는 아이콘(시계)입니다.

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
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>시나리오를 실행할 날짜 및 시간을 입력합니다. 형식 사용 <code>MM/DD/YYYY h:mm A</code>. 예: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL 매일]</strong> </p> <p>시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL 요일]</strong> </p> <p>일: 시나리오를 실행할 요일을 선택합니다. 하나 이상의 요일을 선택할 수 있습니다.</p> <p>시간: 선택한 일자에 시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 해당 월의 일]</strong> </p> <p>일: 시나리오를 실행할 월을 선택합니다. 하나 이상의 요일을 선택할 수 있습니다.</p> <p>시간: 선택한 일자에 시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 지정 날짜]</strong> </p> <p>월: 시나리오를 실행할 월을 선택합니다. 하나 이상의 월을 선택할 수 있습니다.</p> <p>일: 시나리오를 실행할 월을 선택합니다. 하나 이상의 요일을 선택할 수 있습니다.</p> <p>시간: 선택한 일자에 시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code></p> </li> 
       </ul> <p>주: 시나리오가 해당 일자에 실행되려면 일자가 있어야 합니다. 예를 들어, 해당 달에는 31번째 날이 없으므로 해당 달의 31일에만 예약된 시나리오는 2월, 4월, 6월, 9월 또는 11월에 실행되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 고급 예약]</td> 
      <td>시나리오를 실행할 특정 시간 간격을 정의할 수 있습니다. 주중 또는 월 단위 시간 간격을 지정할 수 있습니다. 각 간격에 대해 <strong>[!UICONTROL 추가]</strong> [!UICONTROL 실행 시나리오] 필드에 설명된 대로 필드를 채웁니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시작]</td> 
      <td>시나리오를 실행할 날짜 및 시간을 입력합니다. 형식 사용 <code>MM/DD/YYYY h:mm A</code>. 예: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>시나리오를 실행할 날짜 및 시간을 입력합니다. 형식 사용 <code>MM/DD/YYYY h:mm A</code>. 예: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 확인]** 예약 설정을 저장하고 시나리오로 돌아갑니다.
