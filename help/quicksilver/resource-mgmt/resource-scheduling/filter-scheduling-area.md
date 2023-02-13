---
product-area: resource-management
navigation-topic: resource-scheduling
title: 예약 영역에서 정보를 필터링합니다.
description: 리소스 예약 영역에서 필터를 사용하면 예약 타임라인에 표시되는 작업 항목을 결정할 수 있습니다. [지정되지 않음] 영역에 표시되는 작업 및 문제와 표시되는 사용자가 포함됩니다.
author: Alina
feature: Resource Management
exl-id: 974b2515-ed10-459d-a317-36e62c52afc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2452'
ht-degree: 0%

---

# 예약 영역에서 정보를 필터링합니다.

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<p>(SEVERAL SECTIONS BELOW LINKED TO THE PRODUCT. SEE NOTES</p>
-->

리소스 예약 영역에서 필터를 사용하면 예약 타임라인에 표시되는 작업 항목을 결정할 수 있습니다. [지정되지 않음] 영역에 표시되는 작업 및 문제와 표시되는 사용자가 포함됩니다.

이 섹션에 설명된 대로 컨텐츠 필터링을 시작하기 전에 Adobe Workfront에서 리소스 예약이 작동하는 방식을 숙지하십시오.\
Workfront의 리소스 예약에 대한 자세한 내용은 문서를 참조하십시오 [리소스 예약 시작](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).\
예약 타임라인에 대한 자세한 내용은 문서를 참조하십시오 [리소스 예약 시작](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

자원 관리자 또는 자신이 속해 있는 프로젝트에 대해 자원이나 개별 팀을 예약할 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

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
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 액세스 이상의 권한 보기</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 권한 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

<!--
<p>(NOTE: sections below - LINKED TO THE ui. DO NOT RENAME/ DELETE)</p>
-->

## 예약 섹션에서 필터 만들기(팀용)

필터에서 정의한 프로젝트, 사용자 및 역할의 작업 및 문제가 작업 중 탭의 예약 타임라인에 표시됩니다. 필터의 옵션을 사용하여 예약 타임라인에서 표시할 프로젝트, 사용자 및 역할을 결정합니다.

>[!NOTE]
>
>작업중 탭(팀의 경우)에서는 필터를 저장할 수 없습니다. 페이지를 새로 고치거나 다른 곳으로 이동하면 필터는 기본 설정으로 되돌아갑니다.

팀의 작업 중 탭에서 타임라인 예약 필터를 만들려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **팀**&#x200B;를 클릭하고, 팀을 선택하고 **작업 로드 밸런서** 왼쪽 패널에서 를 선택하고 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.
1. 클릭 **필터**.
1. 다음 정보를 지정하여 [지정되지 않음] 영역에 표시되는 프로젝트를 결정합니다.

   <!--
   <p>(NOTE: Alina: there was a note that [This step is linked to from the context-sensitive help] but I could not find from where in the UI it is linked.)&nbsp;</p>
   -->

   * **프로젝트 우선 순위:** 예약 타임라인에서 나타낼 프로젝트의 우선순위를 선택합니다. 선택하는 우선 순위가 있는 프로젝트의 작업 및 문제가 예약 타임라인에 표시됩니다.\
      팀에 할당된 작업 또는 문제를 포함하는 프로젝트의 우선 순위만 이 메뉴에서 선택할 수 있습니다.
   * **프로젝트 상태:** 예약 타임라인에서 나타낼 프로젝트의 상태를 선택합니다. 선택한 상태가 있는 프로젝트의 작업 및 문제가 예약 타임라인에 표시됩니다.\
      팀에 할당된 작업이나 문제가 포함된 프로젝트의 상태만 이 메뉴에서 선택할 수 있습니다.
   * **프로젝트:** 예약 타임라인에서 나타낼 프로젝트를 선택합니다. 선택한 프로젝트의 작업 및 문제가 예약 타임라인에 표시됩니다.\
      이전 필드에서 선택한 사항에 따라 선택할 수 있는 프로젝트가 결정됩니다.\
      팀에 할당된 작업이나 문제가 포함된 프로젝트만 이 메뉴에서 선택할 수 있습니다.

1. 다음 정보를 지정하여 예약 타임라인에 표시할 사용자를 결정합니다. 기본적으로 모든 팀 구성원이 표시됩니다.

   <!--
   <p>(NOTE: this step is linked in the UI.)</p>
   -->

   * **역할:** 예약 타임라인에서 표시할 역할을 선택합니다.\
      해당 역할에 할당된 작업만 [지정되지 않음] 영역에 표시됩니다. 그러한 작업을 할당할 수 있는 사용자를 선택하는 역할을 가진 사용자만 표시됩니다.\
      사용자가 작업 역할별로 구성된 예약 타임라인에 표시됩니다.
   * **사용자:** 예약 타임라인에서 나타낼 개별 사용자를 선택합니다.\
      [지정되지 않음] 영역에서 작업의 역할 할당과 일치하는 역할 할당이 있는지 여부에 관계없이 선택한 사용자만 표시됩니다.\
      이 옵션은 [지정되지 않음] 영역에 표시되는 작업 및 문제에 영향을 주지 않습니다.

      <!--   
     <p>(NOTE: Alina: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])</p>   
     -->

1. (선택 사항) 예약 타임라인을 추가로 수정(날짜 범위 변경 등)하고 사용자 지정을 수정하려면 문서를 참조하십시오 [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p>(NOTE: below - LINKED TO THE UI, DO NOT RENAME/ DELETE/ CHANGE)</p>
-->

## 예약 섹션에서 필터를 만들고 수정합니다(여러 프로젝트의 경우)

새 필터를 만들거나 이전에 만든 필터를 적용하거나 이전에 만든 필터를 수정하거나 필터를 삭제할 수 있습니다. 만든 필터는 다른 사용자와 공유할 수 없습니다.

* [예약 섹션에서(프로젝트용) 필터를 만듭니다.](#create-a-filter-in-the-scheduling-section-for-projects)
* [저장된 필터 적용](#apply-a-saved-filter)
* [저장된 필터 수정](#modify-a-saved-filter)
* [저장된 필터 삭제](#delete-a-saved-filter)

### 예약 섹션에서(프로젝트용) 필터를 만듭니다. {#create-a-filter-in-the-scheduling-section-for-projects}

<!--
<p>(NOTE: *****LINKED TO THE PRODUCT FROM THE GLOBAL SCHEDULER >> BOTH THE FIRST AND THE SECOND AREAS) </p>
-->

필터에서 정의한 프로젝트, 사용자 및 역할의 작업 및 문제가 예약 탭의 예약 타임라인에 표시됩니다. 필터의 옵션을 사용하여 예약 타임라인에서 표시할 프로젝트, 사용자 및 역할을 결정합니다.

여러 프로젝트의 예약 탭에서 타임라인에 대한 필터를 생성하려면 다음을 수행합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
1. 클릭 **필터**.\
   ![](assets/scheduling-filter-350x351.png)

1. 을(를) 종료하십시오. **저장한 필터** 필드를 비워 둡니다.
1. 다음 정보를 지정하여 [지정되지 않음] 영역에 표시되는 프로젝트를 결정합니다.

   <!--
   <p>(NOTE: Alina: this step is linked in the UI.) </p>
   -->

   * **Portfolio:** 예약 타임라인에서 표시할 프로그램 및 프로젝트를 포함하는 포트폴리오를 선택합니다.

      선택하는 포트폴리오 내의 프로그램만 **프로그램** 필드.

   * **프로그램:** 예약 타임라인에 표시할 프로젝트를 포함하는 프로그램을 선택합니다.\
      에서 선택 **Portfolio** 필드를 통해 선택할 수 있는 프로그램을 결정합니다.\
      선택한 프로그램 내의 프로젝트만 **프로젝트** 필드.

   * **프로젝트 우선 순위:** 예약 타임라인에서 나타낼 프로젝트의 우선순위를 선택합니다.\
      선택하는 우선순위가 있는 프로젝트만 표시됩니다.

   * **프로젝트 상태:** 예약 타임라인에서 나타낼 프로젝트의 상태를 선택합니다.\
      선택한 상태가 있는 프로젝트만 표시됩니다.

   * **프로젝트 회사:** 작업 및 문제는 사용자가 선택한 회사와 일치하는 프로젝트에 속하는 경우에만 예약 타임라인에 표시됩니다.

   * **프로젝트 그룹:** 작업 및 문제는 선택한 그룹과 일치하는 프로젝트에 속해 있는 경우에만 예약 타임라인에 표시됩니다.

   * **프로젝트:** 예약 타임라인에서 나타낼 프로젝트를 선택합니다. 선택한 프로젝트의 작업 및 문제가 예약 타임라인에 표시됩니다.\
      이전 필드에서 선택한 사항에 따라 선택할 수 있는 프로젝트가 결정됩니다.\
      선택한 프로젝트의 작업 및 문제가 예약 타임라인에 표시됩니다. 팀에 할당된 작업이나 문제가 포함된 프로젝트만 이 메뉴에서 선택할 수 있습니다.

1. 다음 정보를 지정하여 예약 타임라인에 표시할 사용자를 결정합니다. 기본적으로 [지정되지 않음] 영역에서 작업 또는 문제를 지정할 수 있는 사용자만 표시됩니다. 개별 사용자를 선택하면 할당 취소 영역에서 작업을 할당받을 수 있는지 또는 문제를 해결할 수 있는지에 관계없이 예약 타임라인에 사용자가 표시됩니다. 

   <!--
   <p>(NOTE: Alina: this step had a note that it is linked in the UI but I could not find from where.) </p>
   -->

   * **사용자 회사:** 이 필드를 사용하면 다른 회사의 사용자가 예약 타임라인에 표시되지 않도록 제한할 수 있습니다.\
      회사의 사용자를 추가하려면 이 필드를 비워 둡니다. 개별 회사를 지정하는 경우 해당 회사의 사용자만 예약 타임라인에 추가할 수 있습니다. 회사를 지정해도 해당 회사의 사용자가 예약 타임라인에 자동으로 추가되지 않습니다. 대신 아래 필드를 사용하여 특정 사용자를 추가합니다.\
      이 옵션은 [지정되지 않음] 영역에 표시되는 작업 및 문제에 영향을 주지 않습니다.****

   * **사용자 그룹:** 지정한 사용자 그룹의 모든 사용자가 예약 타임라인에 표시됩니다.

   * **팀:** 지정한 팀의 모든 사용자가 예약 타임라인에 표시됩니다.\
      이 옵션은 [지정되지 않음] 영역에 표시되는 작업 및 문제에 영향을 주지 않습니다.

   * **역할:** 예약 타임라인에서 표시할 역할을 선택합니다.\
      해당 역할에 할당된 작업만 [지정되지 않음] 영역에 표시됩니다. 그러한 작업을 할당할 수 있는 사용자를 선택하는 역할을 가진 사용자만 표시됩니다.\
      사용자가 작업 역할별로 구성된 예약 타임라인에 표시됩니다.

   * **사용자:** 예약 타임라인에서 나타낼 개별 사용자를 선택합니다.\
      [지정되지 않음] 영역에서 작업의 역할 할당과 일치하는 역할 할당이 있는지 여부에 관계없이 선택한 사용자만 표시됩니다.\
      이 옵션은 [지정되지 않음] 영역에 표시되는 작업 및 문제에 영향을 주지 않습니다.
   <!--
   <p>NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->

1. 클릭 **새 필터 저장**.\
   데이터가 예약 타임라인에 표시됩니다.

1. (선택 사항) 예약 타임라인을 추가로 수정(날짜 범위 변경 등)하고 사용자 지정을 수정하려면 문서를 참조하십시오 [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 저장된 필터 적용 {#apply-a-saved-filter}

>[!NOTE]
>
>이 옵션은 여러 프로젝트에 대한 리소스를 예약할 때만 적용됩니다( 예약 탭에서). 팀을 위한 자원을 스케줄링하거나(작업 중 탭에서) 단일 프로젝트에 대한 자원을 스케줄링할 때(스태핑 탭에서) 저장된 필터를 적용할 수 없습니다.

이전에 만든 필터를 적용할 수 있습니다.

여러 프로젝트에 대해 저장된 필터를 적용하려면:

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
1. 클릭 **필터**.
1. 에서 **저장한 필터** 필드에서 적용할 필터를 선택합니다.\
   데이터가 예약 타임라인에 표시됩니다.

1. (선택 사항) 예약 타임라인을 추가로 수정(날짜 범위 변경 등)하고 사용자 지정을 수정하려면 문서를 참조하십시오 [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 저장된 필터 수정 {#modify-a-saved-filter}

>[!NOTE]
>
>이 옵션은 여러 프로젝트에 대한 리소스를 예약할 때만 적용됩니다( 예약 탭에서). 팀의 자원을 스케줄링하거나(작업 중 탭에서) 단일 프로젝트에 대한 자원을 스케줄링할 때(스태핑 탭에서) 저장된 필터를 수정할 수 없습니다.

이전에 만든 필터를 수정할 수 있습니다.

여러 프로젝트에 대해 저장된 필터를 수정하려면 다음을 수행합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
1. 클릭 **필터**.
1. 에서 **저장한 필터** 필드의 드롭다운 목록에서 수정할 필터를 선택합니다.
1. 예약 타임라인에 표시할 데이터를 지정합니다.
1. **저장**&#x200B;을 클릭합니다.\
   데이터가 예약 타임라인에 표시됩니다.

1. (선택 사항) 예약 타임라인을 추가로 수정(날짜 범위 변경 등)하고 사용자 지정을 수정하려면 문서를 참조하십시오 [예약 영역에서 지정되지 않은 작업 및 문제를 수동으로 지정](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### 저장된 필터 삭제 {#delete-a-saved-filter}

>[!NOTE]
이 옵션은 여러 프로젝트에 대한 리소스를 예약할 때만 적용됩니다( 예약 탭에서). 팀의 자원을 스케줄링하거나(작업 중 탭에서) 단일 프로젝트에 대한 자원을 스케줄링할 때(스태핑 탭에서) 저장된 필터를 삭제할 수 없습니다.

이전에 만든 필터를 삭제할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 **리소스 > 작업 로드 밸런서**&#x200B;를 선택하고 을 선택합니다. **예약** 를 클릭합니다.
1. 클릭 **필터**.
1. 에서 **저장한 필터** 필드의 드롭다운 목록에서 삭제할 필터 옆에 있는 (x)를 클릭합니다. 

## 예약 섹션에서 필터를 만들고 수정합니다(단일 프로젝트의 경우)

<!--
<p>(NOTE: **** LINKED FROM THE PRODUCT FROM THE PROJECT> STAFFING> SCHEDULING AREA) </p>
-->

필터에서 정의한 사용자, 팀 및 역할의 작업 및 문제는 스태핑 탭의 예약 타임라인에 표시됩니다. 필터의 옵션을 사용하여 예약 타임라인에서 표시할 사용자, 팀 및 역할을 결정합니다.

>[!NOTE]
스태핑 탭(단일 프로젝트의 경우)에서는 필터를 저장할 수 없습니다. 페이지를 새로 고치거나 다른 곳으로 이동하면 필터는 기본 설정으로 되돌아갑니다.

단일 프로젝트에 대한 스태핑 탭의 스케줄 타임라인에 대한 필터를 생성하려면

1. 프로젝트로 이동하여 **작업 로드 밸런서** 왼쪽 패널의 섹션에서 을(를) 선택한 다음 **예약** 왼쪽 위 드롭다운 메뉴에서 을 선택합니다.
1. 다음 정보를 지정하여 예약 타임라인에 표시할 사용자를 결정합니다. 기본적으로 [지정되지 않음] 영역에서 작업 또는 문제를 지정할 수 있는 사용자만 표시됩니다. 개별 사용자를 선택하면 할당 취소 영역에서 작업을 할당받을 수 있는지 또는 문제를 해결할 수 있는지에 관계없이 예약 타임라인에 사용자가 표시됩니다. 

   <!--
   <p><span>(NOTE: Alina: [This step is linked to from the context-sensitive help]) </span> </p>
   -->

   * **사용자 회사:** 이 필드를 사용하면 다른 회사의 사용자가 예약 타임라인에 표시되지 않도록 제한할 수 있습니다.\
      회사의 사용자를 추가하려면 이 필드를 비워 둡니다. 개별 회사를 지정하는 경우 해당 회사의 사용자만 예약 타임라인에 추가할 수 있습니다. 회사를 지정해도 해당 회사의 사용자가 예약 타임라인에 자동으로 추가되지 않습니다. 대신 아래 필드를 사용하여 특정 사용자를 추가합니다.\
      이 옵션은 [지정되지 않음] 영역에 표시되는 작업 및 문제에 영향을 주지 않습니다.

   * **사용자 그룹:** 지정한 사용자 그룹의 모든 사용자가 예약 타임라인에 표시됩니다.

   * **팀:** 지정한 팀의 모든 사용자가 예약 타임라인에 표시됩니다.\
      이 옵션은 [지정되지 않음] 영역에 표시되는 작업 및 문제에 영향을 주지 않습니다.

   * **역할:** 예약 타임라인에서 표시할 역할을 선택합니다.\
      해당 역할에 할당된 작업만 [지정되지 않음] 영역에 표시됩니다. 그러한 작업을 할당할 수 있는 사용자를 선택하는 역할을 가진 사용자만 표시됩니다.\
      사용자가 작업 역할별로 구성된 예약 타임라인에 표시됩니다.

   * **사용자:** 예약 타임라인에서 나타낼 개별 사용자를 선택합니다.\
      [지정되지 않음] 영역에서 작업의 역할 할당과 일치하는 역할 할당이 있는지 여부에 관계없이 선택한 사용자만 표시됩니다.\
      이 옵션은 [지정되지 않음] 영역에 표시되는 작업 및 문제에 영향을 주지 않습니다.
   <!--
   <p>(NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->
