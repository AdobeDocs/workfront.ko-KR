---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: ' [!DNL Workfront Proof]에서 보고서 실행'
description: Workfront Proof을 사용하면 보고서를 볼 수 있으므로 팀의 작업 진행 상황과 효율성을 추적할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# [!DNL Workfront Proof]에서 보고서 실행


>[!IMPORTANT]
>
>* <span class="previe">보고 기능은 [!DNL Workfront Proof]에서 더 이상 사용할 수 없습니다. 보고 탭이 여전히 표시되지만 데이터가 정확하지 않습니다.</span>
> 
>* 이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

Workfront Proof을 사용하면 보고서를 볼 수 있으므로 팀의 작업 진행 상황과 효율성을 추적할 수 있습니다.

[!DNL Workfront Proof] 계정에서 만든 증명 수, 각 증명에 연결된 버전 수, 반환 시간 등을 쉽게 볼 수 있습니다.

## 전제 조건

보고서를 사용할 수 있는지 여부는 [!DNL Workfront Proof] 계정 유형 및 사용자 권한 수준에 따라 다릅니다.

* [계정 사전 요구 사항](#account-prerequisites)
* [사용자 사전 요구 사항](#user-prerequisites)

### 계정 사전 요구 사항 {#account-prerequisites}

보고 정보는 Premium 플랜에서만 사용할 수 있습니다.

### 사용자 사전 요구 사항 {#user-prerequisites}

보고 정보는 계정의 모든 증명에 대한 전체 액세스 권한이 있는 사용자(예:  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)에서 [증명 권한 프로필 이상이 있는 사용자)에게만 제공됩니다.

이 패널에서 다음 작업을 수행할 수 있습니다.

* 표시된 데이터의 시간 범위 제어
* 시간 경과에 따른 지표 변경 분석
* 마우스로 가리키면 선택한 시점의 세부 정보를 확인합니다.
* 선택한 시간 범위에서 생성된 총 증명 수를 확인합니다.
* 완료된 증명 세트에 포함된 평균 버전 수를 확인합니다.

## 보고서 보기 {#viewing-reports}

1. **[!UICONTROL 대시보드]** 페이지로 이동합니다.
1. **[!UICONTROL 보고서]** 탭을 클릭합니다.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. **[!UICONTROL 시간대]** 드롭다운 메뉴에서 지난 24시간, 7일, 30일, 90일 또는 사용자 지정 기간 내에 만든 증명에 대한 정보를 표시할지 여부를 선택합니다.\
   사용자 지정 기간을 선택하는 경우 시작 날짜와 종료 날짜를 선택한 다음 **[!UICONTROL 적용]**&#x200B;을 클릭합니다.\
   선택한 기간에 대해 다음 정보가 표시됩니다.\
   **만들어진 증명:** 선택한 기간 내에 만들어진 증명 수입니다.\
   **증명당 버전:** 선택한 기간 내에 완료된 모든 증명(변경 승인됨 또는 승인됨)에 대한 증명당 평균 버전 수입니다.\
   **반환 시간:** 첫 번째 버전을 만든 시점부터 최종 버전을 결정한 시점까지의 평균 시간입니다.\
   **첫 번째 활동 시간:** 증명을 만든 시점부터 증명에 대한 첫 번째 활동 시간까지의 평균 시간입니다.\
   **지연 증명:** 선택한 기간 내에 하나 이상의 버전이 지연된 완료된 증명(변경 승인됨 또는 변경 승인됨)의 평균 비율입니다.\
   **댓글 및 답글:** 선택한 기간 내에 모든 증명에 대해 수행된 평균 댓글 및 답글 수입니다.

1. (선택 사항) **[!UICONTROL 최소-최대 범위 표시]** 옵션을 선택하거나 선택 해제하여 최소값과 최대값을 그래프에 표시할지 여부를 결정합니다.\
   이 옵션을 선택하면 기록된 최소 값과 최대 값 사이에 파란색 음영이 표시됩니다.

1. (선택 사항) [보고서 필터링](#filtering-reports)에 설명된 대로 표시되는 데이터를 필터링할 수 있습니다.

## 보고서 필터링 {#filtering-reports}

기본적으로 보고서에 표시되는 데이터에는 [!DNL Workfront Proof] 시스템의 모든 정보가 포함됩니다. 필터를 사용하여 요구 사항과 관련된 정보만 표시할 수 있습니다.

보고 정보를 필터링하려면 다음을 수행합니다.

1. **[!UICONTROL 대시보드]** 페이지로 이동합니다.
1. **[!UICONTROL 보고서]** 탭을 클릭합니다.\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. [보고서 보기](#viewing-reports)에 설명된 대로 보고서를 실행합니다.
1. **[!UICONTROL 필터]**&#x200B;를 클릭합니다.

1. 페이지 왼쪽의 다음 필터 옵션 중에서 선택합니다.\
   **[!UICONTROL 증명 유형]:** 보고서에 포함할 증명 유형을 선택합니다.\
   **[!UICONTROL 결정]:** 옵션을 선택하여 특정 결정이 포함된 증명만 수행되었는지 여부를 확인합니다.\
   **[!UICONTROL 받는 사람]:** 선택한 사용자와 공유된 증명과 관련된 정보를 보려면 개별 사용자를 선택하십시오.\
   **[!UICONTROL 증명 소유자]:** 선택한 사용자가 소유한 증명과 관련된 정보를 보려면 개별 사용자를 선택하십시오.\
   **[!UICONTROL 증명 작성자]:** 선택한 사용자가 만든 증명과 관련된 정보를 보려면 개별 사용자를 선택하십시오.\
   **[!UICONTROL 계정]:** 보고서에 포함할 계정을 선택합니다.

1. **[!UICONTROL 적용]**&#x200B;을 클릭합니다.
1. (선택 사항) **[!UICONTROL 최소-최대 범위 표시]** 옵션을 선택하거나 선택 해제하여 최소값과 최대값을 그래프에 표시할지 여부를 결정합니다.\
   이 옵션을 선택하면 기록된 최소 값과 최대 값 사이에 파란색 음영이 표시됩니다.

## 보고서 인쇄

1. **[!UICONTROL 대시보드]** 페이지로 이동합니다.
1. **[!UICONTROL 보고서]** 탭을 클릭한 다음 **[!UICONTROL 인쇄]**&#x200B;를 클릭합니다.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. 사용 가능한 다양한 인쇄 옵션 중에서 선택합니다.\
   인쇄 옵션은 사용하는 브라우저 및 브라우저 버전에 따라 다릅니다.
