---
user-type: administrator
product-area: system-administration;user-management
keywords: 그룹,프로젝트
navigation-topic: work-with-a-groups-objects
title: 그룹의 프로젝트 만들기 및 수정
description: 그룹 영역에서 관리하는 그룹을 볼 때 그룹의 프로젝트를 작성, 편집, 내보내기, 복사 및 삭제할 수 있습니다.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: db90cf52-7c8f-4972-b67f-401657ba9b13
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 그룹의 프로젝트 만들기 및 수정

그룹 영역에서 관리하는 그룹을 볼 때 다음과 같은 방법으로 해당 프로젝트를 보고 작업할 수 있습니다.

* 그룹에 대한 새 프로젝트 만들기
* 프로젝트 편집, 내보내기, 복사 또는 삭제

그룹 위에 그룹이 있는 경우 해당 관리자는 그룹을 위해 이러한 작업을 수행할 수도 있습니다. Workfront 관리자(모든 그룹)의 경우도 마찬가지입니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td >Workfront 플랜</a>*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</a>*</td> 
   <td> <p>플랜 </p> <p>그룹의 그룹 관리자 또는 Workfront 관리자여야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">그룹 관리자</a> 및 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> 
    <ul> 
     <li> <p>프로젝트는 그룹 또는 해당 하위 그룹과 연결되어 있어야 합니다. </p> <p>프로젝트에 그룹을 할당하는 방법에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">프로젝트 개요 영역의 정보 관리</a>를 참조하십시오.</p> </li> 
     <li> <p>또한 프로젝트를 만들었거나 사용자와 공유되었기 때문에 프로젝트를 편집할 권한이 있어야 합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </li> 
    </ul> <p><b>참고</b>: 그룹의 페이지에서 프로젝트를 만들 때 시스템이 해당 그룹에 프로젝트를 할당합니다. 이는 시스템이 프로젝트를 만드는 사용자(프로젝트 소유자)의 홈 그룹에 프로젝트를 할당하는 다른 Workfront 영역에서 프로젝트를 만드는 것과는 다릅니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인해야 하는 경우 Workfront 관리자에게 문의하십시오.

+++

## 그룹 영역에서 그룹에 대한 프로젝트를 보고 작업하고 만듭니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

1. 프로젝트를 만들거나, 보거나, 작업할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **프로젝트** ![주 메뉴의 프로젝트](assets/projects-in-main-menu.png)를 클릭하여 그룹과 연결된 프로젝트 목록을 봅니다.

1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>프로젝트를 사용하여 작업</p> </td> 
      <td> <p>프로젝트를 선택한 다음 도구 모음 단추를 사용하여 <img src="assets/edit-icon.png">을(를) 편집하거나 <img src="assets/share-icon.png">을(를) 공유하거나 <img src="assets/delete.png">을(를) 삭제하십시오.</p> <p>이러한 활동에 대한 자세한 내용은 <a href="../../../manage-work/projects/manage-projects/manage-projects-overview.md" class="MCXref xref">프로젝트 관리: 문서 색인</a>을 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>그룹에 대한 새 프로젝트 만들기</p> </td> 
      <td> 
       <ol> 
        <li value="1"> <p><strong>새 프로젝트</strong>를 클릭한 다음 드롭다운 메뉴에서 옵션을 선택하여 만들 방법을 나타냅니다. </p> <p>자세한 내용은 문서 <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">프로젝트 만들기</a>에서 <a href="../../../manage-work/projects/create-projects/create-project.md#ways-to-create-projects" class="MCXref xref">프로젝트를 만드는 방법</a> 섹션을 참조하십시오.</p> </li> 
        <li value="2"><a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">프로젝트 편집</a>에 설명된 대로 프로젝트 이름을 입력하고 구성합니다.</li> 
       </ol> <p> 그룹에 대해 설정된 프로젝트 환경 설정은 그룹 영역에서 만드는 모든 프로젝트에 영향을 줍니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md" class="MCXref xref">그룹에 대한 프로젝트 환경 설정 구성</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">프로젝트 목록 내보내기</td> 
      <td>목록 위의 도구 모음에서 내보내기 아이콘 <img src="assets/export.png">을(를) 클릭합니다.</td> 
     </tr> 
    </tbody> 
   </table>
