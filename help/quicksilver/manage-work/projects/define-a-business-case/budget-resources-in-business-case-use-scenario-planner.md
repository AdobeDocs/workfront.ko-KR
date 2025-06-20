---
navigation-topic: business-case-and-scorecards
title: 시나리오 플래너를 사용하는 비즈니스 사례의 예산 리소스
description: 리소스 계획의 일부로, Adobe Workfront 시나리오 플래너를 사용하여 비즈니스 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할의 예산을 책정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 0%

---

# 시나리오 플래너를 사용하는 비즈니스 사례의 예산 리소스

<!--Audited: 06/2025-->

리소스 계획의 일부로, Adobe Workfront 시나리오 플래너를 사용하여 비즈니스 사례를 작성할 때 프로젝트에서 작업을 완료하는 데 필요한 작업 역할의 예산을 책정할 수 있습니다.

비즈니스 사례를 만드는 방법에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md)를 참조하세요.

>[!TIP]
>
>시스템 레벨 시나리오 플래너에 입력한 프로젝트에 연결된 이니셔티브에 대한 작업 역할 정보는 이니셔티브를 게재할 때 프로젝트 비즈니스 사례의 리소스 예산 영역에 표시됩니다. 시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이선스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 플래너 개요](../../../scenario-planner/scenario-planner-overview.md)를 참조하십시오.

리소스 플래너를 사용하여 비즈니스 사례에서 리소스의 예산을 책정할 수도 있습니다. 자세한 내용은 다음을 참조하십시오.

* [비즈니스 사례의 예산 리소스](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>프로젝트 작업을 시작할 때 리소스 플래너 또는 시나리오 플래너를 사용할지 여부를 결정하는 것이 좋습니다. 프로젝트 기간 동안 둘 사이를 자주 전환하면 프로젝트에 대한 리소스 예산 책정 방식에 일치하지 않을 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td><p>현재: Ultimate</p> 
   <p>레거시: 비즈니스 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p>전류: 라이트 이상 
   <p>레거시: 검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>제품</p></td> 
   <td><p>시나리오 플래너는 현재 Ultimate Workfront 플랜에 포함되어 있습니다.</p> 
   <p>기존 Workfront 플랜의 경우 이 문서에 설명된 기능에 액세스하려면 Workfront 라이선스 외에 Adobe Workfront Scenario Planner용 라이선스를 구입해야 합니다.</p> <p>Workfront 시나리오 플래너를 얻는 방법에 대한 자세한 내용은 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">시나리오 플래너를 사용하는 데 필요한 액세스</a>를 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>다음에 대한 액세스 권한 편집: </p> 
    <ul> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>재무 데이터</p> </li> 
     <li> <p>시나리오 플래너 </p> </li> 
    </ul> <p>리소스 예산에 필요한 액세스에 대한 자세한 내용은 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Adobe Workfront에서 리소스 예산에 필요한 액세스</a>도 참조하세요.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Adobe Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에 다음을 수행해야 합니다.

* 시나리오 플래너를 사용하여 계획을 생성합니다.

  자세한 내용은 [시나리오 플래너에서 계획 만들기 및 편집](../../../scenario-planner/create-and-edit-plans.md)을 참조하십시오.

* 플랜에 대한 이니셔티브를 만들고 프로젝트에 연결합니다.

  이니셔티브에 필요한 작업 역할 정보를 표시했는지 확인하고 이 정보로 연결된 프로젝트를 업데이트합니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [시나리오 플래너에서 이니셔티브 만들기 및 편집](../../../scenario-planner/create-and-edit-initiatives.md)
   * [시나리오 플래너의 플랜으로 프로젝트 가져오기](../../../scenario-planner/import-projects-to-plans.md)
   * [시나리오 플래너에서 이니셔티브를 게시하여 프로젝트를 업데이트하거나 만듭니다](../../../scenario-planner/publish-scenarios-update-projects.md).

* 이러한 사전 요구 사항은 아니지만 다음 사항도 권장합니다.

   * 프로젝트에 대한 작업을 시나리오 플래너에서 예산이 책정된 작업 역할에 할당합니다.
   * 프로젝트에 대한 작업의 계획된 시간 수를 나타냅니다.

     이를 통해 작업을 완료하는 데 필요한 작업의 양을 파악할 수 있습니다. 이는 작업을 완료하는 데 필요한 리소스 예산 책정 시간을 결정하는 데 도움이 됩니다.

     작업을 계획된 시간과 연결하는 방법에 대한 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md)을 참조하십시오.

## 이니셔티브에 연결된 프로젝트에 시나리오 플래너를 사용하는 비즈니스 사례의 예산 리소스

>[!IMPORTANT]
>
>15년 동안 리소스의 예산을 책정할 수 있습니다. 15년을 초과하는 기간 동안 프로젝트에 대한 리소스의 예산을 책정하는 경우 예산 책정 정보가 정확하지 않을 수 있습니다.
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. 리소스 예산을 책정할 프로젝트로 이동합니다.

   >[!TIP]
   >
   >연결된 이니셔티브가 한 번 이상 게시된 시나리오 플래너의 이니셔티브에 연결된 프로젝트입니다.

1. 왼쪽 패널에서 **비즈니스 사례**&#x200B;를 클릭합니다.
1. (조건부) **리소스 예산 편성** 섹션에서 다음 중 하나를 수행합니다.

   * 시나리오 플래너에서 정보를 게시한 경우 **리소스 예산 책정 영역의 프로젝트 예산 인건비를 계산하는 데 사용할 시간을 선택하십시오** 필드에서 시나리오 플래너를 선택한 다음 **선택**&#x200B;을 클릭합니다.

     ![리소스 플래너의 비즈니스 사례(선택 단추 포함)](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * 이전에 리소스 플래너가 프로젝트 리소스 예산 책정에 선택된 경우 **변경** > **시나리오 플래너** > **선택**&#x200B;을 클릭합니다.

     ![시나리오 플래너의 비즈니스 사례(선택 단추 포함)](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront은 연결된 이니셔티브의 필수 작업 역할 시간을 사용하여 프로젝트의 예산 인건비 및 예산 시간을 계산합니다. 이 옵션이 권장됩니다. 비용은 프로젝트 통화로 비즈니스 사례에 표시됩니다.

     프로젝트를 복사할 때 예산 시간을 새 프로젝트에 복사하도록 선택하면 시나리오 플래너를 사용하여 예산 책정된 시간은 새 프로젝트에 복사되지 않습니다. 리소스 플래너에 예산 책정된 시간만 복사됩니다. 자세한 내용은 [프로젝트 복사](../manage-projects/copy-project.md)를 참조하십시오.

     >[!IMPORTANT]
     >
     >시나리오 플래너를 사용하여 프로젝트에 대한 자원의 예산을 책정할 때 예산 인건비가 Workfront의 다음 영역에 표시됩니다.
     >
     >   
     >   
     >   * 비즈니스 사례의 리소스 예산 영역
     >   * 프로젝트에 연결된 이니셔티브의 인력 비용으로서 시스템 수준 시나리오 플래너. 자세한 내용은 [시나리오 플래너에서 이니셔티브 만들기 및 편집](../../../scenario-planner/create-and-edit-initiatives.md)을 참조하십시오.
     >   
     >

1. (선택 사항) **시나리오 플래너에서 보기**&#x200B;를 클릭하여 프로젝트에 연결된 이니셔티브가 포함된 계획을 엽니다. 새 브라우저 탭에서 시나리오 플래너가 열립니다.
1. (선택 사항) 이니셔티브의 정보를 업데이트합니다. 자세한 내용은 [시나리오 플래너에서 이니셔티브 만들기 및 편집](../../../scenario-planner/create-and-edit-initiatives.md)을 참조하십시오.

   >[!NOTE]
   >
   >프로젝트의 리소스 예산 영역을 업데이트할 때마다 변경 후 이니셔티브를 게시해야 합니다.
