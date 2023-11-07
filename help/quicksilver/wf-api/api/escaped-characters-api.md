---
content-type: api
navigation-topic: api-navigation-topic
title: API 응답에서 이스케이프 처리된 문자
description: API 응답에서 이스케이프 처리된 문자
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# API 응답에서 이스케이프 처리된 문자

일부 API 응답의 구문은 이스케이프 문자를 포함할 수 있습니다. `\` (백슬래시). 이스케이프 문자는 이스케이프 처리된 문자 바로 뒤에 오는 문자 또는 문자열에 특수 값이 있음을 나타냅니다. 예를 들어, `\t` 읽기 장치에 다음 사항을 알려줍니다. `t` 은(는) 다음과 같이 해석해야 합니다. `tab` &quot;t&quot;라는 글자로서가 아닙니다. 백슬래시 다음에 오는 하나 이상의 문자로 이루어진 문자열을 이스케이프 시퀀스라고 합니다.

16진수 이스케이프 처리된 시퀀스에는 유효한 16진수를 사용해야 합니다. 다음 표에는 Adobe Workfront API 응답으로 인코딩된 이스케이프 시퀀스가 나열되어 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>시퀀스 이스케이프 처리</strong> </th> 
   <th><strong>유니코드 문자</strong> </th> 
   <th><strong>표시</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>위치, <em>x</em> 는 0에서 7 사이의 16진수 코드입니다</p> </td> 
   <td>0-7</td> 
   <td>코드 포인트 0에서 7 사이의 유니코드 문자</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>백스페이스</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>탭</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>새 줄</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>세로 탭</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>양식 피드</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>캐리지 리턴</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>여기서 xx는 14에서 31 사이의 16진수 코드입니다</em> </p> </td> 
   <td>14 - 31</td> 
   <td>코드 포인트 14 - 31로 표시되는 유니코드 문자</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (슬래시)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt;(보다 작음)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (백슬래시)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>위치, <em>xxxx</em> 는 127을 초과하는 숫자에 대한 16진수 코드입니다.</p> </td> 
   <td>128+</td> 
   <td>127 이상의 모든 코드 포인트에 대한 유니코드 문자</td> 
  </tr> 
 </tbody> 
</table>
