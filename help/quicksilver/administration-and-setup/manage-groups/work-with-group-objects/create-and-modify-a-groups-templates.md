---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 그룹의 프로젝트 템플릿 만들기 및 수정
description: 그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 관련된 프로젝트 템플릿을 보고 작업할 수 있습니다.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 1%

---

# 그룹의 프로젝트 템플릿 만들기 및 수정

그룹 영역에서 관리하는 그룹을 볼 때 그룹 및 해당 하위 그룹과 관련된 프로젝트 템플릿을 보고 작업할 수 있습니다.

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
  <tr> 
   <td>개체 권한</td>
   <td>보고 작업할 템플릿에 대한 액세스 이상 보기</td> 
  </tr>
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 그룹 영역에서 그룹의 템플릿을 보고 작업하고 만듭니다.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **그룹** ![그룹](assets/groups-icon.png)을 클릭합니다.

1. 템플릿을 만들거나 수정할 그룹의 이름을 클릭합니다.
1. 왼쪽 패널에서 **템플릿**&#x200B;을 클릭하여 그룹 및 해당 그룹에 포함될 수 있는 하위 그룹과 연결된 템플릿을 나열합니다.

   이 목록에서 템플릿을 보려면 보기 액세스 권한이 있어야 합니다. 이 액세스에 대한 자세한 내용은 [템플릿에 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)를 참조하십시오.

1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">템플릿 추가</td> 
      <td> <p><strong>새 템플릿</strong>을 클릭한 다음 사용 가능한 옵션을 사용하여 템플릿을 구성합니다. 이러한 옵션에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">프로젝트 템플릿 만들기</a>를 참조하십시오.</p> <p>템플릿은 자동으로 그룹과 연결됩니다.</p> <p>새 템플릿에 그룹 환경 설정을 적용하는 방법에 대한 자세한 내용은 이 문서의 <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">템플릿 및 템플릿 작업에 환경 설정을 적용하는 방법</a>을 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하나 이상의 템플릿 편집</td> 
      <td> <p>템플릿을 하나 이상 선택하고 편집 아이콘 <img src="assets/edit-icon.png">을(를) 클릭한 다음 사용 가능한 옵션을 사용하여 템플릿을 구성합니다. 이러한 옵션에 대한 자세한 내용은 <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">프로젝트 템플릿 편집</a>을 참조하십시오.</p> <p>편집 아이콘은 선택한 모든 템플릿에 대한 편집 액세스 권한이 있는 경우에만 사용할 수 있습니다. 이 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">템플릿에 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하나 이상의 템플릿 삭제</td> 
      <td> <p>템플릿을 하나 이상 선택한 다음 삭제 아이콘 <img src="assets/delete.png">을(를) 클릭합니다.</p> <p>이 아이콘은 선택한 모든 템플릿에 대한 편집 액세스 권한이 있는 경우에만 사용할 수 있습니다. 이 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">템플릿에 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하나 이상의 템플릿 공유</td> 
      <td> <p>템플릿을 하나 이상 선택하고 공유 아이콘 <img src="assets/share-icon.png">을(를) 클릭한 다음 드롭다운 메뉴에서 다음 옵션 중 하나를 클릭합니다.</p> 
       <ul> 
        <li> <p><strong>템플릿</strong>: 표시되는 <strong>템플릿 액세스</strong> 상자에서 이름을 추가하여 템플릿 자체에 액세스할 사용자를 지정합니다.</p> <p>자세한 내용은 문서 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">프로젝트 템플릿 공유</a>에서 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">템플릿 공유</a> 섹션을 참조하십시오.</p> </li> 
        <li><strong>프로젝트</strong>: 표시되는 <strong>프로젝트 액세스</strong> 상자에서 이름을 추가하여 템플릿에서 만든 프로젝트에 액세스할 사용자를 지정합니다</li> 
       </ul> <p>공유 아이콘은 선택한 모든 템플릿에 대한 공유 액세스 권한이 있는 경우에만 사용할 수 있습니다. 이 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">템플릿에 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">템플릿 목록 내보내기</td> 
      <td><strong>내보내기</strong> <img src="assets/export.png">를 클릭한 다음 내보낸 목록에 사용할 파일 형식을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

## 템플릿 및 템플릿 작업에 환경 설정을 적용하는 방법 {#how-preferences-apply-to-templates-and-template-tasks}

프로젝트 템플릿을 만들면 아래 표에 나열된 설정이 상호 연관된 프로젝트 또는 작업 기본 설정에 의해 자동으로 구성됩니다.

>[!NOTE]
>
>템플릿을 만들 때 그룹과 연결했는지 여부에 따라 그룹 수준 또는 시스템 수준 프로젝트 또는 작업 환경 설정이 프로젝트 템플릿에 영향을 줍니다.
>
>그룹과 연결한 경우 그룹 수준 기본 설정이 적용됩니다. 이 문제는 다음 시나리오에서 발생합니다.
>
>* 이 문서에 설명된 대로 그룹 영역에서 템플릿을 만듭니다
>* 킥스타트 파일을 사용하여 템플릿을 생성할 때 그룹을 지정합니다
>* API를 사용하여 템플릿을 만들 때 그룹을 지정합니다
>
>새 템플릿을 그룹과 연결하지 않은 경우 시스템 수준 기본 설정이 적용됩니다. 이 문제는 아래 시나리오에서 발생합니다. 나중에 템플릿 또는 템플릿 작업에 그룹을 할당해도 그룹의 환경 설정이 영향을 주지 않습니다.
>
>* 템플릿 영역에서 템플릿을 만듭니다
>* 킥스타트 파일을 사용하여 템플릿을 만들 때는 그룹을 지정하지 않습니다
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
   <td> <p>새 템플릿을 그룹에 연결하는 경우 그룹 수준 프로젝트 환경 설정 "성과 지표 메서드"로 구성되고, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 환경 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>상태 유형</p> </td> 
   <td> <p>새 템플릿을 그룹에 연결하는 경우 그룹 수준 프로젝트 환경 설정 "진행 상태에 따라 프로젝트 상태 자동 설정"으로 구성되고, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 환경 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>일정 출처:</p> </td> 
   <td> <p>새 템플릿을 그룹에 연결하는 경우 그룹 수준 프로젝트 환경 설정 "일정 시작"으로 구성되고, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 환경 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>사용자 휴무</p> </td> 
   <td> <p>새 템플릿을 그룹에 연결하는 경우 그룹 수준 프로젝트 환경 설정 "사용자 휴무"로 구성되고, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 환경 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>업데이트 유형</p> </td> 
   <td> <p>새 템플릿을 그룹에 연결하는 경우 그룹 수준 프로젝트 환경 설정 "프로젝트 타임라인이 자동으로 다시 계산됩니다"로 구성되고, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 환경 설정이 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>액세스 섹션 설정</p> </td> 
   <td> <p>새 템플릿을 그룹에 연결하는 경우 "액세스" 섹션의 그룹 수준 작업 환경 설정에 의해 구성되며, 그렇지 않은 경우 동일한 시스템 수준 프로젝트 환경 설정에 의해 구성됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표에 나열된 프로젝트 환경 설정에 대한 자세한 내용은 [시스템 차원의 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

작업 및 문제 환경 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.

>[!NOTE]
>
>* 기존 프로젝트 템플릿에 연결된 그룹을 변경하면 템플릿의 설정이 동일하게 유지됩니다.
>* 기존 템플릿 작업을 다른 템플릿으로 이동하면 새 템플릿과 연관된 그룹에 관계없이 다음 설정이 템플릿 작업에서 변경되지 않습니다.>
>   * 기간 유형
>   * 수익 유형
>   * 비용 유형
>
>  그러나 템플릿 작업은 새 템플릿에 대한 &quot;누군가가 작업에 할당되었을 때&quot; 설정의 영향을 받습니다. 자세한 내용은 문서 [프로젝트 템플릿 편집](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access)의 [액세스](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) 섹션을 참조하십시오.
>
>* 관리자가 프로젝트를 템플릿으로 저장하면 그룹을 포함하여 템플릿에 대한 모든 설정이 프로젝트에서 상속됩니다.
>
>  관리자가 템플릿을 사용하여 작업 또는 문제를 프로젝트로 전환할 때 템플릿에 이미 저장된 내용에 따라 템플릿에 대한 모든 설정이 결정됩니다.
>

### 작업 환경 설정에 의해 구성된 템플릿 작업 설정 {#template-task-settings-configured-by-task-preferences}

템플릿 작업을 만들 때 일부 설정은 상호 연관된 작업 기본 설정에 의해 자동으로 구성됩니다. 이러한 설정은 아래 표에 나열되어 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>기간 유형 </p> </td> 
   <td> <p>템플릿을 그룹에 연결하는 경우 그룹 수준 작업 환경 설정 "기간 유형"으로 구성되고, 그렇지 않은 경우 동일한 시스템 수준 작업 및 문제 환경 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>수익 유형</p> </td> 
   <td> <p>템플릿을 그룹과 연결하는 경우 그룹 수준 작업 환경 설정 "매출 유형"으로, 그렇지 않은 경우 동일한 시스템 수준 작업 및 문제 환경 설정으로 구성됩니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>비용 유형 </p> </td> 
   <td> <p> 템플릿을 그룹에 연결하는 경우 그룹 수준 작업 환경 설정 "비용 유형"으로 구성되고, 그렇지 않은 경우 동일한 시스템 수준 작업 및 문제 환경 설정으로 구성됩니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표에 나열된 작업 환경 설정에 대한 자세한 내용은 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)을 참조하십시오.
