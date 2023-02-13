---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 에서 보고서 실행 [!DNL Workfront Proof]
description: Workfront 증명 을 사용하면 보고서를 볼 수 있으므로 팀의 작업 진행 상황과 효율성을 추적할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 에서 보고서 실행 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

Workfront 증명 을 사용하면 보고서를 볼 수 있으므로 팀의 작업 진행 상황과 효율성을 추적할 수 있습니다.

에서 만든 증명 수를 쉽게 볼 수 있습니다 [!DNL Workfront Proof] 각 증명, 전환 시간 등과 관련된 버전 수

## 전제 조건

보고서를 사용할 수 있는지 여부는 사용 가능한 보고서 유형에 따라 다릅니다. [!DNL Workfront Proof] 계정 및 사용자 권한 수준.

* [계정 사전 요구 사항](#account-prerequisites)
* [사용자 사전 요구 사항](#user-prerequisites)

### 계정 사전 요구 사항 {#account-prerequisites}

보고 정보는 Premium 계획에서만 사용할 수 있습니다.

### 사용자 사전 요구 사항 {#user-prerequisites}

보고 정보는 계정의 모든 증명에 대한 전체 액세스 권한이 있는 사용자(예: 최소 사용자가 있는 사용자)만 사용할 수 있습니다 [증명 권한 프로필 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

이 패널에서 다음을 수행할 수 있습니다

* 표시된 데이터의 시간 범위 제어
* 시간에 따른 지표 변경 사항 분석
* 마우스로 가리키면 선택한 시점의 세부 정보를 확인합니다
* 선택한 시간 범위에서 만든 총 증명 수를 확인합니다
* 완료된 증명 세트에 포함된 평균 버전 수를 확인합니다

## 보고서 보기 {#viewing-reports}

1. 로 이동합니다. **[!UICONTROL 대시보드]** 페이지.
1. 을(를) 클릭합니다. **[!UICONTROL 보고서]** 탭.\
   ![prop_reports.png](assets/proof-reports-350x193.png)

1. 에서 **[!UICONTROL 시간대]** 드롭다운 메뉴에서 지난 24시간, 7일, 30일, 90일 또는 사용자 지정 기간 내에 만든 증명에 대한 정보를 표시할지 여부를 선택합니다.\
   사용자 지정 기간을 선택하는 경우 시작 및 종료 날짜를 선택한 다음 를 클릭합니다 **[!UICONTROL 적용]**.\
   선택한 기간에 대해 다음 정보가 표시됩니다.\
   **작성된 증명:** 선택한 기간 내에 만든 증명 수입니다.\
   **증명 단위 버전:** 선택한 기간 내의 완료된 모든 증명(승인됨 또는 변경 사항으로 승인됨)에 대한 증명당 평균 버전 수\
   **시간 전환:** 첫 번째 버전을 만든 시점부터 최종 버전에서 결정을 내린 시간까지 평균 시간입니다.\
   **첫 번째 활동 시간:** 증명을 만든 시점부터 증명의 첫 번째 활동 시간까지 평균 시간입니다.\
   **늦게 증명:** 선택한 기간 내에 하나 이상의 버전이 있는 완료된 증명(승인됨 또는 변경 사항으로 승인됨)의 평균 비율입니다.\
   **댓글 및 회신:** 선택한 기간 내에 모든 증명에 대해 수행된 평균 댓글 및 답글 수입니다.

1. (선택 사항) **[!UICONTROL 최소-최대 범위 표시]** 그래프에 최소값과 최대값을 표시할지 여부를 결정하는 옵션입니다.\
   이 옵션을 선택하면 최소 및 최대 기록 값 사이에 파란색 음영이 표시됩니다.

1. (선택 사항)에 설명된 대로 표시되는 데이터를 필터링할 수 있습니다. [보고서 필터링](#filtering-reports).

## 보고서 필터링 {#filtering-reports}

기본적으로 보고서에 표시되는 데이터에는 [!DNL Workfront Proof] 시스템. 필터를 사용하여 요구 사항과 관련된 정보만 표시할 수 있습니다.

보고 정보를 필터링하려면:

1. 로 이동합니다. **[!UICONTROL 대시보드]** 페이지.
1. 을(를) 클릭합니다. **[!UICONTROL 보고서]** 탭.\
   ![prop_reports.png](assets/proof-reports-350x193.png)

1. 에 설명된 대로 보고서 실행 [보고서 보기](#viewing-reports).
1. 클릭 **[!UICONTROL 필터]**.

1. 페이지 왼쪽에서 다음 필터 옵션 중에서 선택합니다.\
   **[!UICONTROL 증명 유형]:** 보고서에 포함할 증명 유형을 선택합니다.\
   **[!UICONTROL 결정]:** 옵션을 선택하여 특정 결정을 포함하는 증명만 작성되었는지 여부를 결정합니다.\
   **[!UICONTROL 수신자]:** 개별 사용자를 선택하여 선택한 사용자와 공유되는 증명과 관련된 정보를 봅니다.\
   **[!UICONTROL 증명 소유자]:** 개별 사용자를 선택하여 선택한 사용자가 소유한 증명과 관련된 정보를 봅니다.\
   **[!UICONTROL 증명 작성자]:** 개별 사용자를 선택하여 선택한 사용자가 만든 증명과 관련된 정보를 봅니다.\
   **[!UICONTROL 계정]:** 보고서에 포함할 계정을 선택합니다.

1. 클릭 **[!UICONTROL 적용]**.
1. (선택 사항) **[!UICONTROL 최소-최대 범위 표시]** 그래프에 최소값과 최대값을 표시할지 여부를 결정하는 옵션입니다.\
   이 옵션을 선택하면 최소 및 최대 기록 값 사이에 파란색 음영이 표시됩니다.

## 보고서 인쇄

1. 로 이동합니다. **[!UICONTROL 대시보드]** 페이지.
1. 을(를) 클릭합니다. **[!UICONTROL 보고서]** 탭을 클릭한 다음 **[!UICONTROL 인쇄]**.\
   ![prop_reports_print.png](assets/proof-reports-print-350x191.png)

1. 사용 가능한 다양한 인쇄 옵션 중에서 선택합니다.\
   인쇄 옵션은 사용하는 브라우저 및 브라우저 버전에 따라 다릅니다.
