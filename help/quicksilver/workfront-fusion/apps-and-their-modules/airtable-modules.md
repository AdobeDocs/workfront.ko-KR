---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: 에어테이블 모듈
description: Adobe Workfront Fusion에는 Adobe Workfront 라이선스 외에 Adobe Workfront Fusion 라이센스가 필요합니다.
author: Becky
hidefromtoc: true
source-git-commit: 6955c979d504adb6514ae64bf5108174d7a90ce4
workflow-type: tm+mt
source-wordcount: '1863'
ht-degree: 2%

---


# 에어테이블 모듈


사용 [!DNL Airtable] 커넥터 [!DNL Adobe Workfront Fusion]를 설정하는 경우, [!DNL Airtable] Airtable API에 계정을 만들고, 레코드를 업로드 및 업데이트하고, 레코드를 검색하고, 사용자 지정 API를 호출합니다.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] 작업 자동화 및 통합을 위한] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>조직이 구매해야 합니다 [!DNL Adobe Workfront Fusion] 뿐만 아니라 [!DNL Adobe Workfront] 을 참조하십시오.</td> 
  </tr> 
 </tbody> 
</table>

어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

에 대한 자세한 정보 [!DNL Adobe Workfront Fusion] 라이센스 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 전제 조건

이 문서의 기능을 사용하려면 Airtable 계정이 있어야 합니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Airtable을 Workfront Fusion에 연결 {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. Workfront Fusion 및 **연결 만들기** 원하는 모듈의 대화 상자.
1. 연결의 이름을 입력합니다.
1. (선택 사항) 고급 설정 표시를 클릭하고 Airtable 클라이언트 ID와 클라이언트 암호를 입력합니다.
1. 을(를) 클릭합니다. **계속** 단추를 클릭하여 연결을 만들고 모듈로 돌아갑니다.

## 에어테이블 모듈 및 해당 필드

### 레코드

* [레코드 만들기](#create-a-record)
* [레코드 삭제](#delete-a-record)
* [레코드 가져오기](#get-a-record)
* [레코드 검색](#search-records)
* [레코드 업데이트](#update-a-record)
* [레코드 업로드](#upsert-a-record)
* [감시 레코드](#watch-records)
* [응답 보기](#watch-responses)
* [API 호출 만들기](#make-an-api-call)

#### 레코드 만들기 {#create-a-record}

이 작업 모듈은 새 레코드를 만듭니다.

레코드에 저장할 데이터와 위치를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>연결 </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>기본 </td> 
   <td> <p>새 레코드가 속할 기준을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>테이블 </td> 
   <td> <p>새 레코드가 속할 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>기록</p> </td> 
   <td> <p>새 레코드의 값을 입력합니다. 사용 가능한 필드는 선택한 테이블을 기반으로 합니다.</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>스마트 링크</td> 
   <td> <p>다른 테이블에 연결된 필드에 레코드 ID 대신 이름을 입력하려면 이 옵션을 활성화합니다. 일치하는 레코드가 없으면 연결된 테이블에 레코드가 자동으로 생성됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 레코드 삭제 {#delete-a-record}

이 작업 모듈은 특정 레코드를 삭제합니다.

ID를 지정하고 레코드의 위치를 지정합니다.

이 모듈은 연결이 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>연결 </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>기본 </td> 
   <td> <p>삭제할 레코드가 포함된 베이스를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>테이블 </td> 
   <td> <p>삭제할 레코드가 포함된 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>레코드 ID</td> 
   <td> <p>모듈을 삭제할 레코드의 고유한 Airtable ID를 입력하거나 매핑합니다. 예를 들어 검색 레코드 모듈을 사용하여 ID를 검색할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 레코드 가져오기 {#get-a-record}

이 작업 모듈은 레코드 세부 사항을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>연결 </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>기본 </td> 
   <td> <p>검색할 레코드가 있는 테이블이 포함된 베이스를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>테이블</td> 
   <td> <p> 세부 정보를 검색할 레코드가 포함된 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>레코드 ID</td> 
   <td> <p> 세부 정보를 검색할 레코드의 ID를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 레코드 검색 {#search-records}

이 검색 모듈은 지정한 검색 쿼리와 일치하는 Airtable의 개체에서 레코드를 찾습니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>연결 </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>기본 </td> 
   <td> <p>레코드를 검색할 기준을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>테이블 </td> 
   <td> <p>레코드를 검색할 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>공식</p> </td> 
   <td> <p>레코드를 필터링하는 데 사용되는 공식입니다. 공식은 각 레코드에 대해 평가되며 결과가 아닌 경우 <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>, 또는 <code>#Error!</code> 레코드가 응답에 포함됩니다.</p> <p>와 결합된 경우 <code>view</code>를 지정하면 해당 보기에서 공식을 만족하는 레코드만 반환됩니다.</p> <p>예를 들어 이름이 비어 있지 않은 레코드만 포함하려면 다음을 전달합니다.<code> NOT({Name} = '')</code></p> <p>자세한 내용을 보려면 Airtable 지원 설명서에서 수식 필드 참조에 대한 정보를 검색하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>정렬 </td> 
   <td> <p>정렬 방향과 결과를 정렬할 필드를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>보기 </td> 
   <td> <p>레코드를 검색할 보기를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>제한</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 레코드 업데이트 {#update-a-record}

이 작업 모듈은 특정 레코드를 업데이트합니다.

레코드의 ID와 포함할 새 데이터를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>연결 </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>기본 </td> 
   <td> <p>업데이트할 레코드가 포함된 베이스를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>테이블 </td> 
   <td> <p>업데이트할 레코드가 포함된 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>레코드 ID </td> 
   <td> <p>모듈을 업데이트할 레코드의 고유한 Airtable ID를 입력하거나 매핑합니다. 예를 들어 검색 레코드 모듈을 사용하여 ID를 검색할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>기록</p> </td> 
   <td> <p>새 레코드의 값을 입력합니다. 사용 가능한 필드는 선택한 테이블에 따라 다릅니다.</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>스마트 링크</td> 
   <td> <p>다른 테이블에 연결된 필드에 레코드 ID 대신 이름을 입력합니다. 일치하는 레코드가 없으면 연결된 테이블에 레코드가 자동으로 생성됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 레코드 업로드

이 작업 모듈은 특정 레코드를 업데이트하거나 삽입합니다.

레코드의 ID와 포함할 새 데이터를 지정합니다.

이 모듈은 연결에 액세스하는 사용자 지정 필드 및 값과 함께 레코드와 연결된 표준 필드를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>연결 </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>기본 </td> 
   <td> <p>업데이트할 레코드가 포함된 베이스를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>테이블 </td> 
   <td> <p>업데이트할 레코드가 포함된 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>레코드 ID </td> 
   <td> <p>레코드를 업데이트하는 경우, 모듈을 업데이트할 레코드의 고유한 Airtable ID를 입력하거나 매핑합니다. 예를 들어 검색 레코드 모듈을 사용하여 ID를 검색할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>기록</p> </td> 
   <td> <p>새 레코드의 값을 입력합니다. 사용 가능한 필드는 선택한 테이블에 따라 다릅니다.</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>스마트 링크</td> 
   <td> <p>다른 테이블에 연결된 필드에 레코드 ID 대신 이름을 입력합니다. 일치하는 레코드가 없으면 연결된 테이블에 레코드가 자동으로 생성됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 감시 레코드 {#watch-records}

이 트리거 모듈은 지정된 테이블에서 레코드를 만들거나 업데이트할 때 시나리오를 시작합니다.

>[!NOTE]
>
>이 모듈을 사용하려면 테이블에서 생성 시간 필드 또는 마지막 수정 시간 필드를 만들어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>연결 </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td>기본 </td> 
   <td> <p>새 레코드를 보려는 기준을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>테이블 </td> 
   <td> <p>새 레코드를 보려는 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>구성 트리거</p> </td> 
   <td> <p>트리거 필드</p> <p>A <code>Created Time</code> 또는 <code>Last Modified Time</code> 레코드를 정렬하는 데 사용되는 필드입니다. 없는 경우 <code>Created Time</code> 또는 <code>Last Modified Time</code> 스키마의 필드를 만들어야 합니다. </p> <p>레이블 필드</p> <p>예를 들어, 시작할 위치 선택 대화 상자에서 레코드의 레이블로 사용되는 필드입니다.</p> </td> 
  </tr> 
  <tr> 
   <td>제한</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈에서 볼 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>보기</td> 
   <td> <p>사용할 보기를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>공식</p> </td> 
   <td> <p>레코드를 필터링하는 데 사용되는 공식입니다. 공식은 각 레코드에 대해 평가되며 결과가 아닌 경우 <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code>, 또는 <code>#Error!</code> 레코드가 응답에 포함됩니다.</p> <p>와 결합된 경우 <code>view</code>를 지정하면 해당 보기에서 공식을 만족하는 레코드만 반환됩니다.</p> <p>예를 들어 이름이 비어 있지 않은 레코드만 포함하려면 다음을 전달합니다.<code> NOT({Name} = '')</code></p> <p>자세한 내용은 Airtable 지원 설명서에서 수식 필드 참조에 대한 정보를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 응답 보기

이 트리거 모듈은 양식을 제출할 때 시나리오를 시작합니다.

>[!NOTE]
>
>이 기능은 유료 Airtable Pro Plan에서만 사용할 수 있습니다.

웹 후크 URL을 Workfront Fusion에서 생성한 다음 Airtable의 양식 구성에 추가해야 합니다.

1. Workfront Fusion 시나리오에 Watch 새 응답 모듈을 추가합니다.
1. 웹 후크 URL을 생성하고 복사합니다.

   자세한 내용은 [Adobe Workfront Fusion의 즉각적인 트리거(웹 후크)](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Airtable 계정에 로그인합니다.
1. 양식에 사용할 기본 및 표를 열고 양식 보기를 만듭니다.
1. 필요에 따라 양식을 설정하고, 양식을 아래로 스크롤한 다음, 양식이 제출되면 URL로 리디렉션 옵션을 활성화합니다.
1. 2단계에서 생성된 Webhook URL을 표시된 대화 상자에 입력하고 Webhook URL 바로 다음에 ?record_id={record_id}를 추가하여 모듈의 출력에 레코드 ID를 포함시킨 다음 저장을 클릭합니다. 예를 들어 결과 URL은 다음과 같습니다.
1. Workfront Fusion 시나리오로 돌아가서 Airtable에서 필드를 로드하고 해당 필드를 다른 모듈에 매핑할 수 있도록 Watch Responses 모듈을 실행합니다.
1. 양식을 제출한 후 URL로 리디렉션 옵션이 활성화되고 Webhook URL이 추가된 Airtable에서 양식을 제출합니다(위의 6단계).

   감시 응답 모듈이 트리거되고 원하는 데이터가 로드됩니다.

1. Airtable > Watch Responses 모듈 바로 뒤에 Airtable > Get a Record 모듈을 추가하고 record_id 를 Record ID 필드에 매핑합니다.

이제 양식이 제출될 때마다 Workfront Fusion 시나리오의 Watch Responses 모듈이 트리거되고 Get a Record 모듈이 제출된 양식 세부 사항을 반환합니다.

#### API 호출 만들기

#### 사용자 지정 API 호출

이 작업 모듈을 사용하면 [!DNL Airtable] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Airtable] 모듈.

작업은 지정한 엔티티 유형(할당 객체 유형)을 기반으로 합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>연결</p> </td> 
   <td> <p>Airtable 계정을 Workfront Fusion에 연결하는 방법에 대한 지침은 <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable을 Workfront Fusion에 연결</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>상대 경로 입력 <code>https://api.airtable.com/}</code>. 예: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">메서드</td> 
   <td> <p>API 호출을 구성하는 데 필요한 HTTP 요청 메서드를 선택합니다. 자세한 내용은 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">의 HTTP 요청 메서드 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">헤더</td> 
   <td> <p>요청의 헤더를 표준 JSON 개체 형태로 추가합니다.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 사용자를 위해 인증 헤더를 추가합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">쿼리 문자열</td> 
   <td> <p>API 호출에 대한 쿼리를 키 및 값 형식으로 추가합니다</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">본문</td> 
   <td> <p>표준 JSON 개체 형태로 API 호출에 대한 본문 콘텐츠를 추가합니다.</p> <p>참고:  <p>다음과 같은 조건문을 사용하는 경우 <code>if</code> json에서 따옴표를 조건문 외부에 지정합니다.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
