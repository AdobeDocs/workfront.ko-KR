---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: 작업 및 문제 위임
description: 부재 중에 할당된 작업을 일시적으로 위임할 수 있습니다. 이 문서에서는 작업 및 문제 지정을 위임하는 방법에 대해 설명합니다.
author: Alina
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 72a2927d33f40c4fe08888712bdf62e9a5db9c40
workflow-type: tm+mt
source-wordcount: '1483'
ht-degree: 1%

---

# 작업 및 문제 위임 관리

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

부재 중에 할당된 작업을 일시적으로 위임할 수 있습니다.

작업 및 문제 지정을 위임하거나 승인을 위임할 수 있습니다. 이 문서에서는 작업 및 문제 지정을 위임하는 방법에 대해 설명합니다.

작업 위임에 대한 일반적인 내용은 [작업 개요 위임](../../manage-work/delegate-work/delegate-work-overview.md).

## 액세스 요구 사항

>[!IMPORTANT]
>
>* 대리인으로 선택하는 사용자는 사용자에게 위임하는 작업 및 문제에 대한 권한과 동일한 권한을 받습니다.
>* 권한은 액세스 수준 내에서 작동해야 하며, 액세스 수준이 사용자의 액세스 수준보다 낮을 수 있습니다.

   >
   >   
   >   예를 들어, 사용자에게 액세스 수준의 작업에 대한 보기 액세스 권한만 있고 사용자에게 위임하는 작업에 대한 관리 권한이 있는 경우, 사용자에게 위임하는 작업에 대한 관리 권한을 받습니다. 그러나 위임된 작업에 대해 사용자와 동일한 작업을 수행할 수는 없습니다. 부재 시 작업을 업데이트할 수 있도록 시스템 관리자에게 작업에 대한 편집 액세스 권한을 요청해야 합니다.
   >
   >   
   >   사용자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* 위임이 이미 시작된 후 지정된 항목의 경우 항목이 지정된 후 최대 1시간이 소요될 수 있습니다 [!DNL Workfront] 새로 할당된 항목을 대리자와 공유하려면 다음을 수행하십시오.



이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>검토 이상</p>

>[!NOTE]
>
>요청 라이센스가 있을 때 작업에 할당될 수 있지만 다른 사용자에게 작업을 위임할 수 없습니다. [!DNL Workfront] 에서는 검토 또는 요청 사용자에게 작업을 할당하지 않는 것이 좋습니다.

</tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업 및 문제에 대한 액세스 편집 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> 사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>할당된 작업 또는 문제에 대한 권한 보기 또는 그 이상의 권한</p> 
    <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*어떤 플랜, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## 전제 조건

이 문서에 설명된 활동을 수행하려면 먼저 다음을 확인해야 합니다.

* 사용자 [!DNL Workfront] 또는 그룹 관리자가 활성화됨 [!UICONTROL 사용자가 로그된 시간 관련 작업 및 문제를 삭제할 수 있도록 허용] 설정 [!UICONTROL 설정] 영역 [!DNL Workfront] 인스턴스.

   자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## 다른 사용자에게 작업 및 문제 위임

작업을 다른 사람에게 위임하기 전에, 사용자에게 연락하여 작업 항목에 대한 위임인으로 지정되도록 하는 것이 좋습니다. 일을 위임하기 전에 그들의 구두 승인을 요청하여, 당신이 부재 중에 일을 끝낼 시간이 있는지 확인하라.

작업 및 문제 위임에 대한 일반적인 내용은 [작업 및 문제 위임 개요](delegate-work.md).

작업 및 문제를 다른 사용자에게 위임하려면

1. 로 이동합니다. [!UICONTROL **홈**] 영역을 클릭한 다음 [!UICONTROL **위임**] 맨 위에 [!UICONTROL **작업 목록**].

   ![](assets/delegate-button-in-home.png)

1. 에서 [!UICONTROL **작업 및 문제 위임**] 탭에서 다음을 업데이트합니다.

   * [!UICONTROL **작업 및 문제를**]: 작업 및 문제를 위임할 사용자 이름을 입력한 다음 목록에 표시될 때 선택합니다. 사용자를 하나만 선택할 수 있습니다.\

      위임으로 선택하는 사용자는 위임한 작업 및 문제에 대한 권한과 동일한 권한을 받습니다. 자세한 내용은 [작업 및 문제 개요 위임](delegate-work-overview.md).

   * [!UICONTROL **시작 날짜**]: 작업 항목 위임을 시작할 달력에서 날짜를 선택합니다.

      >[!TIP]
      >
      >시작 날짜는 과거일 수 없습니다.

   * [!UICONTROL **종료 날짜 없음**]: 위임의 종료 날짜를 지정하지 않으려면 이 옵션을 선택합니다.

   * [!UICONTROL **종료 날짜**]: 위임을 중지할 날짜를 달력에서 선택합니다.

      >[!TIP]
      >
      >종료 날짜를 선택하지 않으면 현재 날짜에 대해서만 위임을 사용할 수 있습니다.

      ![](assets/delegate-box-expanded-in-home.png)

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   다음 상황이 발생합니다.

   * 작업이 지정된 사용자에게 위임됩니다. 선택한 기간 내에 날짜가 있는 불완전한 작업 또는 문제(위임을 활성화한 후 새로 지정된 작업 포함)가 위임됩니다.
   >[!TIP]
   >
   >   위임의 기간 내에 날짜가 있는 완료된 작업 항목은 위임되지 않습니다.


   * 화면의 오른쪽 상단 모서리에 메시지가 표시되어 다른 사용자에게 작업 위임을 활성화했는지 확인합니다. 확인 메시지에 위임 사용자의 이름이 표시됩니다.

   * 작업 및 문제가 다른 사용자에게 위임된다는 표시는 대부분의 영역에 표시됩니다. [!DNL Workfront]. 대리자 이름을 포함하지 않는 영역에 대한 자세한 내용은 [작업 및 문제 개요 위임](delegate-work-overview.md).

   * 다음 [!UICONTROL **위임**] 단추 [!UICONTROL 홈] 영역 변경 [!UICONTROL **위임 편집**] 위임이 적소에 있음을 나타냅니다.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * 이벤트 알림 및 개인 알림이 활성화되면 위임에 대한 이메일 확인도 받게 됩니다.

   * 대리자로 선택한 사용자는 해당 이벤트 알림이 활성화된 경우 위임에 대한 이메일을 수신합니다.

      개인 이메일 알림 활성화에 대한 자세한 내용은 [고유한 이벤트 알림 활성화 또는 비활성화](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).





## 위임 편집 또는 중지

위임 종료 날짜를 선택한 경우 또는 수동으로 중지할 수 있는 경우, 위임을 만료하도록 할 수 있습니다. 위임의 날짜가 변경된 경우 위임의 기간을 수정할 수도 있습니다.

1. 로 이동합니다. [!UICONTROL 홈] 영역을 클릭한 다음 [!UICONTROL 위임 편집] 작업 목록 오른쪽 위 모서리에서 을 클릭합니다.
1. 에서 [!UICONTROL 작업 및 문제 위임] 탭에서 다음 중 하나를 수행합니다.
   * 수정 [!UICONTROL **시작 날짜**] 또는 [!UICONTROL **종료 날짜**]
   * 클릭 [!UICONTROL **위임 중지**]

   >[!TIP]
   >
   >    위임이 이미 시작된 경우 위임의 종료 날짜만 편집할 수 있습니다.

   ![](assets/stop-delegation-screen-in-home.png)

1. (조건부) 클릭 [!UICONTROL **저장**] 새 위임 날짜를 저장하려면

   또는

   클릭 [!UICONTROL **위임 중지**] 확인 상자에서 위임 중지를 확인합니다.

   위임은 날짜를 업데이트하거나 중지했으며 위임된 사용자가 작업 및 문제와 관련하여 제거되었습니다. 작업 및 문제에 대한 권한은 그대로 유지됩니다.


## 위임된 작업 및 위임 정보 찾기

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

작업 및 문제가 위임되면 에는 몇 가지 영역이 있습니다 [!DNL Workfront] 위임된 작업이나 대리인이 누구인지 확인할 수 있는 곳

* [지정 상자에서 위임 찾기](#locate-delegates-in-the-assignments-box)
* [에서 위임된 작업 찾기 [!UICONTROL 홈]](#locate-delegated-work-in-home)


### 에서 위임 찾기 [!UICONTROL 지정] 상자

시스템 또는 그룹 관리자가 시스템에서 작업 위임을 사용할 수 있게 되면 [!UICONTROL 지정] 상자에 액세스할 수 있는 모든 위치에 다음 탭이 표시됩니다.

* [!UICONTROL **지정**]: 작업 또는 문제에 지정된 사용자가 여기에 표시됩니다.
* [!UICONTROL **위임**]: 작업 또는 문제 담당자에 의해 대리자로 지정된 사용자가 여기에 표시됩니다.

에 액세스할 수 있습니다 [!UICONTROL 지정] 상자를 엽니다.

* 작업 또는 문제 헤더

   ![](assets/assignments-and-delegates-panel-in-task-header.png)

   다음 [!UICONTROL 지정] 작업 또는 문제 헤더의 필드가 [!UICONTROL 지정 및 위임].

* 다음 [!DNL Workload Balancer] 수동으로 작업 또는 문제 할당

   ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> 에서는 대리자를 볼 수 없습니다 [!UICONTROL 지정] 작업 또는 문제 편집 상자의 섹션

작업 또는 문제가 위임되고 [!UICONTROL 위임] 하위 탭이 비어 있으면 다음 시나리오 중 하나가 존재할 수 있습니다.

* 작업 또는 문제에 할당되지 않았습니다.
* 작업 또는 문제 날짜가 위임 시간 기간을 벗어납니다.

>[!TIP]
>
>위임된 작업 및 문제에 대한 계획 또는 실제 시간은 다음과 같은 리소스 관리 도구에서 고려하지 않습니다. [!DNL Workload Balancer] 또는 [!DNL Resource Planner] 에 대해 지속 기간을 한 번의 방문으로 설정해야 합니다. 시간은 지정된 사용자만 연결됩니다.

### 에서 위임된 작업 찾기 [!UICONTROL 홈]

1. 로 이동합니다. [!UICONTROL **홈**] 영역을 클릭한 다음 필터 드롭다운 메뉴를 클릭하고 다음 옵션 중 하나 이상을 선택합니다.
   * [!UICONTROL **위임됨**]: 을 입력하여 본인에게 위임된 작업 및 문제를 확인합니다.
   * [!UICONTROL **나에게 위임됨**]: 다른 사용자가 자신에게 위임한 작업 및 문제를 보려면
   * [!UICONTROL **내가 위임함**]: 다른 사용자에게 위임된 작업 및 문제를 보려면

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. 을(를) 클릭합니다. [!UICONTROL 정렬] 드롭다운 메뉴를 사용하여 다음 기준에 따라 목록을 정렬합니다.
   * [!UICONTROL 계획된 완료]. 기본 정렬 옵션입니다.
   * [!UICONTROL 계획된 시작]
   * [!UICONTROL 커밋 일자]
   * [!UICONTROL 프로젝트]
   * [!UICONTROL 내 우선 순위]
1. 에서 그룹화 확장 [!UICONTROL **작업 목록**] 위임된 작업 항목을 조회하려면 다음 시나리오가 있습니다.
   * 다른 사용자에게 위임한 항목의 경우 대리자의 이름이 [!UICONTROL **작업 목록**] 뿐만 아니라 [!UICONTROL **지정 및 위임**] 오른쪽에 있는 필드.

   * 사용자에게 위임된 항목의 경우 할당자의 이름이 [!UICONTROL **작업 목록**] 뿐만 아니라 **[!UICONTROL 지정 및 위임]** 오른쪽에 있는 필드.
   >[!TIP]
   >
   >    위임이 오늘 일자 이후의 일자에 시작하도록 설정된 경우 위임의 시작 날짜도 [!UICONTROL 작업 목록]. 위임된 항목이 선택한 그룹에 표시됩니다 [!UICONTROL 작업 목록]를 반환합니다. 예를 들어 [!UICONTROL 계획 완료 일자]을 지정하면, 위임된 항목이 해당 계획 완료 일자와 일치하는 그룹화에 표시됩니다.
