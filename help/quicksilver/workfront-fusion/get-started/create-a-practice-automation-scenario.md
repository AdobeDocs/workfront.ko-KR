---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: ' [!DNL Adobe Workfront Fusion]에서 연습 자동화 시나리오 만들기'
description: 이 문서에서는 Adobe Workfront Fusion을 사용하여 자동화 시나리오를 만드는 방법에 대해 설명합니다. 자동화 시나리오는 데이터 조작 및 변형을 포함한 Workfront 프로세스를 자동화합니다. 이 예제에서는 프로젝트를 검색한 다음 해당 프로젝트와 관련된 모든 작업을 반환하는 시나리오를 만드는 프로세스를 안내합니다.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 8769ed5844e340e007f844370791e93393696819
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 연습 자동화 시나리오 만들기

자동화 시나리오는 데이터 조작 및 변형을 포함한 Workfront 프로세스를 자동화합니다. 이 문서는 프로젝트를 검색한 다음 해당 프로젝트와 관련된 모든 작업을 반환하는 시나리오를 만드는 프로세스를 안내합니다.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront 플랜</td>  
      <td>임의</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront 라이선스</td>  
      <td>
        새로운 기능: 표준<br>
        또는<br>
        현재: 작업 시간 이상
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion 라이선스</td>  
      <td> 
        현재: Workfront Fusion 라이센스 요구 사항이 없습니다.<br>
        또는<br>
        레거시: 모두
      </td>  
    </tr>  
    <tr>  
      <td>제품</td>  
      <td> 
        새로운 기능: Select 또는 Prime Workfront 플랜: 조직에서 Adobe Workfront Fusion을 구매해야 합니다.<br>
        Ultimate Workfront Plan: Workfront Fusion이 포함됩니다.<br>
        또는<br>
        현재: 조직은 Adobe Workfront Fusion을 구매해야 합니다.
      </td>  
    </tr> 
  </tbody>  
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

+++

## 자동화 연습 시나리오 만들기

[!DNL Adobe Workfront Fusion]을(를) 사용하면 반복적인 작업을 자동화하여 중요한 작업에 집중할 수 있습니다. 다양한 앱 및 서비스에서 데이터를 자동으로 관리하는 시나리오를 만듭니다.

각 시나리오는 앱 내에서 데이터를 처리하거나 다른 앱과 서비스 간에 데이터를 전송하는 방법을 안내하는 모듈로 구성됩니다. 예를 들어 [!DNL Workfront] 프로젝트를 자동으로 찾고 해당 작업을 나열하는 시나리오를 Fusion에서 만들 수 있습니다. 이러한 방식으로 Fusion은 일상적인 작업을 처리함으로써 시간과 노력을 절약합니다.

이 연습 시나리오는 [!DNL Workfront] 프로젝트를 검색하고 프로젝트의 작업을 반환하는 시나리오를 만드는 과정을 안내합니다.

![](assets/create-practice-scenario-wf-only-350x157.png)

### 시작하기 전에

이 연습에 사용할 수 있는 Workfront 작업이 포함된 프로젝트를 만드십시오. 프로젝트에 작업을 추가하는 외에 추가적인 구성을 수행할 필요는 없습니다.

Workfront에서 프로젝트를 만드는 방법에 대한 자세한 내용은 xxx를 참조하십시오.

### 1. 시나리오 만들기 및 이름 지정

1. [!DNL Workfront Fusion] 계정에 로그인합니다.
1. 왼쪽 패널에서 **[!UICONTROL 시나리오]** ![](assets/scenarios-icon.png)을(를) 클릭합니다.

   >[!NOTE]
   >
   >왼쪽 탐색 패널이나 해당 아이콘이 보이지 않으면 메뉴 ![메뉴](assets/main-menu-icon-left-nav.png) 아이콘을 클릭합니다.

1. [!UICONTROL **폴더**] 패널에서 **[!UICONTROL 폴더 추가]** 아이콘 ![](assets/add-folder-icon.png)을(를) 클릭한 다음 첫 번째 폴더에 대해 &quot;연습 시나리오&quot;와 같은 이름을 입력하십시오.

1. 폴더를 열고 페이지의 오른쪽 상단에서 **[!UICONTROL 새 시나리오 만들기]**&#x200B;를 클릭합니다.

1. 이 연습에서는 **[!DNL Adobe Workfront]** 앱을 선택한 다음 맨 아래의 **검색**&#x200B;을 클릭합니다.


1. 왼쪽 상단에서 **[!UICONTROL 새 시나리오]** 자리 표시자 이름을 선택한 다음 &quot;연습 시나리오 1&quot;과 같은 이름을 입력하십시오.

   ![](assets/name-the-scenario.png)

1. 아래의 [첫 번째 모듈에 연결](#2-connect-the-first-module)을 사용하여 계속합니다.

### 2. 첫 번째 모듈 연결

이제 [!DNL Workfront] 계정에 대해 인증된 연결을 설정해야 합니다. 시나리오에 추가하는 모든 모듈에는 해당 앱에 대한 연결이 있어야 합니다.

1. **[!DNL Workfront]** 상자의 **[!UICONTROL 연결]**&#x200B;에서 **[!UICONTROL 추가]**&#x200B;를 클릭한 다음 &quot;Olivia의 Workfront 계정&quot;과 같은 연결 이름을 입력하고 **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
1. 표시되는 창에서 연결을 인증합니다.

   연결을 인증하는 프로세스는 앱 간에 약간 다를 수 있습니다. 다음 프로세스는 [!DNL Workfront]에 한정되지만 많은 앱과 유사합니다.

   1. [!DNL Workfront] 도메인을 입력한 다음 **[!UICONTROL 계속]**&#x200B;을 클릭합니다.
   1. [!DNL Workfront]에 로그인합니다.
   1. [!DNL Workfront Fusion]이(가) 요청하는 액세스를 검사한 다음 **[!UICONTROL 액세스 허용]**&#x200B;을 클릭합니다.

   도움이 필요하면 [연결 개요](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)를 참조하세요.

### 3. 첫 번째 모듈 구성

[!DNL Workfront Fusion]을(를) [!DNL Workfront] 계정에 연결한 후 액세스 권한이 있는 [!DNL Workfront] 프로젝트와 첫 번째 모듈에서 처리할 데이터를 지정할 수 있습니다.

1. [!UICONTROL 레코드 종류] 상자에서 **[!UICONTROL 프로젝트]**&#x200B;을 선택합니다. 이렇게 하면 프로젝트만 검색하도록 모듈이 설정됩니다.

   >[!TIP]
   >
   >&quot;[!UICONTROL project]&quot;이라는 단어를 입력하면 목록에서 **[!UICONTROL Project]**&#x200B;을(를) 찾을 수 있습니다.

1. **[!UICONTROL 결과 집합]** 상자에서 **[!UICONTROL 첫 번째 일치하는 레코드]**&#x200B;을 선택합니다. 이 옵션은 기준을 충족하는 첫 번째 레코드만 반환하도록 모듈을 설정합니다. 이 예제에서는 하나의 레코드만 반환되어야 합니다.
1. **[!UICONTROL 검색 조건]** 영역에서 특정 프로젝트를 반환하는 필터를 설정합니다.

   | 필드 | 개 액션 |
   |--------|-------------|
   | 검색 기준 필드 | 값을 검색할 필드를 선택합니다. 이 예제에서는 **[!UICONTROL 이름]**&#x200B;을(를) 선택합니다. |
   | 검색 기준 | 첫 번째 드롭다운 메뉴에서 **[!UICONTROL 이름]**&#x200B;을(를) 선택합니다. |
   | 기본 연산자 | 두 번째 드롭다운에서 [!UICONTROL 포함(대/소문자 구분 안 함)]을 선택합니다. 이렇게 하면 전체 이름을 입력하지 않거나 대/소문자가 잘못된 이름(예: 모두 대문자)을 입력하더라도 모듈이 이름에 선택한 단어가 포함된 프로젝트를 찾을 수 있습니다. |
   | 텍스트 상자 | 검색 중인 프로젝트 이름에 있는 단어 또는 구를 입력합니다. |

+++ 를 확장하여 화면 예제를 봅니다.
   ![](assets/search-name.png)
+++

1. **[!UICONTROL 출력]** 목록에서 모듈에서 출력할 필드를 선택합니다. 이 예제에서는 **[!UICONTROL ID]** 및 **[!UICONTROL 이름]** 필드를 선택합니다.

   >[!TIP]
   >
   >**Cmd+F**([!DNL Mac] OS) 또는 **Ctrl-F**([!DNL Windows] OS)를 사용하여 필드를 빠르게 찾을 수 있습니다.

1. **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >이는 트리거 모듈이 아니므로 시작할 위치를 선택하지 않습니다. 이제 트리거 모듈을 사용할 때 트리거 모듈을 시작할 위치를 선택합니다.
   >
   >
   >자세한 내용은 [트리거 모듈의 시작 위치 선택 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md)을 참조하세요.

1. 모듈을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL 이름 바꾸기]**&#x200B;를 클릭한 다음 모듈에서 수행할 작업을 설명하는 이름을 입력한 다음(&quot;프로젝트 검색&quot; 등) **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

   모듈 바로 아래에 이름이 표시됩니다. 그 아래에 [!DNL Workfront Fusion]에 모듈에서 수행되는 작업 유형에 대한 간단한 설명이 포함되어 있습니다.

   ![](assets/module-renamed-wf.png)

1. [두 번째 모듈 추가 및 구성](#add-and-configure-the-second-module)을 계속합니다.

### 4. 두 번째 모듈 추가 및 구성

1. **[!UICONTROL 다른 모듈을 추가]**&#x200B;하려면 모듈의 오른쪽에 있는 부분 원을 클릭하십시오.
1. 응용 프로그램 목록에서 [!DNL Workfront]을(를) 선택한 다음 검색 모듈 **[!UICONTROL 관련 레코드 읽기]**&#x200B;를 선택하십시오.
1. **[!UICONTROL 연결]** 상자에서 이전 모듈에 대해 만든 연결을 선택합니다. 이 모듈이 이전 모듈과 동일한 연결을 사용하고 있는지 확인해야 합니다.
1. 프로젝트와 관련된 레코드를 읽으려면 **[!UICONTROL 레코드 종류]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL 프로젝트]**&#x200B;을(를) 선택하십시오.

   >[!TIP]
   >
   >&quot;project&quot;라는 단어를 입력하면 목록에서 **[!UICONTROL Project]**&#x200B;을(를) 찾을 수 있습니다.

1. **[!UICONTROL 상위 레코드 ID]** 필드를 클릭합니다. 이 필드에는 작업을 반환하려는 프로젝트의 Workfront ID가 필요합니다.

   필드를 클릭하면 **[!UICONTROL 상위 레코드 ID]** 필드에서 Workfront의 프로젝트를 식별하는 데 사용할 수 있는 변수 목록이 열립니다.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. 변수 **[!UICONTROL ID]**&#x200B;을(를) 클릭하여 **[!UICONTROL 상위 레코드 ID]** 필드에 추가하십시오. 이렇게 하면 첫 번째 모듈에서 반환된 ID를 두 번째 모듈에서 작업할 프로젝트의 식별자로 사용하여 반환된 작업이 해당 프로젝트에 속하도록 할 수 있습니다.
1. **[!UICONTROL 컬렉션]** 필드에서 **[!UICONTROL 작업]**&#x200B;을(를) 선택합니다. 이 모듈은 선택한 프로젝트와 연결된 작업을 반환함을 나타냅니다.
1. **[!UICONTROL 출력]** 필드에서 **[!UICONTROL Id]** 및 **[!UICONTROL 이름]**&#x200B;을(를) 선택합니다.
1. **[!UICONTROL 확인]** 클릭

   이제 작업 시나리오가 있습니다.

1. 두 번째 모듈에 &quot;프로젝트와 연결된 작업 반환&quot;과 같은 이름을 지정한 다음 [시나리오 테스트](#test-the-scenario)를 계속합니다.

## 시나리오 테스트

시나리오를 활성화하기 전에 한 번 이상 실행하고 결과를 보고 테스트하는 것이 중요합니다. 이렇게 하면 시나리오에 데이터가 흐르는 방식을 이해하고 오류를 찾는 데 도움이 됩니다.

1개의 프로젝트가 반환되고 해당 프로젝트와 관련된 작업이 반환되도록 선택했습니다. 시나리오를 실행할 경우 그렇게 해야 합니다.

1. 시나리오 편집기의 왼쪽 아래에서 **[!UICONTROL 한 번 실행]**&#x200B;을 클릭합니다.
1. 시나리오 실행이 끝나면 첫 번째 모듈 위의 버블을 클릭합니다.

   ![](assets/click-bubble.png)

   표시되는 상자에서 모듈이 반환한 프로젝트에서 가져온 실제 데이터를 포함하여 모듈이 처리한 데이터 번들에 대한 정보를 볼 수 있습니다.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. 두 번째 모듈 위의 실행 검사기 버블을 클릭하면 정보 입력 및 프로젝트에 포함된 작업의 집합인 출력을 볼 수 있습니다.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   다음 문서에서 시나리오 실행 정보를 읽는 방법에 대해 자세히 알아볼 수 있습니다.

   * 일반 정보는 [시나리오 실행 흐름  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)을(를) 참조하십시오.
   * 처리된 번들에 대한 자세한 내용은  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)의 [시나리오 실행, 주기 및 단계를 참조하십시오.

1. [!DNL Workfront Fusion]에서 왼쪽 아래 모서리 근처에 있는 **[!UICONTROL 저장]** ![](assets/save-icon.png)을 클릭하여 시나리오에 대한 진행률을 저장합니다.

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

이 예제 시나리오에는 트리거 모듈이 없습니다. 실제 데이터에 사용하는 시나리오인 경우 트리거 모듈로 시작하고 마지막으로 활성화할 수 있습니다. 시나리오를 활성화하면 기본적으로 15분마다 실행됩니다. 실행할 시기와 빈도를 정의하여 변경할 수 있습니다.

시나리오 활성화에 대한 자세한 내용은 [Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)에서 시나리오 활성화 또는 비활성화를 참조하십시오.[!UICONTROL 

일정에 대한 자세한 내용은 [[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)에서 시나리오 예약 을 참조하십시오.
