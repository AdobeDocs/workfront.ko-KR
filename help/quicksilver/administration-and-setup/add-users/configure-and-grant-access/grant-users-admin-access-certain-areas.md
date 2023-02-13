---
title: 특정 영역에 대한 관리자 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 시스템의 특정 영역에 대한 플랜 라이선스 관리 액세스 권한을 사용자에게 부여할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# 특정 영역에 대한 관리자 액세스 권한 부여

<!--Linked in several places, do not rename or change URL.-->

Adobe Workfront 관리자는 액세스 수준을 사용하여 시스템의 특정 영역에 대한 플랜 라이선스 관리 액세스 권한을 사용자에게 부여할 수 있습니다.

>[!NOTE]
>
>이는 사용자에게 다음에 설명된 Workfront에 대한 전체 관리자 액세스 권한을 제공하는 것과는 다릅니다. [사용자에게 전체 관리자 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)&#x200B;.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront의 특정 영역에 대한 계획 사용자 관리 액세스 권한 부여

>[!IMPORTANT]
>
>사용자를 설정한 후 참조할 수 있도록 기본 액세스 수준을 그대로 두는 것이 좋습니다. 액세스 레벨을 사용자 정의하려면 기본 액세스 레벨을 복사하고 복사본을 수정합니다. 시스템 관리자 및 외부 사용자를 제외하고 모든 액세스 수준에 대해 이 작업을 수행할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **액세스 수준**.
1. 사용자에게 Workfront의 특정 영역에 대한 관리자 액세스 권한을 부여하는 데 사용할 액세스 수준의 이름을 클릭합니다.
1. 에서 **에 대한 관리자 액세스 허용** 섹션에 있는 확인란을 선택하여 필요한 관리 액세스를 부여합니다.

   이러한 옵션을 사용하면 다음 기능을 부여할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 프로세스</td> 
      <td><p>시스템 전체에서 특정 그룹에 사용할 승인 프로세스를 만들고 관리합니다.</p><p>이 액세스 권한이 없으면 사용자는 액세스 권한이 있는 항목에 대한 임시 승인 프로세스만 만들 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">회사</td> 
      <td><p>Workfront에서 새 회사 추가 및 기존 회사 편집</p>
      <p>이 액세스 권한이 없으면 사용자는 기존 회사만 볼 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 정의 양식</td> 
      <td><p>그룹 내에서 사용자 지정 양식을 만들고 편집(필드 추가, 편집 및 삭제)합니다.</p><p>이 액세스 권한이 없으면 사용자는 기존 양식을 기여 또는 관리할 액세스 권한이 있는 객체에만 첨부할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">환율</td> 
      <td> <p>Workfront에서 새 통화를 추가합니다.</p> <p>이 액세스 권한이 없으면 사용자는 기존 통화를 자신이 만드는 프로젝트에만 추가할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td><p>Workfront의 개체에 대한 모든 비용을 봅니다.</p><p>사용자가 새 비용 유형을 생성할 수 없습니다.</p><p>이 액세스 권한이 없으면 사용자는 다음을 볼 수만 있습니다.</p>
       <ul>
        <li>관리하는 프로젝트, 작업 또는 문제에 대한 비용</li>
        <li>그들 자신의 비용</li>
        <li>부하의 경비</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 역할</td> 
      <td> <p>이 액세스 권한을 통해 사용자는 다음을 수행할 수 있습니다.</p> 
       <ul> 
        <li>기존 작업 역할 보기 및 편집</li> 
        <li>새 작업 역할 추가</li> 
        <li>역할 청구 및 비용 비율 편집</li> 
       </ul> <p><b>중요 사항</b>: Job 역할에 Planner 사용자 관리 액세스 권한을 부여하는 경우, Financial Data 액세스 설정 역할 청구 및 비용 비율 편집이 사용자에 대해 자동으로 사용으로 설정됩니다. 나중에 계획자 사용자의 작업 역할에 대한 관리자 액세스를 사용하지 않도록 설정하면 역할 청구 및 비용 비율 편집 설정이 여전히 사용으로 설정되어 있으므로 작업 역할이 사용자에게 계속 표시됩니다. 이러한 경우 작업 역할을 보기 위해 사용자의 액세스를 제거해야 하는 경우 사용자의 역할 청구 및 비용 비율 편집 권한 설정을 비활성화해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">재무 데이터에 대한 액세스 권한 부여</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">내 그룹의 마일스톤</td> 
      <td>설정의 이정표 경로 메뉴 아래에서 시스템의 모든 이정표 경로를 봅니다. 사용자는 해당 그룹에 속하는 이정표 경로를 편집하거나 삭제할 수도 있습니다. 사용자는 해당 그룹에 할당되지 않은 이정표 경로를 관리(편집 또는 삭제)할 수 없습니다.<br><p>이 액세스 권한이 없으면 사용자는 기존 이정표 경로만 보고 관리할 수 있는 프로젝트에 적용할 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td>Workfront에서 미리 알림 알림을 만들고 관리합니다.<br>이 액세스 권한이 없으면 사용자는 알림을 받고 보는 것으로 제한됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임시트 및 시간</td> 
      <td> <p>사용자가 Workfront의 모든 시간 및 작업표를 볼 수 있습니다.</p> <p>이 옵션을 비활성화하면 사용자는 몇 시간만 볼 수 있습니다.</p> 
       <ul> 
        <li>관리하는 프로젝트, 작업 또는 문제</li> 
        <li>자신의 작업표</li> 
        <li>사용자에게 보고하는 사용자의 작업표</li> 
        <li>그들이 승인하는 작업표</li> 
       </ul> <p><b>메모</b>:  <p>이 옵션을 활성화하든 사용하지 않든, 그룹 관리자는 관리하는 그룹 및 하위 그룹에 대한 작업표 프로필을 만들어 사용자 프로필이 편집 가능한 그룹 구성원에게 할당할 수 있습니다.</p> <p>이 옵션을 활성화하면 관리 그룹의 사용자뿐만 아니라 시스템의 모든 사용자에 대해 작업표 프로필(및 시간)로 생성된 작업표를 볼 수 있으므로 일부 그룹 관리자에게 너무 많은 액세스 권한을 제공할 수 있습니다. 이렇게 많은 액세스 권한이 필요하지 않은 그룹 관리자에 대해 이 옵션을 비활성화할 수 있습니다.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 완료되면 를 클릭합니다 **저장**.
1. 에 설명된 대로 사용자에게 새 액세스 수준을 할당합니다. [사용자 추가](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >사용자에게 사용자에게 관리자 액세스 권한을 부여할 수 있습니다. 사용자가 사용자 계정을 관리할 수 있도록 사용자에게 관리자 액세스 권한을 제공하는 방법에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
