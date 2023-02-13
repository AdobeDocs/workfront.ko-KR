---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion에서 시나리오 예약
description: 기본적으로 시나리오는 15분마다 실행됩니다. 활성화된 시나리오가 실행되는 시기와 빈도를 정의하여 이 설정을 변경할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# 에서 시나리오 예약 [!DNL Adobe Workfront Fusion]

기본적으로 시나리오는 15분마다 실행됩니다. 활성화된 시나리오가 실행되는 시기와 빈도를 정의하여 이 설정을 변경할 수 있습니다.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p>  </td>    </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 시나리오 예약

1. 시나리오 세부 사항 페이지의 오른쪽 위 모서리에서 **[!UICONTROL 옵션]** > **[!UICONTROL 예약]**

   또는

   을(를) 클릭합니다. **[!UICONTROL 예약]** 시나리오 트리거 모듈에서 (시계) 아이콘을 클릭합니다.

1. 다음 필드에 정보를 입력합니다.

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 실행 시나리오]</td> 
      <td> <p>시나리오를 실행할 빈도를 선택한 다음 간격을 선택합니다.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL 일정한 간격으로]</strong> </p> <p>실행 사이의 시간(분)을 입력합니다. 기본값은 15분입니다.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>시나리오를 실행할 날짜와 시간을 입력합니다. 형식 사용 <code>MM/DD/YYYY h:mm A</code>. 예: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL 매일]</strong> </p> <p>시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL 요일]</strong> </p> <p>일: 시나리오를 실행할 요일을 선택합니다. 1일 이상을 선택할 수 있습니다.</p> <p>시간: 선택한 날짜에 시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the month]</strong> </p> <p>일: 시나리오를 실행할 월의 일을 선택합니다. 1일 이상을 선택할 수 있습니다.</p> <p>시간: 선택한 날짜에 시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 지정된 날짜]</strong> </p> <p>개월: 시나리오를 실행할 월을 선택합니다. 한 달 이상을 선택할 수 있습니다.</p> <p>일: 시나리오를 실행할 월의 일을 선택합니다. 1일 이상을 선택할 수 있습니다.</p> <p>시간: 선택한 날짜에 시나리오를 실행할 시간을 입력합니다. 형식 사용 <code>h:mm A</code>. 예: <code>11:00 PM</code></p> </li> 
       </ul> <p>참고: 해당 날짜에 시나리오를 실행하려면 날짜가 있어야 합니다. 예를 들어 그 달의 31일에만 예약된 시나리오는 2월, 4월, 6월, 9월 또는 11월에 실행되지 않습니다. 이러한 달은 31일이 없기 때문입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced Scheduling]</td> 
      <td>시나리오를 실행할 특정 시간 간격을 정의할 수 있습니다. 시간 간격, 평일 또는 월을 지정할 수 있습니다. 각 간격에 대해 <strong>[!UICONTROL Add]</strong> [!UICONTROL Run 시나리오] 필드에 설명된 대로 필드를 채웁니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 시작]</td> 
      <td>시나리오를 실행할 날짜 및 시간을 입력합니다. 형식 사용 <code>MM/DD/YYYY h:mm A</code>. 예: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>시나리오를 실행할 날짜와 시간을 입력합니다. 형식 사용 <code>MM/DD/YYYY h:mm A</code>. 예: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 확인]** 예약 설정을 저장하고 시나리오로 돌아가려면
