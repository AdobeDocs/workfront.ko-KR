---
title: 인터페이스 모듈
description: 인터페이스 모듈
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 2%

---

# 인터페이스 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오는 Intact를 사용하는 워크플로우를 자동화하고 여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

시나리오 만들기에 대한 지침이 필요한 경우 [에서 시나리오 만들기 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

모듈에 대한 자세한 내용은 [의 모듈 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Intect 모듈을 사용하려면 Internet 계정이 있어야 합니다.

## Workfront Fusion에 연결

### 인증 [!DNL Workfront Fusion] intact에서 변경

전 [!DNL Workfront Fusion] 연결 가능 [!DNL Intacct]를 승인해야 합니다.

Intact 계정에서 **[!UICONTROL 회사]** 탭.

1. 클릭 **회사 정보**.
1. 로 이동합니다 **보안** 탭.
1. 클릭 [!UICONTROL 편집] 오른쪽 위 모서리에서
1. 웹 서비스 권한 을 선택합니다.
1. 더하기 아이콘을 클릭합니다
1. sender_id로 AzuquaMPP를 입력합니다.
1. (선택 사항) 연결에 대한 설명을 입력합니다

### 에서 연결 설정 [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

에 대한 연결을 만들 수 있습니다 [!DNL Intacct] 내에서 직접 계정 [!DNL Intacct] 모듈.

1. 아무 통합 모듈에서나 **[!UICONTROL 추가]** 연결 필드 옆에 있습니다.
1. 인터 자격 증명을 입력합니다

   * 회사 ID
   * 사용자 ID
   * 암호

1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## 인터페이스 모듈 및 해당 필드

구성 시 [!DNL Intacct] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 앱이나 서비스에서 액세스 수준 등의 요소에 따라 추가 인터페이스 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 사용자 지정 API 호출 만들기]](#make-a-custom-api-call)
* [[!UICONTROL 레코드 검색]](#search-records)

### [!UICONTROL 사용자 지정 API 호출 만들기] {#make-a-custom-api-call}

이 작업 모듈을 사용하면 [!DNL Intacct] API. 이렇게 하면 다른 방식으로 수행할 수 없는 데이터 흐름 자동화를 만들 수 있습니다 [!DNL Intacct] 모듈.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>연결</p> </td> 
   <td> <p>계정 연결에 대한 지침은 [!DNL Workfront Fusion] 2.0 참조 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Workfront Fusion에서 연결 설정</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">본문 XML</td> 
   <td> <p>본문 내에 XML만 포함합니다. 요청에는 인증 헤더가 자동으로 포함됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 레코드 검색]

이 검색 모듈은 특정 검색 기준과 일치하는 레코드 목록을 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>연결</p> </td> 
   <td> <p>계정 연결에 대한 지침은 [!DNL Workfront Fusion] 2.0 참조 <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Workfront Fusion에서 연결 설정</a> 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 레코드 유형]</td> 
   <td> <p>검색할 레코드 유형을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>검색 기준</p> </td> 
   <td> 
    <ul> 
     <li> <p>검색할 필드를 선택합니다</p> </li> 
     <li> <p>검색에 사용할 연산자를 선택합니다</p> </li> 
     <li> <p>검색할 값을 입력합니다</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">결과 집합</td> 
   <td>일치하는 모든 레코드를 반환할지, 일치하는 첫 번째 레코드만 반환할지 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">제한</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">정렬 기준</td> 
   <td>결과를 정렬할 필드를 선택합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">주문</td> 
   <td>오름차순 또는 내림차순 정렬 여부를 선택합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">출력</td> 
   <td> <p>이 모듈의 출력 번들에 포함할 정보를 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">대/소문자 구분</td> 
   <td>이 옵션을 활성화하여 쿼리를 대/소문자를 구분합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">비공개 엔티티로 쿼리</td> 
   <td>모듈에서 개인 엔티티를 검색하도록 하려면 이 옵션을 활성화합니다.</td> 
  </tr> 
 </tbody> 
</table>
