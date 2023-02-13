---
content-type: api
navigation-topic: api-navigation-topic
title: API 응답에서 이스케이프 처리된 문자
description: API 응답에서 이스케이프 처리된 문자
author: John
feature: Workfront API
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 8%

---

# API 응답에서 이스케이프 처리된 문자

일부 API 응답 구문에는 이스케이프 문자가 포함될 수 있습니다. `\` (백슬래시). 이스케이프 문자는 이스케이프 처리된 문자 바로 뒤에 오는 문자 또는 문자열에 특수 값이 있음을 나타냅니다. 예, `\t` 는 읽기 장치에 `t` 는 `tab` &quot;t&quot;가 아니라 백슬래시 다음에 나오는 하나 이상의 문자 문자열을 이스케이프 시퀀스라고 합니다.

16진수 이스케이프 처리된 시퀀스는 유효한 16진수를 사용해야 합니다. 다음 표에는 Adobe Workfront API 응답으로 인코딩된 이스케이프 시퀀스가 나와 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>이스케이프 시퀀스</strong> </th> 
   <th><strong>유니코드 문자</strong> </th> 
   <th><strong>를 나타냅니다</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>위치, <em>x</em> 0에서 7까지의 숫자에 대한 16진수 코드입니다</p> </td> 
   <td>0-7</td> 
   <td>코드 포인트 0에서 7까지로 표시되는 유니코드 문자</td> 
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
   <td> <p>\u00<em>xx</em></p> <p><em>여기서 xx는 14~31의 16진수 코드입니다</em> </p> </td> 
   <td>14 - 31</td> 
   <td>코드 점으로 표시되는 유니코드 문자 14~31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (슬래시)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (보다 작음)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (슬래시)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>위치, <em>xxxx</em> 127을 초과하는 수에 대한 16진수 코드입니다</p> </td> 
   <td>128+</td> 
   <td>127을 초과하는 코드 포인트에 대한 유니코드 문자</td> 
  </tr> 
 </tbody> 
</table>
