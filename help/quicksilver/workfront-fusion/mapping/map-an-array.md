---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe] Workfront Fusion에서 배열 매핑'
description: Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다. 이 문서는 더 이상 사용되지 않지만, 이 기능을 다루는 새 문서에 대한 링크를 포함합니다.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]에서 배열 매핑

>[!IMPORTANT]
>
>Adobe Workfront Fusion 설명서가 새 위치로 이동했습니다.
>
>이 문서의 정보는 이제 문서에서 찾을 수 있습니다.
>
>* [배열 또는 배열 요소 매핑](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-an-array.html)
>
>모든 책갈피를 업데이트하십시오.
>
>이 문서는 더 이상 업데이트되지 않으며 곧 제거될 예정입니다.

배열은 다음을 포함할 수 있는 특수한 유형의 항목입니다.

* 하나 이상의 텍스트 값(단순 배열)
* 동일한 유형의 컬렉션 하나 이상(복잡한 배열)

>[!INFO]
>
>**예:** [!UICONTROL 전자 메일 보기] 모듈은 모든 전자 메일에 대한 첨부 파일 배열을 반환합니다. 모든 첨부 파일은 이름, 콘텐츠, 크기 등을 포함할 수 있는 컬렉션을 나타냅니다.

자세한 내용은 [항목 데이터 형식 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)을 참조하세요.

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
   <p>레거시 라이선스 요구 사항: 작업 자동화 및 통합을 위한 [!UICONTROL [!DNL Workfront Fusion]] </p>
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



## 전체 배열 매핑

1. 배열을 매핑할 모듈에서 배열을 매핑할 필드를 클릭합니다. 배열이 매핑된 필드입니다.

1. 표시되는 상자에서 항목을 매핑합니다.

   패널을 사용하면 다른 유형의 항목과 동일한 방식으로 필드를 매핑할 수 있습니다. 각 항목을 따로 채우지 않고 다른 배열을 대상 필드에 매핑하려면 [!UICONTROL 맵] 단추를 사용합니다. 이 경우 두 배열(소스 배열과 타겟 배열)의 구조가 동일해야 합니다.

   배열에 항목을 원하는 수만큼 추가할 수 있습니다.

반복기를 사용하여 배열을 개별 번들로 나눌 수 있습니다. 자세한 내용은  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md)의 [[!UICONTROL 반복자] 모듈을 참조하십시오.

## 항목을 새 배열에 매핑

Workfront Fusion의 일부 필드를 사용하면 요소를 배열에 매핑할 수 있습니다. 예를 들어 Workfront 보드 > 체크리스트 항목 추가 모듈에서 체크리스트 항목의 배열을 만들 수 있습니다. 모듈이 실행되면 모든 체크리스트 항목이 카드에 추가됩니다.

&quot;항목 추가&quot;를 표시하는 모든 모듈 필드는 배열을 만듭니다.

![항목 추가](assets/add-item.png)

배열에 요소를 추가하려면 다음을 수행합니다.

1. **항목 추가** 클릭
1. 열리는 패널에서 항목에 대한 세부 정보를 입력합니다.
1. **추가**&#x200B;를 클릭합니다.
1. (선택 사항) 배열에 추가할 각 요소에 대해 1-3단계를 반복합니다.

## 배열 요소 매핑


### 번호별 배열 요소 매핑

배열 요소는 배열 이름 뒤에 대괄호로 숫자로 표시됩니다. 이 인덱스 번호를 사용하여 배열의 개별 요소를 필드에 매핑할 수 있습니다.

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>Workfront Fusion의 배열 인덱싱이 1부터 시작됩니다.

배열 요소를 매핑하려면 다음을 수행합니다.

1. 요소를 매핑할 필드를 클릭합니다.

   매핑 패널이 열립니다.

1. 매핑할 요소가 포함된 배열을 찾습니다.
1. 배열 옆에 있는 드롭다운 화살표를 클릭합니다.
1. 매핑할 요소를 클릭합니다.

   요소는 색인 1을 사용하여 매핑됩니다. 이렇게 하면 배열의 첫 번째 요소가 매핑됩니다.

1. 배열의 다른 요소를 매핑하려면 [1]을(를) 클릭하고 매핑할 배열 요소의 인덱스 번호를 입력하십시오.

   ![](assets/access-another-element.png)

### 지정된 키로 배열의 요소 매핑

일부 배열에는 메타데이터, 특성 등과 같은 키 값 항목이 있는 컬렉션이 포함되어 있습니다. 이러한 값 중 하나를 사용하기 위해 주어진 키 값으로 요소를 조회하고 값 항목에서 해당 값을 얻을 수 있습니다. `map()` 및 `get()` 함수의 조합을 사용하는 수식을 사용하는 것이 좋습니다.



>[!BEGINSHADEBOX]

다음 예제에서는 [!DNL Jira] 앱의 출력을 보여 줍니다.

![](assets/output-of-jira-app-350x100.png)

이 예제는 ID가 10108인 특정 첨부 파일에 대한 첨부 파일 배열에서 파일 이름을 가져옵니다.

이 예는 다음 출력을 생성합니다.

![](assets/output-from-jira-350x261.png)

공식은 다음과 같이 설명할 수 있습니다.

* `map`

   1. `map()` 함수의 첫 번째 매개 변수는 전체 배열 항목입니다.
   1. 두 번째 매개 변수는 값 항목의 원시 이름입니다. 원시 이름을 얻으려면 [!UICONTROL 매핑] 패널의 항목 위로 마우스를 가져갑니다.

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >모든 매개 변수는 대/소문자를 구분합니다. 이 특정 예에서 항목의 레이블은 대문자로만 원시 이름과 다르지만 원시 이름을 사용해야 합니다.

   1. 세 번째 매개 변수는 키 항목의 원시 이름입니다.

      ![](assets/3rd-parameter-350x166.png)

   1. 네 번째 매개 변수는 지정된 키 값입니다.

  `map()` 함수는 배열을 반환하므로(지정된 키 값을 가진 요소가 더 있을 수 있으므로) `get()` 함수를 적용하여 첫 번째 요소를 가져와야 합니다.

* `get`

   1. `get()` 함수의 첫 번째 매개 변수는 `map()` 함수의 결과입니다.

   1. 두 번째 매개 변수는 요소의 색인입니다. 이 예제에서 인덱스는 `1`입니다.

이 예는 다음 출력을 생성합니다.

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

`map()` 함수에 대한 자세한 내용은 [배열 함수](/help/quicksilver/workfront-fusion/functions/array-functions.md)를 참조하십시오.

`get()` 함수에 대한 자세한 내용은 [일반 함수](/help/quicksilver/workfront-fusion/functions/general-functions.md)를 참조하십시오.

## 배열 요소를 일련의 번들로 변환

배열은 [!UICONTROL 반복자] 모듈을 사용하여 일련의 번들로 변환할 수 있습니다. 자세한 내용은 [[!UICONTROL 반복자] 모듈](/help/quicksilver/workfront-fusion/modules/iterator-module.md)을 참조하세요.

![](assets/series-of-bundles.png)

