---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: 예약 영역에서 역할 및 그룹 구성원에 관계없이 사용자 지정 허용
description: 리소스 예약에서, 사용자에게 할당되는 작업의 역할 할당이나 문제와 일치하는 사용자 프로필에 정의된 역할이 있는 사용자만 할당할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# 예약 영역에서 역할 및 그룹 구성원에 관계없이 사용자 지정 허용

>[!IMPORTANT]
>  
><span class="preview">이 문서에 설명된 예약 기능은 2023년 1월 23.1 릴리스부터 Adobe Workfront에서 더 이상 사용되지 않고 제거됩니다.   </span>
>  
> <span class="preview"> 이 문서는 2023년 초에 23.1 릴리스 직후 제거됩니다. 지금은 이에 따라 책갈피를 업데이트하는 것이 좋습니다. </span>
> 
><span class="preview"> 이제 작업 로드 밸런서를 사용하여 자원에 대한 작업 일정을 예약할 수 있습니다. </span>
>  
> <span class="preview">작업 로드 밸런서를 사용하여 리소스를 예약하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [작업 로드 밸런서](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

기본적으로, 자원 스케줄링 도구를 사용할 때 작업의 역할 할당이나 사용자에게 할당된 문제와 일치하는 사용자 프로필에 정의된 역할이 있는 사용자만 할당할 수 있습니다.

해당 사용자에게 작업의 역할 할당이나 사용자에게 할당되는 문제와 일치하는 사용자 프로필에 정의된 역할이 있는지 여부에 관계없이, 작업 및 문제를 사용자에게 할당하도록 Adobe Workfront을 구성할 수 있습니다. 작업이나 문제에 사용자를 할당하고 해당 사용자에게 작업이나 문제에 대한 역할 할당과 일치하는 역할이 없는 경우 원래 역할 할당이 제거되고 역할 할당이 할당되는 사용자의 역할에 변경됩니다.

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
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 보기 이상의 액세스 권한</p> <p><strong>메모</strong>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업 및 업데이트 문제에 대한 권한 이상을 제공할 수 있습니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 역할에 관계없이 사용자에게 할당 허용

1. 여러 프로젝트, 개별 프로젝트 또는 팀의 예약 타임라인으로 이동합니다.

   * **여러 프로젝트의 경우**:  을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
   * **개별 프로젝트의 경우**: 프로젝트로 이동하여 **작업 로드 밸런서** 왼쪽 패널의 섹션에서 을(를) 선택한 다음 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.
   * **팀**: 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **팀**&#x200B;를 클릭하고, 팀을 선택하고 **작업 로드 밸런서** 왼쪽 패널에서 를 선택하고 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.

1. 을(를) 클릭합니다. **설정** 아이콘을 클릭합니다.
1. 옵션 비활성화 **일치하는 역할을 가진 사용자에게 지정 제한**.
1. 클릭 **예약으로 돌아가기**.

## 그룹 멤버십에 관계없이 사용자에게 할당 허용

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

기본적으로, 프로젝트(프로젝트를 편집할 때 정의된 그룹)와 연관된 그룹의 멤버인 사용자만 할당할 수 있습니다.

>[!IMPORTANT]
>
>이 설정은 프로젝트와 연결된 그룹의 멤버만 고려하며 해당 그룹의 하위 그룹의 멤버는 고려하지 않습니다.

해당 사용자가 작업 또는 문제가 있는 프로젝트와 연결된 그룹의 구성원인지 여부에 관계없이 모든 사용자에게 작업 및 문제를 할당하도록 Workfront을 구성할 수 있습니다.

1. 여러 프로젝트, 개별 프로젝트 또는 팀의 예약 타임라인으로 이동합니다.

   * **여러 프로젝트의 경우**:  을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
   * **개별 프로젝트의 경우**: 프로젝트로 이동하여 **작업 로드 밸런서** 왼쪽 패널의 섹션에서 을(를) 선택한 다음 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.
   * **팀**: 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **팀**&#x200B;를 클릭하고, 팀을 선택하고 **작업 로드 밸런서** 왼쪽 패널에서 를 선택하고 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.

1. 을(를) 클릭합니다. **설정** 아이콘을 클릭합니다.
1. 옵션 비활성화 **프로젝트와 연관된 그룹에 지정 제한**.
1. 클릭 **예약으로 돌아가기**.

 
