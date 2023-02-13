---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 프로젝트에 대한 타임라인 재계산 구성
description: 타임라인을 다시 계산하면 프로젝트 외부의 힘이 프로젝트 타임라인에 미치는 영향을 확인할 수 있습니다. 프로젝트의 타임라인은 프로젝트에 대한 계획 및 예상 날짜를 나타냅니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 프로젝트에 대한 타임라인 재계산 구성

타임라인을 다시 계산하면 프로젝트 외부의 힘이 프로젝트 타임라인에 미치는 영향을 확인할 수 있습니다. 프로젝트의 타임라인은 프로젝트에 대한 계획 및 예상 날짜를 나타냅니다.

로서의 [!DNL Adobe Workfront] 관리자는 시스템의 모든 프로젝트에 대한 타임라인을 수동으로 재계산할 수 있습니다. 프로젝트 소유자는 개별 프로젝트에 대한 타임라인을 수동으로 다시 계산할 수도 있습니다. 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

이 문서에서는 [!DNL Workfront] 관리자는 언제, 어떻게 [!DNL Workfront] 에서 프로젝트 환경 설정을 구성하여 프로젝트 타임라인을 자동으로 계산합니다. [!UICONTROL 설정] 영역.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자 액세스 수준</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 자동 다시 계산 구성

로서의 [!DNL Adobe Workfront] 관리자는 [!DNL Workfront] 프로젝트 타임라인을 자동으로 다시 계산합니다. [!DNL Workfront] 매일 밤 또는 프로젝트 범위가 변경되거나 둘 다 프로젝트 타임라인을 재계산할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 프로젝트].**

1. 에서 **[!UICONTROL 타임라인]** 섹션에서 아래 설정을 활성화하거나 비활성화합니다. 기본적으로 두 설정이 모두 활성화됩니다.

   * **매일 밤:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] 상태가 [!UICONTROL 현재] 그리고 지난 3개월 동안 업데이트되었습니다.

      이 경우 [!DNL Workfront] 가 있는 모든 프로젝트의 타임라인을 다시 계산합니다. [!UICONTROL 업데이트 유형] 의 [!UICONTROL 자동] 또는 [!UICONTROL 자동 및 변경 시].

   * **프로젝트의 범위가 변경되는 경우**: 프로젝트 범위 변경을 구성하는 사항에 대한 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      이 경우 [!DNL Workfront] 업데이트 유형이 있는 모든 프로젝트의 타임라인을 재계산합니다. [!UICONTROL 자동 및 변경 시] 또는 [!UICONTROL 변경만 시].
프로젝트 업데이트 유형에 대한 자세한 내용은 [프로젝트 업데이트 유형 개요](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   시스템의 모든 프로젝트의 타임라인은 각 프로젝트의 업데이트 유형에 따라 자동으로 다시 계산됩니다.

## 전체 타임라인에 대한 타임라인 다시 계산 [!DNL Workfront] 인스턴스

를 실행할 수 있습니다 [!UICONTROL 타임라인 다시 계산] 진단에서 모든 타임라인을 수동으로 다시 계산하기 [!DNL Workfront] 시스템. 이를 통해 모든 프로젝트 관리자는 계획 날짜와 예상 날짜 모두에 외부 변경 내용이 미치는 영향을 즉시 확인할 수 있습니다. 자세한 내용은 [진단 기능을 사용하여 자동화된 프로세스를 트리거합니다](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
