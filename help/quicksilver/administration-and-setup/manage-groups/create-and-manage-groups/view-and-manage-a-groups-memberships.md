---
user-type: administrator
product-area: system-administration;user-management
keywords: 추가,사용자,그룹,추가,다른,할당,관리자,제거,사용자,보기,역할,구성원,내보내기,멤버십,데이터
navigation-topic: create-and-manage-groups
title: 그룹의 멤버십 보기 및 관리
description: Adobe Workfront 관리자는 관리하는 그룹의 구성원을 보고, 추가하고, 제거하고, 내보내고, 활성화하고, 비활성화할 수 있습니다. 또한 프로필을 편집하고, 프로필에 업데이트를 추가하고, 해당 프로필을 그룹의 추가 그룹 관리자로 지정할 수 있습니다.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 그룹 멤버십 보기 및 관리

Adobe Workfront 관리자는 관리하는 그룹의 구성원을 보고, 추가하고, 제거하고, 내보내고, 활성화하고, 비활성화할 수 있습니다. 또한 프로필을 편집하고, 프로필에 업데이트를 추가하고, 해당 프로필을 그룹의 추가 그룹 관리자로 지정할 수 있습니다.

그룹 위에 그룹이 있는 경우 해당 관리자는 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>그룹의 그룹 관리자 또는 시스템 관리자여야 합니다.</td>
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹 멤버십 보기 및 관리

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹**&#x200B;을 클릭합니다.

   표시되는 목록에서 Workfront 관리자는 모든 그룹과 하위 그룹을 볼 수 있습니다. 그룹 관리자는 자신이 관리하는 그룹과 하위 그룹만 볼 수 있습니다.

1. 편집할 그룹의 이름을 클릭합니다.
1. 왼쪽 메뉴에서 **그룹 구성원**&#x200B;을(를) 선택한 상태로 표시되는 페이지에서 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">사용자를 그룹에 추가</td> 
      <td> 
       <ol> 
        <li><strong>구성원 추가</strong> <img src="assets/add-icon-plus-in-circle.png">를 클릭하고 사용자 이름을 입력한 다음 표시될 때 선택합니다.</li>
        <li> <p>추가하려는 다른 사용자에 대해 이 작업을 반복합니다.</p> <p>해당 사용자를 추가하지 않기로 결정한 경우 이름 오른쪽에 있는 X를 클릭할 수 있습니다.</p> </li>
        <li>완료되면 <strong>완료</strong>를 클릭하세요.</li>
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹에서 사용자 제거</td> 
      <td> 
       <ol> 
        <li>사용자 이름을 하나 이상 선택한 다음 <strong>구성원 제거</strong><img src="assets/remove-icon---x-in-circle.png">를 클릭합니다.</li> 
        <li> <p>표시되는 경고 메시지에서 <strong>제거</strong>를 클릭합니다.</p> <p><strong>목록에서 사용자 및 그룹 검색</strong>을 클릭하고 상자에 이름을 입력한 다음 표시될 때 이름을 클릭하여 목록에서 제거할 사용자를 찾을 수 있습니다.</p> <p><b>참고</b>:  
          <ul> 
           <li>이 그룹이 제거할 사용자의 홈 그룹인 경우 먼저 사용자 프로필에 다른 홈 그룹을 할당해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">홈 그룹 개요</a> 및 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>을 참조하세요.</li> 
           <li>그룹에 그룹 관리자가 한 명만 있고 그룹에서 제거해야 하는 경우 먼저 그룹에 다른 그룹 관리자를 할당해야 합니다.</li> 
           <li>사용자는 개별적으로 하위 그룹뿐만 아니라 상위 그룹에도 속할 수 있습니다. 하위 그룹에서 제거할 경우 상위 그룹의 일부로 유지됩니다. 마찬가지로 상위 그룹에서 제거하면 하위 그룹의 일부로 유지됩니다. 사용자가 상위 그룹에 대한 액세스 권한을 허용하지 않도록 하려면 하위 그룹과 상위 그룹이 두 위치에 개별적으로 나열되는 경우 모두 해당 사용자를 제거해야 합니다.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 프로필 정보 편집</td> 
      <td> 
       <ol> 
        <li>사용자 이름을 하나 이상 선택한 다음 <strong>편집</strong> <img src="assets/edit-icon.png">을(를) 클릭합니다.</li> 
        <li> <p>사용자의 프로필 정보를 변경합니다.</p> <p>변경 내용에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>을 참조하십시오.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 멤버십 데이터 내보내기</td> 
      <td> 
       <ol> 
        <li>사용자 이름을 하나 이상 선택한 다음 <strong>내보내기</strong> <img src="assets/export.png">를 클릭합니다.</li> 
        <li> <p>데이터를 PDF, Excel 또는 탭으로 구분된 파일로 내보냅니다.</p> <p>데이터 내보내기에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">데이터 내보내기</a>를 참조하십시오.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">구성원의 그룹 역할 보기 및 편집</td> 
      <td> <p><strong>그룹 역할</strong> 열에는 각 구성원의 역할이 나열됩니다. 그룹 관리자는 멤버 역할을 두 번 눌러 변경할 수 있습니다.</p> <p>그룹 관리자가 아닌 그룹 구성원의 경우 이 열을 편집할 수 없습니다.</p> <p>그룹 관리자는 항상 목록의 맨 위에 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 구성원에게 주석 보내기</td> 
      <td> 
       <ol> 
        <li>최소 한 명 이상의 그룹 구성원을 선택한 다음 도구 모음에서 <strong>사용자에게 업데이트 보내기</strong>를 클릭합니다.</li> 
        <li><p>사용자 및 해당 사용자 프로필의 업데이트 영역에 보낼 주석을 입력합니다.</p>
        <p>자세한 내용은 <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">다른 사용자에게 다이렉트 메시지 보내기</a>를 참조하십시오.</p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront에서 사용자 활성화</td> 
      <td>비활성 사용자를 한 명 이상 선택한 다음 <strong>사용자 활성화</strong>를 클릭하여 Workfront에서 활성화합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront에서 사용자 비활성화</td> 
      <td>활성 사용자를 한 명 이상 선택한 다음 <strong>사용자 비활성화</strong><img src="assets/deactivate-user.png">를 클릭하여 Workfront에서 비활성화합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">열별 정렬</td> 
      <td>열의 제목을 클릭하여 해당 열의 내용을 기준으로 목록을 정렬합니다.</td> 
     </tr> 
    </tbody> 
   </table>
