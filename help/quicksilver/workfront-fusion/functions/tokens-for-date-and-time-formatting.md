---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: ' [!DNL Adobe Workfront Fusion]의 날짜 및 시간 형식에 대한 토큰'
description: ' [!DNL Adobe Workfront Fusion mapping]  패널에서 날짜 및 시간 형식에 대한 다음 토큰을 사용할 수 있습니다.'
author: Becky
feature: Workfront Fusion
exl-id: 19d0608e-7902-4d09-b71d-e6ae8ed7a6fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 5%

---

# [!DNL Adobe Workfront Fusion]의 날짜 및 시간 형식에 대한 토큰

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

## 년, 월, 일 토큰

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>토큰 </th> 
   <th>출력 </th> 
   <th> <p>설명</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>YY </code> </td> 
   <td><code>70 71 ... 29 30</code> </td> 
   <td> <p> 2자리 연도</p> </td> 
  </tr> 
  <tr> 
   <td><code>YYYY </code> </td> 
   <td><code>1970 1971 ... 2029 2030 </code> </td> 
   <td> <p>4자리 연도</p> </td> 
  </tr> 
  <tr> 
   <td><code>Y</code> </td> 
   <td><code>1970 1971 ... 9999 +10000 +10001</code> </td> 
   <td> <p>[!UICONTROL 연도(숫자 및 기호 포함)]</p> </td> 
  </tr> 
  <tr> 
   <td><code>Q</code> </td> 
   <td><code>1 2 3 4 </code> </td> 
   <td> <p> 사분기</p> </td> 
  </tr> 
  <tr> 
   <td><code>Qo</code> </td> 
   <td><code>1st 2nd 3rd 4th </code></td> 
   <td> <p>서수가 있는 사분기</p> </td> 
  </tr> 
  <tr> 
   <td><code>M</code> </td> 
   <td><code>1 2 ... 11 12</code></td> 
   <td> <p>월 번호</p> </td> 
  </tr> 
  <tr> 
   <td><code>Mo </code> </td> 
   <td><code>1st 2nd ... 11th 12th</code> </td> 
   <td> <p>서수가 있는 [!UICONTROL Month]</p> </td> 
  </tr> 
  <tr> 
   <td><code>MM</code> </td> 
   <td><code>01 02 ... 11 12 </code> </td> 
   <td> <p> 앞에 0이 있는 월 숫자</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMM</code> </td> 
   <td><code>Jan Feb ... Nov Dec</code></td> 
   <td> <p> 월 약어</p> </td> 
  </tr> 
  <tr> 
   <td><code>MMMM</code> </td> 
   <td><code> January February ... November December</code> </td> 
   <td> <p> 월 이름</p> </td> 
  </tr> 
  <tr> 
   <td><code>D</code> </td> 
   <td><code>1 2 ... 30 31 </code></td> 
   <td> <p>일(한 달 기준)</p> </td> 
  </tr> 
  <tr> 
   <td><code>Do</code> </td> 
   <td><code>1st 2nd ... 30th 31st</code></td> 
   <td> <p> 서수가 있는 날짜</p> </td> 
  </tr> 
  <tr> 
   <td><code>DD</code> </td> 
   <td><code>01 02 ... 30 31</code></td> 
   <td> <p> 앞에 0이 있는 날짜</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDD</code> </td> 
   <td><code>1 2 ... 364 365 </code></td> 
   <td> <p>일(한 해 기준)</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDo</code> </td> 
   <td><code>1st 2nd ... 364th 365th</code> </td> 
   <td> <p>서수가 있는 [!UICONTROL Day of year]</p> </td> 
  </tr> 
  <tr> 
   <td><code>DDDD </code> </td> 
   <td><code>001 002 ... 364 365</code> </td> 
   <td> <p> 앞에 0이 있는 요일</p> </td> 
  </tr> 
 </tbody> 
</table>

## 주 연도, 주 및 요일 토큰

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>토큰 </th> 
   <th>출력 </th> 
   <th> <p>설명</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>d</code> </td> 
   <td><code>0 1 ... 5 6 </code> </td> 
   <td> <p> 요일</p> </td> 
  </tr> 
  <tr> 
   <td><code>do</code> </td> 
   <td><code>0th 1st ... 5th 6th </code> </td> 
   <td> <p>[!UICONTROL 서수가 있는 요일]</p> </td> 
  </tr> 
  <tr> 
   <td><code>dd </code> </td> 
   <td><code>Su Mo ... Fr Sa </code> </td> 
   <td> <p>요일 약어</p> </td> 
  </tr> 
  <tr> 
   <td><code>ddd</code> </td> 
   <td><code>Sun Mon ... Fri Sat </code> </td> 
   <td> <p> 요일 약어</p> </td> 
  </tr> 
  <tr> 
   <td><code>dddd </code> </td> 
   <td><code>Sunday Monday ... Friday Saturday</code> </td> 
   <td> <p> 요일 이름</p> </td> 
  </tr> 
  <tr> 
   <td><code>E</code> </td> 
   <td><code>1 2 ... 6 7 </code> </td> 
   <td> <p> 요일(ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>w </code> </td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>주(한 해 기준)</p> </td> 
  </tr> 
  <tr> 
   <td><code>wo </code> </td> 
   <td><code>1st 2nd ... 52nd 53rd</code> </td> 
   <td> <p>[!UICONTROL 서수 포함 주]</p> </td> 
  </tr> 
  <tr> 
   <td><code>ww </code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p>선행 0이 있는 주</p> </td> 
  </tr> 
  <tr> 
   <td><code>W</code></td> 
   <td><code>1 2 ... 52 53 </code> </td> 
   <td> <p>주(ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>Wo</code> </td> 
   <td><code>1st 2nd ... 52nd 53rd </code> </td> 
   <td> <p> 서수가 있는 주(ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>WW</code> </td> 
   <td><code>01 02 ... 52 53 </code> </td> 
   <td> <p> 선행 0이 있는 주(ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>gg</code></td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>주 연도</p> </td> 
  </tr> 
  <tr> 
   <td><code>gggg </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> 주 연도</p> </td> 
  </tr> 
  <tr> 
   <td><code>GG </code> </td> 
   <td><code>70 71 ... 29 30 </code> </td> 
   <td> <p>주(ISO)</p> </td> 
  </tr> 
  <tr> 
   <td><code>GGGG </code> </td> 
   <td><code>1970 1971 ... 2029 2030</code> </td> 
   <td> <p> 주(ISO)</p> </td> 
  </tr> 
 </tbody> 
</table>

## 시간, 분, 초, 밀리초 및 오프셋 토큰

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>토큰 </p> </th> 
   <th>출력 </th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>H</code> </td> 
   <td><code>0 1 ... 22 23</code></td> 
   <td> <p>24시간</p> </td> 
  </tr> 
  <tr> 
   <td><code>HH</code> </td> 
   <td><code>00 01 ... 22 23</code></td> 
   <td> <p> 앞에 0이 있는 24시간</p> </td> 
  </tr> 
  <tr> 
   <td><code>h</code> </td> 
   <td><code>1 2 ... 11 12</code></td> 
   <td> <p> 12시간</p> </td> 
  </tr> 
  <tr> 
   <td><code>hh </code> </td> 
   <td><code>01 02 ... 11 12</code> </td> 
   <td> <p> 앞에 0이 있는 12시간</p> </td> 
  </tr> 
  <tr> 
   <td><code>k</code> </td> 
   <td><code>1 2 ... 23 24</code></td> 
   <td> <p> 24시간</p> </td> 
  </tr> 
  <tr> 
   <td><code>kk</code></td> 
   <td><code>01 02 ... 23 24</code> </td> 
   <td> <p> 앞에 0이 있는 24시간</p> </td> 
  </tr> 
  <tr> 
   <td><code>A</code></td> 
   <td><code>AM PM </code> </td> 
   <td> <p>Post 또는 ante meridiem(대문자)</p> </td> 
  </tr> 
  <tr> 
   <td><code>a</code> </td> 
   <td><code>am pm </code> </td> 
   <td> <p> Post 또는 ante meridiem(소문자)</p> </td> 
  </tr> 
  <tr> 
   <td><code>m</code> </td> 
   <td><code> 0 1 ... 58 59</code> </td> 
   <td> <p> 분</p> </td> 
  </tr> 
  <tr> 
   <td><code>mm</code> </td> 
   <td><code>00 01 ... 58 59</code> </td> 
   <td> <p>[!UICONTROL 분,] 앞에 0</p> </td> 
  </tr> 
  <tr> 
   <td><code>s</code> </td> 
   <td><code>0 1 ... 58 59</code> </td> 
   <td> <p> 초</p> </td> 
  </tr> 
  <tr> 
   <td><code>ss</code> </td> 
   <td><code>00 01 ... 58 59</code></td> 
   <td> <p>초(앞에 0이 있음)</p> </td> 
  </tr> 
  <tr> 
   <td><code>S</code> </td> 
   <td><code>0 1 ... 8 9 </code> </td> 
   <td> <p> 분수 초</p> </td> 
  </tr> 
  <tr> 
   <td><code>SS</code> </td> 
   <td><code>00 01 ... 98 99</code> </td> 
   <td> <p> 앞에 0이 있는 분수 초</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSS</code> </td> 
   <td><code>000 001 ... 998 999</code> </td> 
   <td> <p> 앞에 두 개의 0이 있는 분수 초</p> </td> 
  </tr> 
  <tr> 
   <td><code>SSSS ... SSSSSSSSS</code> </td> 
   <td><code>000[0..] 001[0..] ... 998[0..] 999[0..] </code> </td> 
   <td> <p> 분수 초</p> </td> 
  </tr> 
  <tr> 
   <td><code>Z</code> </td> 
   <td><code>-07:00 -06:00 ... +06:00 +07:00 </code></td> 
   <td> <p>시간대</p> </td> 
  </tr> 
  <tr> 
   <td><code>ZZ</code> </td> 
   <td><code>-0700 -0600 ... +0600 +0700 </code></td> 
   <td> <p>시간대</p> </td> 
  </tr> 
  <tr> 
   <td><code>X</code> </td> 
   <td><code>1360013296</code> </td> 
   <td> <p> Unix 타임스탬프</p> </td> 
  </tr> 
  <tr> 
   <td><code>x</code> </td> 
   <td><code>1360013296123</code></td> 
   <td> <p> Unix 밀리초 타임스탬프</p> </td> 
  </tr> 
 </tbody> 
</table>
