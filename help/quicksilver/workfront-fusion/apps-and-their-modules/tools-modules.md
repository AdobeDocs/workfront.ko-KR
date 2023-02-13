---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 도구
description: 다음 [!DNL Adobe Workfront Fusion Tools] 섹션에는 시나리오를 향상시킬 수 있는 몇 가지 유용한 모듈이 포함되어 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 0%

---

# [!UICONTROL 도구]

다음 [!DNL Adobe Workfront Fusion Tools] 섹션에는 시나리오를 향상시킬 수 있는 몇 가지 유용한 모듈이 포함되어 있습니다.

[!UICONTROL 도구] 모듈은 앱 목록 또는 [!UICONTROL 도구] 아이콘 ![](assets/tools-icon-small.png) 화면 하단에 있습니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr>
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 도구] 및 해당 필드

* [Triggers](#triggers)
* [액션](#actions)
* [누적](#aggregators)
* [트랜스포머](#transformers)

### Triggers

#### [!UICONTROL 기본 트리거]

이 모듈을 사용하면 사용자 지정 트리거를 만들고 해당 입력 번들을 정의할 수 있습니다.

이 모듈은 연락처 또는 지정된 이메일 주소(예: [!UICONTROL 이메일] >[!UICONTROL 이메일 보내기], 또는 [!DNL Gmail] >[!UICONTROL 이메일 보내기] 모듈)이나 필요할 때마다 트리거할 간단한 미리 알림입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>배열 항목을 추가하여 사용자 지정 번들을 만듭니다. 배열은 이름 - 값 쌍으로 구성됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 액션

* [[!UICONTROL 여러 변수 가져오기]](#get-multiple-variables)
* [[!UICONTROL 변수 가져오기]](#get-variable)
* [[!UICONTROL 증분 함수]](#increment-function)
* [[!UICONTROL 여러 변수 설정]](#set-multiple-variables)
* [[!UICONTROL 변수 설정]](#set-variable)
* [[!UICONTROL Sleep]](#sleep)

#### [!UICONTROL 여러 변수 가져오기]

이 모듈은 이전에 [!UICONTROL 변수 설정] 또는 [!UICONTROL 여러 변수 설정] 모듈.

이 모듈은 변수가 [!UICONTROL 여러 변수 가져오기] 모듈이 있습니다. 유일한 요구 사항은 [!UICONTROL 도구] > [!UICONTROL 변수 설정] 또는 [!UICONTROL 도구] > [!UICONTROL 여러 변수 설정] 모듈이 먼저 실행됩니다. [!UICONTROL 도구] > [!UICONTROL 여러 변수 가져오기] 모듈. 모듈이 실행되는 순서에 대한 자세한 내용은 [라우터 모듈 입력 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>모듈에 가져올 변수를 추가합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 변수 이름]</td>
        <td>추가하는 각 변수에 대해 가져올 변수의 이름을 매핑합니다.</td>
    </tr>
</table>

>[!INFO]
>
>**예:**  다음은 를 사용할 수 있는 예입니다 [!UICONTROL 설정]/[!UICONTROL 변수 가져오기(여러 개)] 모듈:
>
>* 다른 경로에서도 나중에 사용할 수 있도록 계산된 값을 저장하는 방법 이 기능은 값이 여러 모듈에서 사용되고 수식이 너무 복잡할 때 유용합니다.
>* 수식을 디버깅하려면 모듈에 사용된 수식이 올바른 결과를 나타내지 않는 경우 수식을 복사하여 [!UICONTROL 변수 설정] 관련 모듈 앞에 삽입하는 모듈입니다. 모듈 연결 해제 [!UICONTROL 변수 설정] 시나리오를 모듈 및 실행합니다. 확인 [!UICONTROL 변수 설정] 모듈의 출력, 조정 또는 단순화, 시나리오를 다시 실행한 후 문제가 해결될 때까지 계속 진행합니다.



#### [!UICONTROL 변수 가져오기]

이 모듈은 이전에 [!UICONTROL 변수 설정] 또는 [!UICONTROL 여러 변수 설정] 모듈.

이 모듈은 변수가 [!UICONTROL 변수 가져오기] 모듈이 있습니다. 유일한 요구 사항은 [!UICONTROL 도구] > [!UICONTROL 변수 설정] 또는 [!UICONTROL 도구] > [!UICONTROL 여러 변수 설정] 모듈이 먼저 실행됩니다. [!UICONTROL 도구] > [!UICONTROL 변수 가져오기] 모듈. 모듈이 실행되는 순서에 대한 자세한 내용은 [라우터 모듈 입력 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 변수 이름]</td> 
   <td> <p>모듈이 가져올 변수의 이름을 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 증분 함수]

이 모듈은 각 모듈의 작업 후 1씩 증가하는 값을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 값 재설정]</td> 
   <td> <p>모듈이 값을 증가시킬 시기를 선택합니다. </p> 
    <ul> 
     <li>[!UICONTROL 한 주기 후]</li> 
     <li>[!UICONTROL 시나리오 실행 후]</li> 
     <li>[!UICONTROL Never]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:**
>
>이 모듈의 용도 중 하나는 그룹의 사용자에게 작업, 리드, 이메일 등에 대한 &quot;라운드 로빈&quot; 할당을 구현하는 것입니다. 알고리즘에서는 그룹의 담당자를 합리적인 순서로 선택합니다. 일반적으로 목록의 맨 위에서 맨 아래로 이동합니다. 알고리즘이 목록 끝에 도달하면 그 다음 할당을 목록 맨 위의 사용자에게 제공하고 계속 목록을 아래로 지정합니다.
>
>다음 시나리오는 홀수 번호가 매겨진 시나리오 실행 후 첫 번째 수신자에게, 그리고 번호가 매겨진 시나리오 실행 후 두 번째 수신자에게 이메일을 보냅니다.
>
>![](assets/example-email-350x246.gif)
>
>1. 이 시나리오를 만들려면 다음을 수행하십시오.
>1. 모듈 설정 **[!UICONTROL 값 재설정]** 필드를 사용하지 않습니다.
>1. 홀수 값의 경로를 설정합니다. 다음과 같은 모듈러 수학 함수를 사용하여 이 경로의 필터를 설정합니다. `1`:

>
>   ![](assets/odd-350x459.png)
>
>  **참고**: 을 변경하는 것을 잊지 마십시오 [!UICONTROL 같음] 기본 연산자 [!UICONTROL 텍스트] 연산자 [!UICONTROL 숫자] 연산자를 사용할 수 있습니다.
>
>1. 다음과 같은 모듈러스 수학 함수를 사용하여 짝수 값에 대한 경로를 설정합니다 `0`:
>
>시나리오가 실행될 때마다 증분 함수가 하나 추가됩니다. 필터는 증가분을 확인하고 해당 값에 따라 작동하므로 이메일이 균일하게 배포됩니다.

#### [!UICONTROL 여러 변수 설정]

이 모듈은 경로 내의 다른 모듈에서 매핑할 수 있는 변수를 만듭니다. 변수를 [!UICONTROL 변수 가져오기] 또는 [!UICONTROL 여러 변수 가져오기] 시나리오 내의 모든 경로에 대한 모듈입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>모듈을 설정할 변수를 추가합니다.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변수 이름] </td> 
   <td>각 변수에 대해 변수 이름을 입력합니다. 이 이름은 다른 모듈의 변수를 매핑할 때 표시됩니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변수 값] </td> 
   <td>각 변수에 대해 변수 값을 입력합니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable Lifetime] </td> 
   <td> <p>변수가 유효한 기간을 선택합니다(동일한 값 유지).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: 변수는 한 주기에 유효합니다. 한 시나리오 실행의 여러 웹 후크를 받은 경우 유용합니다(더 많은 웹 후크 = 더 많은 주기). </li> 
     <li><strong>[!UICONTROL One Execution]</strong>: 변수는 하나의 시나리오 실행에 유효합니다. 한 실행에는 하나 이상의 주기가 포함될 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 변수 설정]

이 모듈은 경로 내의 다른 모듈에서 매핑할 수 있는 변수를 만듭니다. 변수를 [!UICONTROL 변수 가져오기] 또는 [!UICONTROL 여러 변수 가져오기] 시나리오 내의 모든 경로에 대한 모듈입니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 변수 이름] </td> 
   <td>변수 이름을 입력합니다. 이 이름은 다른 모듈의 변수를 매핑할 때 표시됩니다. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable Lifetime] </td> 
   <td> <p>변수가 유효한 기간을 선택합니다(동일한 값 유지).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: 변수는 한 주기에 유효합니다. 한 시나리오 실행의 여러 웹 후크를 받은 경우 유용합니다(더 많은 웹 후크 = 더 많은 주기). </li> 
     <li><strong>[!UICONTROL One Execution]</strong>: 변수는 하나의 시나리오 실행에 유효합니다. 한 실행에는 하나 이상의 주기가 포함될 수 있습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 변수 값] </td> 
   <td>변수의 값을 입력하거나 매핑합니다. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sleep]

이 모듈을 사용하면 최대 300초(5분) 동안 시나리오 흐름을 지연할 수 있습니다.

이 함수는 예를 들어 [!DNL target] 대량 SMS 또는 이메일을 보낼 때 인간의 동작을 모방하거나 서비스 서버를 로드합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Delay]</p> </td> 
   <td> <p>시나리오가 일시 중지될 시간(초)을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>장기간 동안 흐름을 일시 중지하려면 시나리오를 두 가지 시나리오로 분할하는 것이 좋습니다.
>
>* 첫 번째 시나리오에는 일시 중지 전에 부분이 포함됩니다.
>* 두 번째 시나리오에는 그 다음에 부품이 포함됩니다.
>
>첫 번째 시나리오는 현재 타임스탬프와 함께 데이터 저장소에 필요한 모든 정보를 저장하는 것으로 끝납니다. 두 번째 시나리오는 데이터 저장소에서 의도한 지연 시간보다 오래된 타임스탬프가 있는 레코드를 주기적으로 확인하고, 레코드를 검색하고, 데이터 처리를 완료하고, 데이터 저장소에서 레코드를 제거합니다.
>
>데이터 저장소에 대한 자세한 내용은 [데이터 저장소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>특정 데이터 저장소 모듈에 대한 자세한 내용은 [[!UICONTROL 데이터 저장소] 모듈](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### 누적

* [[!UICONTROL 숫자 누적]](#numeric-aggregator)
* [[!UICONTROL 테이블 누적]](#table-aggregator)
* [[!UICONTROL 텍스트 누적]](#text-aggregator)

#### [!UICONTROL 숫자 누적]

이 모듈에서 숫자 값을 검색한 다음 선택한 함수(SUM, AVG, COUNT, MAX, MIN) 중 하나를 적용하고 결과를 하나의 번들로 반환할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 소스 모듈]</p> </td> 
   <td> <p>필드를 집계할 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate 함수]</p> </td> 
   <td> <p>값을 집계하는 데 사용할 함수를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>집계된 출력을 그룹화할 표현식을 정의합니다. 이 표현식은 하나 이상의 매핑된 항목을 포함할 수 있습니다. 그런 다음 집계된 데이터는 이 표현식의 값을 사용하여 그룹으로 분리됩니다. 각 그룹은 키(평가된 표현식)와 값(집계된 값)으로 별도의 번들로 출력됩니다. 키를 후속 모듈에서 필터로 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 빈 집계 후 처리 중지]</td> 
   <td>결과가 없는 경우 시나리오를 중지하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Value]</p> </td> 
   <td> <p>집계할 값을 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 테이블 누적]

이 모듈은 받은 번들의 선택한 필드의 값을 지정된 열 및 행 구분 기호를 사용하여 단일 번들로 병합합니다(테이블을 만들 수 있음).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 소스 모듈]</p> </td> 
   <td> <p>필드를 집계할 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 집계된 필드]</td> 
   <td> <p> 하나의 번들에 집계할 값이 들어 있는 위에서 선택한 모듈에서 필드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 열 구분 기호]</p> </td> 
   <td> <p>결과 번들의 필드 값 열을 분리할 구분 기호 유형을 선택하거나 입력합니다. [!UICONTROL Other]를 선택하는 경우 값을 구분 기호로 구분하는 데 사용할 문자를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 행 구분 기호]</p> </td> 
   <td> <p>결과 번들의 필드 값 행을 구분하는 구분 기호 유형을 선택하거나 입력합니다. [!UICONTROL Other]를 선택하는 경우 값을 구분 기호로 구분하는 데 사용할 문자를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>집계된 출력을 그룹화할 표현식을 정의합니다. 이 표현식은 하나 이상의 매핑된 항목을 포함할 수 있습니다. 그런 다음 집계된 데이터는 이 표현식의 값을 사용하여 그룹으로 분리됩니다. 각 그룹은 키(평가된 표현식)와 값(집계된 값)으로 별도의 번들로 출력됩니다. 키를 후속 모듈에서 필터로 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 빈 집계 후 처리 중지]</td> 
   <td>결과가 없는 경우 시나리오를 중지하려면 이 옵션을 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 텍스트 누적]

이 모듈은 수신된 번들의 선택한 필드의 값을 단일 번들로 병합합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 소스 모듈]</p> </td> 
   <td> <p>필드를 집계할 모듈을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 행 구분 기호]</p> </td> 
   <td> <p>결과 번들의 필드 값 행을 구분하는 구분 기호 유형을 선택하거나 입력합니다. [!UICONTROL Other]를 선택하는 경우 값을 구분 기호로 구분하는 데 사용할 문자를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>하나 이상의 매핑된 항목이 포함된 표현식을 정의합니다. 집계된 데이터는 같은 표현식의 값이 있는 그룹에서 분리됩니다. 각 그룹은 평가된 표현식과 집계된 텍스트가 있는 키가 포함된 별도의 번들로 출력됩니다. 이렇게 하면 키를 후속 모듈에서 필터로 사용할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> 모듈을 집계할 텍스트를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 빈 집계 후 처리 중지]</td> 
   <td>결과가 없는 경우 시나리오를 중지하려면 이 옵션을 선택합니다.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**예:** 텍스트 집계를 사용하여 더 많은 값(예: 고객 이름 또는 노트)을 단일 번들에 삽입하고 이메일 본문 또는 이메일 제목에 있는 모든 값을 포함하는 이메일을 보낼 수 있습니다.

### 트랜스포머

* [[!UICONTROL 문자열 작성]](#compose-a-string)
* [[!UICONTROL 텍스트 인코딩 변환]](#convert-the-encoding-of-the-text)
* [[!UICONTROL 스위치]](#switch)

#### [!UICONTROL 문자열 작성]

모든 값을 문자열 데이터 유형(텍스트)으로 변환합니다. 이렇게 하면 이진 데이터와 같은 매핑 시 매핑이 더 쉬워집니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p>텍스트로 변환할 데이터를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 텍스트 인코딩 변환]

입력한 입력 텍스트(또는 이진 데이터)를 선택한 인코딩으로 변환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL 입력 데이터]</p> </td> 
   <td> <p>변환할 콘텐츠를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 입력 데이터 코드 페이지]</td> 
   <td> <p>입력 데이터의 인코딩 유형을 선택합니다. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Output data codepage]</p> </td> 
   <td> <p>대상(출력) 데이터의 인코딩 유형을 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 스위치]

제공된 값 목록과 일치하는지 입력 값을 확인합니다. 결과를 기반으로 출력을 반환합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>평가할 표현식을 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 일치시키기 위해 정규 표현식 사용]</td> 
   <td> <p>정규 표현식을 사용하려면 이 옵션을 활성화하십시오. 이 모듈은 정확한 일치 항목이 아니라 정규 표현식을 기반으로 사례를 결정합니다.</p> 
    <div> 
     <p>정규 표현식은 각 문자가 메타문자이거나, 특별한 의미를 가지거나, 리터럴 의미가 있는 정규 문자인 일련의 문자입니다. 이러한 문자 및 메타문자는 텍스트를 검색하는 데 사용할 수 있는 패턴을 식별합니다. 예를 들어 이름을 검색하려는 경우 대문자로 시작하는 두 개의 연속된 단어로 구성된 패턴을 검색하도록 정규 표현식을 설정할 수 있습니다. 정규 표현식은 텍스트를 검색하고 조작하는 강력한 도구입니다.</p> 
     <p>정규 표현식의 논의는 이 기사의 범위를 벗어난다. 다음 리소스를 권장합니다.</p> 
     <ul> 
      <li>메타문자 전체 목록은 다음을 참조하십시오. <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">정규 표현식</a> mdn 웹 문서</li> 
      <li>정규 표현식을 만드는 방법에 대한 자습서는 다음과 같습니다 <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>정규 표현식을 테스트하려면 <a href="https://regex101.com/">정규 표현식 101</a> 웹 사이트입니다. 왼쪽 패널에서 ECMAScript(JavaScript) FLAVOR를 선택합니다.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cases] </td> 
   <td> <p>입력에 [!UICONTROL Pattern] 필드에 입력한 값이 포함되어 있으면 [!UICONTROL Output] 필드에 입력한 값이 반환됩니다.</p> <p>입력이 [!UICONTROL Pattern] 필드에 설정한 값과 일치하지 않으면 다음 중 하나가 발생합니다.</p> 
    <ul> 
     <li>[!UICONTROL Else] 필드의 값이 반환됩니다</li> 
     <li>[!UICONTROL Else] 필드에 값이 없으면 출력이 반환되지 않습니다.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>사례 필드에 설정된 기준이 충족되지 않을 때 반환되는 값을 입력합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
