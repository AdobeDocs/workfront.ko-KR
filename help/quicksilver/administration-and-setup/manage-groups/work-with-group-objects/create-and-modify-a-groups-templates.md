---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 프로젝트 템플릿 만들기 및 수정
description: 그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 연관된 프로젝트 템플릿을 보고 작업할 수 있습니다.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# 그룹의 프로젝트 템플릿 만들기 및 수정

그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 연관된 프로젝트 템플릿을 보고 작업할 수 있습니다.

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
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고 작업할 템플릿에 대한 액세스 권한 이상을 봅니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 찾아야 하는 경우 Workfront 관리자에게 문의하십시오.

## 그룹 영역에서 그룹 템플릿을 보고, 작업하고, 생성할 수 있습니다

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **그룹** ![](assets/groups-icon.png).

1. 템플릿을 만들거나 수정할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **템플릿** 그룹과 연관된 템플릿 및 하위 그룹 목록을 만들려면 다음과 같이 하십시오.

   이 목록에서 템플릿을 보려면 템플릿에 대한 보기 액세스 권한이 있어야 합니다. 이 액세스에 대한 자세한 내용은 [템플릿에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">템플릿 추가</td> 
      <td> <p>클릭 <strong>새 템플릿</strong>를 만든 다음 사용 가능한 옵션을 사용하여 구성합니다. 이러한 옵션에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">프로젝트 템플릿 만들기</a>.</p> <p>템플릿은 그룹과 자동으로 연결됩니다.</p> <p>그룹 환경 설정이 새 템플릿에 적용되는 방법에 대한 자세한 내용은 <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">템플릿 및 템플릿 작업에 환경 설정이 적용되는 방식</a> 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 하나 이상 편집</td> 
      <td> <p>하나 이상의 템플릿을 선택하고 편집 아이콘을 클릭합니다 <img src="assets/edit-icon.png">를 입력한 다음 사용 가능한 옵션을 사용하여 구성합니다. 이러한 옵션에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">프로젝트 템플릿 편집</a>.</p> <p>편집 아이콘은 선택한 모든 템플릿에 대한 편집 액세스 권한이 있는 경우에만 사용할 수 있습니다. 이 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">템플릿에 대한 액세스 권한 부여</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 하나 이상 삭제</td> 
      <td> <p>템플릿을 하나 이상 선택한 다음 삭제 아이콘을 클릭합니다 <img src="assets/delete.png">.</p> <p>이 아이콘은 선택한 모든 템플릿에 대한 편집 액세스 권한이 있는 경우에만 사용할 수 있습니다. 이 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">템플릿에 대한 액세스 권한 부여</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하나 이상의 템플릿 공유</td> 
      <td> <p>하나 이상의 템플릿을 선택하고 공유 아이콘을 클릭합니다 <img src="assets/share-icon.png">를 클릭한 다음 드롭다운 메뉴에서 다음 옵션 중 하나를 클릭합니다.</p> 
       <ul> 
        <li> <p><strong>템플릿</strong>: 에서 <strong>템플릿 액세스</strong> 표시되는 상자에 이름을 추가하여 템플릿 자체에 액세스할 사용자를 지정합니다.</p> <p>자세한 내용은 섹션을 참조하십시오 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">템플릿 공유</a> 기사 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">프로젝트 템플릿 공유</a>.</p> </li> 
        <li><strong>프로젝트</strong>: 에서 <strong>프로젝트 액세스</strong> 표시되는 상자에 이름을 추가하여 템플릿에서 만든 프로젝트에 액세스할 사용자를 지정합니다</li> 
       </ul> <p>공유 아이콘은 선택한 모든 템플릿에 대한 공유 액세스 권한이 있는 경우에만 사용할 수 있습니다. 이 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">템플릿에 대한 액세스 권한 부여</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 목록 내보내기</td> 
      <td>클릭 <strong>내보내기</strong> <img src="assets/export.png">를 선택한 다음 내보낸 목록에 사용할 파일 형식을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

## 템플릿 및 템플릿 작업에 환경 설정이 적용되는 방식 {#how-preferences-apply-to-templates-and-template-tasks}

프로젝트 템플릿을 만들면 아래 표에 나열된 설정이 관련 프로젝트 또는 작업 기본 설정에 의해 자동으로 구성됩니다.

>[!NOTE]
>
>그룹 수준이나 시스템 수준 프로젝트 또는 작업 환경 설정은 템플릿을 만들 때 해당 템플릿을 그룹과 연결했는지 여부에 따라 프로젝트 템플릿에 영향을 줍니다.
>
>그룹과 연결한 경우 그룹 수준 기본 설정이 적용됩니다. 이 문제는 다음 시나리오에서 발생합니다.
>
>* 이 문서에 설명된 대로 그룹 영역에서 템플릿을 만듭니다
>* 킥스타트 파일을 사용하여 템플릿을 만들 때 그룹을 지정합니다
>* API를 사용하여 템플릿을 만들 때 그룹을 지정합니다
>
>새 템플릿을 그룹과 연결하지 않은 경우 시스템 수준 기본 설정이 적용됩니다. 이 문제는 아래 시나리오에서 발생할 때 발생합니다. (나중에 템플릿 또는 템플릿 작업에 그룹을 할당해도 그룹의 기본 설정은 영향을 주지 않습니다.)
>
>* 템플릿 영역에서 템플릿을 생성합니다
>* Kickstart 파일을 사용하여 템플릿을 만들 때 그룹을 지정하지 않습니다
>* API를 사용하여 템플릿을 만들 때 그룹을 지정하지 않습니다
>


* [프로젝트 및 작업 환경 설정에 의해 구성된 프로젝트 템플릿 설정](#project-template-settings-configured-by-project-and-task-preferences)
* [작업 환경 설정에 의해 구성된 템플릿 작업 설정](#template-task-settings-configured-by-task-preferences)

### 프로젝트 및 작업 환경 설정에 의해 구성된 프로젝트 템플릿 설정 {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>성과 지수 방법</p> </td> 
   <td> <p>새 템플릿을 그룹과 연결하는 경우 그룹 수준 프로젝트 기본 설정 "성과 인덱스 방법"으로 구성하거나, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 기본 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>상태 유형</p> </td> 
   <td> <p>새 템플릿을 그룹과 연결하는 경우 "진행 상태에 따라 프로젝트의 조건을 자동으로 설정"으로 그룹 수준 프로젝트 기본 설정에 의해 구성되거나, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 기본 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>예약 위치</p> </td> 
   <td> <p>새 템플릿을 그룹과 연결하는 경우 그룹 수준 프로젝트 기본 설정 "스케줄 시작"으로 구성하거나, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 기본 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>사용자 시간 초과</p> </td> 
   <td> <p>새 템플릿을 그룹과 연결하는 경우 그룹 수준 프로젝트 기본 설정 "사용자 시간 해제"로 구성하거나 그렇지 않은 경우 동일한 시스템 수준 프로젝트 기본 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>업데이트 유형</p> </td> 
   <td> <p>새 템플릿을 그룹과 연결하면 "프로젝트 타임라인이 자동으로 다시 계산됩니다"라는 그룹 수준 프로젝트 기본 설정에 의해 구성되거나, 그렇지 않으면 동일한 시스템 수준 프로젝트 기본 설정이 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>섹션 설정 액세스</p> </td> 
   <td> <p>새 템플릿을 그룹과 연결하는 경우 "액세스" 섹션에서 그룹 수준 작업 기본 설정에 의해 구성되며 그렇지 않은 경우 동일한 시스템 수준 프로젝트 기본 설정이 구성됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표에 나열된 프로젝트 환경 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

작업 및 문제 기본 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* 기존 프로젝트 템플릿과 연결된 그룹을 변경하면 템플릿의 설정이 동일하게 유지됩니다.
>* 기존 템플릿 작업을 다른 템플릿으로 이동하는 경우 새 템플릿과 연관된 그룹에 관계없이 템플릿 작업에서 다음 설정이 변경되지 않습니다.>
   >   * 기간 유형
   >   * 수익 유형
   >   * 비용 유형
>
>  하지만 템플릿 작업은 새 템플릿의 &quot;When someone is assigned to a task&quot; 설정에 영향을 받습니다. 자세한 내용은 섹션을 참조하십시오 [액세스](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) 기사 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* 관리자가 프로젝트를 템플릿으로 저장하면 그룹을 포함하여 템플릿에 대한 모든 설정이 프로젝트에서 상속됩니다.
>
>  관리자가 템플릿을 사용하여 작업이나 문제를 프로젝트로 변환하면 템플릿에 대한 모든 설정은 템플릿에 이미 저장된 내용에 의해 결정됩니다.

### 작업 환경 설정에 의해 구성된 템플릿 작업 설정 {#template-task-settings-configured-by-task-preferences}

템플릿 작업을 만들면 해당 설정 중 일부는 관련 작업 기본 설정에 의해 자동으로 구성됩니다. 이러한 설정은 아래 표에 나와 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>기간 유형 </p> </td> 
   <td> <p>그룹을 사용하여 템플릿을 연결하는 경우 그룹 레벨 태스크 기본 설정 "기간 유형"으로 구성되거나, 그렇지 않은 경우 동일한 시스템 레벨 태스크 및 문제 기본 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>수익 유형</p> </td> 
   <td> <p>템플리트를 그룹과 연관시키는 경우 그룹 레벨 태스크 환경설정 "수익 유형"에 의해 구성되거나, 그렇지 않은 경우 동일한 시스템 레벨 태스크 및 출고 기본 설정이 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>비용 유형 </p> </td> 
   <td> <p> 템플리트를 그룹과 연관시키는 경우 그룹 레벨 태스크 환경설정 "원가 유형"에 의해 구성되거나, 그렇지 않은 경우 동일한 시스템 레벨 태스크 및 출고 환경설정.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 테이블에 나열된 작업 환경 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
