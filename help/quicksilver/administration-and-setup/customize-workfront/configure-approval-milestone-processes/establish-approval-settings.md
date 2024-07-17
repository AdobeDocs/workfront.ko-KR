---
title: 전역 승인 설정 구성
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Adobe Workfront 관리자는 Workfront에서 승인 프로세스에 대한 전역 설정을 결정할 수 있습니다. 이 설정은 시스템의 모든 작업 항목 승인 프로세스에 영향을 줍니다.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# 전역 승인 설정 구성

Adobe Workfront 관리자는 Workfront에서 승인 프로세스에 대한 전역 설정을 결정할 수 있습니다. 이 설정은 시스템의 모든 작업 항목 승인 프로세스에 영향을 줍니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>시스템 관리자이거나 승인 프로세스에 대한 관리 액세스 권한이 있는 플랜 라이선스가 있어야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전역 승인 설정 구성

1. Workfront에 Workfront 관리자로 로그인합니다.
1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. **프로세스** > **승인** 을 클릭합니다.

1. **승인** 영역 이름 옆의 **설정** 아이콘 ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. 표시되는 **승인 설정** 상자에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스에 맞게 계획된 완료 일자에 &lt;number&gt;일 추가</td> 
      <td> <p>승인이 필요한 작업의 계획된 완료 일자에 시간을 추가하려면 분, 시간, 일, 주 또는 개월 수를 지정합니다. "경과 시간" 분, 시간, 일 또는 주를 선택하여 시스템 작업 일정 달력에 지정된 주말, 휴일 및 휴무 시간을 포함하는 시간을 추가합니다.</p> 
      <p>예를 들어 작업이 금요일에 할당되고 기간이 3일인 경우, 작업 완료 날짜가 월요일로 설정됩니다(토요일과 일요일이 주말이라고 가정). 작업의 기간이 3일(경과되지 않음)인 경우 작업 완료 날짜가 수요일로 설정됩니다.</p>
      <p><b>참고</b>: 작업에 대한 승인을 수용할 추가 시간을 사용하면 작업 및 프로젝트의 타임라인이 영향을 받습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인자는 프로젝트 팀에 속해 있지 않아도 됩니다(역할이 포함된 승인 프로세스의 경우).</td> 
      <td> <p>승인 프로세스에 역할이 포함되어 있을 때 승인자가 프로젝트 팀에 속해 있지 않아도 되는 경우 선택합니다. 작업 역할에 승인 결정을 할당할 때 프로젝트에서 사용자와 관련된 역할이 있는 사용자만 승인을 볼 수 있습니다. 이 설정을 사용하면 해당 작업 역할을 가진 모든 사용자가 프로젝트 팀에 있든 없든 승인 요청을 받습니다. 사용자의 프로젝트 역할 편집에 대한 자세한 내용은 <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">프로젝트 팀 관리</a>를 참조하십시오. </p> 
      <p><b>팁</b>: 역할에 승인을 할당하고 옵션 <b>승인자가 프로젝트 팀에 속해 있지 않아도 됩니다(역할이 포함된 승인 프로세스의 경우)</b>이(가) 비활성화되었지만 프로젝트 팀에 승인의 역할과 일치하는 역할이 없으면 승인이 프로젝트 소유자에게 다시 할당됩니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">승인 위임 비활성화</td> 
      <td> <p>시스템의 사용자가 다른 사용자에게 승인을 위임할 수 있는 기능을 비활성화하려면 이 옵션을 선택하십시오. 이 옵션을 선택하면 승인을 위임하는 옵션이 Workfront에서 제거되고 기존 승인 위임이 중지됩니다.</p> <p>Workfront에서 승인을 위임하는 방법에 대한 자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">승인 요청 위임</a> 을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">프로젝트, 작업 또는 문제가 승인 보류 상태일 때 사용자 정의 양식 편집 허용</td> 
      <td> <p>사용자가 승인 보류 중 상태일 때 프로젝트, 작업 및 문제의 사용자 정의 양식을 편집할 수 있도록 하려면 이 옵션을 선택합니다. 기본 설정입니다.</p> 
      <p>이 옵션을 선택한 경우:</p> 
       <ul> 
       <li>모든 승인자(및 사용자 정의 양식을 편집할 수 있는 액세스 권한이 있는 다른 사용자)는 오브젝트가 현재 승인 경로 또는 승인 단계에 관계없이 승인 보류 중일 때 사용자 정의 양식을 변경할 수 있습니다.</li> 
       <li>승인 프로세스 중에 사용자 정의 양식을 변경해도 변경 전에 이루어진 승인 결정에는 영향을 주지 않습니다.</li> 
       <li> <p>프로젝트, 작업 또는 문제에 대한 모든 변경 사항은 이 설정에 관계없이 동일한 방식으로 추적됩니다. </p> <p>예를 들어 업데이트 스트림에서 추적할 사용자 정의 양식 필드를 추가한 경우 양식의 모든 변경 사항이 오브젝트의 업데이트 스트림에서 추적됩니다.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 새로 생성된 승인 보류 요청을 불러 올 수 있도록 허용</td> 
      <td> <p>사용자가 첫 번째 상태에서 문제를 회수할 수 있는지 또는 승인 보류 중인 요청을 회수할 수 있는지 여부를 구성하려면 이 옵션을 선택합니다. 요청 대기열을 구성하여 문제 또는 요청의 첫 번째 상태를 승인 프로세스와 연결할 수 있습니다. </p> 
      <p>요청 대기열에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a>를 참조하십시오.</p> 
      <p>다음 중 하나를 수행하십시오.</p> 
       <ul> 
       <li>사용자가 문제 또는 요청의 첫 번째 상태에 대한 승인을 회수할 수 있도록 하려면 이 옵션을 선택합니다. 이 경우 승인 보류 중인 새 문제 또는 요청에 대해 회수&lt; 버튼이 표시됩니다. 리콜을 선택하면 해당 문제도 삭제된다는 경고가 표시됩니다. 리콜을 확인한 후 문제가 삭제됩니다. </li> 
       <li> <p>사용자가 첫 번째 상태가 승인 보류 중인 문제 또는 요청을 다시 호출하지 않도록 하려면 이 옵션을 선택 취소합니다. 새 문제 또는 요청에서 회수&lt; 버튼이 표시되지 않으며 승인을 받아야 합니다. 기본 옵션입니다.</p> 
       <p>승인 대기 중인 항목 검토에 대한 자세한 내용은 <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">승인 보기 </a>를 참조하십시오.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **변경 내용 저장**&#x200B;을 클릭합니다.
