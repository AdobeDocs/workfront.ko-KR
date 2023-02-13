---
user-type: administrator
product-area: system-administration;user-management
keywords: add,users,group,add,another,assign,administrator,remove,user,view,roles,members,export,membership,data
navigation-topic: create-and-manage-groups
title: 그룹 멤버십 보기 및 관리
description: Adobe Workfront 관리자는 관리하는 그룹의 구성원을 보고, 추가, 제거, 내보내기, 활성화 및 비활성화할 수 있습니다. 프로필을 편집하고 프로필에 업데이트를 추가하고 그룹의 추가 그룹 관리자로 지정할 수도 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# 그룹 멤버십 보기 및 관리

Adobe Workfront 관리자는 관리하는 그룹의 구성원을 보고, 추가, 제거, 내보내기, 활성화 및 비활성화할 수 있습니다. 프로필을 편집하고 프로필에 업데이트를 추가하고 그룹의 추가 그룹 관리자로 지정할 수도 있습니다.

그룹 위에 그룹이 있으면 해당 관리자가 사용자 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹의 경우)도 마찬가지입니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹 멤버십 보기 및 관리

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹**.

   표시되는 목록에서 Workfront 관리자는 모든 그룹 및 하위 그룹을 볼 수 있습니다. 그룹 관리자는 관리하는 그룹 및 하위 그룹만 볼 수 있습니다.

1. 편집할 그룹의 이름을 클릭합니다.
1. 나타나는 페이지에서 **그룹 구성원** 왼쪽 메뉴에서 선택한 경우 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">사용자를 그룹에 추가</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">클릭 <strong>구성원 추가</strong> <img src="assets/add-icon-plus-in-circle.png">을(를) 입력하여 사용자 이름을 입력한 다음 표시되는 경우 선택합니다.</li> 
        <li value="2"> <p>추가하려는 다른 사용자에 대해 이 과정을 반복합니다.</p> <p>해당 사용자를 추가하지 않기로 결정한 경우 이름 오른쪽에 있는 X를 클릭할 수 있습니다.</p> </li> 
        <li value="3">클릭 <strong>완료</strong> 끝나면</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹에서 사용자 제거</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">사용자 이름을 하나 이상 선택한 다음 <strong>멤버 제거</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>클릭 <strong>제거</strong> 경고 메시지에 이 표시됩니다.</p> <p>을 클릭하여 목록에서 제거할 사용자를 찾을 수 있습니다 <strong>목록에서 사람 및 그룹 검색</strong>상자에 해당 이름을 입력한 다음 표시되는 이름을 클릭합니다.</p> <p><b>메모</b>:  
          <ul> 
           <li>이 그룹이 제거하려는 사용자의 홈 그룹인 경우 먼저 사용자 프로필에서 다른 홈 그룹을 할당해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">홈 그룹 개요</a> 및 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</li> 
           <li>그룹에 한 명의 그룹 관리자만 있고 그룹에서 해당 관리자를 제거해야 하는 경우 먼저 다른 그룹 관리자를 그룹에 할당해야 합니다.</li> 
           <li>사용자는 하위 그룹뿐만 아니라 상위 그룹에도 개별적으로 속할 수 있습니다. 하위 그룹에서 사용자를 제거하면 해당 그룹은 상위 그룹의 일부로 남습니다. 마찬가지로 상위 그룹에서 해당 그룹을 제거하면 해당 하위 그룹의 일부로 남습니다. 사용자가 상위 그룹에 대한 액세스 권한을 허용하지 않도록 하려면 두 위치에 개별적으로 나열되는 경우 하위 그룹뿐만 아니라 상위 그룹에서도 사용자를 모두 제거해야 합니다.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자의 프로필 정보 편집</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">사용자 이름을 하나 이상 선택한 다음 <strong>편집</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>사용자의 프로필 정보를 변경합니다.</p> <p>수행할 수 있는 변경 사항에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 멤버십 데이터 내보내기</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">사용자 이름을 하나 이상 선택한 다음 <strong>내보내기</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>데이터를 PDF, Excel 또는 탭으로 구분된 파일로 내보냅니다.</p> <p>데이터 내보내기에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">데이터 내보내기</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">구성원의 그룹 역할 보기 및 편집</td> 
      <td> <p>다음 <strong>그룹 역할</strong> 열에는 각 멤버의 역할이 나열됩니다. 그룹 관리자는 구성원의 역할을 두 번 눌러 변경할 수 있습니다.</p> <p>그룹 관리자가 아닌 그룹 구성원의 경우 이 열을 편집할 수 없습니다.</p> <p>그룹 관리자는 항상 목록의 맨 위에 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">그룹 구성원에게 주석 보내기</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">사용자 이름을 하나 이상 선택한 다음 <strong>업데이트</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">설명을 입력합니다.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront에서 사용자 활성화</td> 
      <td>비활성 사용자를 한 명 이상 선택한 다음 <strong>사용자 활성화</strong> Workfront에서 활성화하면 됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront에서 사용자 비활성화</td> 
      <td>활성 사용자를 한 명 이상 선택한 다음 <strong>사용자 비활성화</strong><img src="assets/deactivate-user.png"> Workfront에서 비활성화하는 중입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">열별 정렬</td> 
      <td>열 제목을 클릭하여 해당 열의 내용을 기준으로 목록을 정렬합니다.</td> 
     </tr> 
    </tbody> 
   </table>
