---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server 모듈
description: 다음을 사용할 수 있습니다 [!DNL Adobe Workfront Fusion] Microsoft SQL Server에 연결할 수 없습니다.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] 모듈

다음을 사용할 수 있습니다 [!DNL Adobe Workfront Fusion] 에 연결 [!UICONTROL Microsoft SQL Server].

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

## 사용 [!DNL Microsoft SQL Server] 모듈

저장 프로시저를 통해 데이터베이스 서버에서 직접 사용자 지정 로직을 실행할 수 있습니다. [!DNL Adobe Workfront Fusion] 입력/출력 매개 변수와 레코드세트의 인터페이스를 동적으로 로드하여 각 매개 변수 또는 값을 개별적으로 매핑할 수 있습니다. 시나리오 구성을 시작하기 전에 데이터베이스에 연결하는 데 사용하는 계정에 `INFORMATION_SCHEMA.ROUTINES` 및 `INFORMATION_SCHEMA.PARAMETERS` 보기.

When [!DNL Fusion] 에 대한 연결을 설정합니다. [!DNL SQL server] 대상, [!DNL Fusion] 사용자는 호스트(서버가 호스팅되는 도메인 이름 또는 IP 주소)와 포트를 식별합니다. [!DNL Fusion] 사용 가능한 모든 호스트 및 포트에 연결할 수 있습니다.

에서 사용하는 특정 IP 주소에 대한 정보 [!DNL Workfront Fusion]를 참조하십시오. [액세스하기 위한 IP 주소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

저장 프로시저 만들기에 대한 자세한 내용은 [!DNL Microsoft SQL Server] 설명서.

>[!NOTE]
>
>[!DNL Workfront Fusion] 여러 개의 레코드 집합을 지원하지 않습니다. 첫 번째 항목만 처리됩니다.

## 문제 해결 오류 [!UICONTROL ER_LOCK_WAIT_TIMEOUT: 잠금 대기 시간 제한을 초과했습니다. 트랜잭션 다시 시작]

이 오류는 여러 모듈을 사용하여 동일한 데이터를 수정할 때 발생합니다. SQL 트랜잭션으로 인해 발생합니다.

SQL 모듈이 실행되면 트랜잭션이 시작됩니다. 시나리오가 완전히 실행된 후에 트랜잭션이 완료됩니다.

다른 모듈에서 동일한 데이터에 액세스하려고 하면 이전 트랜잭션이 완료될 때까지 기다려야 합니다. 시나리오가 완료된 후 첫 번째 트랜잭션이 완료되므로 두 번째 트랜잭션은 결코 시작할 수 없습니다.

### 솔루션:

자동 커밋 을 설정합니다. 모듈 실행이 완료된 후 즉시 모든 트랜잭션을 자동 커밋(커밋)합니다.

1. 을(를) 클릭합니다. [!UICONTROL 시나리오 설정] 아이콘 ![](assets/scenario-settings-icon.png)화면 하단에 있습니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자동 커밋]** 확인란을 선택합니다.
1. 클릭 **[!UICONTROL 확인]** 시나리오 설정을 저장하려면 을 클릭합니다.
