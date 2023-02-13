---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion의 날짜 및 시간 함수
description: Adobe Workfront Fusion 매핑 패널에서 다음 날짜 및 시간 기능을 사용할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 76c63afc-4bb6-4895-9bba-6b3913ecbcf6
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '1867'
ht-degree: 1%

---

# 의 날짜 및 시간 함수 [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p><p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL formatDate (날짜; 형식; [시간대])]

다음과 같은 날짜 값이 있는 경우 이 함수를 사용하십시오. `12-10-2021 20:30`과 같이 텍스트 값으로 서식을 지정할 수 있습니다. `Dec 10, 2021 8:30 PM`.

예를 들어 동일한 시나리오에서 한 앱 또는 웹 서비스의 날짜 형식을 연결된 앱 또는 웹 서비스의 날짜 형식으로 변경해야 하는 경우 유용합니다.

자세한 내용은 [날짜](../../workfront-fusion/mapping/item-data-types.md#date) 및 [텍스트](../../workfront-fusion/mapping/item-data-types.md#text) 기사 [Adobe Workfront Fusion의 항목 데이터 유형](../../workfront-fusion/mapping/item-data-types.md).

### 매개변수

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>매개변수</th> 
   <th>필요한 데이터 유형* </th> 
   <th>기능</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 날짜] </td> 
   <td>일자 </td> 
   <td> <p>날짜 값을 텍스트 값으로 변환합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL format] </td> 
   <td>텍스트 </td> 
   <td> <p>날짜/시간 형식 토큰을 사용하여 형식을 지정할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">의 날짜 및 시간 형식에 대한 토큰 [!DNL Adobe Workfront Fusion]</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL timezone] </td> 
   <td>텍스트 </td> 
   <td> <p>(선택 사항) 전환에 사용되는 시간대를 지정할 수 있도록 해줍니다. </p> <p>인식된 시간대의 목록을 보려면 위키백과의 "TZ 데이터베이스 이름" 열을 참조하십시오 <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">tz 데이터베이스 시간대 목록</a>. 이 열에 나열된 값만 함수에 의해 유효한 시간대로 인식됩니다. 다른 값은 무시되며 프로필에 지정된 시나리오 시간대가 대신 사용됩니다. 자세한 내용은 문서의 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">에서 프로필 설정 변경 [!DNL Adobe Workfront Fusion]</a>.</p> <p>이 매개 변수를 생략하면 프로필 설정에 지정된 시나리오 시간대가 적용됩니다. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

다른 유형을 제공하면 형식 강제 적용이 적용됩니다. 자세한 내용은 [형식 강제 적용 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### 반환 값 및 유형

다음 `formatDate` 함수는 지정된 형식 및 시간대에 따라 지정된 날짜 값의 텍스트 표현을 반환합니다. 데이터 유형은 텍스트입니다.

>[!INFO]
>
>**예:** 시나리오와 웹 시간대 가 모두 `Europe/Prague` 를 참조하십시오.
>
>![](assets/date&time-functions-examples-350x61.png)
>
>* `formatDate(1. Date created;MM/DD/YYYY)`
   >
   >    10/01/2018 반환
>
>* `formatDate(1. Date created; YYYY-MM-DD hh:mm A)`
   >
   >   오전 2018-10-01 09:32를 반환합니다
>
>* `formatDate(1. Date created;DD.MM.YYYY HH:mm;UTC)`
   >
   >    01.10.2018 07:32를 반환합니다.
>
>* `formatDate(now;DD.MM.YYYY HH:mm)`
   >
   >    19.03.2019 15:30을 반환합니다.


## [!UICONTROL parseDate(text; 형식; [시간대])]

날짜를 나타내는 텍스트 값이 있는 경우(예: `12-10-2019 20:30` 또는 `Aug 18, 2019 10:00 AM`)을 날짜 값(이진 머신 판독 가능한 표현)으로 변환(구문 분석)하려고 합니다. 자세한 내용은 [날짜](../../workfront-fusion/mapping/item-data-types.md#date) 및 [텍스트](../../workfront-fusion/mapping/item-data-types.md#text) 기사 [의 항목 데이터 유형 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

### 매개변수

두 번째 열은 예상 유형을 나타냅니다. 다른 유형을 제공하면 형식 강제 적용이 적용됩니다. 자세한 내용은 [형식 강제 적용 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>매개변수</th> 
   <th>필요한 데이터 유형* </th> 
   <th>기능</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL text] </td> 
   <td>텍스트 </td> 
   <td> <p>날짜 값을 텍스트 값으로 변환합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL format] </td> 
   <td>텍스트 </td> 
   <td> <p>날짜/시간 형식 토큰을 사용하여 형식을 지정할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md" class="MCXref xref">Adobe Workfront Fusion의 날짜 및 시간 형식에 대한 토큰</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>DD.MM.YYYY HH:mm</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL timezone] </td> 
   <td>텍스트 </td> 
   <td> <p>(선택 사항) 전환에 사용되는 시간대를 지정할 수 있도록 해줍니다. </p> <p>인식된 시간대의 목록을 보려면 위키백과의 "TZ 데이터베이스 이름" 열을 참조하십시오 <a href="https://en.wikipedia.org/wiki/List_of_tz_database_time_zones">tz 데이터베이스 시간대 목록</a>. 이 열에 나열된 값만 함수에 의해 유효한 시간대로 인식됩니다. 다른 값은 무시되며 프로필에 지정된 시나리오 시간대가 대신 사용됩니다. 자세한 내용은 문서의 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Adobe Workfront Fusion에서 프로필 설정 변경</a>.</p> <p>이 매개 변수를 생략하면 프로필 설정에 지정된 시나리오 시간대가 적용됩니다.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>예: </b></span></span><code>Europe/Prague</code>, <code>UTC</code></p> </td> 
  </tr> 
 </tbody> 
</table>

다른 유형을 제공하면 형식 강제 적용이 적용됩니다. 자세한 내용은 [형식 강제 적용 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

### 반환 값 및 유형

이 함수는 지정하는 형식 및 시간대에 따라 텍스트 문자열을 날짜로 변환합니다. 값의 데이터 유형은 날짜입니다.

>[!INFO]
>
>**예:** 다음 예에서 반환된 날짜 값은 ISO 8601에 따라 표시되지만 결과의 데이터 유형은 날짜입니다.
>
>* `parseDate(2016-12-28;YYYY-MM-DD)`
   >
   >    2016-12-28T00 반환:00:00.00Z
>
>* `parseDate(2016-12-28 16:03;YYYY-MM-DD HH:mm)`
   >
   >    2016-12-28T16 반환:03:00.00Z
>
>* `parseDate(2016-12-28 04:03 pm; YYYY-MM-DD hh:mm a)`
   >
   >    2016-12-28T16 반환:03:06.00Z
>
>* `parseDate(1482940986;X)`
>
>  2016-12-28T16 반환:03:06.00Z

## [!UICONTROL addDays(날짜; number)] {#adddays-date-number}

날짜에 주어진 일수를 추가한 결과로 새 날짜를 반환합니다. 일수를 빼려면 음수를 입력합니다.

>[!INFO]
>
>**예:**
>
>* `addDays(2016-12-08T15:55:57.536Z;2)`
   >
   >    2016-12-10T15 반환:55:57.536Z
>
>* `addDays(2016-12-08T15:55:57.536Z;-2)`
   >
   >    2016-12-6T15 반환:55:57.536Z


## [!UICONTROL addHours (date; number)] {#addhours-date-number}

날짜에 주어진 시간 수를 추가한 결과 새 날짜를 반환합니다. 시간을 빼려면 음수를 입력합니다.

>[!INFO]
>
>**예:**
>
>* `addHours(2016-12-08T15:55:57.536Z; 2)`
   >
   >    2016-12-08T17 반환:55:57.536Z
>
>* `addHours(2016-12-08T15:55:57.536Z;-2)`
   >
   >    2016-12-08T13 반환:55:57.536Z


## [!UICONTROL addMinutes(날짜; number)] {#addminutes-date-number}

날짜에 주어진 시간(분)을 추가한 결과 새 날짜를 반환합니다. 분을 빼려면 음수를 입력합니다.

>[!INFO]
>
>**예:**
>
>* `addMinutes(2016-12-08T15:55:57.536Z;2)`
   >
   >    2016-12-08T15 반환:57:57.536Z
>
>* `addMinutes(2016-12-08T15:55:57.536Z;-2)`
   >
   >    2016-12-08T15 반환:53:57.536Z


## [!UICONTROL addMonths (date; number)] {#addseconds-date-number}

날짜에 주어진 개월 수를 추가한 결과 새 날짜를 반환합니다. 월을 빼려면 음수를 입력합니다.

>[!INFO]
>
>**예:**
>
>* `addMonths(2016-08-08T15:55:57.536Z;2)`
   >
   >    2016-10-08T15 반환:55:57.536Z
>
>* `addMonths(2016-08-08T15:55:57.536Z;-2)`
   >
   >    2016-06-08T15 반환:55:57.536Z


## [!UICONTROL addSeconds (date; number)]

날짜에 주어진 시간(초)을 추가한 결과 새 날짜를 반환합니다. 초를 빼려면 음수를 입력합니다.

>[!INFO]
>
>**예:**
>
>* `addSeconds(2016-12-08T15:55:57.536Z;2)`
   >
   >   2016-12-08T15 반환:55:59.536Z
>
>* `addSeconds(2016-12-08T15:55:57.536Z;-2)`
   >
   >   2016-12-08T15 반환:55:55.536Z


## [!UICONTROL addYears(날짜; number)]

날짜에 주어진 연도 수를 추가한 결과 새 날짜를 반환합니다. 연도를 빼려면 음수를 입력합니다.

>[!INFO]
>
>**예:**
>
>* `addYears(2016-08-08T15:55:57.536Z;2)`
   >
   >    2018-08-08T15 반환:55:57.536Z
>
>* `addYears(2016-12-08T15:55:57.536Z; -2)`
   >
   >    2014-08-08T15 반환:55:57.536Z


## [!UICONTROL setSecond(날짜; number)]

이 함수는 매개 변수에 지정된 초 수를 사용하여 새 날짜를 반환합니다.

0에서 59까지의 숫자를 지정합니다. 숫자가 해당 범위를 벗어나는 경우 함수는 이전 분(음수) 또는 후속 분(양수)(에서)에서 두 번째 를 반환합니다.

범위 밖의 숫자를 지정해야 하는 경우에는 다음을 사용하는 것이 좋습니다[!UICONTROL  addSeconds]섹션에 설명된 대로 [addSeconds (date; number)](#addseconds-date-number).

>[!INFO]
>
>**예:**
>
>* `setSecond(2015-10-07T11:36:39.138Z;10)`
   >
   >    2015-10-07T11 반환:36:10.138Z
>
>* `setSecond(2015-10-07T11:36:39.138Z; 6)`
   >
   >    2015-10-07T11 반환:37:01.138Z


## [!UICONTROL setMinute(날짜; number)]

이 함수는 매개 변수에 지정된 분이 있는 새 날짜를 반환합니다.

0에서 59까지의 숫자를 지정합니다. 숫자가 해당 범위를 벗어나는 경우 함수는 이전 시간(음수) 또는 후속 시간(양수)에서 1분을 반환합니다.

범위 밖의 숫자를 지정해야 하는 경우에는, 위에 설명된 대로 addMinutes를 사용하는 것이 좋습니다. [addMinutes(날짜; number)](#addminutes-date-number).

>[!INFO]
>
>**예:**
>
>* `setMinute(2015-10-07T11:36:39.138Z;10)`
   >
   >    2015-10-07T11 반환:10:39.138Z
>
>* `setMinute(2015-10-07T11:36:39.138Z;61)`
   >
   >    2015-10-07T12 반환:01:39.138Z


## [!UICONTROL setHour (날짜; number)]

이 함수는 매개 변수에 지정된 시간이 있는 새 날짜를 반환합니다.

0에서 23까지의 숫자를 지정합니다. 숫자가 이 범위를 벗어나는 경우 함수는 이전 날짜로부터 1시간(음수) 또는 다음 날(양수의 경우)을 반환합니다.

범위 밖의 숫자를 지정해야 하는 경우에는 다음에 설명된 대로 addHours를 사용하는 것이 좋습니다. [addHours (date; number)](#addhours-date-number).

>[!INFO]
>
>**예:**
>
>* `setHour(2015-08-07T11:36:39.138Z;6)`
   >
   >   2015-08-07T06 반환:36:39.138Z
>
>* `setHour(2015-08-07T11:36:39.138;-6)`
   >
   >    2015-08-06T18 반환:36:39.138Z


## [!UICONTROL setDay(날짜; 날짜 번호/이름(영어)]

이 함수는 매개 변수에 지정된 날짜를 사용하여 새 날짜를 반환합니다.

이 함수를 사용하여 요일을 1일로 설정하고 일요일은 7로 설정할 수 있습니다. 1에서 7까지의 숫자를 지정하는 경우, 결과 날짜는 현재(일요일부터 토요일) 주 내에 있습니다. 숫자가 해당 범위를 벗어나는 경우 함수는 이전 주(음수의 경우) 또는 다음 주(양수의 경우)의 일을 반환합니다.

범위 밖의 숫자를 지정해야 하는 경우에는, 위에 설명된 대로 addDays를 사용하는 것이 좋습니다. [addDays(날짜; number)](#adddays-date-number).

>[!INFO]
>
>**예:**
>
>* `setDay(2018-06-27T11:36:39.138Z;Monday)`
   >
   >   2018-06-25T11 반환:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;1)`
   >
   >   2018-06-24T11 반환:36:39.138Z
>
>* `setDay(2018-06-27T11:36:39.138Z;7)`
   >
   >   2018-06-30T11 반환:36:39.138Z


## [!UICONTROL setDate (날짜; number)]

이 함수는 매개 변수에 지정된 월의 날짜가 있는 새 날짜를 반환합니다.

1부터 31까지의 숫자를 지정합니다. 숫자가 이 범위를 벗어나는 경우 함수는 이전 월의 일(음수 경우) 또는 다음 달(양수 경우)을 반환합니다.

>[!INFO]
>
>**예:**
>
>* `setDate(2015-08-07T11:36:39.138Z;5)`
   >
   >   2015-08-05T11 반환:36:39.138Z
>
>* `setDate(2015-08-07T11:36:39.138Z;32)`
   >
   >   2015-09-01T11 반환:36:39.138Z


## [!UICONTROL setMonth (날짜; 월 번호/이름(영어)]

이 함수는 매개 변수에 지정된 월을 사용하여 새 날짜를 반환합니다.

1부터 12까지의 숫자를 지정합니다. 숫자가 이 범위를 벗어나는 경우 함수는 이전 연도의 월(음수) 또는 다음 연도(양수) 를 반환합니다.

>[!INFO]
>
>**예:**
>
>* `setMonth(2015-08-07T11:36:39.138Z;5)`
   >
   >   2015-05-07T11 반환:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;17)`
   >
   >   2016-05-07T11 반환:36:39.138Z
>
>* `setMonth(2015-08-07T11:36:39.138Z;january)`
   >
   >   2015-01-07T12 반환:36:39.138Z


## [!UICONTROL setYear(날짜) number)]

매개 변수에 지정된 연도를 사용하여 새 날짜를 반환합니다.

>[!INFO]
>
>**예:**
>
>* `setYear(2015-08-07T11:36:39.138Z;2017)`
   >
   >   2017-08-07T11 반환:36:39.138Z


## [!UICONTROL dateDifference (날짜1; 날짜2; Unit)]

지정된 단위로 표시된 두 날짜의 차이를 나타내는 숫자를 반환합니다.

날짜2는 일자1에서 제외됩니다.

다음 시간 값 중 하나를 `unit` 매개 변수:

* 밀리초
* 초
* 분
* 시간
* 일
* 주
* 개월

단위를 지정하지 않으면 함수는 차이를 밀리초 단위로 반환합니다.

>[!INFO]
>
>**예:**
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z)`
   >
   >    반환 `600,000`
>
>* `dateDifference(2021-05-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;hours)`
   >
   >    반환 `4`
>
>* `dateDifference2021-06-11T18:10:00.000Z;2021-05-11T18:00:00.000Z;months)`
   >
   >    반환 `1`


## 추가 예

### 월의 n일 계산 방법

이 섹션은 [!DNL Workfront Fusion] 에서 [!DNL Exceljet] 한 달에 n번째 요일을 가져오는 방법을 설명하는 웹 페이지입니다.

월의 n번째 요일(예: 첫 번째 화요일, 세 번째 금요일 등)에 해당하는 날짜를 계산해야 하는 경우 다음 공식을 사용할 수 있습니다.

![](assets/date&time-functions-calc-nth-day-350x31.png)

```
{{addDays(setDate(1.date; 1); 1.n * 7 - formatDate(addDays(setDate(1.date; 1); "-" + 1.dow); "E"))}}
```

수식은 다음 항목을 포함합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>1.n</code> </td> 
   <td> <p> n일:</p> 
    <ul> 
     <li><code>1</code> 첫 번째 화요일에</li> 
     <li><code>2</code> 2일 화요일</li> 
     <li><code>3</code> 3일 화요일 등이요</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>2.dow</code> </td> 
   <td> <p> 요일:</p> 
    <ul> 
     <li><code>1</code> - 월요일</li> 
     <li><code>2</code> - 화요일</li> 
     <li><code>3</code> - 수요일</li> 
     <li><code>4</code> - 목요일</li> 
     <li><code>5</code> 금요일</li> 
     <li><code>6</code> - 토요일</li> 
     <li><code>7</code> - 일요일</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><code>1.date</code> </td> 
   <td> <p> 날짜는 월을 결정합니다. 이번 달에 n번째 요일을 계산하려면 <code>now</code> 변수를 채우는 방법을 설명합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

예를 들어, 한 개의 특정 사례만 계산하려는 경우(예: 매 수요일) 해당 항목을 바꿀 수 있습니다 `1.n` 및 `2.dow` 를 입력합니다. 이번 달의 두 번째 수요일에는 다음 값을 사용합니다.

* `1.n` = `2`
* `1.dow` = `3`
* `1.date` = `now`

![](assets/nth-day-variable-value-350x33.png)

### 설명:

* `setDate(now;1)` 현재 월의 첫 번째 반환
* `formatDate(....;E)` 요일 반환(1, 2, ... 6)

## 날짜 사이의 일 수를 계산하는 방법

다음 표현식을 사용할 수도 있습니다.

![](assets/calculate-days-between-dates-350x68.png)

```
{{round((2.value - 1.value) / 1000 / 60 / 60 / 24)}}
```

>[!NOTE]
>
>* 값 `D1`및 `D2` 날짜 유형 값이어야 합니다. 문자열 유형 값(예: 20.10.2018)인 경우 `parseDate()` 함수를 날짜 유형 값으로 변환하는 데 사용됩니다.
>
>* 다음 `round()` 함수는 날짜 중 하나가 일광 절약 시간제 내에 있고 다른 날짜가 없는 경우에 사용됩니다. 이러한 경우 시간 차이는 1시간 미만입니다. 정수가 아닌 결과를 위해 24로 나눌 수 있습니다. 1시간 일광 절약 시간제가 빠집니다. 비율을 갖지 않도록 라운드플레이트를 실행합니다


### 월의 마지막 일/밀리초를 계산하는 방법

날짜 범위(예: 검색 모듈에서)를 지정할 때 범위가 전체 이전 월에 닫힌 간격(해당 제한 지점을 모두 포함하는 간격)으로 지정된 경우 해당 월의 마지막 날을 계산해야 합니다.

2019-09-01 ≤ D ≤ 2019-09-30

아래 공식은 이전 월의 마지막 날을 계산하는 한 가지 방법을 보여줍니다.

![](assets/last-day-prev-month.png)

```
{{addDays(setDate(now; 1); -1)}}
```

어떤 경우에는 달의 마지막 날뿐만 아니라 말 그대로 마지막 밀리초를 계산해야 합니다.

2019-09-01T00:00:00.000Z ≤ D ≤ 2019-09-30T23:59:59.99Z

이 수식은 이전 달의 마지막 밀리초를 계산하는 방법을 보여 줍니다.

![](assets/last-millisecond-prev-month-350x45.png)

```
{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD"; "UTC") - 1; "x")}}
```

표준 시간대 설정을 사용하는 결과가 필요한 경우 UTC 인수를 생략하십시오.

![](assets/omit-utc-argument-350x45.png)

`{{parseDate(parseDate(formatDate(now; "YYYYMM01"); "YYYYMMDD") - 1; "x")}}`

그러나 다음과 같이 &quot;less or equal&quot; 연산자 대신 &quot;less than&quot; 연산자를 &quot;less than&quot;으로 바꾸면서, 대신 절반-열린 간격(제한 점 중 하나를 제외하는 간격)을 사용하는 것이 좋습니다.

`2019-09-01 ≤ D < 2019-10-01`

`2019-09-01T00:00:00.000Z ≤ D < 2019-10-01T00:00:00.000Z`
