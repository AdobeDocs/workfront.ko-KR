---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe] Workfront Fusion의 시나리오에 필터 추가'
description: 일부 시나리오에서는 특정 기준을 충족하는 번들로만 작업해야 합니다. 필터를 사용하여 해당 번들을 선택할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]의 시나리오에 필터 추가

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
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
   </td>    </tr> 
  </tr> 
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

## 전제 조건

두 모듈 사이에 필터를 추가하려면 먼저 두 모듈을 시나리오에 추가해야 합니다.

## 다음 두 모듈 사이에 필터를 추가합니다.

1. 왼쪽 패널에서 **[!UICONTROL 시나리오]** ![](assets/scenarios-icon.png)을(를) 클릭한 다음 시나리오를 선택하여 엽니다.
1. 창의 오른쪽 위 모서리에서 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.
1. 모듈 사이의 연결 선을 클릭합니다.
1. 표시되는 상자에 필터에 대한 **[!UICONTROL 레이블]**&#x200B;을(를) 입력합니다.
1. 필터 **[!UICONTROL 조건]**&#x200B;을(를) 정의합니다.

   두 상자에 하나 또는 두 개의 피연산자를 입력할 수 있습니다. 두 상자 모두에 피연산자를 입력하면 그 사이의 드롭다운 메뉴에서 연산자를 선택하여 피연산자 사이의 관계를 지정할 수 있습니다.

   >[!TIP]
   >
   >[한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)에 설명된 대로 피연산자 필드에 매핑하는 것과 같은 방식으로 값을 입력할 수 있습니다.

   예를 들어 필터가 [!DNL Adobe Workfront]에서 XML로 끝나는 파일을 찾아 [!DNL Dropbox]에 전달하려면 첫 번째 상자에 **[!UICONTROL 파일 이름]**&#x200B;을 입력하고두 번째 상자에 **[!UICONTROL xml]**&#x200B;이 있습니다. 이 두 메뉴 사이의 드롭다운 메뉴에서 **[!UICONTROL 다음으로 끝남(대/소문자 구분 안 함)]**&#x200B;을 선택합니다. 이 필터는 첫 번째 모듈(Workfront)에서 들어오는 번들에 적용됩니다. XML 파일이 포함된 번들만 다음 모듈([!DNL Dropbox])로 전달됩니다.

   ![](assets/set-up-filter-box-350x368.jpg)

1. **[!DNL OK]**&#x200B;을(를) 클릭합니다.

## 필터 복사

현재 시나리오 편집기에는 필터를 복사하는 기능이 포함되어 있지 않습니다.

>[!NOTE]
>
>필터의 양쪽에 있는 모듈을 복사하면 필터도 복사됩니다.
>
>모듈 복사에 대한 자세한 내용은 [모듈 또는 시나리오 복사 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)를 참조하십시오.

모듈을 복사하지 않고 필터를 복사하려면 다음 해결 방법으로 [!DNL Google] Chrome을 사용할 수 있습니다.

1. [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome] 확장을 설치합니다.
1. [!DNL Workfront Fusion]에서 시나리오를 엽니다.
1. Chrome 3점 메뉴를 클릭한 다음 **[!UICONTROL 추가 도구*]* > **[!UICONTROL 개발자 도구]**&#x200B;를 클릭합니다.

1. 맨 위의 메뉴 표시줄에 표시되는 [!UICONTROL 개발자 도구] 패널에서 [!UICONTROL Workfront Fusion] 탭을 클릭합니다.

   ![](assets/copy-a-filter-350x174.png)

1. 왼쪽 막대에서 **[!UICONTROL 도구]** 아이콘 ![](assets/devtools-tools-icon.png)을(를) 클릭합니다.

1. **[!UICONTROL 필터 복사]**&#x200B;를 클릭한 다음 오른쪽 패널에서 **[!UICONTROL 필터 복사]** 도구를 구성합니다.

   1. **[!UICONTROL Source 모듈]**&#x200B;을(를) 복사할 필터 바로 뒤에 모듈로 설정하십시오.
   1. **[!UICONTROL 대상 모듈]**&#x200B;을(를) 복사할 필터 바로 앞에 모듈로 설정하십시오.

1. **[!UICONTROL 실행]**&#x200B;을 클릭합니다.
