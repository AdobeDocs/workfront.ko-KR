---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 고급 할당 만들기
description: 고급 지정을 사용하여 태스크 또는 출고 지정을 관리할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# 고급 할당 만들기

고급 지정을 사용하여 태스크 또는 출고 지정을 관리할 수 있습니다.

고급 지정을 수행할 때 다음 발령 정보를 조정할 수 있습니다.

* 작업 또는 문제에 사용자를 할당합니다(고급 할당 외부에서 이 작업을 수행할 수 있음).
* 각 할당자가 할당된 시간 수를 조정하고 재분배합니다.
* 작업 또는 문제의 소유자 또는 기본 담당자로 지정할 사용자를 결정합니다.
* 작업 또는 문제 작업 시 각 사용자가 수행할 역할을 지정합니다.

>[!NOTE]
>
>사용자를 작업에 지정할 때 해당 스케줄에 따른 가용성은 작업 및 문제의 계획 및 예상 날짜에 영향을 줍니다. 예약에 대한 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## 고급 할당을 수행할 수 있는 Adobe Workfront 영역

이 문서에서는 작업 또는 문제 헤더의 사전 지정에 액세스하는 방법에 대해 설명합니다.

또한 다음 Workfront 영역에서 고급 할당을 수행할 수도 있습니다.

* 지정 필드가 뷰에 표시될 때 목록 및 보고서에서 사용됩니다.
* 작업을 편집할 때 지정 섹션에서 자세한 내용은 [작업 편집](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 작업 또는 문제 헤더의 지정 영역에서
* 작업 로드 밸런서에서 자세한 내용은 [작업 로드 밸런서를 사용하여 수동으로 작업 할당](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

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
   <td> <p>작업 및 문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 또는 문제에 대한 권한 또는 그 이상의 권한 기여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 고급 할당

1. 작업 또는 문제를 할당할 프로젝트로 이동합니다.
1. 클릭 **작업** 또는 **문제** 왼쪽 패널에서 목록의 작업 또는 문제 이름을 클릭합니다.

   >[!TIP]
   >
   >지정된 사람이 두 명 이상인 경우 작업이나 문제 목록에서 직접 고급 할당을 수행할 수 있습니다. 의 내부를 클릭합니다. **지정** 작업이나 문제와 같은 줄에 있는 필드를 클릭한 다음 **사람 아이콘** 고급 지정 창을 열려면 고급 할당을 계속 만들려면 5단계로 건너뜁니다.\
   >![](assets/nwe-advanced-assignments-350x55.png)   >

1. 클릭 **할당 대상** 에서 **지정** 작업 또는 문제 헤더의 필드

   또는

   작업이나 문제가 이미 할당된 경우 지정 이름을 누릅니다.

1. 클릭 **고급**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 에서 **사람, 역할 및 팀 검색** 필드에서 사용자, 역할 또는 팀의 이름을 입력하고 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   >[!NOTE]
   >
   >사용자 이름에 특수 문자가 포함되어 있으면 검색 필드에 특수 문자를 포함해야 합니다.

1. (선택 사항) **사람, 역할 또는 팀 검색** 상자를 사용하여 작업 또는 문제에 여러 리소스를 추가합니다.

   >[!TIP]
   >
   >* 여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
   >
   >
   >* 사용자 지정을 추가할 때 아바타, 사용자의 기본 역할 또는 이메일 주소를 확인하여 동일한 이름을 사용하는 사용자를 구별하십시오. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.
   >
   >
   >* 사용자, 작업 역할 또는 팀이 비활성화되기 전에 할당된 경우 작업 항목에 지정된 상태로 유지됩니다. 이 경우 다음을 권장합니다.
      >   
      >   * 작업 항목을 활성 자원에 재지정합니다.
      >   * 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


1. 의 각 사용자에 대해 **할당자** 열에서 다음 정보를 지정합니다.


   * **소유자**: 할당자의 이름을 마우스로 가리킨 다음 을 클릭합니다 **기본 구성** 소유자 필드에서 담당자를 임무 또는 문제 소유자로 표시하려면 다음 단계를 수행합니다. 녹색 확인란은 지정된 사용자가 해당 작업의 주요 연락처임을 나타냅니다. Adobe Workfront은 작업이나 문제에 지정하는 첫 번째 사용자 또는 작업 역할을 소유자 또는 기본 지정으로 표시합니다. 팀은 작업 또는 문제의 기본 소유자를 지정할 수 없습니다.

      >[!IMPORTANT]
      >
      >Workfront 관리자 또는 그룹 관리자가 프로젝트 환경 설정을 지정하는 방법에 따라, Workfront에서는 작업에 여러 사용자가 할당되어 있을 때 작업 소유자의 일정을 사용하여 작업 타임라인을 계산할 수 있습니다. 여러 작업 할당자에 대한 자세한 내용은 문서의 &quot;작업에 여러 사용자 할당&quot; 섹션을 참조하십시오 [작업 할당](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **할당** : 작업의 기간 유형이 간단하면 각 사용자 또는 작업 역할을 작업에 할당할 시간을 지정합니다. 각 사용자에 대해 지정된 모든 시간의 합은 **계획 시간** 배부 열 하단의 필드. 다른 모든 경우에는 할당자가 작업이나 문제를 해결하는 데 사용할 시간(또는 할당)의 백분율을 지정합니다.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

      >[!TIP]
      >
      >
      >   
      >   
      >   * 작업에 대한 할당 할당을 수동으로 수정한 후 작업의 계획 시간이 그에 따라 업데이트될 수 있습니다. 자세한 내용은 문서의 &quot;사용자 할당을 관리할 때 작업 계획 시간 업데이트&quot; 섹션을 참조하십시오 [계획 시간 개요](../../../manage-work/tasks/task-information/planned-hours.md).
      >   * 문제에 대한 할당 배당은 수동으로 수정할 수 없습니다.
      >   * 작업에 할당된 팀의 할당을 수동으로 수정할 수 없습니다.


   * **할당자의 역할:** 이 지정을 이행할 때 사용자가 사용해야 하는 역할을 선택합니다.  기본적으로 사용자의 기본 역할 이 표시됩니다. 할당자의 역할 상자에서 을 클릭하여 다른 역할을 선택합니다.  작업 또는 문제를 역할에 먼저 할당한 다음 해당 역할을 두 번째 할당으로 수행할 수 있는 사용자를 추가하면, 작업 및 문제에 이미 할당된 역할을 수행할 수 있는 사용자를 위해 제안된 사용자 목록이 필터링됩니다.

      ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   * **기간 유형**: 작업에만 사용할 수 있습니다. 기간 유형 이름을 클릭하고 드롭다운 메뉴에서 기간 유형을 선택합니다. 기간 유형에 대한 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **기간:** 작업에 대한 관리 권한이 있으면 작업에 대해 이 필드를 업데이트할 수 있습니다.

      자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 할당 정보를 벌크 편집할 때 사용자, 시간, 할당 및 작업 소유자를 지정하는 것과 유사한 대화 상자가 나타납니다.

   * **계획 시간**: 기간 유형이 계산된 지정 또는 단순 일 경우 계획 시간 수를 갱신합니다. 따라서 각 리소스의 할당 백분율 또는 시간이 균등하게 분배됩니다. Workfront은 기간 유형이 계산된 작업 시간 또는 투입 중심인 계획 시간을 계산합니다. 자세한 내용은 [작업 기간 및 기간 유형 개요](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

      ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. **저장**&#x200B;을 클릭합니다.
