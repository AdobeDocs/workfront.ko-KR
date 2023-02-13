---
title: 전역 승인 설정 구성
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Adobe Workfront 관리자는 Workfront에서 승인 프로세스에 대한 전역 설정을 결정할 수 있습니다. 이러한 설정은 시스템의 모든 작업 항목 승인 프로세스에 영향을 줍니다.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 3%

---

# 전역 승인 설정 구성

Adobe Workfront 관리자는 Workfront에서 승인 프로세스에 대한 전역 설정을 결정할 수 있습니다. 이러한 설정은 시스템의 모든 작업 항목 승인 프로세스에 영향을 줍니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>시스템 관리자이거나 승인 프로세스에 대한 관리자 액세스 권한이 있는 계획 라이센스가 있어야 합니다</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전역 승인 설정 구성

1. Workfront as a Workfront 관리자에 로그인합니다.
1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **프로세스** > **승인** .

1. 을(를) 클릭합니다. **설정** 아이콘 ![](assets/gear-icon-settings.png) 다음 **승인** 영역 이름.

1. 에서 **승인 설정** 표시되는 상자에 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">추가 &lt;number&gt; 승인 프로세스를 수용할 계획 완료 일자 일수</td> 
      <td> <p>승인이 필요한 작업의 계획 완료 날짜에 시간을 추가할 분, 시간, 일, 주 또는 개월 수를 지정합니다. "경과" 분, 시간, 일 또는 주를 선택하여 시스템 작업 일정 달력에 지정된 주말, 휴일 및 비근무 시간을 포함하는 시간을 추가합니다.</p> 
      <p>예를 들어, 금요일에 작업이 지정되고 기간이 3일 경과된 경우, 작업 완료 날짜는 월요일로 설정됩니다(토요일과 일요일이 주말로 가정). 작업에 3일(경과되지 않음)의 기간이 있는 경우 작업 완료 날짜가 수요일로 설정됩니다.</p>
      <p><b>참고</b>: 작업에 대한 승인을 위해 수용 가능한 추가 시간을 추가하면 작업의 타임라인과 프로젝트의 타임라인에 영향을 줍니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인자가 프로젝트 팀에 속해 있지 않아도 됩니다(역할이 포함된 승인 진행의 경우)</td> 
      <td> <p>승인 프로세스에 역할이 포함되어 있을 때 프로젝트 팀에 승인자가 없을 필요가 있는 경우 이를 선택합니다. 작업 역할에 승인 결정을 할당할 때 프로젝트에서 해당 역할과 연관된 역할을 가진 사용자만 승인을 볼 수 있습니다. 이 설정을 사용하면 해당 작업 역할을 가진 모든 사용자가 프로젝트 팀에 있는지 여부에 따라 승인 요청을 받습니다. 사용자의 프로젝트 역할 편집에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">프로젝트 팀 관리</a>. </p> 
      <p><b>팁</b>: 역할 및 옵션에 승인을 지정하는 경우 <b>승인자는 프로젝트 팀에 있을 필요가 없습니다(역할을 포함하는 승인 프로세스의 경우)</b> 이 비활성화되어 있지만 승인 시 역할과 일치하는 프로젝트 팀의 역할이 없습니다. 승인이 프로젝트 소유자에게 재할당됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 위임 비활성화</td> 
      <td> <p>시스템 사용자가 다른 사용자에게 승인을 위임할 수 있는 기능을 비활성화하려면 이 옵션을 선택합니다. 이 옵션을 선택하면 승인을 위임하는 옵션이 Workfront에서 제거되고 기존의 모든 승인 위임이 중지됩니다.</p> <p>Workfront에서 승인 위임에 대한 자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">승인 요청 위임</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">프로젝트, 작업 또는 문제가 승인 보류 중인 상태일 때 사용자 지정 양식 편집 허용</td> 
      <td> <p>사용자가 승인 보류 중 상태일 때 프로젝트, 작업 및 문제의 사용자 지정 형식을 편집할 수 있도록 하려면 이 옵션을 선택합니다. 기본 설정입니다.</p> 
      <p>이 옵션을 선택한 경우:</p> 
       <ul> 
       <li>현재 승인 경로 또는 승인 단계와 관계없이 객체가 승인 보류 중일 때 모든 승인자(및 사용자 지정 양식을 편집할 수 있는 액세스 권한이 있는 다른 사용자)가 사용자 지정 양식을 변경할 수 있습니다.</li> 
       <li>승인 프로세스 중에 사용자 지정 양식에 변경한 사항은 변경 전에 내린 승인 결정에는 영향을 주지 않습니다.</li> 
       <li> <p>프로젝트, 작업 또는 문제에 대한 모든 변경 내용은 이 설정에 관계 없이 동일한 방식으로 추적됩니다. </p> <p>예를 들어 업데이트 스트림에서 추적할 사용자 지정 양식 필드를 추가한 경우 양식의 모든 변경 사항이 개체의 업데이트 스트림에서 추적됩니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 새로 생성된 승인 보류 요청을 불러 올 수 있도록 허용</td> 
      <td> <p>사용자가 첫 번째 상태에 대해 문제를 회수할 수 있는지 또는 승인 보류 중인 요청을 회수할 수 있는지를 구성하려면 이 옵션을 선택합니다. 요청 큐를 구성하여 문제 또는 요청의 첫 번째 상태를 승인 프로세스와 연결할 수 있습니다. </p> 
      <p>요청 큐에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a>.</p> 
      <p>다음 중 하나를 수행하십시오.</p> 
       <ul> 
       <li>사용자가 문제 또는 요청의 첫 번째 상태에 대한 승인을 회수할 수 있도록 하려면 이 옵션을 선택합니다. 이 경우 승인 상태가 보류 중인 새 문제 또는 요청에 대해 회수&lt; 단추를 볼 수 있습니다. 문제를 상기하도록 선택하면 해당 문제도 삭제된다는 경고가 표시됩니다. 그 문제는 그들이 그것을 상기시킨 것을 확인한 후 삭제된다. </li> 
       <li> <p>사용자가 첫 번째 상태가 승인 보류 중인 요청이나 문제를 회수하지 못하도록 하려면 이 옵션을 선택 취소합니다. 새 문제 또는 요청에 대한 회수&lt; 단추가 표시되지 않으며 승인을 받아야 합니다. 기본 옵션입니다.</p> 
       <p>승인을 기다리는 항목을 검토하는 방법에 대한 자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">승인 보기 </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **변경 사항을 저장합니다.**
