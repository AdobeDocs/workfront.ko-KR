---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Adobe Workfront Fusion에서 문자 강제 변환
description: 이 문서에서는 다음 방법을 설명합니다 [!DNL Adobe Workfront Fusion] 는 예상 및 예기치 않은 데이터 형식의 값을 받을 때 작동합니다.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# 형식 강제 변환 [!DNL Adobe Workfront Fusion]

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

### 문자 강제 변환

이 문서에서는 다음 방법을 설명합니다 [!DNL Adobe Workfront Fusion] 는 예상 및 예기치 않은 데이터 형식의 값을 받을 때 작동합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>예상</th> 
   <th>수신됨</th> 
   <th> <p>설명</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>배열 </td> 
   <td>배열 </td> 
   <td> <p>값은 변경되지 않은 상태로 전달됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>배열 </td> 
   <td>기타 </td> 
   <td> <p>수신된 값이 배열 유형이 아닌 경우 [!DNL Workfront Fusion] 는 배열을 만들며 첫 번째(및 유일한) 요소는 받은 값이 됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>부울 </td> 
   <td>부울 </td> 
   <td> <p>값은 변경되지 않은 상태로 전달됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>부울 </td> 
   <td>숫자 </td> 
   <td> <p>값이 0인 경우에도 값이 논리적 Yes로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>부울 </td> 
   <td>텍스트 </td> 
   <td> <p>값이 false이거나 값이 비어 있으면 논리 No로 변환됩니다. 그렇지 않으면 논리적 Yes로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>부울 </td> 
   <td>기타 </td> 
   <td> <p>수신된 값이 존재할 때마다(null이 아님) 값이 논리적 Yes로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>버퍼 </td> 
   <td>버퍼 </td> 
   <td> <p>값은 코드 페이지가 예상대로 수행될 경우에만 변경되지 않고 전달됩니다. 코드 페이지가 다른 경우 [!DNL Workfront Fusion] 은(는) 수신된 값을 요청된 코드 페이지로 전환하려고 합니다. 이 전환이 지원되지 않는 경우 [!DNL Workfront Fusion] 은 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>버퍼 </td> 
   <td>부울 </td> 
   <td> <p>이 값은 텍스트(true/false)로 변환된 다음 텍스트로 변환하기 위해 위에 언급된 단계에 따라 이진 데이터로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>버퍼 </td> 
   <td>날짜 </td> 
   <td> <p>이 값은 ISO 8601 텍스트로 변환된 다음 텍스트로 변환하는 데 언급된 단계에 따라 이진 데이터로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>버퍼 </td> 
   <td>숫자 </td> 
   <td> <p>이 값은 텍스트로 변환하는 데 위에서 언급한 단계에 따라 텍스트로 변환된 다음 이진 데이터로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>버퍼 </td> 
   <td>텍스트 </td> 
   <td> <p>값이 이진 데이터로 변환되고 예상대로 인코딩됩니다. 필요한 인코딩을 지정하지 않으면 utf8 인코딩이 사용됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>버퍼 </td> 
   <td>기타 </td> 
   <td> <p>[!DNL Workfront Fusion] 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 </td> 
   <td>컬렉션 </td> 
   <td> <p>값은 변경되지 않은 상태로 전달됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>컬렉션 </td> 
   <td>기타 </td> 
   <td> <p>[!DNL Workfront Fusion] 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>날짜 </td> 
   <td>날짜 </td> 
   <td> <p>값은 변경되지 않은 상태로 전달됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>날짜 </td> 
   <td>텍스트 </td> 
   <td> <p>[!DNL Workfront Fusion] 는 텍스트를 날짜로 변환하려고 합니다. 전환이 실패하면 유효성 검사 오류를 반환합니다. 날짜에는 일, 월 및 연도가 포함되어야 합니다. 날짜에는 시간과 시간대가 포함될 수 있습니다. 기본 시간대는 설정을 기반으로 합니다. 예:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>날짜 </td> 
   <td>기타 </td> 
   <td> <p>[!DNL Workfront Fusion] 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>숫자 </td> 
   <td>숫자 </td> 
   <td> <p>값은 변경되지 않은 상태로 전달됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>숫자 </td> 
   <td>텍스트 </td> 
   <td> <p>[!DNL Workfront Fusion] 는 텍스트를 숫자로 변환하려고 합니다. 전환이 실패하면 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>숫자 </td> 
   <td>기타 </td> 
   <td> <p>[!DNL Workfront Fusion] 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>텍스트 </td> 
   <td>텍스트 </td> 
   <td> <p>값은 변경되지 않은 상태로 전달됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>텍스트 </td> 
   <td>배열 </td> 
   <td> <p>지정된 배열이 텍스트로의 변환을 지원하는 경우 값이 변환됩니다. 그렇지 않은 경우, [!DNL Workfront Fusion] 은 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>텍스트 </td> 
   <td>부울 </td> 
   <td> <p>값이 텍스트(true/false)로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>텍스트 </td> 
   <td>버퍼 </td> 
   <td> <p>이진 데이터에 대해 텍스트 인코딩이 지정된 경우 값이 텍스트로 변환됩니다. 그렇지 않은 경우, [!DNL Workfront Fusion] 은 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>텍스트 </td> 
   <td>날짜 </td> 
   <td> <p>이 값은 ISO 8601 텍스트로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>텍스트 </td> 
   <td>숫자 </td> 
   <td> <p>값이 텍스트로 변환됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>텍스트 </td> 
   <td>기타 </td> 
   <td> <p>[!DNL Workfront Fusion] 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>시간 </td> 
   <td>시간 </td> 
   <td> <p>값은 변경되지 않은 상태로 전달됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>시간 </td> 
   <td>텍스트 </td> 
   <td> <p>[!DNL Workfront Fusion] 시간을 시간으로 전환하려고 합니다.:minutes:초 형식입니다. 전환이 실패하면 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>시간 </td> 
   <td>기타 </td> 
   <td> <p>[!DNL Workfront Fusion] 유효성 검사 오류를 반환합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
