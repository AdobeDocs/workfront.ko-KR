---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 고급 할당 만들기
description: 고급 할당을 사용하여 작업 또는 문제 할당을 관리할 수 있습니다.
author: Alina
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: ad5d6bfda24119076df8336ed291c0ba63e2c88a
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 0%

---

# 고급 할당 만들기

{{highlighted-preview}}

고급 할당을 사용하여 작업 또는 문제 할당을 관리할 수 있습니다.

고급 발령을 수행할 때 다음 발령 정보를 조정할 수 있습니다.

* 작업 또는 문제에 사용자를 할당합니다(고급 할당 외부에서 수행할 수 있음).
* 각 할당자가 할당된 시간을 조정하고 재배포합니다.
* 작업 또는 문제의 소유자 또는 기본 피할당자로 지정되어야 하는 사용자를 결정합니다.
* 작업 또는 문제를 작업할 때 각 사용자가 수행할 역할을 지정합니다.
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>작업에 사용자를 할당할 때 예약에 따라 가용성이 작업 및 문제의 계획 및 예상 일자에 영향을 줍니다. 일정에 대한 자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## 고급 할당을 수행할 수 있는 Adobe Workfront 영역

이 문서에서는 작업 또는 문제 헤더에서 고급 할당에 액세스하는 방법에 대해 설명합니다.

또한 Workfront의 다음 영역에서 고급 할당을 수행할 수 있습니다.

* 목록 및 보고서에서 할당 필드가 보기에 표시됩니다.
* 작업을 편집할 때 할당 섹션에서 다음을 수행합니다. 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 작업 또는 문제 헤더의 할당 영역에서 다음을 수행합니다.
* 업무 균형자에서. 자세한 내용은 [업무 균형자 를 사용하여 수동으로 작업 할당](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 또는 문제에 대한 상위 권한 기여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 고급 할당 만들기

1. 작업 또는 문제를 할당할 프로젝트로 이동합니다.
1. 클릭 **작업** 또는 **문제** 왼쪽 패널에서 작업 또는 문제의 이름을 클릭합니다.

   >[!TIP]
   >
   >배정된 인원이 2명 이상인 경우 작업 또는 문제 목록에서 직접 고급 배정을 할 수 있습니다. 내부를 클릭합니다. **할당** 작업 또는 문제와 같은 줄에 있는 필드를 클릭한 다음 **사람 아이콘** 고급 지정 창을 엽니다. 5단계로 건너뛰고 고급 할당을 계속 작성합니다.\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. 클릭 **할당 대상** 다음에서 **할당** 작업 또는 문제의 헤더에 있는 필드

   또는

   작업 또는 문제가 이미 할당된 경우 할당명을 클릭합니다.

1. 클릭 **고급**.

   프로덕션 환경의 샘플 이미지:
   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

   <span class="preview">미리보기 환경의 샘플 이미지:</span>
   ![고급을 클릭합니다](assets/assignments-box-in-task-header.png)

1. 다음에서 **사람, 역할 및 팀 검색** 필드에서 사용자, 역할 또는 팀의 이름을 입력한 다음 드롭다운 목록에 나타나면 이름을 클릭합니다.

   >[!NOTE]
   >
   >사용자 이름에 특수 문자가 포함되어 있으면 검색 필드에 특수 문자를 포함해야 합니다.

1. (선택 사항)에서 피할당자를 계속 추가합니다. **사람, 역할 또는 팀 검색** 작업 또는 문제에 여러 리소스를 추가하는 상자.

   >[!TIP]
   >
   >* 여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
   >
   >
   >* 사용자 할당을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소에 따라 이름이 동일한 사용자가 구분되는지 확인합니다.
   >사용자를 추가할 때 이를 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
   >사용자의 이메일을 보려면 사용자의 액세스 수준에서 연락처 정보 보기 설정을 활성화해야 합니다. 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* 비활성화되기 전에 사용자, 작업 역할 또는 팀이 할당된 경우 작업 항목에 할당된 상태로 유지됩니다. 이 경우 다음 사항을 권장합니다.
   >   
   >   * 작업 항목을 활성 리소스에 재할당합니다.
   >   * 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.
   >

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. 의 각 사용자에 대해 **할당자** 열에서 다음 정보를 지정합니다.


   * **소유자**: 피할당자의 이름 위에 마우스를 놓고 클릭 **기본 항목으로 설정** 소유자 필드에서 피할당자를 작업 또는 문제 소유자로 표시하려는 경우. 녹색 확인란은 지정된 사용자가 작업 또는 문제의 기본 담당자임을 나타냅니다. Adobe Workfront은 작업 또는 문제에 할당한 첫 번째 사용자 또는 작업 역할을 소유자 또는 기본 할당으로 표시합니다. 팀을 작업 또는 문제의 기본 소유자로 지정할 수 없습니다.

     >[!IMPORTANT]
     >
     >Workfront 관리자 또는 그룹 관리자가 프로젝트 환경 설정을 설정하는 방법에 따라 Workfront은 작업에 여러 명의 사용자를 할당한 경우 작업 소유자의 일정을 사용하여 작업의 타임라인을 계산할 수 있습니다. 여러 작업 할당자에 대한 자세한 내용은 문서의 &quot;작업에 여러 사용자 할당&quot; 섹션을 참조하십시오 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **할당** : 작업의 기간 유형이 간단한 경우 각 사용자 또는 작업 역할이 작업에 할당되어야 하는 시간을 지정합니다. 각 사용자에 대해 할당된 모든 시간의 합계는 **계획된 시간** 할당 열 하단의 필드. 다른 모든 경우에는 할당자가 작업 또는 문제를 해결하는 데 소비할 시간(또는 할당)의 백분율을 지정합니다.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * 작업에 대한 할당 할당을 수동으로 수정한 후 작업의 계획된 시간이 그에 따라 업데이트될 수 있습니다. 자세한 내용은 문서의 &quot;사용자 할당 관리 시 작업 계획 시간 업데이트&quot; 섹션을 참조하십시오 [계획된 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * 문제에 대한 할당 할당을 수동으로 수정할 수 없습니다.
     >   * 작업에 할당된 팀의 할당은 수동으로 수정할 수 없습니다.
     >   
     >

   * **할당자의 역할:** 이 할당을 수행할 때 사용자가 사용해야 하는 역할을 선택합니다.  사용자의 기본 역할 이 기본적으로 표시됩니다. 피할당자의 역할 상자를 클릭하여 다른 역할을 선택합니다.  먼저 작업 또는 문제를 역할에 할당한 다음 해당 역할을 수행할 수 있는 사용자를 두 번째 할당으로 추가하면 제안된 사용자 목록이 작업 및 문제에 이미 할당된 역할을 수행할 수 있는 사용자에 대해 필터링됩니다.

     프로덕션 환경의 샘플 이미지:
     ![](assets/advanced-assignments-box-select-a-role-350x243.png)

     <span class="preview">미리보기 환경의 샘플 이미지:</span>
     ![피할당자의 역할](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **기간 유형**: 작업에만 사용할 수 있습니다. 기간 유형 이름을 클릭하고 드롭다운 메뉴에서 기간 유형 을 선택합니다. 기간 유형에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **기간:** 작업에 대한 관리 권한이 있는 경우 작업에 대해 이 필드를 업데이트할 수 있습니다.

     자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 할당 정보를 일괄 편집할 때 사용자, 시간, 할당 및 작업 소유자를 할당하는 유사한 대화 상자가 나타납니다.

   * **계획된 시간**: 기간 유형이 계산된 할당 또는 단순인 경우 계획된 시간을 업데이트합니다. 결과적으로 각 리소스에 대한 할당 백분율 또는 시간이 균등하게 분배됩니다. Workfront은 기간 유형이 계산된 작업 또는 작업량 고정 시 계획된 시간을 계산합니다. 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

     프로덕션 환경의 샘플 이미지:
     ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

     <div class="preview">

     미리보기 환경의 샘플 이미지:
     ![고급 할당](assets/advanced-assignments-duration-type-allocations.png)

     </div>

1. **저장**&#x200B;을 클릭합니다.
