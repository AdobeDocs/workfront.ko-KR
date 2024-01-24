---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 데이터 저장소 모듈
description: An [!DNL Adobe Workfront Fusion] 데이터베이스 또는 간단한 테이블과 유사한 데이터 저장소는 시나리오의 데이터를 저장할 수 있으므로 개별 시나리오 또는 시나리오 실행 간에 데이터를 전송할 수 있습니다. 동기화 중에 데이터 저장소를 사용하여 다양한 시스템의 새 데이터를 저장할 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# [!UICONTROL 데이터 저장소] 모듈

An [!DNL Adobe Workfront Fusion] 데이터베이스 또는 간단한 테이블과 유사한 데이터 저장소는 시나리오의 데이터를 저장할 수 있으므로 개별 시나리오 또는 시나리오 실행 간에 데이터를 전송할 수 있습니다. 동기화 중에 데이터 저장소를 사용하여 다양한 시스템의 새 데이터를 저장할 수 있습니다.

데이터 저장소 모듈을 사용하면 의 레코드를 추가, 교체, 업데이트, 검색, 삭제, 검색 또는 카운트할 수 있습니다. [!DNL Adobe Workfront Fusion] 데이터 저장소입니다.

데이터 저장소 만들기, 편집 및 문제 해결에 대한 자세한 내용은 [의 데이터 저장소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Workfront Fusion의 데이터 저장소에 대한 비디오 소개는 다음을 참조하십시오.

* [데이터 저장소](https://video.tv.adobe.com/v/3427029/){target=_blank}

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

## 전제 조건

사용 [!UICONTROL 데이터 저장소] 모듈에서는 먼저 데이터 저장소를 만들어야 합니다.

데이터 저장소 만들기에 대한 자세한 내용은 [의 데이터 저장소 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL 데이터 저장소] 모듈 및 해당 필드

데이터 저장소 모듈을 구성할 때 [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이러한 필드와 함께 앱이나 서비스의 액세스 수준 등의 요소에 따라 추가 데이터 스토어 필드가 표시될 수 있습니다. 모듈의 굵은 제목은 필수 필드를 나타냅니다.

필드나 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

모두 [!UICONTROL 데이터 저장소] 모듈은 작업 유형 모듈입니다.

* [레코드 추가/바꾸기](#addreplace-a-record)
* [레코드 업데이트](#update-a-record)
* [레코드 가져오기](#get-a-record)
* [레코드 존재 확인](#check-the-existence-of-a-record)
* [레코드 삭제](#delete-a-record)
* [모든 레코드 삭제](#delete-all-records)
* [레코드 검색](#search-records)
* [레코드 수](#count-records)

### [!UICONTROL 레코드 추가/바꾸기]

이 작업 모듈은 레코드를 추가하거나 대체합니다.

데이터 저장소 및 레코드 키를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

>[!NOTE]
>
>데이터 저장소에 이미 있는 레코드를 동일한 이름 및 로 추가하려고 하면 모듈에 오류가 발생합니다. [!UICONTROL 기존 레코드 덮어쓰기] 옵션이 비활성화되었습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소]</td> 
   <td> <p> 레코드를 만들 데이터 저장소를 선택하거나 추가합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 키] </td> 
   <td> <p>모듈이 추가하거나 대체할 레코드의 고유 키를 입력합니다. 키는 나중에 레코드를 검색하는 데 사용할 수 있습니다. 이 필드를 비워 두면 키가 자동으로 생성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 기존 레코드 덮어쓰기] </td> 
   <td> <p>레코드를 덮어쓰려면 이 옵션을 활성화합니다. 덮어쓰려는 레코드는 위의 키 필드에 지정해야 합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드] </td> 
   <td> <p>레코드의 필드에 원하는 값을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 업데이트]

이 작업 모듈은 레코드를 업데이트합니다.

데이터 저장소 및 레코드 키를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소]</td> 
   <td> <p> 레코드를 만들 데이터 저장소를 선택하거나 추가합니다. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 키] </td> 
   <td> <p>모듈을 업데이트할 레코드의 고유 키를 입력합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 누락된 레코드 삽입] </td> 
   <td> <p>지정된 키가 있는 레코드가 없는 경우 새 레코드를 만들려면 이 옵션을 활성화합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 레코드]</td> 
   <td> <p> 갱신할 레코드의 필드에 원하는 값을 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 가져오기]

이 작업 모듈은 레코드를 검색합니다.

데이터 저장소 및 레코드 키를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소]</td> 
   <td> <p> 레코드를 검색할 데이터 저장소를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 키] </td> 
   <td> <p>모듈을 검색할 레코드의 고유 키를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 존재 확인]

이 작업 모듈은 특정 레코드가 존재하는지 여부를 지정합니다.

데이터 저장소 및 레코드 키를 지정합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소] </td> 
   <td> <p>레코드 존재를 확인할 데이터 저장소를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 키] </td> 
   <td> <p>모듈이 존재하는지 확인할 레코드의 고유 키를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 삭제]

이 작업 모듈은 레코드를 삭제합니다.

데이터 저장소 및 레코드 키를 지정합니다.

모듈은 연결에서 액세스하는 사용자 지정 필드 및 값과 함께 레코드 및 관련 필드의 ID를 반환합니다. 이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소] </td> 
   <td> <p>레코드 존재를 확인할 데이터 저장소를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 키] </td> 
   <td> <p>모듈에서 삭제할 레코드의 고유 키를 입력합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 모든 레코드 삭제]

이 작업 모듈은 특정 데이터 저장소에서 모든 레코드를 삭제합니다.

데이터 저장소를 지정합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소] </td> 
   <td> <p>모든 레코드를 삭제할 데이터 저장소를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 검색]

이 검색 모듈은 데이터 저장소의 개체에서 지정한 검색 쿼리와 일치하는 레코드를 찾습니다.

이 정보는 시나리오의 후속 모듈에 매핑할 수 있습니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소]</td> 
   <td> <p> 검색할 데이터 저장소를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>검색 필터를 설정합니다.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">정렬할 각 필드에 대해 다음 필드를 입력합니다.</p> <p style="font-weight: bold;">[!UICONTROL 키]</p> <p>결과를 정렬할 열 이름을 선택합니다.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>결과를 오름차순으로 정렬할지 아니면 내림차순으로 정렬할지 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 제한]</td> 
   <td> <p> 최대 검색 결과 수 설정 [!DNL Workfront Fusion] 는 한 실행 주기 동안 를 반환합니다.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 모듈이 결과를 반환하지 않더라도 라우트 실행을 계속합니다.]</td> 
   <td> <p> 활성화된 경우 이 모듈이 속한 경로는 이 모듈이 결과를 반환하지 않는 경우에도 계속 처리됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 수]

이 작업 모듈은 데이터 저장소의 레코드에 번호를 지정합니다.

데이터 저장소를 지정합니다.

이 모듈을 구성할 때 다음 필드가 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 데이터 저장소] </td> 
   <td> <p>계산할 레코드가 포함된 데이터 저장소를 선택합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
