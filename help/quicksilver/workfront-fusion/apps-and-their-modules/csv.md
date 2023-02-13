---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Adobe Workfront Fusion CSV 모듈을 사용하여 CSV 파일을 만들고 수신된 텍스트 값 또는 파일에서 CSV 텍스트를 구문 분석할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# CSV

다음 [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] 모듈을 사용하여 CSV 파일을 만들고 수신된 텍스트 값 또는 파일에서 CSV 텍스트를 구문 분석할 수 있습니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화를 위한]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL CSV 만들기]

다음 [!UICONTROL CSV 만들기] 누적 을 사용하면 수신된 텍스트 값에서 csv 텍스트를 만들 수 있습니다.

집계에 대한 자세한 내용은 [의 누적 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 소스 모듈]</td>
        <td>필요한 필드를 집계하는 데 사용할 모듈을 선택합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 집계된 필드]</td>
        <td>사용 가능한 필드 목록에서 집계할 필드를 선택합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 첫 번째 행에 머리글 포함]</td>
        <td>결과에 헤더를 포함하려면 이 옵션을 선택합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>결과를 그룹화할 필터를 입력합니다. 예를 들어 날짜를 입력합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 빈 집계 후 처리 중지]</td>
        <td>결과가 없는 경우 시나리오를 중지하려면 이 옵션을 선택합니다.</td>
    </tr>
</table>

## [!UICONTROL CSV 만들기(고급)]

다음 [!UICONTROL CSV 만들기(고급)] 누적 을 사용하면 수신된 텍스트 값에서 CSV 텍스트를 만들 수 있습니다. 여기서는 결과 CSV 파일의 CSV 열을 정의하는 데이터 구조를 사용합니다. 정의된 열이 CSV 모듈 설정에서 필드로 표시되며 시나리오의 이후 모듈에 매핑할 수 있습니다.

집계에 대한 자세한 내용은 [의 누적 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 소스 모듈]</td> 
   <td>필요한 필드를 집계하는 데 사용할 앱 모듈을 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 데이터 구조]</td> 
   <td> <p>원하는 방식으로 필드를 집계할 데이터 구조를 선택합니다. 데이터 구조를 정의한 후 항목을 해당 필드에 매핑할 수 있습니다.</p> <p>자세한 내용은 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">의 데이터 구조 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 첫 번째 행에 머리글 포함] </td> 
   <td>결과에 헤더를 포함하려면 이 옵션을 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>결과를 그룹화할 필터를 입력합니다. 예를 들어 날짜를 입력합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 빈 집계 후 처리 중지] </td> 
   <td>결과가 없는 경우 시나리오를 중지하려면 이 옵션을 선택합니다. </td> 
  </tr> 
 </tbody> 
</table>


<p>Google 연락처를 열 "전체 이름"과 "이메일"이 두 개인 CSV 파일로 내보내려고 한다고 가정합니다. [!UICONTROL Google 연락처] &gt;[!UICONTROL 그룹에서 연락처 가져오기] 모듈의 출력 번들은 다음 구조를 갖습니다. 이메일 주소는 <code>[!UICONTROL Emails[]]</code> 항목: 컬렉션 배열이며 각 컬렉션에는 두 항목이 포함됩니다. <code>Label</code> 및 <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>간단한 [!DNL Create CSV] 모듈에서는 번들의 최상위 항목에 해당하는 확인란 목록이 제공됩니다. 확인 표시를 하면 <code>Full name</code> 및 <code>Emails</code> 항목, [!UICONTROL CSV 만들기] 모듈은 다음 출력을 생성하며, 이것은 사용자가 원하는 출력이 아닐 수 있습니다.</p>
<p>"email","fullName"</p>
<p>"[object]","Shon Winer"</p>
<p>"[object]","Lizeth Fulmore"</p>
<p>"[object]","Hilario Gullatt"</p>
<p>"[개체]","Abby Eisenbarth"</p>
<p>항목 이후 <code>Full Name</code> 는 간단한 Text 유형으로 내보내기만 하면 됩니다. 하지만, <code>Emails</code>컬렉션 배열이라는 복잡한 형식의 컬렉션은 기본적으로 컬렉션과 배열이 텍스트로 변형되는 방법인 [개체 개체 개체]로 내보내집니다. 자세한 내용은 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion의 항목 데이터 유형</a>.</p>
<p>의 컨텐츠를 내보내려면 <code>Email </code>첫 번째 컬렉션의 항목 <code>Emails[]</code> 배열을 대신 사용하려면 [!UICONTROL CSV 만들기(고급)] 모듈을 사용해야 합니다. 모듈을 사용하여 CSV 파일의 개별 열을 정의하고 중첩된 열을 포함하여 항목을 CSV 파일에 매핑할 수 있습니다.</p>
<ol>
<li value="1">시나리오에 [!UICONTROL CSV 만들기(고급)] 모듈을 삽입하고 해당 구성을 엽니다.</li>
<li value="2">을(를) 클릭합니다. <strong>[!UICONTROL Add]</strong> 새 데이터 구조를 만들려면 [!UICONTROL 데이터 구조] 필드 옆에 있는 버튼을 클릭합니다.</li>
<li value="3"> <p>데이터 구조 이름에 쓰고 <strong>[!UICONTROL 항목 추가]</strong> 개별 열을 추가하는 단추. 두 열을 내보내려면 다음을 수행합니다. 전체 이름 및 "이메일"의 결과 데이터 구조는 다음과 같습니다.</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>데이터 구조를 성공적으로 정의하면 항목을 매핑할 수 있도록 각 개별 열에 해당하는 필드가 [!UICONTROL CSV 만들기(고급)] 모듈 구성에 표시되어야 합니다. 에서 첫 번째 항목을 가져옵니다. <code>[!UICONTROL Emails[]]</code> 배열 및 해당 항목 매핑 <code>Email </code>필드/열 전자 메일로 보내기:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>시나리오를 실행합니다. 항목 이후 <code>Emails[1]: Email</code> 열 "이메일"에 매핑되는 단순 유형의 텍스트입니다. 이제 올바르게 내보냅니다.</p> <p>"전체 이름","이메일"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL CSV 구문 분석]

다음 [!UICONTROL CSV 구문 분석] 변압기를 사용하여 수신된 텍스트 값 또는 파일의 CSV 텍스트를 구문 분석할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 열 수]</td> 
   <td>CSV 파일에 열 수를 지정합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV에 헤더 포함]</td> 
   <td> <p>CSV 텍스트의 첫 번째 행에 머리글이 포함된 경우 이 옵션을 선택합니다.</p> <p>참고: 모듈은 이러한 헤더를 사용하여 출력의 열에 레이블을 지정하지 않습니다. 대신 이 필드를 사용하면 헤더가 출력 데이터에 포함되지 않습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 구분 기호 유형]</td> 
   <td> <p>CSV 파일의 구분 기호를 선택합니다. 구분 기호는 별도의 값이나 필드 사이의 경계를 나타내는 텍스트 문자입니다.</p> 
    <ul> 
     <li>[!UICONTROL Comma]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Other]</p> <p>[!UICONTROL Other]를 선택하는 경우 CSV 파일에서 값을 구분하는 데 사용하는 구분 기호 문자를 입력합니다. 문자를 하나만 입력해야 합니다.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 따옴표가 없는 필드 내에서 따옴표 보존]</td> 
   <td>따옴표를 유지하려면 이 옵션을 활성화하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>구문 분석할 CSV 파일을 입력하거나 매핑합니다.<p>참고: <p>데이터가 이진 형식으로 제공되는 경우(일반적으로 파일에서) 'toString()' 함수를 사용하여 이진 데이터를 [!UICONTROL String]으로 변환해야 합니다.</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
