---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion의 흐름 제어
description: 시나리오를 만들거나 편집할 때 데이터가 시나리오를 통해 이동하는 방식을 제어하도록 설정을 구성할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 1%

---

# Adobe Workfront Fusion의 흐름 제어

시나리오를 만들거나 편집할 때 데이터가 시나리오를 통해 이동하는 방식을 제어하도록 설정을 구성할 수 있습니다.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 반복

을(를) 사용할 수 있습니다 [!UICONTROL 반복] 모듈을 사용하여 지정된 횟수만큼 작업을 반복할 수 있습니다. A [!UICONTROL 반복] 모듈이 번들을 하나씩 생성합니다.

예를 들어 [!UICONTROL 반복] 모듈로 &quot;Hello 1&quot; &quot;Hello 2&quot; 등의 피사체를 사용하여 5개의 이메일을 전송하는 것입니다 **[!UICONTROL 이메일] >[!UICONTROL 전자 메일 보내기]** 모듈로 [!UICONTROL 반복] 모듈.

를 사용하려면 [!UICONTROL 반복] 모듈:

1. 을(를) 클릭합니다. [!UICONTROL 흐름 제어] 아이콘 ![](assets/flow-control-icon.gif) 화면 하단에서 을(를) 클릭한 다음 **[!UICONTROL 반복]** 를 클릭합니다.
1. 을(를) 클릭합니다. [!UICONTROL 반복] 번들 를 클릭한 다음 **[!UICONTROL 자동으로 연결]** 를 입력합니다.
1. 에서 [!UICONTROL 흐름 제어] 표시되는 상자에 원하는 반복(출력 번들)의 수를 입력합니다 **[!UICONTROL 반복]** 상자.

   이메일 예제에서는 5를 입력합니다.

   ![](assets/repeater-2-350x207.png)

   항목의 값은 마다 **[!UICONTROL 단계]** 필드를 선택하여 볼 수 있습니다 **[!UICONTROL 고급 설정 표시]**. 이 숫자는 기본적으로 1입니다.

1. 클릭 **[!UICONTROL 확인]** 를 **[!UICONTROL 흐름 제어]** 상자.

1. 에 연결된 앱 또는 서비스 모듈을 클릭합니다. [!UICONTROL 반복] 모듈.
1. 표시되는 상자에 반복할 정보를 입력합니다.

   이메일 예제에서는 Hello를 [!UICONTROL 제목] 상자, 맵 `i` 반복 모듈에서

   ![](assets/repeater-3-350x207.png)

| 항목 | 설명 |
|---|---|
| [!UICONTROL 초기값] | 모듈을 설정할 번호를 입력하거나 매핑합니다 `i` 첫 번째 반복에서 기본값은 1입니다. |
| [!UICONTROL 반복] | 모듈을 반복할 횟수를 입력하거나 매핑합니다. 이 숫자는 0보다 크거나 같고 10,000보다 작거나 같아야 합니다. |
| [!UICONTROL 단계] | 이 숫자는 모듈이 값을 증가시키는 숫자입니다. `i`. 기본값은 1입니다. |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>반복 수는 의 값으로 결정되지 않습니다. `i`프로그래밍 방식에서 반복될 수 있습니다. 모듈은 [!UICONTROL 반복] 필드. 값 `i` 각 이터레이션으로 변경 [!DNL repeater] 모듈로 매핑되고 이후 모듈에 매핑할 수 있습니다. 위의 예는 값을 매핑합니다. `i` Hello 메시지에 삽입하여 &quot;Hello 1,&quot; Hello 2&quot;를 읽는 메시지가 나타납니다.

## [!UICONTROL 반복기]

An [!UICONTROL 반복기] 는 배열을 일련의 번들로 변환하는 특별한 유형의 모듈입니다. 각 배열 항목은 [!UICONTROL 반복기] 모듈 출력. 자세한 내용은 [[!UICONTROL 반복기] 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## 어레이 누적

어레이 집계는 여러 번들을 하나의 번들로 병합할 수 있는 특별한 유형의 모듈입니다. 자세한 내용은 [[!UICONTROL 누적] Adobe Workfront Fusion의 모듈](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL 라우터]

다음 [!UICONTROL 라우터] 모듈을 사용하면 여러 경로에 플로우를 분기하고 각 경로 내에서 데이터를 다르게 처리할 수 있습니다. 한 번 [!UICONTROL 라우터] 모듈이 번들을 수신하고, 연결된 각 경로들에 해당 경로가 연결된 순서대로 전달됩니다 [!UICONTROL 라우터] 모듈. 자세한 내용은 [라우터 모듈 입력 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
