---
title: MariaDB 모듈
description: 에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL MariaDB]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL MariaDB] 모듈

에서 [!DNL Adobe Workfront Fusion] 시나리오, [!DNL MariaDB]여러 타사 애플리케이션 및 서비스에 연결할 수 있습니다.

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

를 사용하려면 [!DNL MariaDB] 모듈이면 반드시 [!DNL MariaDB] 계정이 필요합니다.

## Connect [!DNL MariaDB] to [!DNL Workfront Fusion]

에 대한 연결을 만들 수 있습니다 [!DNL MariaDB] 내에서 직접 계정 [!DNL MariaDB] 모듈.

1. 어떤 경우에서도 [!DNL MariaDB] 모듈 **[!UICONTROL 추가]** 다음 [!UICONTROL 연결] 필드.
1. 다음 필드를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 연결 이름]</p> </td> 
      <td> <p>새 연결의 이름을 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>데이터베이스 인스턴스의 IP 주소 또는 호스트 이름을 입력합니다. 이 호스트는 네트워크 외부에서 액세스할 수 있어야 합니다.</p> <p>예: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>기본 포트는 3306입니다. 비표준 포트를 사용하는 경우 이 번호를 포트로 설정하십시오. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 데이터베이스 이름]</td> 
      <td>상호 작용할 데이터베이스의 이름을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Username]</td> 
      <td>사용자 이름 입력.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Password]</td> 
      <td>암호를 입력합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **[!UICONTROL 계속]** 연결을 만들고 모듈로 돌아갑니다.

## [!DNL MariaDB] 모듈 및 해당 필드

구성 시 [!DNL MariaDB] 모듈, [!DNL Workfront Fusion] 아래 나열된 필드를 표시합니다. 이와 함께 추가 [!DNL MariaDB] 앱이나 서비스에서 액세스 수준과 같은 요소에 따라 필드가 표시될 수 있습니다. 모듈에서 굵게 표시된 제목은 필수 필드를 나타냅니다.

필드 또는 함수 위에 맵 단추가 표시되면 이 단추를 사용하여 해당 필드에 대한 변수와 함수를 설정할 수 있습니다. 자세한 내용은 [의 한 모듈에서 다른 모듈로 정보 매핑 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 쿼리 실행(고급)

이 작업 모듈은 제공한 쿼리를 기준으로 데이터베이스에서 정보를 검색합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL MariaDB] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>모듈이 데이터를 검색하는 데 사용할 SQL 쿼리를 입력합니다.</p> <p>중요 사항: 쿼리에 사용되는 변수는 정리되지 않습니다. SQL 주입을 방지하기 위해 변수를 올바르게 정리해야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 테이블에서 행 선택(고급)]

이 모듈은 데이터베이스에서 레코드를 읽습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>연결 방법에 대한 지침은 [!DNL MariaDB] 계정 대상 [!DNL Workfront Fusion]를 참조하십시오. <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] to [!DNL Workfront Fusion]</a> 참조하십시오.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 테이블]</td> 
   <td> <p>읽을 레코드가 포함된 테이블을 선택합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>행을 선택할 필터를 설정합니다</p> 
    <ul> 
     <li> <p>검색할 필드를 선택합니다</p> </li> 
     <li> <p>검색에 사용할 연산자를 선택합니다</p> </li> 
     <li> <p>검색할 값을 입력하거나 매핑합니다.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 정렬] </td> 
   <td> <p>결과를 정렬할 각 수준에 대해 <strong>[!UICONTROL 항목 추가]</strong>그런 다음 결과를 정렬 기준으로 사용할 필드를 선택하고, 오름차순 또는 내림차순으로 정렬할지 여부를 선택합니다</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 제한]</td> 
   <td> <p>각 시나리오 실행 주기 동안 모듈이 반환할 최대 레코드 수를 입력하거나 매핑합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>
