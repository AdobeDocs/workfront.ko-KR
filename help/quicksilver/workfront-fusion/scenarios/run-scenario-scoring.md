---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 시나리오 채점 전문가 실행
description: ' [!DNL Adobe Workfront Fusion]에서 잠긴 시나리오 관리'
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: ed100c6ba32a6fbff6fa68ac7a4bfb38db861b17
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Adobe Workfront Fusion에서 시나리오 채점 전문가 실행

시나리오 채점 전문가는 모범 사례를 따르는 방식으로 시나리오가 구성되도록 하는 데 도움이 될 수 있습니다. 시나리오를 확인하고 구조 및 조직에 대한 권장 사항을 제공합니다.

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

시나리오 채점 전문가 실행

1. 왼쪽 패널의 **[!UICONTROL 시나리오]** 탭을 클릭합니다.
1. 시나리오 채점 전문가를 실행할 시나리오를 선택합니다.
1. 시나리오의 아무 곳이나 클릭하여 시나리오 편집기를 입력합니다.
1. 화면 하단 근처에 있는 시나리오 채점 전문가 아이콘 ![시나리오 채점 전문가](assets/scoring-expert-icon.png)을(를) 클릭합니다.

   시나리오 채점 전문가 패널이 열립니다.
1. **평가**&#x200B;를 클릭합니다.

시나리오 채점 전문가가 10점 만점을 반환하고 합격 또는 실패한 검사를 표시합니다. 검사가 실패한 경우 시나리오 채점 전문가가 시나리오가 이러한 검사를 충족하는지 확인하는 방법에 대한 권장 사항을 제공합니다.

![시나리오 점수](assets/scenario-score.png)

## 시나리오 채점 확인

시나리오 채점 전문가는 다음 검사를 사용합니다.

* 시나리오에 이름을 지정해야 합니다.
* 모든 모듈에 레이블이 지정되어야 합니다.
* 시나리오는 정해진 일정에 따라 실행되어야 합니다.

  지침은 [시나리오 예약](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md)을 참조하세요.
* 시나리오 블루프린트 크기는 5MB 미만이어야 합니다.

  자세한 내용은 [Fusion 성능 보호](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios)를 참조하십시오.
* Workfront 인스턴트 트리거 모듈을 사용하는 경우 필터링해야 합니다.

  자세한 내용은  [!DNL Workfront] > [!UICONTROL 이벤트 보기] 모듈에서 [이벤트 구독 필터](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module)를 참조하십시오.





