---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 비활성화
description: ' [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리 액세스 권한이 있는 사용자는 시스템에서 더 이상 사용되지 않는 작업 역할을 비활성화할 수 있습니다. 작업 역할을 삭제하는 대신 비활성화하면 해당 역할과 관련된 모든 내역 정보를 유지할 수 있습니다.'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# 작업 역할 비활성화

[!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리 액세스 권한이 있는 사용자는 시스템에서 더 이상 사용되지 않는 작업 역할을 비활성화할 수 있습니다. 작업 역할을 삭제하는 대신 비활성화하면 해당 역할과 관련된 모든 내역 정보를 유지할 수 있습니다.

이전에 비활성화되었던 작업 역할을 다시 활성화할 수도 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 계획*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 라이센스*</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 역할에 대한 관리 액세스</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 작업 역할 비활성화의 영향

작업 역할을 비활성화하면 다음 영역에 더 이상 표시되지 않습니다.

* [!UICONTROL 할당] 자동 완성 필드(작업, 템플릿 작업, 문제, 승인 및 라우팅 규칙의 경우)
* 목록 및 보고서의 [!UICONTROL 할당] 필드
* 사용자 프로필

  >[!NOTE]
  >
  >사용자에게 새 역할을 추가할 때 비활성화된 작업 역할이 표시되지 않습니다. 그러나 사용자가 비활성화되기 전에 작업 역할과 연결된 경우 [!UICONTROL 기본 역할] 및 [!UICONTROL 다른 역할] 필드에 계속 표시됩니다.

* 레이아웃 템플릿 할당을 포함하여 개체에 대한 [!UICONTROL 공유] 대화 상자
* 사용자 정의 양식의 자동 완성 필드
* [!UICONTROL 리소스 풀]의 [!UICONTROL 풀 구성원] 필드
* 사용자가 프로젝트에 대한 청구 요금을 오버라이드할 때 [!UICONTROL 청구 요금] 편집 화면의 [!UICONTROL 작업 역할] 필드
* 프로젝트의 [!UICONTROL Kanban 보드에 할당 추가] 대화 상자
* 누군가 [!DNL Adobe Workfront Scenario Planner]을(를) 사용하고 있을 때 계획 또는 이니셔티브의 [!UICONTROL 작업 역할] 필드.

  [!DNL Scenario Planner]은(는) 새 [!DNL Adobe Workfront] 경험에서만 사용할 수 있으며 추가 라이선스가 필요합니다. [!DNL Workfront Scenario Planner]에 대한 자세한 내용은 [개요 [!DNL Scenario Planner] 개요](../../../scenario-planner/scenario-planner-overview.md)를 참조하세요.

>[!TIP]
>
>비활성화된 역할은 항상 목록, 보고서 및 [!UICONTROL 업무 균형자]와 같은 기타 도구의 필터에 표시됩니다.

## 작업 역할 비활성화 전 고려 사항

과거에 사용했을 수 있는 역할과 관련된 모든 내역 정보를 유지할 수 있도록 사용되지 않게 되는 작업 역할을 삭제하는 것보다 비활성화하는 것이 좋습니다.

>[!NOTE]
>
>비활성화 이전에 작업 역할에 할당된 모든 작업은 할당된 상태로 유지됩니다.

사용하지 않는 작업 역할을 비활성화하기 전에 다음 작업을 수행하는 것이 좋습니다.

* 비활성화하려는 역할에 할당된 객체에 대한 보고서를 작성하고 이를 활성 작업 역할에 재지정합니다. 보고서 작성에 대한 자세한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)를 참조하십시오.

  >[!TIP]
  >
  >비활성화된 역할이 할당된 작업 또는 문제를 필터링할 보고서를 만들 수 있습니다. 그런 다음 보고서를 사용하여 미결 작업 또는 문제를 활성 역할에 재할당합니다.

* 비활성화하려는 작업 역할에 할당된 모든 승인 프로세스, 현재 승인 경로 및 라우팅 규칙 또는 기타 객체에 대한 인벤토리를 작성하여 활성 역할에 재할당합니다.

  >[!TIP]
  >
  >요청 대기열을 사용할 때 라우팅 규칙에서 기본 피할당자로 할당된 작업 역할을 비활성화하면 해당 역할이 유지되고 요청이 여전히 비활성화된 역할로 라우팅됩니다. 팀을 비활성화하기 전에 활성 역할로 라우팅 규칙을 업데이트하는 것이 좋습니다.

  승인 프로세스 및 절차순서 규칙 생성에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## 작업 역할 비활성화

1. [!DNL Adobe Workfront]의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을 클릭합니다.

1. 왼쪽 패널에서 **[!UICONTROL &#x200B;작업 역할].**&#x200B;을 클릭합니다.
1. (선택 사항) **[!UICONTROL 필터]** 드롭다운 메뉴에서 **[!UICONTROL 활성]**&#x200B;을(를) 선택하여 활성 작업 역할만 표시합니다.
1. 비활성화할 작업 역할의 이름을 클릭합니다.
1. **[!UICONTROL 활성 상태임]** 드롭다운 메뉴에서 **[!UICONTROL 아니요]**&#x200B;를 선택합니다.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.

   작업 역할이 비활성화되어 레이아웃 템플릿과 연결된 작업 등에 더 이상 할당할 수 없습니다. [!DNL Workfront]의 모든 작업 역할 사용에 대한 자세한 내용은 [작업 역할 개요](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)를 참조하십시오.
