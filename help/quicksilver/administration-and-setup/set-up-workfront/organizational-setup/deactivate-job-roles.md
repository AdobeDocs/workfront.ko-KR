---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 작업 역할 비활성화
description: 로서의 [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리자 액세스 권한이 있는 사용자는 시스템에서 사용되지 않는 작업 역할을 비활성화할 수 있습니다. 작업 역할을 삭제하는 대신 비활성화하면 작업 역할과 연관된 모든 기록 정보를 유지할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# 작업 역할 비활성화

로서의 [!DNL Adobe Workfront] 관리자 또는 작업 역할에 대한 관리자 액세스 권한이 있는 사용자는 시스템에서 사용되지 않는 작업 역할을 비활성화할 수 있습니다. 작업 역할을 삭제하는 대신 비활성화하면 작업 역할과 연관된 모든 기록 정보를 유지할 수 있습니다.

이전에 비활성화된 작업 역할을 다시 활성화할 수도 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 계획*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 라이센스*</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 역할에 대한 관리자 액세스</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 작업 역할 비활성화의 영향

작업 역할을 비활성화하면 더 이상 다음 영역에 표시되지 않습니다.

* 다음 [!UICONTROL 지정] typeahead 필드(작업, 템플릿 작업, 문제, 승인 및 라우팅 규칙)
* 다음 [!UICONTROL 지정] 목록 및 보고서 필드
* 사용자 프로필

   >[!NOTE]
   >
   >사용자에게 새 역할을 추가하면 비활성화된 작업 역할이 표시되지 않습니다. 그러나 그것은 계속해서 [!UICONTROL 기본 역할] 및 [!UICONTROL 기타 역할] 사용자가 비활성화되기 전에 작업 역할과 연관된 경우 필드입니다.

* 다음 [!UICONTROL 공유] 레이아웃 템플릿 할당 포함 객체의 대화 상자
* 사용자 지정 양식의 필드 입력
* 다음 [!UICONTROL 풀 구성원] 필드 [!UICONTROL 리소스 풀]
* 다음 [!UICONTROL 작업 역할] 필드 [!UICONTROL 청구 비율] 사용자가 프로젝트에 대한 청구 비율을 재정의할 때 화면 편집
* 다음 [!UICONTROL 간판 보드에 지정 추가] 프로젝트의 대화 상자
* 다음 [!UICONTROL 작업 역할] 누군가 Analytics Mobile Apps 또는 Analytics Premium을 사용할 때 [!DNL Adobe Workfront Scenario Planner].

   다음 [!DNL Scenario Planner] 는 새로운 [!DNL Adobe Workfront] 경험을 사용하려면 추가 라이센스가 필요합니다. 에 대한 정보 [!DNL Workfront Scenario Planner]를 참조하십시오. [다음 [!DNL Scenario Planner] 개요](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>비활성화된 역할은 항상 목록, 보고서 및 기타 도구(예: [!DNL Workload Balancer].

## 작업 역할을 비활성화하기 전의 고려 사항

이전에 사용했을 수 있는 역할과 연관된 모든 기록 정보를 유지할 수 있도록 사용되지 않는 작업 역할을 삭제하는 대신 비활성화하는 것이 좋습니다.

>[!NOTE]
>
>비활성화하기 전에 작업 역할에 할당된 모든 작업은 할당된 상태로 유지됩니다.

사용하지 않은 작업 역할을 비활성화하기 전에 다음을 수행하는 것이 좋습니다.

* 비활성화하려는 역할에 지정된 객체에 대한 보고서를 작성하여 활성 작업 역할에 재지정합니다. 보고서 작성에 대한 자세한 내용은 [보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >비활성화된 역할이 할당된 모든 작업 또는 문제에 대해 필터링할 보고서를 만들 수 있습니다. 그런 다음 보고서를 사용하여 미결 태스크나 문제를 활성 역할에 재지정합니다.

* 모든 승인 프로세스, 현재 승인 경로, 공정순서 규칙 또는 비활성화하려는 작업 역할에 할당된 다른 객체의 인벤토리를 수행하여 활성 역할에 재지정합니다.

   >[!TIP]
   >
   >요청 큐를 사용할 때, 라우팅 규칙에서 기본 할당자로 지정된 작업 역할을 비활성화하면 역할은 그대로 유지되며 요청은 여전히 비활성화된 역할로 라우팅됩니다. 팀을 비활성화하기 전에 활성 역할이 있는 라우팅 규칙을 업데이트하는 것이 좋습니다.

   승인 프로세스 및 공정순서 규칙 생성에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [작업 항목에 대한 승인 프로세스 생성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## 작업 역할 비활성화

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 을 클릭합니다&#x200B;. **[!UICONTROL 작업 역할].**
1. (선택 사항)에서 **[!UICONTROL 필터]** 드롭다운 메뉴에서 **[!UICONTROL 활성]** 활성 작업 역할만 표시합니다.
1. 비활성화할 작업 역할의 이름을 클릭합니다.
1. 에서 **[!UICONTROL 활성 상태]** 드롭다운 메뉴에서 **[!UICONTROL 아니요]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

   작업 역할이 비활성화되어 더 이상 작업, 레이아웃 템플릿 관련 등에 할당할 수 없습니다. 의 모든 작업 역할 사용에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오. [작업 역할 개요](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
