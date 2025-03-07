---
title: 사용자 정의 액세스 수준 만들기 및 수정
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 사용자 정의 액세스 수준을 만들고 사용자에게 적용할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 3e48bebde0171c13b4168d7eb5d693b07cb9e396
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 6%

---

# 사용자 정의 액세스 수준 만들기 및 수정

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Adobe Workfront 관리자는 사용자 정의 액세스 수준을 만들고 사용자에게 적용할 수 있습니다. 액세스 수준으로 작업할 때는 사용자가 서로 개체를 공유할 때 부여하는 개체 권한으로 함께 작업하는 방법을 이해하는 것이 중요합니다. 액세스 수준에 대한 자세한 내용은 다음을 참조하십시오.

* [새로운 액세스 수준 개요](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>사용자를 설정한 후에 참조할 수 있도록 기본 제공 액세스 수준을 변경하지 않는 것이 좋습니다. 액세스 수준을 사용자 지정하려면 기본 액세스 수준을 복사하고 복사본을 수정합니다. 시스템 관리자 및 외부 사용자를 제외한 모든 액세스 수준에 대해 이 작업을 수행할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>새로운 기능: 표준
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 액세스 수준 만들기 또는 편집

{{step-1-to-setup}}

1. 왼쪽 패널에서 **액세스 수준**&#x200B;을 클릭합니다.
1. 복사하고 사용자 지정할 액세스 수준을 선택한 다음 **복사**&#x200B;를 클릭합니다.

   또는

   이전에 복사한 기존 액세스 수준을 편집하는 경우 해당 이름을 클릭합니다.

1. 표시되는 상자에서 다음 중 하나를 수행하여 사용자 정의 액세스 수준 구성을 시작합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>액세스 수준의 이름을 입력합니다. </p> <p>액세스 수준을 복사해서 새로 만드는 경우 기본 이름은 액세스 수준 이름(복사)입니다. 여기서 액세스 수준 이름은 복사한 액세스 수준입니다.</p> <p><strong>팁</strong>: 복사 이름에 액세스 수준의 원래 이름을 포함하는 것이 좋습니다. 예를 들어 ACME 회사에서 Standard 액세스 수준의 사본에 ACME Standard라는 이름을 지정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명 </td> 
      <td>액세스 수준에 대한 설명을 입력합니다. 이 액세스 수준을 가진 사용자가 액세스할 수 있는 내용을 여기에 나열하는 것이 유용합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">라이선스 유형</td> 
      <td>여기서 선택한 라이센스가 만들거나 편집하는 액세스 수준 유형과 가장 밀접하게 연관된 라이센스인지 확인합니다. 선택한 라이센스에 따라 액세스 수준에 사용할 수 있는 설정이 결정됩니다. 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">새 라이선스 개요</a> 또는 <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">라이선스 개요</a>를 참조하십시오.</td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) **라이선스 유형** 상자에서 **표준** 또는 **계획**&#x200B;을 선택한 경우 **관리 액세스 허용** 섹션으로 스크롤한 후 이 액세스 수준을 갖게 될 사용자에 대한 관리 액세스 권한을 선택하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스</td> 
      <td>시스템 전체에서 그리고 특정 그룹에 사용할 승인 프로세스를 만들고 관리합니다.<p>이 액세스 권한이 없으면 사용자는 관리 액세스 권한이 있는 항목에 대해 임시 승인 프로세스만 만들 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">회사</td> 
      <td>Workfront에서 새 회사를 추가하고 기존 회사를 편집합니다.<br><p>이 액세스 권한이 없으면 사용자는 기존 회사만 볼 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식</td> 
      <td>그룹 내의 모든 사용자 정의 양식을 만들고 관리합니다. <br><p>이 액세스 권한이 없으면 사용자는 기여 또는 관리할 액세스 권한이 있는 개체에만 기존 양식을 첨부할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">환율</td> 
      <td> Workfront에서 새 통화를 추가합니다. <p>이 액세스 권한이 없으면 사용자는 자신이 만드는 프로젝트에만 기존 통화를 추가할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td>Workfront의 개체에 대한 모든 비용을 봅니다.<p>이 액세스 권한이 없으면 사용자는 다음만 볼 수 있습니다.</p>
       <ul>
        <li>관리하는 프로젝트, 작업 또는 문제의 경비</li>
        <li>자신의 경비</li>
        <li>부하 직원의 비용</li>
       </ul><p><b>참고</b>: 사용자가 새 경비 유형을 만들 수 없습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 역할</td> 
      <td> 이 액세스 권한을 통해 사용자는 다음 작업을 수행할 수 있습니다. 
       <ul> 
        <li>기존 작업 역할 보기 및 편집</li> 
        <li>새 작업 역할 추가</li> 
        <li>역할 청구 및 비용 요금 편집</li> 
       </ul> 
       <p>작업 역할에 대한 관리 액세스 권한이 있는 Standard 또는 Planner 사용자가 사용할 수 있는 재무 데이터에 대한 중요한 정보는 <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">작업 역할에 대한 관리 액세스 권한이 있는 Standard 또는 Planner 사용자</a>를 참조하십시오.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 그룹의 마일스톤</td> 
      <td>설정 의 마일스톤 경로 메뉴에서 시스템의 모든 마일스톤 경로를 봅니다. 사용자는 자신의 그룹에 속한 모든 마일스톤 경로를 편집하거나 삭제할 수도 있습니다. 사용자는 그룹 그룹에 할당되지 않은 마일스톤 경로를 관리(편집 또는 삭제)할 수 없습니다.<p>이 액세스 권한이 없으면 사용자는 기존 마일스톤 경로를 보고 관리할 수 있는 액세스 권한이 있는 프로젝트에만 적용할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td>Workfront에서 미리 알림을 만들고 관리합니다.<p>이 액세스 권한이 없으면 사용자는 알림을 받고 볼 수 있는 것으로 제한됩니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트 및 시간</td> 
      <td> 그룹 관리자는 자신이 관리하는 그룹 및 하위 그룹의 사용자에게 타임시트 프로필을 할당할 수 있습니다. <p>이 옵션을 활성화하지 않으면 그룹 관리자는 자신이 관리하는 그룹 및 하위 그룹의 다른 사용자에게 타임시트 프로필을 만들 수 있지만 할당할 수 없습니다.</p> <p>Standard 또는 Plan 라이선스가 있는 다른 모든 사용자는 Workfront에서 모든 시간과 타임시트를 볼 수 있습니다.</p> <p>이 옵션을 활성화하지 않으면 사용자는 다음에 대한 시간만 볼 수 있습니다.</p> 
       <ul> 
        <li>프로젝트, 작업 또는 문제</li> 
        <li>자신의 타임시트</li> 
        <li>사용자에게 보고하는 사람의 타임시트</li> 
        <li>해당 사용자가 승인한 타임시트</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **추가 제한 설정**&#x200B;을 클릭한 다음 액세스 수준에 대해 다음 제한 중 하나를 설정합니다.

   >[!IMPORTANT]
   >
   >공급업체(조직에 없는 모든 사용자)와 같은 외부 사용자의 경우 작업, 프로젝트, 업데이트, 공지 사항, 기타 회사, 팀 및 그룹에 대한 액세스를 제한하는 것이 좋습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">작업 또는 문제를 할당할 때 전체 프로젝트에 대한 액세스 권한을 부여하지 마십시오.</td> 
      <td> 작업 또는 문제에 할당된 사용자가 상위 프로젝트에 대한 권한을 획득하지 못하도록 합니다(프로젝트 권한에서 허용하는 경우에도 마찬가지임).<p>프로젝트에 대한 권한을 구성하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">프로젝트 편집</a> 문서의 <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> 섹션을 참조하십시오.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">프로젝트, 작업, 문제 등에서 문서 액세스 권한을 상속하지 마십시오.</td> 
      <td>문서가 상위 개체에 설정된 권한을 상속하지 못하도록 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">대화에 포함된 업데이트만 보기</td> 
      <td> 사용자 이름 또는 팀 이름이 포함된 주석만 볼 수 있습니다. <p> <p><b>참고</b>: 사용자가 Workfront의 항목을 구독할 수 없습니다. 항목 구독에 대한 자세한 내용은 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Adobe Workfront에서 항목 구독</a>을 참조하세요.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 주석을 삭제하도록 허용하지 않음 </td> 
      <td> 사용자가 항목에 대한 주석을 삭제하지 못하도록 합니다.  <p><b>참고</b>: 다른 사용자의 댓글을 삭제할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">소속 회사, 그룹 및 팀만 보기</td> 
      <td>사용자가 자신이 속한 회사, 그룹 및 팀과만 항목을 보고 공유할 수 있도록 해줍니다.<p><strong>참고</strong>: 요청자 또는 기여자 라이선스가 있는 사용자는 이 옵션을 선택하더라도 자신이 속하지 않은 회사를 볼 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획된 시간 또는 실제 근로시간 표시 허용 안 함</td> 
      <td>사용자가 액세스할 수 있는 작업 항목의 계획된 및 실제 시간을 볼 수 없습니다. 그러나 자신이 기록한 실제 근로시간 또는 자신에게 보고하는 사람이 기록한 근로시간을 볼 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 공지를 삭제하도록 허용하지 않음</td> 
      <td>사용자가 공지 센터에서 공지를 삭제하지 못하도록 합니다. 자세한 내용은 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">공지 보내기</a>를 참조하십시오.</td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부 및 선택 사항) 여러 회사에 속한 사용자에 대해 Workfront 시스템을 설정한 경우 **다른 회사의 직원들은**&#x200B;의 사용자만 볼 수 있도록  섹션에서 해당 회사가 속한 회사에 따라 다른 사용자로 가시성을 제한합니다.

   자신의 회사 또는 기본 회사로 지정한 회사의 사용자만 보도록 사용자를 제한할 수 있습니다. 기본 회사는 일반적으로 대부분의 사용자가 근무하는 Workfront 계정을 나타냅니다. 기본 회사에 대한 자세한 내용은 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하세요.

   >[!NOTE]
   >
   >두 명의 사용자가 서로 다른 두 회사에 속하지만 둘 다 기본 회사의 사용자를 볼 수 있는 경우 기본 회사와 연관된 업데이트 영역을 볼 수 있습니다.

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나를 계속 사용하십시오(예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)).
1. **저장**&#x200B;을 클릭합니다.

   액세스 수준이 만들어지면 사용자에게 이를 할당할 수 있습니다(시스템 관리자 액세스 수준이 아닌 경우).

   자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

   Adobe 관리자가 사용자에게 시스템 관리자 액세스 수준을 할당하는 방법에 대한 자세한 내용은 [사용자에게 전체 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)를 참조하십시오.

## 작업 역할에 대한 관리 액세스 권한이 있는 표준 또는 플래너 사용자 {#planner-users}

작업 역할에 대해 표준 또는 계획자 사용자에게 관리 액세스 권한을 부여하는 경우 사용자에 대해 자동으로 역할 청구 및 비용 요금 편집 설정이 활성화됩니다.

나중에 사용자의 작업 역할에 대한 관리 액세스를 비활성화하면 역할 청구 및 비용 요금 편집 설정이 계속 활성화되어 있기 때문에 작업 역할이 사용자에게 계속 표시됩니다.

이 경우 작업 역할을 보려면 사용자의 액세스 권한을 제거해야 합니다. 사용자의 역할 청구 및 비용 요금 편집 권한 설정을 비활성화해야 합니다. 지침은 [재무 데이터에 대한 액세스 권한 부여](grant-access-financial.md)를 참조하십시오.



