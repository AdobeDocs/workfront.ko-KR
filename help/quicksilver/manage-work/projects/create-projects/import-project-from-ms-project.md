---
product-area: projects
navigation-topic: create-projects
title: Microsoft 프로젝트에서 프로젝트 가져오기
description: Microsoft Project에서 Adobe Workfront으로 프로젝트를 가져오고 모든 프로젝트를 하나의 애플리케이션에서 관리할 수 있습니다. Microsoft 프로젝트에서 프로젝트를 가져올 때마다 Workfront에 새 프로젝트가 만들어집니다.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 2%

---

# Microsoft 프로젝트에서 프로젝트 가져오기

Microsoft Project에서 Adobe Workfront으로 프로젝트를 가져오고 모든 프로젝트를 하나의 애플리케이션에서 관리할 수 있습니다. Microsoft 프로젝트에서 프로젝트를 가져올 때마다 Workfront에 새 프로젝트가 만들어집니다.

>[!IMPORTANT]
>
>일부 Microsoft 프로젝트 필드가 Workfront으로 전송되지 않습니다.
>
>Workfront과 Microsoft 프로젝트 간의 필드 호환성에 대한 자세한 내용은 [Microsoft 프로젝트 필드를 Adobe Workfront 프로젝트에 매핑](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## 액세스 요구 사항

P&amp;P에 대한 초안:

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
   <td> <p>현재 라이선스: 표준 </p> 
   또는
   <p>기존 라이센스: 계획 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트를 만들 때 프로젝트에 대한 관리 권한을 자동으로 받습니다 </p> <p> 프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 프로젝트 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">프로젝트에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트를 만들 때 프로젝트에 대한 관리 권한을 자동으로 받습니다 </p> <p> 프로젝트 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront에서 프로젝트 공유</a>.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## MS 프로젝트에서 프로젝트 만들기

프로젝트 영역(주 메뉴)이나 포트폴리오 또는 프로그램의 프로젝트 영역에서 프로젝트를 생성할 수 있습니다.

1. Microsoft 프로젝트로 이동하고 Workfront에서 가져올 프로젝트를 엽니다.
1. 클릭 **파일**, 그런 다음 **다른 이름으로 저장** 프로젝트를 .xml 파일로 저장하려면 다음을 수행합니다.

1. Workfront에 로그인합니다.
1. 다음 중 하나를 수행하십시오.

   * 을(를) 클릭합니다. **기본 메뉴** ![](assets/main-menu-icon.png)를 클릭합니다. **프로젝트**&#x200B;를 확장한 다음 **새 프로젝트**.
   * 포트폴리오로 이동한 다음 확장합니다. **새 프로젝트**.
   * 프로그램으로 이동한 다음 **새 프로젝트**.
   * 그룹 관리자인 경우 관리하는 그룹의 프로젝트 섹션에서 프로젝트를 만들 수도 있습니다. 자세한 내용은 [그룹의 프로젝트 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. 을(를) 선택합니다 **MS 프로젝트 가져오기** 선택 사항입니다.

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 클릭 **파일 선택**&#x200B;그런 다음 Microsoft Project에서 내보낸 컴퓨터의 .xml 파일을 찾습니다.
1. 선택한 파일을 가져옵니다.

   Workfront은 가져오기 프로세스를 시작하고 Microsoft 프로젝트에서 내보낸 파일을 기반으로 새 프로젝트를 만듭니다.

   가져오기 프로세스가 완료되면 가져오기가 성공적으로 완료되었음을 확인하는 새 프로젝트 페이지로 이동합니다.

   >[!NOTE]
   >
   >Workfront은 파일 업로드에 대한 15분 시간 제한을 갖습니다. 파일 업로드가 이보다 오래 걸리는 경우에는 프로젝트를 더 작은 프로젝트로 분류하고 별도로 가져오는 것이 좋습니다. Workfront으로 가져온 후에는 작업을 한 프로젝트에서 다른 프로젝트로 이동하여 하나의 프로젝트로 결합합니다. 작업 이동에 대한 자세한 내용은 [작업 이동](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (선택 사항) Workfront에서 프로젝트를 계속 편집합니다. 프로젝트 편집에 대한 자세한 내용은 [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md).

   템플릿에서 새 프로젝트의 상태는 프로젝트 환경 설정 영역에서 Workfront 관리자가 정의한 상태나 그룹 프로젝트 환경 설정 영역의 그룹 관리자가 정의한 상태와 같습니다. 프로젝트 환경 설정 구성에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
