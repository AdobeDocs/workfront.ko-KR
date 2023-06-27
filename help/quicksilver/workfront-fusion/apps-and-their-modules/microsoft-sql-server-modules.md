---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 커넥터
navigation-topic: apps-and-their-modules
title: Microsoft Server 모듈
description: 다음을 사용할 수 있습니다. [!DNL Adobe Workfront Fusion] Microsoft SQL Server에 연결합니다.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# [!DNL Microsoft SQL Server] 모듈

다음을 사용할 수 있습니다. [!DNL Adobe Workfront Fusion] 에 연결하려면 [!UICONTROL Microsoft Server].

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

## 사용 [!DNL Microsoft SQL Server] 모듈

저장 프로시저를 통해 데이터베이스 서버에서 직접 사용자 지정 논리를 실행할 수 있습니다. [!DNL Adobe Workfront Fusion] 각 매개 변수 또는 값을 개별적으로 매핑할 수 있도록 입력/출력 매개 변수 및 레코드세트의 인터페이스를 동적으로 로드합니다. 시나리오 구성을 시작하기 전에 데이터베이스에 연결하기 위해 사용하는 계정에 대한 읽기 액세스 권한이 있는지 확인하십시오 `INFORMATION_SCHEMA.ROUTINES` 및 `INFORMATION_SCHEMA.PARAMETERS` 보기.

날짜 [!DNL Fusion] 에 대한 연결을 설정합니다. [!DNL SQL server] 대상, [!DNL Fusion] 사용자는 호스트(서버가 호스팅된 도메인 이름 또는 IP 주소) 및 포트를 식별합니다. [!DNL Fusion] 사용 가능한 모든 호스트 및 포트에 연결할 수 있습니다.

에서 사용하는 특정 IP 주소에 대한 정보 [!DNL Workfront Fusion], 참조 [액세스하기 위한 IP 주소 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

저장 프로시저 만들기에 대한 자세한 내용은 [!DNL Microsoft SQL Server] 설명서를 참조하십시오.

>[!NOTE]
>
>[!DNL Workfront Fusion] 는 여러 레코드세트를 지원하지 않습니다. 첫 번째 작업만 처리됩니다.

## 문제 해결 오류 [!UICONTROL ER_LOCK_WAIT_TIMEOUT: 잠금 대기 시간 제한이 초과되었습니다. 트랜잭션을 다시 시작해 보십시오.]

이 오류는 여러 모듈을 사용하여 동일한 데이터를 수정할 때 발생합니다. 이 오류는 SQL 트랜잭션으로 인해 발생합니다.

SQL 모듈이 실행되면 트랜잭션이 시작됩니다. 시나리오가 완전히 실행된 후에 트랜잭션이 완료됩니다.

다른 모듈이 동일한 데이터에 액세스하려고 하면 이전 트랜잭션이 완료될 때까지 기다려야 합니다. 시나리오가 종료된 후에 첫 번째 거래가 종료되므로 두 번째 거래는 결코 시작할 수 없다.

### 해결 방법:

자동 커밋을 켭니다. 자동 커밋은 모듈 실행이 완료된 직후 모든 트랜잭션을 완료(커밋)합니다.

1. 다음을 클릭합니다. [!UICONTROL 시나리오 설정] 아이콘 ![](assets/scenario-settings-icon.png)화면 맨 아래에.
1. 다음을 클릭합니다. **[!UICONTROL 자동 커밋]** 확인란.
1. 클릭 **[!UICONTROL 확인]** 시나리오 설정을 저장합니다.
