---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 에서 기본 시나리오 만들기 [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion을 사용하여 간단한 자동화 시나리오를 만드는 방법에 대해 알아봅니다. 자동화 시나리오는 데이터 조작 및 변형을 포함한 Workfront 프로세스를 자동화합니다. 다음 예에서는 를 검색하는 시나리오를 만드는 프로세스를 안내합니다. [!DNL Workfront] Workfront 및 의 작업이 프로젝트로 전환됩니다.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# 에서 기본 시나리오 만들기 [!DNL Adobe Workfront Fusion]

의 역할 [!DNL Adobe Workfront Fusion] 는 동일한 작업을 반복하지 않고 새로운 작업에 집중할 수 있도록 프로세스를 자동화하는 것입니다. 앱과 서비스 내 및 간의 작업을 연결하여 데이터를 자동으로 전송하고 변환하는 시나리오를 만듭니다. 앱 또는 서비스에서 데이터에 대한 시계를 만들고 해당 데이터를 처리하여 원하는 결과를 제공하는 시나리오입니다.

다음 예에서는 를 검색하는 시나리오를 만드는 프로세스를 안내합니다. [!DNL Workfront] Workfront 및 의 작업이 프로젝트로 전환됩니다.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## 연습 시나리오 만들기

### 시나리오 만들기 시작

1. 다음에서 **시나리오** 영역, 클릭 **새 시나리오 만들기**.

   <!--To locate the Scenarios area, see navigation article-->

   중앙에 빈 모듈이 들어 있는 시나리오 편집기가 표시됩니다.

   <!--picture?-->

1. 다음 항목 선택 **[!UICONTROL 새 시나리오]** 왼쪽 위 모서리에 자리 표시자 이름을 입력한 다음 이름을 입력합니다.
1. 계속 [첫 번째 모듈 추가 및 구성](#add-and-configure-the-first-module) 아래요.

### 첫 번째 모듈 추가 및 구성

1. 빈 모듈을 클릭하여 모듈을 선택할 앱을 선택합니다.

   앱 목록이 모듈 오른쪽에 나타납니다.

1. 선택 **[!DNL Adobe Workfront]**. 표시되지 않는 경우 목록 맨 아래에 있는 검색 막대를 클릭하고 &quot;Workfront&quot;를 입력한 다음 목록에 나타나면 선택합니다.

   목록이 모두 표시되도록 변경됩니다. [!DNL Workfront] 사용할 수 있는 모듈입니다.

1. 다음을 클릭합니다. **[!UICONTROL 검색]** 모듈.

   모듈 구성 창이 열립니다.

1. 다음에서 [!UICONTROL 연결] 상자에서 Workfront 연결을 선택합니다.

   Workfront 연결이 없는 경우 다음을 참조하십시오 [에 대한 연결 만들기 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. 다음에서 [!UICONTROL 레코드 유형] 상자, 선택 **[!UICONTROL 작업]**. 이 옵션은 작업만 검색하도록 모듈을 설정합니다.

   다음을 찾을 수 있습니다. **[!UICONTROL 작업]** &quot; &quot;라는 단어를 입력하면[!UICONTROL 작업].&quot;

1. 다음에서 **[!UICONTROL 결과 집합]** 상자, 선택 **[!UICONTROL 첫 번째 일치 레코드]**.

   이 옵션은 기준을 충족하는 첫 번째 레코드만 반환하도록 모듈을 설정합니다.
1. 다음에서 **[!UICONTROL 검색 기준]** 영역에서 특정 작업을 반환하도록 기준을 구성합니다.

   1. 아래 첫 번째 상자에서 [!UICONTROL 검색 기준]검색에 포함할 필드를 선택합니다. 이 예에서는 을 선택합니다. **[!UICONTROL 이름]**.

      다음을 찾을 수 있습니다. **[!UICONTROL 이름]** &quot; &quot;라는 단어를 입력하면[!UICONTROL 이름].&quot;
   1. 연산자의 경우 옆에 있는 드롭다운 화살표를 클릭합니다. **있음** 및 다음으로 변경 [!UICONTROL **다음 포함(대/소문자 구분 안 함)**].

      이렇게 하면 전체 이름을 입력하지 않거나 대/소문자가 잘못된 이름(예: 모두 대문자)을 입력하더라도 모듈이 이름에 선택한 단어가 포함된 프로젝트를 찾을 수 있습니다.
   1. 의 마지막 필드에서 [!UICONTROL 검색 기준]를 클릭하고 검색 중인 작업 이름에 있는 단어 또는 구를 입력합니다.

1. 다음에서 **[!UICONTROL 출력]** 목록에서 모듈이 출력할 필드를 선택합니다. 이 예에서는 **[!UICONTROL ID]** 및 **[!UICONTROL 이름]** 필드.

   >[!TIP]
   >
   >다음을 사용할 수 있습니다. **Cmd+F** ([!DNL Mac] OS) 또는 **Ctrl-F** ([!DNL Windows] OS)를 사용하여 필드를 신속하게 찾을 수 있습니다.

1. 클릭 **[!UICONTROL 확인]** 모듈 구성을 저장합니다.

1. 모듈을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 이름 바꾸기]**&#x200B;을 클릭하고 모듈에서 수행할 작업을 설명하는 이름을 입력한 다음(&quot;작업 검색&quot; 등) **[!UICONTROL 확인]**.

   모듈 바로 아래에 이름이 표시됩니다. 그 아래로는 [!DNL Workfront Fusion] 에는 모듈에서 수행한 작업 유형에 대한 간단한 설명이 포함됩니다.

   ![](assets/module-renamed-wf.png)

1. 계속 [두 번째 모듈 추가 및 구성](#add-and-configure-the-second-module).

## 두 번째 모듈 추가 및 구성

1. 모듈 오른쪽에 있는 부분 원을 마우스로 가리킨 다음 을 클릭합니다 **[!UICONTROL 다른 모듈 추가]**.
1. 선택 [!DNL Adobe Workfront] 응용 프로그램 목록에서 모듈을 선택합니다 **[!UICONTROL 개체 변환]**.
1. 다음에서 [!UICONTROL 연결] 필드에서 이전 모듈에서 사용한 것과 동일한 Workfront 연결을 선택합니다.
1. 다음에서 **[!UICONTROL 레코드 유형]** 필드, 선택 **[!UICONTROL 작업]**- 모듈이 작업을 전환하기 때문입니다.
1. 다음에서 **[!UICONTROL 변환 대상]** 필드, 선택 **프로젝트**.
1. 작업 ID 필드 옆에 있는 맵 토글을 클릭하여 활성화합니다.

   활성화되면 토글이 파란색으로 바뀝니다. 이를 통해 이전 모듈의 작업 ID를 매핑할 수 있습니다.

   ![맵 전환](assets/map-toggle.png)
1. 다음을 클릭합니다. **[!UICONTROL 작업 ID]** 필드.

   프로젝트로 전환할 작업의 ID로 사용할 항목을 선택할 수 있는 패널이 열립니다. 매핑을 활성화했으므로 패널에는 이전 모듈의 출력이 포함됩니다. ID를 이전 모듈의 출력으로 선택했으므로 이제 패널에서 사용할 수 있습니다.

   이 패널을 매핑 패널이라고 합니다. 매핑 패널에 대한 자세한 내용은 [한 모듈에서 다른 모듈로 정보 매핑](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. 선택 **ID** 매핑 패널에서 참조할 수 있습니다.

   ID 필드가 ID 블록으로 표시됩니다. 매핑된 원본 모듈 번호와 매핑된 필드를 표시합니다.

   ![맵 ID](assets/map-id.png)

1. 다음을 클릭합니다. **템플릿 ID** 필드에서 이 프로젝트에 사용할 Workfront 템플릿의 이름을 입력한 다음 목록에 표시될 때 선택합니다.
1. 클릭 **[!UICONTROL 확인]** 모듈 구성을 저장합니다.

1. 모듈을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 이름 바꾸기]**&#x200B;을 클릭하고, 모듈에서 수행할 작업을 설명하는 이름을 입력한 다음(&quot;프로젝트로 변환&quot;), **[!UICONTROL 확인]**.

1. 계속 [시나리오 테스트](#test-the-scenario).

## 시나리오 테스트

시나리오를 활성화하기 전에 한 번 이상 실행하고 결과를 보고 테스트하는 것이 중요합니다. 이렇게 하면 시나리오에 데이터가 흐르는 방식을 이해하고 오류를 찾는 데 도움이 됩니다.

이 시나리오에서는 테스트가 성공하면 새 작업을 찾아 프로젝트로 변환합니다.

1. 클릭 **[!UICONTROL 한 번 실행]** (시나리오 편집기의 왼쪽 아래 모서리)를 참조하십시오.
1. 시나리오 실행이 완료되면 첫 번째 모듈 위의 버블을 클릭하여 모듈이 반환한 작업에서 가져온 데이터를 포함하여 모듈이 처리한 데이터 번들에 대한 정보를 볼 수 있습니다.

1. 두 번째 모듈 위의 실행 검사기 버블을 클릭하여 입력(작업)과 출력(변환된 프로젝트)을 확인합니다.

   검사 버블의 데이터에 대한 자세한 내용은 다음을 참조하십시오.

   * 일반적인 정보는 다음을 참조하십시오. [의 시나리오 실행 흐름 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * 처리된 번들에 대한 자세한 내용은 [의 시나리오 실행, 주기 및 단계 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 위치 [!DNL Workfront Fusion], 클릭 **[!UICONTROL 저장]** 왼쪽 아래 모서리 근처에 있습니다.

   >[!IMPORTANT]
   >
   >원하는 만큼 자주 저장하고 시나리오를 테스트합니다.

>[!TIP]
>
>각 모듈에 대한 메모를 추가하는 옵션이지만 유용한 방법을 권장합니다.
>
>1. 마우스 오른쪽 단추 클릭 [!DNL Workfront] 모듈을 클릭한 다음 **[!UICONTROL 메모 추가]**.
>1. 표시되는 노트에 모듈에 대한 개요를 입력합니다.
>
>    한 모듈에 대해 여러 메모를 추가할 수 있습니다.
>
>1. 닫기 **[!UICONTROL 메모]** 영역입니다.
>
>     시나리오에 메모를 추가하면 주황색 점이 **[!UICONTROL 메모]** 아이콘 ![](assets/notes-icon-w-dot.png) 시나리오 편집기 하단에서.
>
>1. 다음을 클릭합니다. **[!UICONTROL 메모]** 아이콘 ![](assets/notes-icon-w-dot.png) 메모를 확인합니다.
>

## 시나리오 활성화

시나리오를 만드는 마지막 단계는 활성화하는 것입니다.

이 시나리오는 특정 작업을 검색하는 것이므로 활성화할 필요가 없습니다. 시나리오를 활성화하면 일정에 따라 또는 애플리케이션에서 특정 작업이 발생할 때 시나리오가 실행됩니다. 시나리오를 활성화하면 기본적으로 15분마다 실행됩니다. 실행할 시기와 빈도를 정의하여 변경할 수 있습니다.

시나리오 활성화에 대한 자세한 내용은 다음을 참조하십시오. [에서 시나리오 활성화 또는 비활성화 [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

일정에 대한 자세한 내용은 [시나리오 예약 위치 [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## 다음 단계

* [트리거 모듈 추가](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) 를 사용하면 시나리오가 정기적으로 새 요청을 검색하고 프로젝트로 변환할 수 있습니다.
* 요청이 입력될 때마다 시나리오를 실행할 수 있도록 하려면 웹후크를 추가합니다.
* 필터를 추가하여 특정 요청만 프로젝트로 변환되도록 합니다.
* 새 프로젝트의 이름을 사용자 지정하는 함수를 추가합니다.
* 오류 처리를 추가하여 시나리오가 오류에 대해 복원력이 있는지 확인합니다.

