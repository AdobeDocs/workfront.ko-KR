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
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 1%

---

# 사용자 정의 영역 활성화

<!--Audited: 11/2024-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. [!DNL Adobe Workfront Planning]을(를) 구입한 모든 고객의 미리 보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

조직의 분기가 달력 날짜(예: 업무일 또는 쇼핑일) 이외의 특정 기준을 기반으로 하는 경우, 보고를 위해 사용자 정의 분기를 만들 수 있습니다.

<div class="preview">

회사에서 구매한 제품에 따라 Workfront 설정 영역에서 다음 분기 수를 구성할 수 있습니다.

* [!DNL Workfront]만 구입한 고객은 [!DNL Adobe Workfront] 시스템에 대해 최대 8개의 사용자 정의 분기를 구성할 수 있습니다.
* [!DNL Workfront] 및 [!DNL Workfront Planning]을(를) 구매한 고객은 [!DNL Planning]에서도 사용할 수 있는 [!DNL Workfront] 시스템에 대해 최대 100분기를 구성할 수 있습니다.

</div>

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Workfront] 시스템에 대한 사용자 정의 영역 설정

{{step-1-to-setup}}

1. **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 프로젝트].**&#x200B;을 클릭합니다.

1. **[!UICONTROL 타임라인]** 섹션에서 **[!UICONTROL 사용자 정의 영역 사용]**&#x200B;을 선택합니다.

1. 사용자 정의 분기의 이름을 입력합니다(예: &quot;2021년 1분기 회계&quot;).
1. 사용자 정의 분기의 시작 및 종료 날짜를 선택합니다.

   ![사용자 지정 분기](assets/custom-quarters-nwe.png)

1. (선택 사항) 시스템에 사용자 정의 영역을 추가하려면 **[!UICONTROL 사용자 정의 영역 추가]**&#x200B;를 클릭합니다.

   >[!IMPORTANT]
   >
   > <span class="preview">회사에서 [!DNL Workfront Planning]을(를) 구입한 경우 분기 간에 차이가 있거나 중복되는 경우 사용자 정의 분기를 저장할 수 없습니다. </span>
   ><span class="preview">![겹침 경고가 있는 사용자 지정 분기](assets/custom-quarters-with-overlap-warning.png)</span>
   >[!DNL Workfront]명의 고객에게만 분기 간 간격 및 중복이 허용됩니다.

1. (선택 사항 및 조건부) 회사에서 [!DNL Workfront Planning] 없이 [!DNL Workfront]만 구입한 경우 회계 분기를 참조하는 보고 요소를 만듭니다.


   **예:** [!UICONTROL 프로젝트] 목록에 대한 필터를 만들고 사용자 정의 분기를 참조하는 프로젝트의 계획된 완료 날짜를 포함합니다.

   ![사용자 지정 분기가 있는 프로젝트 필터](assets/example-of-project-filter-with-custom-quarters.png)

   &quot;이번 분기&quot;, &quot;다음 분기&quot; 및 &quot;지난 분기&quot;에 대한 참조가 사용자 정의 분기에 대한 새 참조로 대체됩니다.

   보고 요소에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)를 참조하십시오.

   필터 만들기에 대한 자세한 내용은 [필터 만들기 또는 편집 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)을 참조하세요.
1. <span class="preview">(선택 사항 및 조건부) [!DNL Workfront Planning]에 액세스할 수 있는 경우 레코드 유형 페이지로 이동하여 타임라인 보기를 엽니다. 보기에 새 사용자 정의 분기가 표시됩니다. </span>
