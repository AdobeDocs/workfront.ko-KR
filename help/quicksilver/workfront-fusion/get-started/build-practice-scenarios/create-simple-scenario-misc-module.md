---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: ' [!DNL Adobe Workfront Fusion]에서 간단한 시나리오 만들기'
description: Adobe Workfront Fusion을 사용하여 간단한 자동화 시나리오를 만드는 방법에 대해 알아봅니다. 자동화 시나리오는 데이터 조작 및 변형을 포함한 Workfront 프로세스를 자동화합니다. 이 예에서는 문제를 검색한 다음 이를 프로젝트로 변환하는 시나리오를 만드는 프로세스를 안내합니다.
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 기본 시나리오 만들기

[!DNL Adobe Workfront Fusion]의 역할은 같은 작업을 반복해서 반복하지 않고 새로운 작업에 집중할 수 있도록 프로세스를 자동화하는 것입니다. 앱과 서비스 내 및 간의 작업을 연결하여 데이터를 자동으로 전송하고 변환하는 시나리오를 만듭니다. 앱 또는 서비스에서 데이터에 대한 시계를 만들고 해당 데이터를 처리하여 원하는 결과를 제공하는 시나리오입니다.

이 예에서는 Workfront에서 문제를 검색하고 이 문제를 프로젝트로 변환하는 시나리오를 만드는 프로세스를 안내합니다.

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

1. **시나리오** 영역에서 **새 시나리오 만들기**&#x200B;를 클릭합니다.

   <!--To locate the Scenarios area, see navigation article-->

   중앙에 빈 모듈이 들어 있는 시나리오 편집기가 표시됩니다.

   <!--picture?-->

1. 왼쪽 상단에서 **[!UICONTROL 새 시나리오]** 자리 표시자 이름을 선택한 다음 이름을 입력하십시오.
1. 아래의 [첫 번째 모듈을 추가 및 구성](#add-and-configure-the-first-module)을 계속합니다.

### 첫 번째 모듈 추가 및 구성

1. 빈 모듈을 클릭하여 모듈을 선택할 앱을 선택합니다.

   앱 목록이 모듈 오른쪽에 나타납니다.

1. **[!DNL Adobe Workfront]**&#x200B;을(를) 선택합니다. 표시되지 않는 경우 목록 맨 아래에 있는 검색 막대를 클릭하고 &quot;Workfront&quot;를 입력한 다음 목록에 나타나면 선택합니다.

   목록이 변경되어 사용할 수 있는 [!DNL Workfront] 모듈이 모두 표시됩니다.

1. **[!UICONTROL 검색]** 모듈을 클릭합니다.

   모듈 구성 창이 열립니다.

1. [!UICONTROL 연결] 상자에서 Workfront 연결을 선택합니다.

   Workfront 연결이 없는 경우 [연결 만들기 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)를 참조하십시오.
1. [!UICONTROL 레코드 종류] 상자에서 **[!UICONTROL 문제]**&#x200B;를 선택합니다. 이렇게 하면 모듈이 문제만 검색하도록 설정됩니다.

   &quot;[!UICONTROL 문제]&quot;이라는 단어를 입력하면 목록에서 **[!UICONTROL 문제]**&#x200B;를 찾을 수 있습니다.

1. **[!UICONTROL 결과 집합]** 상자에서 **[!UICONTROL 첫 번째 일치하는 레코드]**&#x200B;을 선택합니다.

   이 옵션은 기준을 충족하는 첫 번째 레코드만 반환하도록 모듈을 설정합니다.
1. **[!UICONTROL 검색 조건]** 영역에서 특정 문제를 반환하도록 조건을 구성하십시오.

   1. [!UICONTROL 검색 조건] 아래의 첫 번째 상자에서 검색에 포함할 필드를 선택합니다. 이 예제에서는 **[!UICONTROL 이름]**&#x200B;을(를) 선택합니다.

      단어 &quot;[!UICONTROL 이름]&quot;을(를) 입력하면 목록에서 **[!UICONTROL 이름]**&#x200B;을(를) 찾을 수 있습니다.
   1. 연산자의 경우 **존재** 옆에 있는 드롭다운 화살표를 클릭하고 [!UICONTROL **포함(대/소문자 구분 안 함)**](으)로 변경합니다.

      이렇게 하면 전체 이름을 입력하지 않거나 대/소문자가 잘못된 이름(예: 모두 대문자)을 입력하더라도 모듈이 이름에 선택한 단어가 포함된 프로젝트를 찾을 수 있습니다.
   1. [!UICONTROL 검색 조건]의 마지막 필드에 검색 중인 문제의 이름에 있는 단어 또는 구를 입력하십시오.

1. **[!UICONTROL 출력]** 목록에서 모듈에서 출력할 필드를 선택합니다. 이 예제에서는 **[!UICONTROL ID]** 및 **[!UICONTROL 이름]** 필드를 선택합니다.

   >[!TIP]
   >
   >**Cmd+F**([!DNL Mac] OS) 또는 **Ctrl-F**([!DNL Windows] OS)를 사용하여 필드를 빠르게 찾을 수 있습니다.

1. **[!UICONTROL 확인]**&#x200B;을 클릭하여 모듈 구성을 저장합니다.

1. 모듈을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 이름 바꾸기]**&#x200B;를 클릭한 다음 모듈에서 수행할 작업을 설명하는 이름을 입력한 다음(&quot;문제 검색&quot; 등) **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

   모듈 바로 아래에 이름이 표시됩니다. 그 아래에 [!DNL Workfront Fusion]에 모듈에서 수행되는 작업 유형에 대한 간단한 설명이 포함되어 있습니다.

   ![](assets/)

1. [두 번째 모듈 추가 및 구성](#add-and-configure-the-second-module)을 계속합니다.

## 두 번째 모듈 추가 및 구성

1. 모듈 오른쪽의 부분 원을 마우스로 가리킨 다음 **[!UICONTROL 다른 모듈 추가]**&#x200B;를 클릭합니다.
1. 응용 프로그램 목록에서 [!DNL Adobe Workfront]을(를) 선택한 다음 **[!UICONTROL 기타 작업]** 모듈을 선택합니다.

   기타 작업 모듈을 사용하면 전용 모듈이 없는 Workfront에서 작업을 수행할 수 있습니다. 이 예에서는 이 모듈을 사용하여 문제를 프로젝트로 변환합니다.
1. [!UICONTROL 연결] 필드에서 이전 모듈에서 사용한 것과 동일한 Workfront 연결을 선택합니다.
1. 수행할 작업이 문제와 관련되어 있으므로 **[!UICONTROL 레코드 종류]**필드에서 **[!UICONTROL 문제]**&#x200B;을(를) 선택합니다.
1. **[!UICONTROL Action]** 필드에서 **convertToProject**&#x200B;을(를) 선택합니다. 선택한 문제를 프로젝트로 변환하는 작업입니다.
1. **[!UICONTROL ID]** 필드를 클릭합니다.

   프로젝트로 전환할 문제의 ID로 사용할 항목을 선택할 수 있는 패널이 열립니다. 패널에는 이전 모듈의 출력이 포함됩니다. ID를 이전 모듈의 출력으로 선택했으므로 이제 패널에서 사용할 수 있습니다.

   이 패널을 매핑 패널이라고 합니다. 매핑 패널에 대한 자세한 내용은 [한 모듈에서 다른 모듈로 정보 매핑](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)을 참조하십시오.
1. 매핑 패널에서 **ID**&#x200B;을(를) 선택합니다.

   ID 필드가 ID 블록으로 표시됩니다. 매핑된 원본 모듈 번호와 매핑된 필드를 표시합니다.

   ![맵 ID](assets/map-id.png)

1. (선택 사항) 프로젝트 섹션에서 소유자 ID 필드를 찾아 필드에 이름을 입력한 다음 표시될 때 선택합니다. 이렇게 하면 프로젝트 소유자로 설정되고 Workfront에서 를 더 쉽게 찾을 수 있습니다.

   >[!TIP]
   >
   >**Cmd+F**([!DNL Mac] OS) 또는 **Ctrl-F**([!DNL Windows] OS)를 사용하여 필드를 빠르게 찾을 수 있습니다.

1. **[!UICONTROL 확인]**&#x200B;을 클릭하여 모듈 구성을 저장합니다.

1. 모듈을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 이름 바꾸기]**&#x200B;를 클릭한 다음 모듈에서 수행할 작업을 설명하는 이름을 입력한 다음(&quot;프로젝트로 변환&quot; 등) **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

1. [시나리오 테스트](#test-the-scenario)를 계속합니다.

## 시나리오 테스트

시나리오를 활성화하기 전에 한 번 이상 실행하고 결과를 보고 테스트하는 것이 중요합니다. 이렇게 하면 시나리오에 데이터가 흐르는 방식을 이해하고 오류를 찾는 데 도움이 됩니다.

이 시나리오의 경우 테스트가 성공하면 문제를 찾아 프로젝트로 전환할 수 있습니다.

1. 시나리오 편집기의 왼쪽 아래에서 **[!UICONTROL 한 번 실행]**&#x200B;을 클릭합니다.
1. 시나리오 실행이 완료되면 첫 번째 모듈 위의 버블을 클릭하여 모듈이 반환한 문제에서 가져온 데이터를 포함하여 모듈이 처리한 데이터 번들에 대한 정보를 볼 수 있습니다.

1. 두 번째 모듈 위의 실행 검사기 버블을 클릭하여 입력(문제)과 출력(변환된 프로젝트)을 확인합니다.

   검사 버블의 데이터에 대한 자세한 내용은 다음을 참조하십시오.

   * 일반 정보는 [시나리오 실행 흐름  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)을(를) 참조하십시오.
   * 처리된 번들에 대한 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)의 [시나리오 실행, 주기 및 단계를 참조하십시오.

1. [!DNL Workfront Fusion]에서 왼쪽 아래 모서리 근처에 있는 **[!UICONTROL 저장]**&#x200B;을 클릭하여 시나리오에 대한 진행 상황을 저장합니다.

   >[!IMPORTANT]
   >
   >원하는 만큼 자주 저장하고 시나리오를 테스트합니다.

>[!TIP]
>
>각 모듈에 대한 메모를 추가하는 옵션이지만 유용한 방법을 권장합니다.
>
>1. [!DNL Workfront] 모듈을 마우스 오른쪽 단추로 클릭한 다음 **[!UICONTROL 메모 추가]**&#x200B;를 클릭합니다.
>1. 표시되는 노트에 모듈에 대한 개요를 입력합니다.
>
>    한 모듈에 대해 여러 메모를 추가할 수 있습니다.
>
>1. **[!UICONTROL 메모]** 영역을 닫습니다.
>
>     시나리오에 메모를 추가하면 시나리오 편집기 하단의 **[!UICONTROL 메모]** 아이콘 ![](assets/notes-icon-w-dot.png)에 주황색 점이 표시됩니다.
>
>1. 메모를 보려면 **[!UICONTROL 메모]** 아이콘 ![](assets/notes-icon-w-dot.png)을(를) 클릭하십시오.
>

## 시나리오 활성화

시나리오를 만드는 마지막 단계는 활성화하는 것입니다.

이 시나리오는 특정 문제를 검색하는 것이므로 활성화할 필요가 없습니다. 시나리오를 활성화하면 일정에 따라 또는 애플리케이션에서 특정 작업이 발생할 때 시나리오가 실행됩니다. 시나리오를 활성화하면 기본적으로 15분마다 실행됩니다. 실행할 시기와 빈도를 정의하여 변경할 수 있습니다.

시나리오 활성화에 대한 자세한 내용은 [Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)에서 시나리오 활성화 또는 비활성화를 참조하십시오.[!UICONTROL 

일정에 대한 자세한 내용은 [[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)에서 시나리오 예약 을 참조하십시오.
