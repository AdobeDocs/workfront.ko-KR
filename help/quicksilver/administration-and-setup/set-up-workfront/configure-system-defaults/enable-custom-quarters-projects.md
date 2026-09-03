---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 사용자 정의 영역 활성화
description: '조직의 분기가 달력 날짜(예: 업무일 또는 쇼핑일) 이외의 특정 기준을 기반으로 하는 경우, 보고를 위해 사용자 정의 분기를 만들 수 있습니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: 902
ht-degree: 2%

---

# 사용자 정의 영역 활성화

<!--Audited: 03/2026-->

<!--remove Production and Preview references at release-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


조직의 분기가 달력 날짜(예: 업무일 또는 쇼핑일) 이외의 특정 기준을 기반으로 하는 경우, 보고를 위해 사용자 정의 분기를 만들 수 있습니다.

회사에서 구매한 제품에 따라 Workfront 설정 영역에서 다음 분기 수를 구성할 수 있습니다.

* [!DNL Workfront]만 구입한 고객은 [!DNL Adobe Workfront] 시스템에 대해 최대 8개의 사용자 정의 분기를 구성할 수 있습니다.
* [!DNL Workfront] 및 [!DNL Workfront Planning]을(를) 구매한 고객은 [!DNL Planning]에서도 사용할 수 있는 [!DNL Workfront] 시스템에 대해 최대 100분기를 구성할 수 있습니다.

<div class="preview">

* [!DNL Workfront] 및 [!DNL Workfront Planning]을(를) 구매한 고객은 각 사용자 정의 분기에 대해 사용자 정의 주를 구성할 수 있습니다. 사용자 지정 주가 [!DNL Planning] 타임라인 보기에 표시됩니다.

</div>

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 패키지</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>[!UICONTROL Workflow Standard] 또는 [!UICONTROL Workfront Plan] 라이선스</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## [!DNL Workfront] 시스템에 대한 사용자 정의 영역 설정

사용자 정의 영역 설정은 사용하는 환경에 따라 다릅니다.

### 프로덕션 환경에서 [!DNL Workfront] 시스템에 대한 사용자 정의 분기 설정

{{step-1-to-setup}}

1. **[!UICONTROL 사용자 지정 분기]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 사용자 정의 영역 사용]**&#x200B;을 선택합니다.

1. 사용자 정의 분기의 이름을 입력합니다(예: &quot;2021년 1분기 회계&quot;).
1. 사용자 정의 분기의 시작 및 종료 날짜를 선택합니다.

   ![사용자 지정 분기](assets/custom-quarters-nwe.png)

1. (선택 사항) 시스템에 사용자 정의 영역을 추가하려면 **[!UICONTROL 사용자 정의 영역 추가]**&#x200B;를 클릭합니다.

   >[!IMPORTANT]
   >
   > 회사에서 [!DNL Workfront Planning]을(를) 구입한 경우 분기 간에 차이가 있거나 중복되는 경우 사용자 정의 분기를 저장할 수 없습니다.
   >![겹침 경고가 있는 사용자 지정 분기](assets/custom-quarters-with-overlap-warning.png)
   >[!DNL Workfront]명의 고객에게만 분기 간 간격 및 중복이 허용됩니다.

1. (선택 사항 및 조건부) 회사에서 [!DNL Workfront Planning] 없이 [!DNL Workfront]만 구입한 경우 회계 분기를 참조하는 보고 요소를 만듭니다.

   **예:** [!UICONTROL 프로젝트] 목록에 대한 필터를 만들고 사용자 정의 분기를 참조하는 프로젝트의 계획된 완료 날짜를 포함합니다.

   ![사용자 지정 분기가 있는 프로젝트 필터](assets/example-of-project-filter-with-custom-quarters.png)

   &quot;이번 분기&quot;, &quot;다음 분기&quot; 및 &quot;지난 분기&quot;에 대한 참조가 사용자 정의 분기에 대한 새 참조로 대체됩니다.

   보고 요소에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)를 참조하십시오.

   필터 만들기에 대한 자세한 내용은 [필터 만들기 또는 편집 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.
1. (선택 사항 및 조건부) 회사에서 Workfront Planning을 구입하고 [!DNL Workfront Planning]에 대한 액세스 권한이 있는 경우 레코드 유형 페이지로 이동하여 타임라인 보기를 엽니다. 보기에 새 사용자 정의 분기가 표시됩니다.
자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.

<div class="preview">

### 미리 보기 환경에서 [!DNL Workfront] 시스템에 대한 사용자 지정 분기 설정

>[!NOTE]
>
>조직에서 워크플로 패키지 외에 Planning 패키지를 구매했거나 Workfront Planning을 독립형 패키지로 구매한 경우, 사용자 정의 분기 외에 사용자 정의 주를 구성할 수 있습니다.
> 
>Workfront 보고서 및 목록에는 사용자 지정 주를 사용할 수 없습니다.

{{step-1-to-setup}}

1. **[!UICONTROL 사용자 지정 분기]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 사용자 정의 영역 사용]**&#x200B;을 선택합니다.

1. 사용자 정의 분기의 이름을 입력합니다. 예를 들어 &quot;2021년 1분기 회계&quot;
1. 사용자 정의 분기의 시작 및 종료 날짜를 선택합니다.

1. (선택 사항) **새 사용자 지정 주 시퀀스 시작** 옵션을 선택합니다.

   이 옵션을 선택하면 이 옵션은 계획 타임라인 보기에서 사용자 정의 분기의 시작을 분기의 첫 번째 사용자 정의 주의 시작으로 설정합니다.
1. (선택 사항) **사용자 지정 주 레이블 형식** 영역에서 사용자 지정 주 레이블에 대한 **형식**&#x200B;을(를) 선택합니다. 다음 선택 사항 중 하나를 선택합니다.

   * **W1, W2, W3 ...** . 기본 형식입니다.
   * **FW1, FW2, FW3...**
   * **주1, 주2, 주3, ...**
   * **사용자 지정**

1. (조건부) **형식** 필드에 대해 **사용자 지정**&#x200B;을(를) 선택한 경우 **사용자 지정 레이블**&#x200B;을(를) 입력하여 사용자 지정 주를 식별하십시오.

   사용자 정의 주가 Planning 타임라인 보기에 표시됩니다.

   >[!TIP]
   >
   >사용자 지정 레이블을 추가할 때 최대 100자를 입력할 수 있습니다.
   >
   >첫 번째 주의 이름을 표시할 수 있으며 다음 주는 같은 레이블을 사용하고 그 뒤에 순차적 번호를 사용합니다.
   >
   >예를 들어 &quot;회계 주&quot;의 **사용자 지정 레이블**&#x200B;은 &quot;회계 주 1, 회계 주 2, 회계 주 3 ...&quot;의 레이블을 추가합니다. 를 시퀀스 내 나머지 주에 연결합니다.

1. (선택 사항) 시스템에 사용자 정의 영역을 추가하려면 **[!UICONTROL 사용자 정의 영역 추가]**&#x200B;를 클릭합니다.

   >[!IMPORTANT]
   >
   > 회사에서 [!DNL Workfront Planning]을(를) 구입한 경우 분기 간에 차이가 있거나 중복되는 경우 사용자 정의 분기를 저장할 수 없습니다.
   >![겹침 경고가 있는 사용자 지정 분기](assets/custom-quarters-with-overlap-warning-red-outline.png)
   >[!DNL Workfront]명의 고객에게만 분기 간 간격 및 중복이 허용됩니다.

1. (선택 사항 및 조건부) Workfront에서 사용자 정의 분기를 보려면 사용자 정의 분기를 참조하는 보고 요소를 만듭니다.

   **예:** [!UICONTROL 프로젝트] 목록에 대한 필터를 만들고 사용자 정의 분기를 참조하는 프로젝트의 계획된 완료 날짜를 포함합니다.

   ![사용자 지정 분기가 있는 프로젝트 필터](assets/example-of-project-filter-with-custom-quarters.png)

   &quot;이번 분기&quot;, &quot;다음 분기&quot; 및 &quot;지난 분기&quot;에 대한 참조가 사용자 정의 분기에 대한 새 참조로 대체됩니다.

   보고 요소에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)를 참조하십시오.

   필터 만들기에 대한 자세한 내용은 [필터 만들기 또는 편집 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.
1. (선택 사항 및 조건부) Workfront Planning에서 사용자 정의 분기 및 주를 보려면 레코드 유형 페이지로 이동하여 타임라인 보기를 엽니다. 보기에는 새 사용자 정의 분기 및 주가 표시됩니다.

자세한 내용은 [타임라인 보기 관리](/help/quicksilver/planning/views/manage-the-timeline-view.md)를 참조하십시오.

</div>
