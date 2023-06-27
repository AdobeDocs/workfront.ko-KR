---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 의 시나리오에 필터 추가 [!DNL Adobe] Workfront Fusion
description: 일부 시나리오에서는 특정 기준을 충족하는 번들로만 작업해야 합니다. 필터를 사용하여 해당 번들을 선택할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 의 시나리오에 필터 추가 [!DNL Adobe Workfront Fusion]

일부 시나리오에서는 특정 기준을 충족하는 번들로만 작업해야 합니다. 필터를 사용하여 해당 번들을 선택할 수 있습니다.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

두 모듈 사이에 필터를 추가하고 이전 모듈에서 받은 번들이 특정 필터 조건을 충족하는지 확인할 수 있습니다.

* 번들이 그러한 경우 시나리오의 다음 모듈로 전달됩니다.
* 그렇지 않으면 번들 처리가 종료됩니다.

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
  </tr> 
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

## 전제 조건

두 모듈 사이에 필터를 추가하려면 먼저 두 모듈을 시나리오에 추가해야 합니다.

## 다음 두 모듈 사이에 필터를 추가합니다.

1. 클릭 **[!UICONTROL 시나리오]** ![](assets/scenarios-icon.png) 왼쪽 패널에서 시나리오를 선택하여 엽니다.
1. 창의 오른쪽 위 모서리에서 을(를) 클릭합니다 **[!UICONTROL 편집]**.
1. 모듈 사이의 연결 선을 클릭합니다.
1. 표시되는 상자에 a **[!UICONTROL 레이블]** 필터용입니다.
1. 필터 정의 **[!UICONTROL 조건]**.

   두 상자에 하나 또는 두 개의 피연산자를 입력할 수 있습니다. 두 상자 모두에 피연산자를 입력하면 그 사이의 드롭다운 메뉴에서 연산자를 선택하여 피연산자 사이의 관계를 지정할 수 있습니다.

   >[!TIP]
   >
   >피연산자 필드에에 설명된 대로 매핑하는 것과 동일한 방식으로 값을 입력할 수 있습니다 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   예를 들어 필터가 [!DNL Adobe Workfront] xml로 끝나고 전달합니다. [!DNL Dropbox]를 입력하면 됩니다. **[!UICONTROL 파일 이름]** 첫 번째 상자 및 .**[!UICONTROL xml]** 두 번째 상자에서 이 두 메뉴 사이의 드롭다운 메뉴에서 **[!UICONTROL 다음으로 끝남(대/소문자 구분 안 함)]**. 이 필터는 첫 번째 모듈(Workfront)에서 들어오는 번들에 적용됩니다. XML 파일이 포함된 번들만 다음 모듈([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. 클릭 **[!DNL OK]**.

## 필터 복사

현재 시나리오 편집기에는 필터를 복사하는 기능이 포함되어 있지 않습니다.

>[!NOTE]
>
>필터의 양쪽에 있는 모듈을 복사하면 필터도 복사됩니다.
>
>모듈 복사에 대한 자세한 내용은 [에서 모듈 또는 시나리오 복사 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

모듈을 복사하지 않고 필터를 복사하려면 [!DNL Google] Chrome을 참조하십시오.

1. 설치 [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 확장명.
1. 위치 [!DNL Workfront Fusion]을 클릭하여 시나리오를 엽니다.
1. Chrome 3점 메뉴를 클릭한 다음 **[!UICONTROL 기타 도구*]* > **[!UICONTROL 개발자 도구]**.

1. 다음에서 [!UICONTROL 개발자 도구] 패널 을 표시하려면 맨 위에 있는 메뉴 막대에서 [!UICONTROL Workfront Fusion] 탭.

   ![](assets/copy-a-filter-350x174.png)

1. 다음을 클릭합니다. **[!UICONTROL 도구]** 아이콘 ![](assets/devtools-tools-icon.png) 왼쪽 바에 있습니다.

1. 클릭 **[!UICONTROL 필터 복사]**&#x200B;을(를) 구성한 다음 **[!UICONTROL 필터 복사]** 오른쪽 패널의 도구:

   1. 설정 **[!UICONTROL 소스 모듈]** 을(를) 복사할 필터 바로 뒤에 있는 모듈로 사용하십시오.
   1. 설정 **[!UICONTROL Target 모듈]** 를 복사할 필터 바로 앞에 있는 모듈로 사용하십시오.

1. 클릭 **[!UICONTROL 실행]**.
