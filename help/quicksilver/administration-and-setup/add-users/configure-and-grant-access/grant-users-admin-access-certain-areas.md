---
title: 사용자에게 특정 영역에 대한 관리 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 플랜 라이선스 사용자에게 시스템의 특정 영역에 대한 관리 액세스 권한을 부여할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 2%

---

# 사용자에게 특정 영역에 대한 관리 액세스 권한 부여

<!--Linked in several places, do not rename or change URL.-->

Adobe Workfront 관리자는 액세스 수준을 사용하여 플랜 라이선스 사용자에게 시스템의 특정 영역에 대한 관리 액세스 권한을 부여할 수 있습니다.

>[!NOTE]
>
>사용자에게 Workfront에 대한 전체 관리 액세스 권한을 부여하는 것과 다릅니다. 자세한 내용은 [사용자에게 전체 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)를 참조하십시오&#x200B;.

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
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 플랜 사용자에게 Workfront의 특정 영역에 대한 관리 액세스 권한 부여

>[!IMPORTANT]
>
>사용자를 설정한 후에 참조할 수 있도록 기본 제공 액세스 수준을 변경하지 않는 것이 좋습니다. 액세스 수준을 사용자 지정하려면 기본 액세스 수준을 복사하고 복사본을 수정합니다. (시스템 관리자 및 외부 사용자를 제외한 모든 액세스 수준에 대해 이 작업을 수행할 수 있습니다.)

{{step-1-to-setup}}

1. 왼쪽 패널에서 **액세스 수준**&#x200B;을 클릭합니다.
1. 사용자에게 Workfront의 특정 영역에 대한 관리 액세스 권한을 부여하는 데 사용할 액세스 수준의 이름을 클릭합니다.
1. **관리 액세스 허용** 섹션에서 필요한 관리 액세스 권한을 부여하는 확인란을 선택하십시오.

   이러한 옵션을 사용하면 다음 기능을 부여할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스</td> 
      <td><p>시스템 전체에서 그리고 특정 그룹에 사용할 승인 프로세스를 만들고 관리합니다.</p><p>이 액세스 권한이 없으면 사용자는 관리 액세스 권한이 있는 항목에 대해 임시 승인 프로세스만 만들 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">회사</td> 
      <td><p>Workfront에서 새 회사 추가 및 기존 회사 편집</p>
      <p>이 액세스 권한이 없으면 사용자는 기존 회사만 볼 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식</td> 
      <td><p>그룹 내에서 사용자 정의 양식을 만들고 편집(필드 추가, 편집 및 삭제)합니다.</p><p>이 액세스 권한이 없으면 사용자는 기여 또는 관리에 대한 액세스 권한이 있는 개체에만 기존 양식을 첨부할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">환율</td> 
      <td> <p>Workfront에서 새 통화를 추가합니다.</p> <p>이 액세스 권한이 없으면 사용자는 자신이 만드는 프로젝트에 기존 통화만 추가할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td><p>Workfront의 개체에 대한 모든 비용을 봅니다.</p><p>사용자가 새 경비 유형을 만들 수 없습니다.</p><p>이 액세스 권한이 없으면 사용자는 다음만 볼 수 있습니다.</p>
       <ul>
        <li>관리하는 프로젝트, 작업 또는 문제의 경비</li>
        <li>자신의 경비</li>
        <li>부하 직원의 비용</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 역할</td> 
      <td> <p>이 액세스 권한을 통해 사용자는 다음 작업을 수행할 수 있습니다.</p> 
       <ul> 
        <li>기존 작업 역할 보기 및 편집</li> 
        <li>새 작업 역할 추가</li> 
        <li>역할 청구 및 비용 요금 편집</li> 
       </ul> <p><b>중요</b>: 플래너 사용자에게 작업 역할에 대한 관리 액세스 권한을 부여하면 사용자에 대해 [역할 청구 및 비용 요금 편집] 재무 데이터 액세스 설정이 자동으로 활성화됩니다. 나중에 플래너 사용자의 작업 역할에 대한 관리 액세스를 비활성화하면 역할 청구 및 비용 요금 편집 설정이 계속 활성화되어 있기 때문에 작업 역할이 사용자에게 계속 표시됩니다. 이 경우 작업 역할을 보려면 사용자의 액세스 권한을 제거해야 합니다. 사용자의 역할 청구 및 비용 요금 편집 권한 설정을 비활성화해야 합니다. 지침은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 그룹의 마일스톤</td> 
      <td>설정 의 마일스톤 경로 메뉴에서 시스템의 모든 마일스톤 경로를 봅니다. 사용자는 자신의 그룹에 속한 모든 마일스톤 경로를 편집하거나 삭제할 수도 있습니다. 사용자는 그룹 중 어느 것에도 할당되지 않은 마일스톤 경로를 관리(편집 또는 삭제)할 수 없습니다.<br><p>이 액세스 권한이 없으면 사용자는 기존 마일스톤 경로를 보고 관리할 수 있는 액세스 권한이 있는 프로젝트에만 적용할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td>Workfront에서 미리 알림을 만들고 관리합니다.<br>이 액세스 권한이 없으면 사용자는 알림을 받고 볼 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트 및 시간</td> 
      <td> <p>사용자가 Workfront의 모든 시간과 타임시트를 볼 수 있도록 허용합니다.</p> <p>이 옵션이 비활성화되면 사용자는 다음에 대한 시간만 볼 수 있습니다.</p> 
       <ul> 
        <li>프로젝트, 작업 또는 문제</li> 
        <li>자신의 타임시트</li> 
        <li>사용자에게 보고하는 사람의 타임시트</li> 
        <li>해당 사용자가 승인한 타임시트</li> 
       </ul> <p><b>참고</b>:  <p>이 옵션의 활성화 여부에 관계없이 그룹 관리자는 자신이 관리하는 그룹 및 하위 그룹에 대한 타임시트 프로필을 만들고 편집할 수 있는 액세스 권한이 있는 그룹 구성원에게 할당할 수 있습니다.</p> <p>이 옵션을 활성화하면 관리하는 그룹의 사용자뿐만 아니라 시스템의 모든 사용자에 대해 타임시트 프로필에서 생성된 타임시트(및 시간)를 볼 수 있으므로 일부 그룹 관리자에게 너무 많은 액세스 권한을 제공할 수 있습니다. 액세스 권한이 필요하지 않은 그룹 관리자에 대해 이 옵션을 비활성화할 수 있습니다.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 완료되면 **저장**&#x200B;을 클릭하세요.
1. [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)에 설명된 대로 사용자에게 새 액세스 수준을 할당합니다.

   >[!NOTE]
   >
   >사용자가 사용자에게 관리 액세스 권한을 부여할 수 있습니다. 사용자가 사용자 계정을 관리할 수 있도록 사용자에게 관리 액세스 권한을 부여하는 방법에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.
