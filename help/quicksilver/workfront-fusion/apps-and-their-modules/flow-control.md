---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion의 흐름 제어
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Adobe Workfront Fusion의 흐름 제어

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [흐름 제어](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/flow-control.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

시나리오를 만들거나 편집할 때 설정을 구성하여 데이터가 시나리오를 통과하는 방식을 제어할 수 있습니다.

## 액세스 요구 사항

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td>
  <td> <p>[!UICONTROL Pro] 이상</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합의 경우 [!UICONTROL [!DNL Workfront Fusion], 작업 자동화의 경우 [!UICONTROL [!DNL Workfront Fusion]]</p>
   </td> 
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

## 반복

[!UICONTROL 반복] 모듈을 사용하여 지정된 횟수만큼 작업을 반복할 수 있습니다. [!UICONTROL Repeater] 모듈은 번들을 하나씩 생성합니다.

예를 들어 [!UICONTROL Repeater] 모듈을 사용하여 **[!UICONTROL Email] >[!UICONTROL Email 보내기]** 모듈을 [!UICONTROL Repeater] 모듈에 연결하여 제목 &quot;Hello 1&quot;, &quot;Hello 2&quot; 등이 포함된 5개의 이메일을 보낼 수 있습니다.

[!UICONTROL 반복] 모듈을 사용하려면:

1. 화면 하단의 [!UICONTROL 흐름 제어] 아이콘 ![](assets/flow-control-icon.gif)을 클릭한 다음 표시되는 메뉴에서 **[!UICONTROL 반복]**&#x200B;을 클릭합니다.
1. [!UICONTROL 반복] 번들을 클릭한 다음 표시되는 상자에서 **[!UICONTROL 자동으로 연결]**&#x200B;을 클릭합니다.
1. 표시되는 [!UICONTROL 흐름 제어] 상자에 **[!UICONTROL 반복]** 상자에 원하는 반복 횟수(출력 번들)를 입력합니다.

   이메일 예제에서 5를 입력합니다.

   ![](assets/repeater-2-350x207.png)

   항목의 값이 각 반복에서 **[!UICONTROL 단계]** 필드에 지정된 값만큼 증가합니다. 이 값은 **[!UICONTROL 고급 설정 표시]**&#x200B;를 선택하여 볼 수 있습니다. 이 숫자는 기본적으로 1입니다.

1. **[!UICONTROL 확인]**&#x200B;을 클릭하여 **[!UICONTROL 흐름 컨트롤]** 상자를 닫습니다.

1. [!UICONTROL 반복] 모듈에 연결된 앱 또는 서비스 모듈을 클릭합니다.
1. 나타나는 상자에 반복할 정보를 입력합니다.

   전자 메일 예제에서는 [!UICONTROL 제목] 상자에 Hello를 입력한 다음 반복 모듈에서 `i`을(를) 매핑합니다.

   ![](assets/repeater-3-350x207.png)

| 항목 | 설명 |
|---|---|
| [!UICONTROL 초기 값] | 첫 번째 반복에서 모듈이 `i`(으)로 설정하려는 번호를 입력하거나 매핑합니다. 기본값은 1입니다. |
| [!UICONTROL 반복] | 모듈이 반복될 횟수를 입력하거나 매핑합니다. 이 숫자는 0보다 크거나 같고, 10,000보다 작거나 같아야 합니다. |
| [!UICONTROL 단계] | 모듈이 `i`의 값을 증가시키는 횟수입니다. 기본값은 1입니다. |

{style="table-layout:auto"}

>[!NOTE]
>
>반복 횟수는 프로그래밍의 루프 안에 있으므로 `i` 값으로 결정되지 않습니다. 모듈은 [!UICONTROL 반복] 필드에 표시된 횟수를 반복합니다. `i` 값은 [!DNL repeater] 모듈의 각 반복에 따라 변경되며 이후 모듈에 매핑될 수 있습니다. 위의 예에서는 `i` 값을 Hello 메시지에 매핑하여 &quot;Hello 1&quot;, &quot;Hello 2&quot; 등을 읽는 메시지가 생성됩니다.

## [!UICONTROL 반복자]

[!UICONTROL 반복자]은(는) 배열을 일련의 번들로 변환하는 특별한 유형의 모듈입니다. 각 배열 항목은 [!UICONTROL 반복자] 모듈 출력에서 별도의 번들입니다. 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)의 [[!UICONTROL 반복자] 모듈을 참조하십시오.

## 배열 집계

배열 집계기는 여러 번들을 하나의 번들로 병합할 수 있는 특별한 유형의 모듈입니다. 자세한 내용은 Adobe Workfront Fusion의 [[!UICONTROL 집계] 모듈](../../workfront-fusion/modules/aggregator-module.md)을 참조하십시오.

## [!UICONTROL 라우터]

[!UICONTROL 라우터] 모듈을 사용하면 흐름을 여러 경로로 분기하고 각 경로 내의 데이터를 다르게 처리할 수 있습니다. [!UICONTROL Router] 모듈이 번들을 받으면, [!UICONTROL Router] 모듈에 경로가 첨부된 순서대로 연결된 각 경로로 전달합니다. 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md)의 [라우터 모듈을 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
