---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 의 항목 데이터 유형 [!DNL Adobe Workfront Fusion]
description: 사용자 [!DNL Adobe Workfront Fusion] 시나리오에는 아래에 나열된 항목 유형이 번들에 포함될 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 의 항목 데이터 유형 [!DNL Adobe Workfront Fusion]

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

## 항목 데이터 유형

아래에 나열된 항목 유형을 번들에 포함할 수 있습니다.

항목 유형에 대한 정보 [!DNL Workfront Fusion] 서로 간의 전환을 허용합니다. 다음을 참조하십시오. [형식 강제 변환 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>텍스트</p> </td> 
   <td> <p>가장 일반적인 항목 유형입니다. 일부 텍스트 항목의 경우, [!DNL Adobe Workfront Fusion] 최대 또는 최소 허용 길이를 충족하는지 또는 항목이 형식 유효성 검사(이메일, URL 또는 파일 이름)를 수행하는지 여부를 확인합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>숫자</p> </td> 
   <td> <p>일부 숫자 항목의 경우, [!DNL Workfront Fusion] 지정된 범위(최소 또는 최대 허용 값)에 대한 입력의 유효성을 검사할 수 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>부울(예/아니요)</p> </td> 
   <td> <p>이 유형은 true 또는 false의 두 가지 값만 있는 항목에 사용됩니다. </p> <p>모듈을 설정할 때 부울 유형이 두 가지 다른 형식으로 나타날 수 있습니다.</p> 
    <ul> 
     <li> <p>필수 확인란은 필드가 필수이고 입력해야 하는 경우에 표시됩니다.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>비워 둘 수 있는 선택적 필드가 선택 상자로 표시되어 다음 세 가지 값 중에서 선택할 수 있습니다. <code>Yes</code>, <code>No</code>, 및 <code>Not defined</code> (기본값).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>다음을 클릭할 수 있습니다. <strong>[!UICONTROL 맵]</strong> 값을 다른 모듈의 항목에 매핑해야 하는 경우</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>일자</p> </td> 
   <td> <p>날짜는 ISO 8601 날짜 형식으로 입력됩니다(예: ). <code>2015-09-18T11:58Z</code>. 에 설명된 대로 프로필 설정에서 시간대를 변경할 수 있습니다 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">에서 프로필 설정 변경 [!DNL Adobe Workfront Fusion]</a>. </p> <p>날짜가 필요한 필드를 클릭하면 모듈 설정에 팝업 캘린더가 표시됩니다. 일부 항목에는 시간이 필요하지 않습니다.</p> <p>날짜 항목의 값은 프로필에서 선택한 로컬 및 웹 시간대를 사용하여 형식이 지정됩니다. 마우스로 항목을 가리키면 날짜 항목의 ISO 8601 버전 값을 표시할 수 있습니다.</p> <p>참고: ISO 값이 표시되지 않으면 항목은 날짜가 아닌 텍스트일 수 있습니다.</p> <p>에 시간을 입력합니다. <code>hours:minutes:seconds</code> 형식(예: )<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>버퍼(이진 데이터)</p> </td> 
   <td> <p>파일 콘텐츠는 일반적으로 버퍼 유형 콘텐츠(이미지 콘텐츠, 비디오 파일 등)로 전송됩니다. 경우에 따라 텍스트 데이터가 이 유형에 포함됩니다(예: 텍스트 파일). [!DNL Workfront Fusion] 2진 코드의 텍스트 데이터를 텍스트로, 2진 코드의 텍스트를 텍스트 데이터로 자동 변환할 수 있습니다. 자세한 내용은 <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]의 매핑 파일 정보</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>컬렉션</p> </td> 
   <td> <p>컬렉션은 여러 하위 항목으로 구성된 항목입니다. 이메일 메시지의 발신자 항목은 컬렉션의 예입니다. 여기에는 발신자 이름(텍스트 유형)과 발신자 이메일 주소(텍스트 유형)가 포함됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>선택(메뉴)</p> </td> 
   <td> <p>에 설명된 대로 모듈 설정을 구성할 때 <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">에서 모듈 설정 구성 [!DNL Adobe Workfront Fusion]</a>, 동일한 유형의 여러 항목 중에서 선택할 수 있습니다. 예제: 설정에 있는 폴더 선택 메뉴 [!DNL Dropbox] 모듈. </p> <p>모듈을 설정할 때 선택 메뉴는 두 가지 형식으로 나타날 수 있습니다.</p> <p> <p>여러 항목을 선택할 수 있는 경우 확인란이 있는 여러 항목이 표시됩니다.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>한 가지 옵션만 가능한 경우 드롭다운 메뉴가 표시됩니다.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>다른 모듈의 항목을 매핑해야 하는 경우 <strong>맵</strong> 단추를 클릭합니다. 이 버튼을 누르면 선택 메뉴 대신 텍스트 필드가 열립니다. 자세한 내용은 <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>배열</p> </td> 
   <td> <p>배열 형식을 사용하여 컬렉션을 포함하여 동일한 형식의 여러 값으로 작업할 수 있습니다. 예로는 [!UICONTROL Email] 모듈이 있습니다. 이 모듈은 첨부 파일 배열을 반환하며 각 첨부 파일에는 이름, 컨텐츠, 크기 등이 포함됩니다. 자세한 내용은 <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">에서 배열 매핑 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>유효성 검사</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 은 각 항목 유형에 대해 유효성 검사를 수행할 수 있습니다. 항목이 유효성 검사를 통과하지 못하면 모듈은 데이터 오류 때문에 처리를 중지합니다. 자세한 내용은 <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">에서 처리하는 동안 오류 발생 [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
