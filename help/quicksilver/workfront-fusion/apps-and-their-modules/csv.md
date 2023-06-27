---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Adobe Workfront Fusion CSV 모듈을 사용하면 CSV 파일을 만들고 수신된 텍스트 값 또는 파일에서 CSV 텍스트를 구문 분석할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 1%

---

# CSV

다음 [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] 모듈을 사용하면 CSV 파일을 만들고 수신된 텍스트 값 또는 파일에서 CSV 텍스트를 구문 분석할 수 있습니다.

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
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재 라이선스 요구 사항: 아니요 [!DNL Workfront Fusion] 라이센스 요구 사항.</p>
   <p>또는</p>
   <p>기존 라이선스 요구 사항: [!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합용], [!UICONTROL [!DNL Workfront Fusion] 작업 자동화용]</p>
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

## [!UICONTROL CSV 만들기]

다음 [!UICONTROL CSV 만들기] 집계기를 사용하면 수신된 텍스트 값에서 csv 텍스트를 만들 수 있습니다.

집계자에 대한 자세한 내용은 [의 집계 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 소스 모듈]</td>
        <td>필요한 필드를 집계하기 위해 사용 중인 모듈을 선택합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 집계된 필드]</td>
        <td>사용 가능한 필드 목록에서 집계할 필드를 선택합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 첫 번째 행에 헤더 포함]</td>
        <td>결과에 헤더를 포함하려면 이 옵션을 선택합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>결과를 그룹화할 필터를 입력합니다. 예를 들어 날짜를 입력합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 빈 집계 후 처리 중지]</td>
        <td>결과가 없을 때 시나리오를 중지하려면 이 옵션을 선택합니다.</td>
    </tr>
</table>

## [!UICONTROL CSV 만들기(고급)]

다음 [!UICONTROL CSV 만들기(고급)] 집계기를 사용하면 수신된 텍스트 값에서 CSV 텍스트를 만들 수 있습니다. 결과 CSV 파일의 CSV 열을 정의하는 데이터 구조를 사용합니다. 정의된 열은 CSV 모듈 설정에서 필드로 표시되며, 시나리오의 이후 모듈에 매핑될 수 있습니다.

집계자에 대한 자세한 내용은 [의 집계 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 모듈]</td> 
   <td>필요한 필드를 집계하기 위해 사용 중인 앱 모듈을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>원하는 방식으로 필드를 집계할 데이터 구조를 선택합니다. 데이터 구조를 정의한 후 해당 필드에 항목을 매핑할 수 있습니다.</p> <p>자세한 내용은 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">의 데이터 구조 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 첫 번째 행에 헤더 포함] </td> 
   <td>결과에 헤더를 포함하려면 이 옵션을 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>결과를 그룹화할 필터를 입력합니다. 예를 들어 날짜를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 빈 집계 후 처리 중지] </td> 
   <td>결과가 없을 때 시나리오를 중지하려면 이 옵션을 선택합니다. </td> 
  </tr> 
 </tbody> 
</table>


<p>Google 연락처를 두 개의 열 "전체 이름" 및 "이메일"이 있는 CSV 파일로 내보내려고 한다고 가정합니다. [!UICONTROL Google Contacts] &gt;[!UICONTROL Get contacts from a group] 모듈의 출력 번들은 다음과 같은 구조를 갖습니다. 이메일 주소는 <code>[!UICONTROL Emails[]]</code> item: 컬렉션의 배열로서, 각 컬렉션에는 두 개의 항목이 포함됩니다. <code>Label</code> 및 <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>If you construct고용 the simple단순한 [!DNL Create CSV] 모듈에서는 번들의 최상위 항목에 해당하는 확인란 목록을 제공합니다. 확인하려는 경우 <code>Full name</code> 및 <code>Emails</code> 항목: [!UICONTROL CSV 만들기] 모듈은 사용자가 원하지 않는 다음 출력을 생성합니다.</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>항목 이후 <code>Full Name</code> 는 단순 텍스트 유형이며 내보내기가 잘 됩니다. 하지만 그 상품은 <code>Emails</code>복잡한 컬렉션 유형 배열인 는 [object Object]로 내보내집니다. 이 개체는 기본적으로 컬렉션과 배열이 텍스트로 변환되는 방식입니다. 자세한 내용은 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion의 항목 데이터 유형</a>.</p>
<p>의 콘텐츠를 내보내려면 <code>Email </code>첫 번째 컬렉션 항목 <code>Emails[]</code> 대신 [!UICONTROL CSV(고급) 만들기] 모듈을 사용해야 합니다. 모듈을 사용하면 CSV 파일의 개별 열을 정의하고 중첩된 열을 포함하여 항목을 해당 열에 매핑할 수 있습니다.</p>
<ol>
<li value="1">시나리오에 [!UICONTROL CSV 만들기(고급)] 모듈을 삽입하고 구성을 엽니다.</li>
<li value="2">다음을 클릭합니다. <strong>[!UICONTROL 추가]</strong> 새 데이터 구조를 만들려면 [!UICONTROL 데이터 구조] 필드 옆에 있는 단추를 클릭합니다.</li>
<li value="3"> <p>데이터 구조의 이름으로 쓰고 <strong>[!UICONTROL 항목 추가]</strong> 단추를 클릭하여 개별 열을 추가합니다. "전체 이름"과 "이메일", 이렇게 두 개의 열을 내보내려면 결과 데이터 구조는 다음과 같습니다.</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>데이터 구조를 정상적으로 정의하면 항목을 매핑할 수 있도록 각 개별 열에 해당하는 필드가 [!UICONTROL CSV(고급) 만들기] 모듈의 구성에 표시됩니다. 에서 첫 번째 항목 가져오기 <code>[!UICONTROL Emails[]]</code> 배열 및 해당 항목 매핑 <code>Email </code>필드/열 이메일로:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>시나리오를 실행합니다. 항목 이후 <code>Emails[1]: Email</code> "이메일" 열에 매핑되는 단순 유형이 텍스트입니다. 지금 올바르게 내보냅니다.</p> <p>"전체 이름","이메일"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL CSV 구문 분석]

다음 [!UICONTROL CSV 구문 분석] 변환기를 사용하면 수신된 텍스트 값 또는 파일에서 CSV 텍스트를 구문 분석할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 열 수]</td> 
   <td>CSV 파일의 열 수를 지정합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV에 헤더 포함]</td> 
   <td> <p>CSV 텍스트의 첫 행에 머리글이 포함된 경우 이 옵션을 선택합니다.</p> <p>참고: 모듈은 이러한 헤더를 사용하여 출력의 열에 레이블을 지정하지 않습니다. 대신 이 필드에서는 헤더가 출력 데이터에 포함되지 않도록 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>CSV 파일의 구분 기호를 선택합니다. 구분 기호는 별도의 값 또는 필드 사이의 경계를 나타내는 텍스트 문자입니다.</p> 
    <ul> 
     <li>[!UICONTROL 쉼표]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Other]</p> <p>[!UICONTROL Other]를 선택하는 경우 CSV 파일에서 값을 구분하는 데 사용하는 구분 기호를 입력합니다. 정확히 하나의 문자를 입력해야 합니다.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 인용되지 않은 필드 내에 따옴표 유지]</td> 
   <td>견적을 유지하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>구문 분석할 CSV 파일을 입력하거나 매핑합니다.<p>참고: <p>데이터가 이진 형식(일반적으로 파일에서)으로 제공되는 경우 'toString()' 함수를 사용하여 이진 데이터를 [!UICONTROL String](으)로 변환해야 합니다.</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
