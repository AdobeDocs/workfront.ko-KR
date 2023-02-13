---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 회사 레벨에서 직무 역할 청구 비율 대체
description: 작업 역할이 생성되면 해당 역할에 대한 시간별 청구 비율을 선택할 수 있습니다. 회사에 고유한 시간별 청구 비율을 생성할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 회사 레벨에서 직무 역할 청구 비율 대체

작업 역할이 생성되면 해당 역할에 대한 시간별 청구 비율을 선택할 수 있습니다. 회사에 고유한 시간별 청구 비율을 생성할 수 있습니다.

프로젝트 레벨에서 회사 수준의 청구 비율이 프로젝트 레벨 비율을 대체하도록 허용하는 옵션을 활성화할 수 있습니다. 자세한 내용은 [회사 수준 청구 단가로 프로젝트 레벨 청구 비율 대체](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>시스템 관리자가 아닌 회사에 대한 관리자 액세스</p> <p>[!UICONTROL Edit] 재무 데이터 액세스</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 특정 Job 역할에 사용되는 설정된 청구 비율을 대체 또는 변경합니다

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 회사]**.
1. Job 역할이 할당된 회사를 찾습니다.
1. 클릭 **[!UICONTROL 회사 편집]** 오른쪽 상단 모서리에서
1. 에서 **[!UICONTROL 청구 비율]** 섹션에서 편집할 작업 역할을 선택하고 해당 작업 역할에 대한 새 청구 비율을 입력합니다 **[!UICONTROL 회사 청구 비율]** 상자.

   >[!NOTE]
   >
   >프로젝트에서 변경된 작업 역할 비율은 해당 프로젝트에만 영향을 줍니다. 회사 수준에서 변경된 비율은 모든 프로젝트에 영향을 줍니다. 자세한 내용은 [Job 역할 청구 비율 대체 및 프로젝트에 대한 수익 계산 개요](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
