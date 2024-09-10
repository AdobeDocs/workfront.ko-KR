---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 프로젝트에 대한 타임라인 재계산 구성
description: 타임라인을 다시 계산하면 관리자는 프로젝트 외부의 힘이 프로젝트의 타임라인에 미치는 영향을 확인할 수 있습니다. 프로젝트의 타임라인은 프로젝트의 계획된 일자와 예상 일자를 나타냅니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 프로젝트에 대한 타임라인 재계산 구성

타임라인을 다시 계산하면 관리자는 프로젝트 외부의 힘이 프로젝트의 타임라인에 미치는 영향을 확인할 수 있습니다. 프로젝트의 타임라인은 프로젝트의 계획된 일자와 예상 일자를 나타냅니다.

[!DNL Adobe Workfront] 관리자는 시스템의 모든 프로젝트에 대한 타임라인을 수동으로 다시 계산할 수 있습니다. 프로젝트 소유자는 개별 프로젝트에 대한 타임라인을 수동으로 다시 계산할 수도 있습니다. 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)을 참조하십시오.

이 문서에서는 [!DNL Workfront] 관리자로서 [!UICONTROL 설정] 영역에서 프로젝트 환경 설정을 구성하여 [!DNL Workfront]이(가) 프로젝트 타임라인을 자동으로 계산하는 방법과 시기를 확인하는 방법에 대해 설명합니다.

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

## 자동 재계산 구성

[!DNL Adobe Workfront] 관리자는 [!DNL Workfront]이(가) 프로젝트 타임라인을 자동으로 다시 계산하는 시기를 구성할 수 있습니다. [!DNL Workfront]은(는) 매일 밤 또는 프로젝트 범위가 변경될 때 또는 둘 다 프로젝트 타임라인을 다시 계산할 수 있습니다.

{{step-1-to-setup}}

1. **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 프로젝트].**&#x200B;을 클릭합니다.

1. **[!UICONTROL 타임라인]** 섹션에서 아래 설정 중 하나 또는 모두를 활성화하거나 비활성화합니다. 기본적으로 두 설정이 모두 활성화됩니다.

   * **매일 밤:** [!DNL Workfront&#x200B;&#x200B;&#x200B;]은(는) 상태가 [!UICONTROL 현재]이고 지난 3개월 동안 업데이트된 프로젝트에 대해서만 24시간마다 한 번씩 밤에 타임라인을 다시 계산합니다. 시스템 로드 및 기타 요인에 따라 재계산 시간이 24시간 이상 지연될 수 있습니다.

     이 경우 [!DNL Workfront]은(는) [!UICONTROL 업데이트 형식]이(가) [!UICONTROL 자동] 또는 [!UICONTROL 자동 및 변경 시]인 모든 프로젝트에 대한 타임라인을 다시 계산합니다.

   * **프로젝트의 범위가 변경될 때**: 프로젝트 범위 변경을 구성하는 항목에 대한 자세한 내용은 [프로젝트 타임라인 다시 계산](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)을 참조하십시오.

     이 경우 [!DNL Workfront]은(는) 업데이트 유형이 [!UICONTROL 자동 및 변경 시] 또는 [!UICONTROL 변경만 시]인 모든 프로젝트에 대한 타임라인을 다시 계산합니다.
프로젝트 업데이트 형식에 대한 자세한 내용은 [프로젝트 업데이트 형식 개요](../../../manage-work/projects/planning-a-project/project-update-type-overview.md)를 참조하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   시스템에 있는 모든 프로젝트의 타임라인이 각 프로젝트의 업데이트 유형에 따라 자동으로 다시 계산됩니다.

## 전체 [!DNL Workfront] 인스턴스에 대한 타임라인 다시 계산

[!UICONTROL 타임라인 다시 계산] 진단을 실행하여 [!DNL Workfront] 시스템의 모든 타임라인을 수동으로 다시 계산할 수 있습니다. 이를 통해 모든 프로젝트 관리자는 계획된 일자와 예상 일자 모두에 대한 외부 변경 사항의 영향을 즉시 확인할 수 있습니다. 자세한 내용은 [진단을 사용하여 자동화된 프로세스를 트리거합니다](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)를 참조하십시오.
