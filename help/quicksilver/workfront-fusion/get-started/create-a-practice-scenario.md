---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion에서 연습 통합 시나리오 만들기
description: 이 문서에서는 Adobe Workfront Fusion과 통합 시나리오를 만드는 방법에 대해 설명합니다. 통합 시나리오는 개별 앱을 서로 연결하여 데이터가 다양한 애플리케이션을 통해 전달되도록 합니다.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '2139'
ht-degree: 0%

---

# Adobe Workfront Fusion에서 연습 통합 시나리오 만들기

이 문서에서는 Adobe Workfront Fusion과 통합 시나리오를 만드는 방법에 대해 설명합니다. 통합 시나리오는 개별 앱을 서로 연결하여 데이터가 다양한 애플리케이션을 통해 전달되도록 합니다.

통합 시나리오를 만들려면 조직에 [!DNL Workfront Fusion for Work Automation and Integration] 라이센스.

Workfront 전용 자동화 시나리오 빌드에 대한 지침은 [Adobe Workfront Fusion에서 연습 자동화 시나리오 만들기](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Workfront Fusion 라이선스에 대한 자세한 내용은 [Adobe Workfront Fusion 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>조직에서 Google 시트에 대한 액세스를 허용하지 않을 수 있습니다. 이 경우 이 통합을 설정할 수 없지만 여기에 제공된 정보는 통합 시나리오가 작동하는 방식에 대한 일반적인 예로 사용할 수 있습니다.

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
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## 연습 시나리오 만들기

의 역할 [!DNL Adobe Workfront Fusion] 는 동일한 작업을 반복하지 않고 새로운 작업에 집중할 수 있도록 프로세스를 자동화하는 것입니다. 앱과 서비스 내 및 간의 작업을 연결하여 데이터를 자동으로 전송하고 변환하는 시나리오를 만듭니다. 앱 또는 서비스에서 데이터에 대한 시계를 만들고 해당 데이터를 처리하여 원하는 결과를 제공하는 시나리오입니다.

시나리오는 앱 내에서 데이터를 변환하거나 앱과 웹 서비스 간에 데이터를 전송하는 방법을 나타내는 일련의 모듈로 구성됩니다.

사용 방법을 배울 때 시나리오를 만들고 모범 사례를 강화하는 방법을 설명합니다. [!DNL Workfront Fusion]이 문서는 단계별 프로세스를 안내합니다. 다음에서 새 레코드를 만드는 시나리오를 만듭니다. [!DNL Workfront] 의 모든 행에 대해 [!DNL Google Sheets] 스프레드시트입니다.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>이와 같은 시나리오는 프로젝트를 사용해야 하는 프로젝트를 나열하는 스프레드시트가 있는 경우에 유용합니다 [!DNL Workfront]. 시나리오는에서 새 행의 스프레드시트를 &quot;확인&quot;하고 새 프로젝트를 추가할 수 있습니다. [!DNL Workfront] 한 개당.

시나리오 생성은 다음과 같은 몇 가지 주요 작업으로 구성됩니다.

## 앱을 선택하고 시나리오 이름을 지정합니다.

1. 다운로드 [스프레드시트](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)을(를) 업로드한 다음 [!DNL Google Drive] 이 연습에서 사용할 수 있습니다.

   또는

   간단한 항목 만들기 또는 찾기 [!DNL Google Sheets] 이 스프레드시트와 유사한 스프레드시트:

   ![](assets/spreadsheet-headers-350x55.png)

1. 로그인 [!DNL Workfront Fusion] 계정입니다.
1. 클릭 **[!UICONTROL 시나리오]** ![](assets/scenarios-icon.png) 왼쪽 패널에서

   >[!NOTE]
   >
   >왼쪽 탐색 패널이나 해당 아이콘이 보이지 않으면 메뉴를 클릭합니다 ![메뉴](assets/main-menu-icon-left-nav.png) 아이콘.

   회색으로 [!UICONTROL 폴더] 패널 을 표시하면 시나리오를 폴더로 구성할 수 있습니다.

   오른쪽 메인 영역 상단에 **[!UICONTROL 모두]** 작성한 시나리오, **[!UICONTROL 활성 시나리오]** 및 **[!UICONTROL 비활성 시나리오]**, 및 **[!UICONTROL 개념]**: 이전에 더 많은 작업이 필요한 시나리오입니다 [!DNL Workfront Fusion] 활성 또는 비활성으로 분류할 수 있습니다.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. 다음에서 [!UICONTROL 폴더] 패널, 클릭 **[!UICONTROL 폴더 추가]** 아이콘 ![](assets/add-folder-icon.png)그런 다음 첫 번째 폴더에 대해 &quot;연습 시나리오&quot;와 같은 이름을 입력합니다.

1. 폴더를 열고 를 클릭합니다. **[!UICONTROL 새 시나리오 만들기]** 페이지의 오른쪽 상단 모서리에서 을 참조하십시오.

   표시되는 랜딩 페이지를 사용하여 빌드할 시나리오에서 사용할 앱을 미리 로드할 수 있습니다.

1. 이 연습에서 을(를) 검색하고 선택합니다. **[!UICONTROL Google Sheets]** 앱.
1. 클릭 **[!UICONTROL 계속]** 오른쪽 상단 모서리입니다.

   시나리오 편집기 중앙에 빈 모듈이 있고 [!DNL Google Sheets] 미리 로드한 앱과 맨 아래에 있는 도구 모음에 있는 일부 옵션이 표시됩니다.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

새 시나리오를 만들 때 시나리오의 이름을 만드는 것으로 시작하는 것이 좋습니다.

1. 다음 항목 선택 **[!UICONTROL 새 시나리오]** 왼쪽 상단 모서리에 자리 표시자 이름을 입력한 다음 &quot;Practice scenario 1&quot;과 같은 이름을 입력합니다.
1. 계속 [첫 번째 모듈 추가 및 구성](#add-and-configure-the-first-module) 아래요.

## 첫 번째 모듈 추가 및 구성

물음표가 있는 빈 모듈은 추가해야 하는 트리거 모듈을 나타냅니다. 이 모듈은 실행될 때마다 시나리오를 시작합니다. 빈 모듈의 시계 아이콘은 예약된 모듈임을 나타냅니다.

![](assets/empty-module.png)

이 모듈에는 시나리오가 감시할 데이터가 포함됩니다.

1. 빈 모듈을 클릭하여 모듈을 선택할 앱을 선택합니다.

   이전에 미리 로드한 앱이 빈 모듈 옆에 표시됩니다. 를 사용하여 모듈이 있는 다른 모든 앱을 추가할 수 있습니다. [!UICONTROL 검색] 상자.

   ![](assets/pre-loaded-apps-350x139.png)

1. 클릭 **[!DNL Google Sheets]**.

   목록이 모두 표시되도록 변경됩니다. [!DNL Google Sheets] 트리거 모듈로 사용할 수 있는 모듈입니다.

1. 트리거 모듈 클릭 **[!UICONTROL 기록 감시]**.

   이제 Google 계정에 대해 인증된 연결을 설정해야 합니다. 시나리오에 추가하는 모든 모듈에는 해당 앱에 대한 연결이 있어야 합니다.

1. 다음에서 **[!DNL Google Sheets]** 상자, 아래 **[!UICONTROL 연결]**, 클릭 **[!UICONTROL 추가]**&#x200B;을(를) 클릭한 다음 &quot;Olivia의 Google 계정&quot;과 같은 연결 이름을 입력하고 **[!UICONTROL 계속]**.
1. 표시되는 창에서 연결을 인증합니다.

   연결을 인증하는 프로세스는 앱 간에 약간 다를 수 있습니다. 앱에 로그인해야 할 수 있습니다. 일반적으로 다음을 클릭해야 합니다. **[!UICONTROL 허용]** 단추를 클릭합니다. 도움이 필요한 경우 다음을 참조하십시오. [연결 개요](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 첫 번째 모듈 구성

연결 후 [!DNL Workfront Fusion] (으)로 [!DNL Google Sheets] 계정, 다음을 지정할 수 있습니다. [!DNL Google Sheets] 액세스 권한이 있는 스프레드시트와 첫 번째 모듈에서 처리할 데이터를 선택합니다.

1. 다음을 클릭합니다. **[!UICONTROL 스프레드시트]** 상자를 선택한 다음 **[!UICONTROL Workfront Fusion 연습 시나리오] #1** 표시되는 목록의 스프레드시트입니다.

   이 스프레드시트에는 2개의 시트(탭)가 포함되어 있으므로 원하는 데이터가 포함된 시트를 지정해야 합니다.

1. 다음에서 **[!UICONTROL 시트]** 드롭다운 목록에서 다음을 선택합니다. **[!UICONTROL 프로젝트]**.

   스프레드시트에는 헤더가 포함되어 있으며 모듈은 이 헤더를 사용하여 처리할 데이터를 식별하려고 합니다.

   ![](assets/spreadsheet-headers-350x55.png)

1. 나가기 **[!UICONTROL 예]** 다음에 대해 선택됨 **[!UICONTROL 표에 머리글이 포함되어 있음]**.

1. 다음에서 **[!UICONTROL 헤더가 있는 행]** 상자에서 포함할 행 범위를 지정할 수 있지만, 이 연습을 수행하려면 기본값 A1:Z1은 그대로 두겠습니다.
1. 다음에서 **[!UICONTROL 제한]** 상자에 1을 입력합니다.

   이렇게 하면 시나리오를 실행할 때마다 모듈은 스프레드시트에서 1개 행만 처리합니다. 이 기능은 시나리오를 작성하는 동안 테스트 실행을 단순화하는 데 유용합니다.

1. 클릭 **[!UICONTROL 확인]**.

   다음 **[!UICONTROL 시작할 위치 선택]** 상자에 스프레드시트에서 모듈 처리를 시작할 위치를 지정하라는 메시지가 표시됩니다.

1. 클릭 **[!UICONTROL 수동으로 선택]**&#x200B;표시되는 목록에서 맨 위 옵션을 선택한 다음 을 클릭합니다. **[!UICONTROL 확인]**.
1. 모듈을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 이름 바꾸기]**&#x200B;을 클릭하고, 모듈에서 수행할 작업을 설명하는 이름을 입력한 다음(&quot;프로젝트 목록 보기&quot;), **[!UICONTROL 확인]**.

   모듈 바로 아래에 이름이 표시됩니다. 그 아래로는 [!DNL Workfront Fusion] 에는 모듈에서 수행한 작업 유형에 대한 간단한 설명이 포함됩니다.

   ![](assets/module-renamed-350x388.png)

1. 계속 [두 번째 모듈 추가 및 구성](#add-and-configure-the-second-module).

## 두 번째 모듈 추가 및 구성

1. 모듈 오른쪽에 있는 부분 원을 클릭하여 **[!UICONTROL 다른 모듈 추가]**.

   이 두 번째 모듈은 [!DNL Workfront] 모듈이지만 을(를) 미리 로드하지 않았습니다. [!DNL Workfront] 앱.

1. 을(를) 찾으려면 [!DNL Workfront] 앱, &quot; 입력 시작[!DNL Workfront]&quot;앱을 클릭한 다음 표시되는 앱을 클릭합니다.
1. 의 목록에서 [!DNL Workfront] 표시되는 모듈에서는 **[!UICONTROL 레코드 만들기]**.

1. Google Sheets 앱을 사용한 이전과 마찬가지로 **[!UICONTROL 추가]** 다음에서 [!DNL Workfront] Workfront Fusion과 Workfront 간에 연결을 추가하는 상자

   이제 스프레드시트의 데이터를 사용하여 수행할 작업을 지정하겠습니다.

1. 클릭 **[!UICONTROL 레코드 유형]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL 프로젝트]** 에서 프로젝트를 만들고 싶어서 [!DNL Workfront] 스프레드시트의 행을 사용합니다.

   >[!TIP]
   >
   >다음을 찾을 수 있습니다. **[!UICONTROL 프로젝트]** &quot; &quot;라는 단어를 입력하면[!UICONTROL 프로젝트].&quot;

   상자가 확장되어 사용 가능한 모든 항목을 표시합니다 [!DNL Workfront] 첫 번째 모듈에서 찾은 정보를 넣을 수 있는 프로젝트 필드입니다.

   다음을 사용합니다. **[!UICONTROL 이름]** 필드: 이 모듈에서 각 프로젝트의 이름을 로 지정하려고 합니다. [!DNL Workfront] 해당 [!UICONTROL Google Sheets] 행.

1. 을(를) 찾아 클릭합니다 **[!UICONTROL 이름]** 필드.

   >[!TIP]
   >
   >다음을 사용할 수 있습니다. **Cmd+F** ([!DNL Mac] OS) 또는 **Ctrl-F**([!DNL Windows] OS)를 사용하여 필드를 신속하게 찾을 수 있습니다.

   이렇게 하면 에서 사용할 수 있는 변수 목록이 열립니다 **[!UICONTROL 이름]** Workfront에서 만든 각 프로젝트의 이름을 정의하는 필드입니다.

   ![](assets/list-of-available-variables-350x261.png)

   목록의 맨 위에 있는 변수는 스프레드시트의 열 헤더에 해당합니다.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. 변수 클릭 **[!UICONTROL 내 프로젝트 이름 (A)]** 을(를) 추가하여 **[!UICONTROL 이름]** 필드.

   이 시나리오에 대한 첫 번째 데이터를 방금 매핑했습니다.

   스프레드시트에서 한 개 더 데이터를에 매핑하겠습니다. [!DNL Workfront]: 각 프로젝트의 시작 일자.

1. 을(를) 찾아 클릭합니다 **[!UICONTROL 계획된 시작 일자]** 필드를 클릭한 다음 **[!UICONTROL 계획된 시작 일자(E)]** 변수를 사용하여 스프레드시트의 해당 열에서 데이터를 가져옵니다.

1. 클릭 **[!UICONTROL 확인]**.

   이제 작업 시나리오가 있습니다.

1. 두 번째 모듈에 &quot;Workfront 프로젝트 만들기&quot;와 같은 이름을 지정한 다음 [시나리오 테스트](#test-the-scenario).

## 시나리오 테스트

시나리오를 활성화하기 전에 한 번 이상 실행하고 결과를 보고 테스트하는 것이 중요합니다. 이렇게 하면 시나리오에 데이터가 흐르는 방식을 이해하고 오류를 찾는 데 도움이 됩니다.

스프레드시트에서 1개 행이 처리되도록 선택하여 Workfront에서 프로젝트를 생성했습니다. 시나리오를 실행할 경우 그렇게 해야 합니다.

1. 클릭 **[!UICONTROL 한 번 실행]** (시나리오 편집기의 왼쪽 아래 모서리)를 참조하십시오.
1. 시나리오 실행이 끝나면 위의 버블을 클릭합니다. [!DNL Google Sheets] 모듈.

   ![](assets/click-bubble.png)

   표시되는 상자에서 시작한 행의 스프레드시트에서 가져온 실제 데이터를 포함하여 모듈이 처리한 데이터 번들에 대한 정보를 볼 수 있습니다.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. 위의 실행 검사기 버블 클릭 [!DNL Workfront] 정보 입력 및 이제 만들어지는 프로젝트의 ID인 출력을 볼 수 있는 모듈 [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   다음 문서에서 시나리오 실행 정보를 읽는 방법에 대해 자세히 알아볼 수 있습니다.

   * 일반적인 정보는 다음을 참조하십시오. [의 시나리오 실행 흐름 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 처리된 번들에 대한 자세한 내용은 [의 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 다음으로 이동 [!DNL Workfront] 시나리오가 만든 프로젝트를 보려면 &quot;soho downtown loft&quot;를 검색하십시오. 스프레드시트의 마지막 행입니다.
1. 위치 [!DNL Workfront Fusion], 클릭 **[!UICONTROL 저장]** ![](assets/save-icon.png) 왼쪽 아래 모서리 근처에 있습니다.

   >[!IMPORTANT]
   >
   >원하는 만큼 자주 저장하고 시나리오를 테스트합니다.

## 시나리오를 완료하고 다시 테스트합니다.

스프레드시트의 다른 모든 행에 대한 프로젝트를 만들도록 시나리오를 구성해야 합니다.

1. 다음을 클릭합니다. **[!UICONTROL 행 보기]** Google Sheets에 대해 생성한 모듈입니다.
1. 변경 **[!UICONTROL 제한]** 100까지.

   스프레드시트에 있는 행 수보다 큰 숫자를 지정하면 시나리오가 해당 행을 모두 캡처합니다.

1. 마우스 오른쪽 단추 클릭 **[!UICONTROL 행 보기]** 모듈, 클릭 **[!UICONTROL 시작할 위치 선택]**, 클릭 **[!UICONTROL 모두]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 확인]**.

1. 클릭 **[!UICONTROL 한 번 실행]** 그리고 실행 검사기 버블에서 발생하는 작업을 확인합니다.

   다음 [!DNL Google] 시트 **[!UICONTROL 행 보기]** 모듈이 한 번 실행되어 모든 행을 읽습니다. 그런 다음 Workfront **[!UICONTROL 레코드 만들기]** 모듈은 스프레드시트의 나머지 20개 행 각각에 대해 프로젝트를 생성하기 위해 20번 실행됩니다.

1. 에 대한 실행 검사기 버블 클릭 [!DNL Workfront] 모듈을 사용하여 20개의 작업을 모두 확인한 다음, 작업 중 하나를 클릭하여 생성된 프로젝트에 대한 정보를 봅니다.
1. 클릭 **[!UICONTROL 저장]** ![](assets/save-icon.png) 왼쪽 아래 모서리 근처.
1. 다음으로 이동 [!DNL Workfront] 을 클릭하여 시나리오가 만든 프로젝트를 확인합니다.

>[!TIP]
>
>각 모듈에 대한 메모를 추가하는 옵션이지만 유용한 방법을 권장합니다.
>
>1. 마우스 오른쪽 단추 클릭 [!DNL Workfront] 모듈을 클릭한 다음 **[!UICONTROL 메모 추가]**.
>1. 표시되는 노트에 모듈에 대한 개요를 입력합니다.
>
>    이 기능은 모듈을 계속 열어 기능을 확인할 필요가 없기 때문에 유용합니다. &quot;스프레드시트에서 이름, 계획된 시작 일자 및 우선 순위가 매핑된 프로젝트 만들기&quot;와 같은 항목을 입력할 수 있습니다.
>
>    의 경우 [!UICONTROL Google Sheets] 모듈에서 &quot;새 행/프로젝트가 추가되었는지 프로젝트 목록 보기&quot;와 같은 항목을 입력할 수 있습니다.
>
>    한 모듈에 대해 여러 메모를 추가할 수 있습니다.
>
>1. 닫기 **[!UICONTROL 메모]** 영역입니다.
>
>    시나리오에 메모를 추가하면 주황색 점이 **[!UICONTROL 메모]** 아이콘 ![](assets/notes-icon-w-dot.png) 시나리오 편집기 하단에서.
>
>1. 다음을 클릭합니다. **[!UICONTROL 메모]** 아이콘 ![](assets/notes-icon-w-dot.png) 메모를 확인합니다.
>



## 시나리오 활성화

실제 데이터에 사용할 시나리오인 경우 마지막으로 활성화할 수 있습니다. 시나리오를 활성화하면 기본적으로 15분마다 실행됩니다. 실행할 시기와 빈도를 정의하여 변경할 수 있습니다.

시나리오 활성화에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront Fusion에서 시나리오 활성화 또는 비활성화](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

일정에 대한 자세한 내용은 [Adobe Workfront Fusion에서 시나리오 예약](../../workfront-fusion/scenarios/schedule-a-scenario.md).
