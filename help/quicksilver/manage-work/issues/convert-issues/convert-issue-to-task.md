---
product-area: projects
navigation-topic: convert-issues
title: Adobe Workfront에서 문제를 작업으로 변환
description: 문제를 제출한 후 문제를 완료하기 위해 추가 작업을 수행해야 하는 경우 문제를 작업으로 변환할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 2%

---

# Adobe Workfront에서 문제를 작업으로 변환

문제를 제출한 후 문제를 완료하기 위해 추가 작업을 수행해야 하는 경우 문제를 작업으로 변환할 수 있습니다.

문제 변환에 대한 일반적인 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제, 작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 보기</p> <p>프로젝트에 대한 권한 기여</p> <p>문제가 변환된 후 작업에 대한 관리 권한을 받습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제를 작업으로 변환

1. 프로젝트로 이동하여 를 클릭합니다 [!UICONTROL **문제** ] 왼쪽 패널에 표시됩니다.
1. 변환할 문제를 클릭하여 문제의 랜딩 페이지로 이동합니다.
1. 을(를) 클릭합니다. [!UICONTROL **자세히**] 문제 메뉴에서 [!UICONTROL **작업으로 변환**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >문제가 승인 프로세스와 연결되어 있거나 이미 해결 객체와 연결되어 있는 경우 Workfront에서는 의 맨 위에 경고가 표시됩니다 [!UICONTROL 프로젝트로 변환] 상자를 사용하여 전환 중에 승인이 제거되거나 확인 객체를 덮어쓰게 됩니다. 자세한 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

1. 에서 작업 이름 업데이트 [!UICONTROL 작업 이름] 섹션을 참조하십시오. 기본적으로 작업의 이름은 원래 문제와 동일합니다.

   ![](assets/convert-to-task-box-nwe.png)

1. 클릭 [!UICONTROL **대상 프로젝트**]&#x200B;를 입력한 다음 새 작업을 배치할 프로젝트의 이름을 [!UICONTROL **대상 프로젝트**] 필드를 선택하고 목록에 표시될 때 선택합니다. 기본적으로 문제의 프로젝트가 선택됩니다.

1. 클릭 [!UICONTROL **개요**]&#x200B;를 입력한 다음 를 입력합니다 [!UICONTROL **설명**] Analytics Mobile Apps 또는 Analytics Premium이 없습니다.

   >[!TIP]
   >
   >   시스템 또는 그룹 관리자는 레이아웃 템플릿을 수정하여 변환 상자의 왼쪽 패널에 있는 섹션의 순서를 변경할 수 있습니다.

1. (선택 사항 및 조건부) [!UICONTROL **옵션**]&#x200B;아래에서 옵션을 선택합니다.

   Workfront 관리자 또는 그룹 관리자는 문제를 변환하는 동안 이러한 환경 설정이 표시되려면 먼저 이러한 환경 설정을 활성화해야 합니다.

   * [!UICONTROL **원래 문제를 유지하고 이 작업에 해결 방법을 연결합니다**]

      선택하지 않으면 원래 문제가 삭제됩니다.

      >[!NOTE]
      >
      >문제에 대한 액세스 권한 또는 삭제 권한이 없는 사용자는 이 설정의 상태에 관계없이 변환 중인 문제를 삭제할 수 없습니다. 문제에 대한 액세스 및 권한에 대한 자세한 내용은 다음을 참조하십시오.
      >   
      >   * [문제에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
      >   * [문제 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


   * [!UICONTROL **이 작업에 액세스할 수 있도록 허용(사용자 이름)**]

      선택하지 않으면 문제의 기본 연락처는 새 작업에 액세스할 수 없습니다.

   * [!UICONTROL **문제의 계획된 완료 일자 유지**]

      선택하지 않으면 [!UICONTROL 계획 완료 일자] 새 작업의 값은 [!UICONTROL 계획 시작 날짜] Analytics JavaScript에서 액세스 권한을 부여합니다. 다음 [!UICONTROL 계획 시작 날짜] 새 작업의 경우 새 작업의 시스템 환경 설정에 따라 설정됩니다.

      >[!NOTE]
      >
      >
      >여기에 표시되는 옵션은 Workfront 관리자가 시스템의 모든 사용자를 위해 구성한 방식에 따라 다릅니다. 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
      >
      >또는 조직의 최상위 그룹이 별도로 구성한 경우 여기에 표시되는 옵션은 6단계에서 선택한 프로젝트와 연결된 그룹에 따라 달라집니다. 자세한 내용은 [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (선택 사항) [!UICONTROL **사용자 지정 Forms**] 새 작업에 사용할 사용자 지정 양식을 첨부합니다.

   >[!TIP]
   >
   >문제에 첨부된 다중 개체 사용자 지정 양식이 문제와 작업에 모두 사용하도록 구성된 경우 양식이 기본적으로 첨부됩니다. 변환 시 문제 양식에 저장된 모든 정보는 작업에 대해 유지됩니다.
   >
   >대상 프로젝트에 프로젝트를 편집할 때 작업 기본 사용자 지정 Forms 필드에 정의된 기본 양식이 있는 경우 해당 작업 양식도 새 작업에 추가됩니다. 원래 문제와 기본 작업 양식의 필드 간에 공통되는 모든 사용자 지정 필드는 문제 필드의 정보로 미리 채워집니다.

1. 클릭 [!UICONTROL **작업으로 변환**].

   원래 문제를 삭제하기로 결정한 경우 문제가 이제 지정된 프로젝트의 작업입니다.

   또는

   이제 문제가 선택한 프로젝트의 새 작업에 연결되며, 원래 문제를 유지하기로 결정한 경우 작업이 완료되면 완료됩니다.

   일부 문제 필드가 작업에 전송됩니다. 자세한 내용은 [프로젝트 및 작업에 대한 원래 문제 정보 보기](#view-original-issue-information-on-projects-and-tasks) 섹션에 자세히 설명되어 있습니다.

1. (선택 사항) 필요에 따라 작업을 계속 편집합니다.

## 프로젝트 및 작업에 대한 원래 문제 정보 보기 {#view-original-issue-information-on-projects-and-tasks}

프로젝트 및 작업 목록, 보고서 또는 프로젝트 세부 정보 영역에서 원래 문제 정보를 볼 수 있습니다. 보고서 작성에 대한 자세한 내용은 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

다음 표는 변환된 프로젝트 및 작업에서 표시되는 문제 필드를 보여줍니다.

| 문제 필드 | 프로젝트 또는 작업 필드 | 프로젝트 목록 또는 보고서 | 프로젝트 세부 사항 영역 | 작업 목록 또는 보고서 | 작업 세부 사항 영역 |
|---|---|---|---|---|---|
| [!UICONTROL 문제 이름] | [!UICONTROL 전환된 문제 이름] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL 기본 담당자] | [!UICONTROL 변환된 문제 작성자 이름] | ✔ | ✔ | ✔ |
| [!UICONTROL 시작 날짜] | [!UICONTROL 전환된 문제 입력 일자] | ✔ |  | ✔ |


>[!CAUTION]
>
>만약 [!UICONTROL 기본 연락처] 문제가 변경되거나 문제가 변환된 후 프로젝트나 작업에서 연결이 해제되면 [!UICONTROL 변환된 문제 작성자 이름 ]업데이트되지 않고 원본이 표시됩니다 [!UICONTROL 기본 연락처] 문제가 전환될 때 문제가 해결되었습니다.
