---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Workfront Fusion의 흐름 제어
description: 시나리오를 만들거나 편집할 때 설정을 구성하여 데이터가 시나리오를 통과하는 방식을 제어할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 1%

---

# Adobe Workfront Fusion의 흐름 제어

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
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
   </td> 
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

## 반복

다음을 사용할 수 있습니다. [!UICONTROL 반복] 지정된 횟수만큼 작업을 반복하는 모듈입니다. A [!UICONTROL 반복] 모듈은 번들을 하나씩 생성합니다.

예를 들어 [!UICONTROL 반복] 을(를) 연결하여 &quot;Hello 1&quot;, &quot;Hello 2&quot; 등의 제목으로 5개의 이메일을 보내는 모듈 **[!UICONTROL 이메일] >[!UICONTROL 이메일 보내기]** 에 대한 모듈 [!UICONTROL 반복] 모듈.

을(를) 사용하려면 [!UICONTROL 반복] 모듈:

1. 다음을 클릭합니다. [!UICONTROL 흐름 제어] 아이콘 ![](assets/flow-control-icon.gif) 화면 하단에서 을(를) 클릭한 다음 **[!UICONTROL 반복]** 을 클릭합니다.
1. 다음을 클릭합니다. [!UICONTROL 반복] 번들을 클릭한 다음 **[!UICONTROL 자동으로 연결]** 을 클릭합니다.
1. 다음에서 [!UICONTROL 흐름 제어] 표시되는 상자에 원하는 반복 횟수(출력 번들)를 입력합니다 **[!UICONTROL 반복]** 상자.

   이메일 예제에서 5를 입력합니다.

   ![](assets/repeater-2-350x207.png)

   항목의 값은 각 반복에서 다음에 지정된 값만큼 증가합니다. **[!UICONTROL 단계]** 필드를 선택합니다. **[!UICONTROL 고급 설정 표시]**. 이 숫자는 기본적으로 1입니다.

1. 클릭 **[!UICONTROL 확인]** 닫으려면 다음을 수행하십시오. **[!UICONTROL 흐름 제어]** 상자.

1. 에 연결된 앱 또는 서비스 모듈을 클릭합니다. [!UICONTROL 반복] 모듈.
1. 나타나는 상자에 반복할 정보를 입력합니다.

   이메일 예제에서 [!UICONTROL 제목] 상자, 맵 `i` repeater 모듈에서 가져왔습니다.

   ![](assets/repeater-3-350x207.png)

| 항목 | 설명 |
|---|---|
| [!UICONTROL 초기 값] | 모듈을 설정할 번호를 입력하거나 매핑합니다. `i` 첫 번째 반복에서 기본값은 1입니다. |
| [!UICONTROL 반복] | 모듈이 반복될 횟수를 입력하거나 매핑합니다. 이 숫자는 0보다 크거나 같고, 10,000보다 작거나 같아야 합니다. |
| [!UICONTROL 단계] | 모듈이 값을 증가시키는 횟수입니다. `i`. 기본값은 1입니다. |

{style="table-layout:auto"}

>[!NOTE]
>
>반복 횟수는 다음 값으로 결정되지 않습니다. `i`: 프로그래밍의 루프에 있는 것과 같습니다. 모듈은 에 표시된 횟수를 반복합니다. [!UICONTROL 반복] 필드. 값 `i` 의 각 반복에 대한 변경 사항 [!DNL repeater] 를 입력합니다. 이 변수는 나중에 모듈에 매핑될 수 있습니다. 위의 예는 의 값을 매핑합니다. `i` 을 Hello 메시지에 포함하면 &quot;Hello 1&quot;, &quot;Hello 2&quot; 등을 읽는 메시지가 생성됩니다.

## [!UICONTROL 반복자]

An [!UICONTROL 반복자] 는 배열을 일련의 번들로 변환하는 특별한 유형의 모듈입니다. 각 배열 항목은에서 별도의 번들입니다. [!UICONTROL 반복자] 모듈 출력입니다. 자세한 내용은 [[!UICONTROL 반복자] 의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## 배열 집계

배열 집계기는 여러 번들을 하나의 번들로 병합할 수 있는 특별한 유형의 모듈입니다. 자세한 내용은 [[!UICONTROL 집계] Adobe Workfront Fusion의 모듈](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL 라우터]

다음 [!UICONTROL 라우터] 모듈을 사용하면 플로우를 여러 경로로 분기하고 각 경로 내의 데이터를 다르게 처리할 수 있습니다. 한 번 [!UICONTROL 라우터] 모듈이 번들을 수신하고, 경로가 첨부된 순서대로 연결된 각 경로로 전달합니다. [!UICONTROL 라우터] 모듈. 자세한 내용은 [의 라우터 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
