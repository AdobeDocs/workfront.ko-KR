---
product-area: resource-management
keywords: working,team,인력,리소스
navigation-topic: the-workload-balancer
title: 작업 로드 밸런서를 찾습니다.
description: 작업 로드 밸런서를 사용하여 작업 자원을 예약하거나 가용성 및 현재 할당을 검토할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 1%

---

# 작업 로드 밸런서를 찾습니다.


작업 로드 밸런서를 사용하여 작업 자원을 예약하거나 가용성 및 현재 할당을 검토할 수 있습니다.

다음과 같은 방법으로 작업 로드 밸런서에 액세스할 수 있습니다.

* Adobe Workfront에 의해 사전 정의된 여러 영역
* 사용자 지정 섹션에 추가

이 문서에서는 작업 로드 밸런서에 액세스할 수 있는 영역에 대해 설명합니다.

>[!NOTE]
>
>작업 로드 밸런서에 액세스하는 데 사용하는 방법과 관계없이 작업 로드 밸런서를 탐색하고 리소스를 관리하는 방법은 동일합니다.
>
>작업 로드 밸런서와 작업 자원 관리 및 스케줄링에 작업 로드 밸런서를 사용하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.
>
>* [작업 로드 밸런서 개요](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [작업 로드 밸런서에서 작업 할당 개요](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [작업 로드 밸런서에서 사용자 할당 관리](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)
>


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>리소스 영역에서 작업 로드 밸런서를 사용할 계획</p>
   <p>작업, 팀 또는 프로젝트의 작업 로드 밸런서를 사용할 때</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>다음 항목에 대한 액세스 권한 보기 이상:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>작업</p> </li> 
     <li> <p>문제</p> </li> 
    </ul> <p><b> 메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 권한 보기 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 미리 정의된 영역에서 작업 로드 밸런서에 액세스

다음 섹션에서는 Workfront 내에서 작업 로드 밸런서에 액세스할 수 있는 위치를 보여줍니다.

### 리소스 영역에서 여러 프로젝트에 대한 작업 로드 밸런서에 액세스

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 **리소스**.
1. 클릭 **작업 로드 밸런서** 왼쪽 패널에 표시됩니다.

   ![](assets/nwe-balancer-global.png)

   기본적으로 작업 로드 밸런서는 리소스 영역에 있는 정보별로 다음을 표시합니다.

   * **할당되지 않은 작업**: 할당되지 않은 작업 항목이 없습니다.
   * **지정된 작업 시간**: 시스템의 모든 활성 사용자.

      지정된 작업 영역에서 사용자를 표시할 때 필터를 사용하는 것이 좋습니다. 자세한 내용은 [작업 로드 밸런서에서 정보 필터링](../workload-balancer/filter-information-workload-balancer.md).

### 팀에 대한 작업 로드 밸런서에 액세스

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 팀 을 클릭합니다.
홈 팀의 페이지가 표시됩니다.

   기본적으로 팀에 대한 작업 로드 밸런서가 표시됩니다.

   ![](assets/nwe-balancer-team-350x172.png)

   팀의 작업 로드 밸런서에는 기본적으로 다음 정보가 표시됩니다.

   * **할당되지 않은 작업**: 팀에 할당되고 사용자에게 할당되지 않은 항목입니다.
   * **지정된 작업 시간**: 모든 임무를 맡은 팀의 모든 멤버들.

      >[!TIP]
      >
      >팀원이 팀에 할당되거나 다른 팀이나 역할에 할당된 작업에 할당될 수 있습니다.



### 프로젝트에 대한 작업 로드 밸런서에 액세스

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)를 클릭한 다음 **프로젝트**.
1. 프로젝트 이름을 클릭하여 프로젝트 페이지를 엽니다.
1. 클릭 **작업 로드 밸런서** 왼쪽 패널에 표시됩니다. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **작업 로드 밸런서**.

   프로젝트에 대한 작업 로드 밸런서가 표시됩니다.

   ![](assets/nwe-balancer-project-350x152.png)

   프로젝트의 작업 로드 밸런서에는 기본적으로 다음 정보가 표시됩니다.

   * **할당되지 않은 작업**: 작업 역할 또는 팀에 할당되고 사용자에게 할당되지 않은 프로젝트의 항목입니다.
   * **지정된 작업 시간**: 프로젝트의 항목에 지정된 사용자입니다.

      >[!TIP]
      >
      >모든 사용자 표시 옵션을 활성화하여 프로젝트에 있는 사용자(할당된 작업 영역)만 대신 시스템의 모든 사용자를 표시할 수 있습니다. 자세한 내용은 [작업 로드 밸런서 탐색](../workload-balancer/navigate-the-workload-balancer.md).


## 사용자 정의 섹션에 작업 로드 밸런서 추가

작업 로드 밸런서를 사용자 지정 섹션에 추가할 수 있습니다.

이미 작업 로드 밸런서에 적용한 대부분의 사용자 지정은 사용자 지정 섹션에 추가할 때 유지됩니다.

1. 다음 영역 중 하나로 이동하여 작업 로드 밸런서에 액세스합니다.

   * 리소스 영역
   * 팀
   * 프로젝트

1. 에 설명된 대로 공유 가능한 링크를 가져와 클립보드에 복사합니다. [링크와 작업 로드 밸런서 공유](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. 에 설명된 대로 외부 페이지로 대시보드를 만듭니다 [대시보드에 외부 웹 페이지 포함](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). 외부 페이지에 대해 2단계에서 얻은 공유 가능한 링크를 사용합니다.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. 에 설명된 대로 사용자 지정 섹션을 만듭니다. [사용자 지정 탭 또는 섹션 만들기](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) 대시보드 를 사용자 지정 탭에 배치합니다.

   사용자 정의 섹션에서 작업 로드 밸런서에 액세스할 때 1단계에서 나열된 원래 영역 중 하나에서 직접 액세스한 것처럼 볼 수 있습니다.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (선택 사항)에 설명된 대로 레이아웃 템플릿에서 사용자 지정 탭을 공유합니다.  [레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) .


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->