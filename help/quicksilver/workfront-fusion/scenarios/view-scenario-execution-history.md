---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion에서 시나리오의 실행 기록 보기
description: 시나리오에 대한 모든 실행에 대한 정보를 표시하거나 시나리오의 모든 실행 시 특정 데이터를 검색할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# 에서 시나리오 실행 내역 보기 [!DNL Adobe Workfront Fusion]

시나리오에 대한 모든 실행에 대한 정보를 표시하거나 시나리오의 모든 실행 시 특정 데이터를 검색할 수 있습니다.

시나리오의 실행 내역은 최근 30일 동안의 모든 시나리오의 실행을 표시합니다.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 시나리오의 모든 실행 보기

### 에서 시나리오 실행 내역 보기 [!UICONTROL 시나리오 세부 사항] 페이지

1. 을(를) 클릭합니다. **[!UICONTROL 시나리오]** 왼쪽 패널의 탭을 클릭한 다음 시나리오를 클릭합니다.

   또는

   시나리오 편집기에서 작업 중이라면 왼쪽 화살표를 클릭합니다 ![](assets/exit-editing-arrow.png) 창문의 왼쪽 위 모서리 근처에 있어요.

1. 오른쪽 목록의 정보를 봅니다.

   ![](assets/open-history-tab-350x202.png)

   C

   을 클릭하여 이 정보의 전체 페이지 보기를 볼 수도 있습니다. 전체 페이지 보기를 사용하면 내역을 필터링하여 특정 실행을 볼 수 있습니다.

   시나리오의 모든 실행에 대해 다음 세부 사항이 나열됩니다.

   * 실행 날짜 **[!UICONTROL 시작됨]**
   * **[!UICONTROL 상태]** (성공 또는 실패)
   * 실행 **[!UICONTROL 기간]**
   * 번호 **[!UICONTROL 작업]**
   * 크기 **[!UICONTROL 데이터 전송]**
   * 링크 대상 **[!UICONTROL 세부 사항]**

### 에서 시나리오 실행 내역 보기 [!UICONTROL 기록] 탭

다음 [!UICONTROL 기록] 탭에는 [!UICONTROL 시나리오 세부 사항] 페이지. 또한 [!UICONTROL 기록] 탭.

1. 을(를) 클릭합니다. **[!UICONTROL 시나리오]** 왼쪽 패널의 탭을 클릭한 다음 시나리오를 클릭합니다.

   또는

   시나리오 편집기에서 작업 중이라면 왼쪽 화살표를 클릭합니다 ![](assets/exit-editing-arrow.png) 창문의 왼쪽 위 모서리 근처에 있어요.

1. 을(를) 클릭합니다. **[!UICONTROL 기록]** 페이지의 왼쪽 위 모서리 근처에 있는 탭
1. (선택 사항) 처리된 번들을 포함하여 선택한 시나리오 실행에 대한 자세한 내용을 보려면 **[!UICONTROL 세부 사항]** 링크를 클릭합니다.

   처리 번들에 대한 자세한 내용은 [의 시나리오 실행 흐름 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >다음 [!UICONTROL 세부 정보] 링크는 실행에 세부 사항을 사용할 수 있는 경우에만 표시됩니다.

## 시나리오 실행 내역 필터링

실행 기록을 필터링하여 지정된 값으로 실행만 볼 수 있습니다.

1. 에 설명된 대로 시나리오에 대한 전체 페이지 기록을 엽니다. [에서 시나리오 실행 내역 보기 [!UICONTROL 기록] 탭](#view-scenario-execution-history-on-the-history-tab) 참조하십시오.
1. 을(를) 클릭합니다. [!UICONTROL 필터] 아이콘 ![](assets/fusion-scenario-filter-icon.png) 을 눌러 필터링합니다.
1. 에서 [!UICONTROL 필터] 대화 상자에서 필터링할 값을 입력합니다.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

필터 아이콘은 현재 활성 필터가 있는 열의 주황색입니다.

## 시나리오 실행 내역 정렬

시나리오 실행 내역을 정렬할 수 있습니다.

1. 에 설명된 대로 시나리오에 대한 전체 페이지 기록을 엽니다. [에서 시나리오 실행 내역 보기 [!UICONTROL 기록] 탭](#view-scenario-execution-history-on-the-history-tab) 참조하십시오.
1. 을(를) 클릭합니다. [!UICONTROL 정렬] 아이콘 사용
1. 선택 사항: 정렬 순서를 바꾸려면 [!UICONTROL 정렬] 다시 아이콘을 클릭합니다.

## 시나리오의 모든 실행 검색

1. 을(를) 클릭합니다. **[!UICONTROL 시나리오]** 아이콘 ![](assets/scenarios-icon.png) 왼쪽 패널에서 시나리오를 클릭합니다.

   또는

   시나리오 편집기에서 작업 중이라면 왼쪽 화살표를 클릭합니다 ![](assets/exit-editing-arrow.png) 창문의 왼쪽 위 모서리 근처에 있어요.

1. 을(를) 클릭합니다. **[!UICONTROL 기록]** 화면의 왼쪽 위 모서리 근처에 있는 탭입니다.
1. 클릭 **[!UICONTROL 전체 텍스트 검색]** 를 클릭합니다.

   또는

   유형 **Ctrl+Shift+F** (Windows) 또는 **Cmd+Shift+F** (Mac) [!UICONTROL 기록 검색] 창이 열립니다.

1. (선택 사항) 특정 텍스트가 포함된 실행을 검색하려면 의 검색 표시줄에 텍스트를 입력합니다 **[!UICONTROL 기록 검색]** 창을 엽니다.

   정확한 텍스트를 검색하려면 텍스트를 큰따옴표로 묶습니다(&quot;example&quot;).

   >[!INFO]
   >
   >**예:** 특정 프로젝트를 만든 실행을 찾으려면 프로젝트 ID를 [!UICONTROL 전체 텍스트 검색] 모음
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (선택 사항) 날짜 범위별로 검색을 제한하려면, [!UICONTROL 날짜 범위별] 영역.

   >[!NOTE]
   >
   >* 실행은 이전 30일 동안만 사용할 수 있습니다.
   >
   >* [!DNL Workfront Fusion] 는 30일 동안 웹 후크 페이로드를 저장합니다. 웹 후크 페이로드를 만든 후 30일 이상 액세스하면 &quot; 오류가 발생합니다.[!UICONTROL 저장소에서 파일을 읽지 못했습니다.]&quot;



1. (선택 사항) 상태별로 검색을 제한하려면, **[!UICONTROL 상태별]** 드롭다운.


   사용 가능한 상태는 다음과 같습니다.

   * [!UICONTROL 모두]

   * [!UICONTROL 오류]

   * [!UICONTROL 경고]

   * [!UICONTROL 성공]

1. (선택 사항) **[!UICONTROL 날짜별 정렬]** 드롭다운.

1. (선택 사항) 시나리오 실행 ID를 복사하려면 **[!UICONTROL 실행 ID 복사]** 아이콘 <img src="assets/copy-fusion-execution-id-icon.png"> 원하는 실행 행에서

1. (선택 사항) [!UICONTROL 전체 텍스트 검색] 정보가 포함된 시나리오 모듈 출력 번들을 검사하려면
