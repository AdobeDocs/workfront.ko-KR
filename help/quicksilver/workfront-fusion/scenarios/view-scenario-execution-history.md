---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion에서 시나리오 내역 보기
description: 시나리오에 대한 모든 실행에 대한 정보를 표시하거나 특정 데이터에 대한 시나리오의 모든 실행을 검색할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 2e26c4e4b5f331ed2e609381ef442f45e90c4faa
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 시나리오 기록 보기

시나리오의 이벤트 또는 실행에 대한 정보를 표시하거나 시나리오의 모든 실행에서 특정 데이터를 검색할 수 있습니다.

시나리오 실행은 시나리오의 단일 실행을 나타냅니다.

시나리오 이벤트는 편집, 활성화 또는 비활성화와 같은 시나리오 수정입니다.

>[!NOTE]
>
>시나리오의 내역은 지난 30일 동안의 모든 시나리오의 이벤트 및 실행을 표시합니다.

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

## 시나리오 내역 보기

### [!UICONTROL 시나리오 세부 정보] 페이지에서 시나리오 기록 보기

1. 왼쪽 패널의 **[!UICONTROL 시나리오]** 탭을 클릭한 다음 시나리오를 클릭합니다.

   또는

   시나리오 편집기에서 시나리오 작업을 수행하는 경우 창의 왼쪽 위 모서리 근처에 있는 왼쪽 화살표 ![](assets/exit-editing-arrow.png)을(를) 클릭합니다.

1. 오른쪽 패널의 **기록** 탭에서 실행 기록을 봅니다.

   시나리오의 모든 실행에 대해 다음 세부 정보가 나열됩니다.

   * 실행이 **[!UICONTROL 시작됨]**&#x200B;인 날짜
   * **[!UICONTROL 상태]**(성공 또는 실패)
   * **[!UICONTROL 기간]** 실행
   * **[!UICONTROL 작업]** 수
   * **[!UICONTROL 데이터 전송]** 크기

   >[!NOTE]
   >
   >실행 세부 정보가 저장소에 기록되는 동안 시나리오 내역에서 최근에 실행된 시나리오 옆에 **처리 중** 배지가 표시됩니다. 처리는 시나리오가 실행된 직후에 발생합니다. 및 은(는) 몇 분 이내로 지속됩니다. 실행이 처리되는 동안에는 시나리오 실행에 대한 세부 정보가 표시되지 않을 수 있습니다.

1. 특정 시나리오 실행에 대한 세부 정보를 보려면 오른쪽 패널에서 해당 실행을 클릭합니다.
1. 이벤트를 보려면 오른쪽 패널의 **이벤트** 탭을 클릭합니다.


### [!UICONTROL 기록] 탭에서 시나리오 기록 보기

[!UICONTROL 기록] 탭에 [!UICONTROL 시나리오 세부 정보] 페이지에서 사용할 수 있는 것보다 더 많은 세부 정보가 표시됩니다. [!UICONTROL 내역] 탭에서 실행을 필터링하고 정렬할 수도 있습니다.

1. 왼쪽 패널의 **[!UICONTROL 시나리오]** 탭을 클릭한 다음 시나리오를 클릭합니다.

   또는

   시나리오 편집기에서 시나리오 작업을 수행하는 경우 창의 왼쪽 위 모서리 근처에 있는 왼쪽 화살표 ![](assets/exit-editing-arrow.png)을(를) 클릭합니다.

1. 페이지의 왼쪽 위 모서리 근처에 있는 **[!UICONTROL 기록]** 탭을 클릭합니다
1. (선택 사항) 처리된 번들을 포함하여 선택한 시나리오 실행에 대한 자세한 내용을 보려면 해당 실행 줄의 **[!UICONTROL 세부 정보]** 단추를 클릭하십시오.

   처리 번들에 대한 자세한 내용은 [시나리오 실행 흐름  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)을(를) 참조하십시오.

   >[!NOTE]
   >
   >* [!UICONTROL 세부 정보] 링크는 실행에 사용 가능한 세부 정보가 있는 경우에만 표시됩니다.
   >
   >* 실행 세부 정보가 저장소에 기록되는 동안 시나리오 내역은 최근에 실행된 시나리오 옆에 **처리 내역** 배지를 표시합니다. 처리는 시나리오가 실행된 직후에 발생합니다. 및 은(는) 몇 분 이내로 지속됩니다. 실행이 처리되는 동안에는 시나리오 실행에 대한 세부 정보가 표시되지 않을 수 있습니다.

1. 이벤트를 보려면 **이벤트 표시** 전환을 활성화하십시오.

## 시나리오 실행 내역 필터링

실행 기록을 필터링하여 지정된 값이 있는 실행만 볼 수 있습니다.

1. 이 문서의 [!UICONTROL 기록] 탭에서 [시나리오 실행 기록 보기](#view-scenario-execution-history-on-the-history-tab)에 설명된 대로 시나리오에 대한 전체 페이지 기록을 엽니다.
1. 필터링할 열의 헤더에서 [!UICONTROL filter] 아이콘 ![](assets/fusion-scenario-filter-icon.png)을(를) 클릭합니다.
1. [!UICONTROL 필터] 대화 상자에서 필터링할 값을 입력합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

필터 아이콘은 현재 활성화된 필터가 있는 열의 주황색입니다.

## 시나리오 실행 내역 정렬

시나리오 실행 기록을 정렬할 수 있습니다.

1. 이 문서의 [!UICONTROL 기록] 탭에서 [시나리오 실행 기록 보기](#view-scenario-execution-history-on-the-history-tab)에 설명된 대로 시나리오에 대한 전체 페이지 기록을 엽니다.
1. 필터링할 열의 머리글에서 [!UICONTROL 정렬] 아이콘을 클릭합니다.
1. 선택 사항: 정렬 순서를 반대로 하려면 [!UICONTROL 정렬] 아이콘을 다시 클릭합니다.

## 시나리오의 모든 실행 검색

1. 이 문서의 [!UICONTROL 기록] 탭에서 [시나리오 실행 기록 보기](#view-scenario-execution-history-on-the-history-tab)에 설명된 대로 시나리오에 대한 전체 페이지 기록을 엽니다.
1. 실행 목록의 맨 위에서 **[!UICONTROL 전체 텍스트 검색]**&#x200B;을 클릭합니다.

   또는

   **Ctrl+Shift+F**(Windows) 또는 **Cmd+Shift+F**(Mac) 입력
[!UICONTROL 내역에서 검색] 창이 열립니다.

1. (선택 사항) 특정 텍스트가 포함된 실행을 검색하려면 **[!UICONTROL 내역에서 검색]** 창의 검색 표시줄에 텍스트를 입력하십시오.

   정확한 텍스트를 검색하려면 텍스트를 큰따옴표(&quot;예&quot;)로 둘러쌉니다.

   >[!INFO]
   >
   >**예:** 특정 프로젝트를 만든 실행을 찾으려면 [!UICONTROL 전체 텍스트 검색] 막대에 프로젝트 ID를 입력하십시오.
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (선택 사항) 날짜 범위별로 검색을 제한하려면 [!UICONTROL 날짜 범위별] 영역에서 원하는 검색의 시작 날짜와 종료 날짜를 선택합니다.

   >[!NOTE]
   >
   >* 이전 30일 동안만 실행할 수 있습니다.
   >
   >* [!DNL Workfront Fusion]이(가) 30일 동안 webhook 페이로드를 저장합니다. 웹후크 페이로드가 생성된 후 30일 이상 지나면 &quot;[!UICONTROL 저장소에서 파일을 읽지 못했습니다.]&quot; 오류가 발생합니다.


1. (선택 사항) 상태별로 검색을 제한하려면 **[!UICONTROL 상태별]** 드롭다운에서 원하는 상태를 선택합니다.


   사용 가능한 상태는 다음과 같습니다.

   * [!UICONTROL 모두]

   * [!UICONTROL 오류]

   * [!UICONTROL 경고]

   * [!UICONTROL 성공]

1. (선택 사항) **[!UICONTROL 날짜별 정렬]** 드롭다운에 결과가 표시되는 순서를 변경합니다.

1. (선택 사항) 시나리오 실행 ID를 복사하려면 **[!UICONTROL 실행 ID 복사]** 아이콘을 클릭합니다 원하는 실행 행의 <img src="assets/copy-fusion-execution-id-icon.png">

1. (선택 사항) [!UICONTROL 전체 텍스트 검색] 결과를 클릭하여 정보가 포함된 시나리오 모듈 출력 번들을 검사합니다.
