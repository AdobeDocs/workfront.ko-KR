---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 회사 만들기 및 편집
description: 에 회사를 추가할 수 있습니다. [!DNL Adobe Workfront] 재무 계획, 보고 목적, 객체에 대한 권한 정의, 정보의 기밀 유지 등에 사용할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1472'
ht-degree: 0%

---

# 회사 만들기 및 편집

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

회사는 의 조직 단위입니다. [!DNL Adobe Workfront] 조직, 조직 내 부서 또는 함께 일하는 클라이언트를 나타낼 수 있습니다. 에 회사를 추가할 수 있습니다. [!DNL Workfront] 재무 계획, 보고 목적, 객체에 대한 권한 정의, 정보의 기밀 유지 등에 사용할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

에서 회사를 관리하려면 다음 항목이 있어야 합니다. [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 라이센스*</p> </td> 
   <td><p>현재: [!UICONTROL Plan]</p>
   또는
   <p>새로운 기능: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음 중 하나:</p> 
    <ul> 
     <li> <p>시스템에서 회사를 편집할 수 있는 [!UICONTROL 시스템 관리자] 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">사용자에게 전체 관리 액세스 권한 부여</a>. </p> </li> 
     <li> <p>회사 관리에 대한 관리 액세스 권한으로, 시스템에서 모든 회사를 편집할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> </li> 
    </ul> <p><b>참고</b>:  
     <ul> 
      <li> <p>그룹 관리자로 할당된 모든 그룹과 연결된 회사를 관리할 수도 있습니다.</p> </li> 
      <li> <p>에 사용자를 추가하고 에서 사용자를 제거하려면 [!DNL Workfront] 시스템에 다음 중 하나가 있어야 합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>. </p> </li> 
        <li> <p>액세스 수준에서 [!UICONTROL 사용자] 설정에 대해 [!UICONTROL 편집]을 선택해야 합니다. 또한 [!UICONTROL Users] 설정의 경우 [!UICONTROL 설정을 미세 조정하십시오] <img src="assets/gear-icon-in-access-levels.png">, [!UICONTROL 만들기] 옵션과 두 [!UICONTROL 사용자 관리] 옵션 중 하나 이상을 활성화해야 합니다. </p> <p> <img src="assets/access-req-users.png"> </p> <p>[!UICONTROL 사용자 관리자(그룹 사용자)] 옵션을 사용하는 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> </li> 
       </ul> <p>액세스 수준의 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 [!DNL Workfront] 관리자. 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 회사에 사용자를 추가하면 얻을 수 있는 이점 {#benefits-of-adding-users-to-a-company}

* 사용자를 부하 직원과 연결하여 회사의 조직도를 작성할 수 있습니다. 동일한 회사의 사용자만 해당 회사의 다른 사용자에 대한 직접 보고서로 추가할 수 있습니다.
* 프로젝트 관리자는 동일한 회사 내에서 사용 가능한 리소스를 식별할 수 있습니다.
* 다음 설정 중 하나 또는 모두를 선택하여 회사 간에 정보를 비공개로 유지할 수 있습니다.

   * 동일한 회사의 사용자가 서로의 요청을 볼 수 있습니다.

     자세한 내용은 [!DNL Workfront] 관리자는 사용자의 회사를 기반으로 요청에 대해 유사한 액세스 권한을 부여할 수 있습니다. 섹션을 참조하십시오. [의 모든 사용자를 위한 작업 및 문제 환경 설정 구성 [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) 이 문서에서 [시스템 전체 작업 및 문제 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     그룹 관리자가 사용자 회사를 기반으로 요청에 유사한 액세스 권한을 부여할 수 있는 방법에 대한 자세한 내용은 을 참조하십시오. [그룹에 대한 작업 및 문제 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * 사용자는 회사와 연결된 요청 대기열만 볼 수 있습니다. 요청 대기열의 가시성 제한에 대한 자세한 내용은 [요청 대기열에 대한 액세스 권한 제공](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * 사용자가 회사 또는 회사 및 기본 회사의 사용자만 보도록 제한할 수 있습니다. 사용자 개인 정보와 관련된 기본 회사 기능에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * 사용자는 회사 사용자만 항목에 대한 업데이트를 볼 수 있도록 제한할 수 있습니다. 회사에 대한 업데이트를 비공개로 만드는 방법에 대한 자세한 내용은 [작업 업데이트](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 에서 회사 만들기 또는 편집 [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

추가할 수 있는 회사 수에는 제한이 없습니다. 그러나 너무 많은 단편화가 작업 항목에 대한 사용자의 가시성을 방해할 수 있으므로 오브젝트 권한과 관련하여 발생할 수 있는 문제로 인해 사용하는 회사 수를 제한하는 것이 좋습니다.

기본적으로 의 인스턴스와 연결된 회사입니다 [!DNL Workfront] 이(가) 이미 다음 위치에 생성되었습니다. [!DNL Workfront] system 및 는 조직의 기본 회사입니다. 고객명과 같은 이름을 가지고 있습니다. 고객 정보에 대한 자세한 내용은에서 확인하십시오. [!DNL Workfront], 참조 [시스템에 대한 기본 정보 구성](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

회사를 추가하거나 편집하려면:

{#step-1-to-setup}

1. 클릭 **[!UICONTROL 회사]**.

   회사 목록이 표시됩니다.
1. 회사를 추가하는 경우 **[!UICONTROL 새 회사]**.

   또는

   기존 회사를 편집하는 경우 회사를 선택한 다음 을 클릭합니다. **[!UICONTROL 편집]** 회사 목록의 맨 위에.

1. 다음 정보를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 기본 정보] 섹션</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: 회사 이름을 입력합니다.</p> </li> 
        <li> <p><b>[!UICONTROL이 활성화됨]</b>: 이 옵션이 활성화되면 사용자는 회사를 찾아 자신이 만들고 편집하는 프로젝트에 첨부할 수 있습니다. 비활성 회사는 프로젝트에 연결할 수 없습니다. 이 옵션은 기본적으로 활성화되어 있습니다.</p> </li> 
        <li> <p><b>[!UICONTROL 기본 회사입니다]</b>: 회사를 조직의 기본 회사로 지정합니다. 기본 회사는 일반적으로 [!DNL Workfront] 대부분의 사용자가 작업하는 계정입니다.</p> <p>1차 회사로 지정된 회사가 한 개 있거나 한 개도 없을 수 있지만, 여러 개의 회사를 1차 회사로 지정할 수는 없습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> <p><b>참고</b>: 액세스 수준을 수정하여 사용자를 다른 사용자(기본 회사 또는 연결된 회사 및 기본 회사에서만)로 표시하도록 제한할 수 있습니다. 기본 회사가 사용자의 액세스 수준으로 작동하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: 회사와 거래하는 그룹이 있는 경우 여기에 그룹의 이름을 추가할 수 있습니다. 이 기능은 그룹이 거래하는 모든 회사에 대해 보고하고 관리해야 하는 그룹 관리자에게 유용합니다.</p> <p><b>중요 사항</b>: 이 회사에서 작업할 그룹을 연결하지 않은 경우, 그룹 관리자는 액세스 수준의 회사에 대한 관리 액세스 권한이 없으면 회사에 액세스할 수 없습니다. 이 액세스 권한 부여 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">사용자에게 특정 영역에 대한 관리 액세스 권한 부여</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">그룹 이름을 입력한 다음 키를 누릅니다 <strong>[!UICONTROL Enter]</strong> 표시되는 시간.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">회사에 그룹을 할당하면 해당 그룹의 그룹 관리자는 회사에 대한 [!UICONTROL 관리] 액세스 권한을 갖게 됩니다. 자세한 내용은 <a href="#group-administrators-and-companies" class="MCXref xref">그룹 관리자 및 회사</a> 이 문서에서.</p> </li> 
        <li> <p><b>[!UICONTROL 회사 구성원]</b>: 회사에 기존 사용자를 추가합니다. 이렇게 하면 이러한 사용자를 이 회사와 연결하게 됩니다.</p> <p>한 회사에 연결하는 사용자 수에는 제한이 없지만 사용자는 두 개 이상의 회사에 연결할 수 없습니다.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL 사용자 지정 Forms] 섹션</td> 
      <td> <p>회사에 추가하려는 필드에서 을(를) 사용할 수 없는 경우 [!DNL Workfront], 사용자 정의 양식을 작성하여 회사와 연결할 수 있습니다. </p> <p>드롭다운 메뉴에서 이 양식을 선택하여 회사에 첨부할 수 있습니다. 활성 사용자 정의 양식만 메뉴에 나열됩니다.</p> <p><strong>참고:</strong> 외부 조회 필드 및 Workfront 기본 필드와 같은 고급 사용자 정의 양식 기능은 회사 편집 대화 상자가 아닌 세부 정보 페이지에서 회사 레코드를 열 때만 사용할 수 있습니다. 회사 목록에서 회사 이름을 클릭하여 세부 정보를 엽니다.</p> <p> 사용자 정의 양식 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">사용자 정의 양식 만들기 또는 편집</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (조건부) 회사를 만드는 경우 **[!UICONTROL 회사 만들기]**.

   또는

   기존 회사를 편집하는 경우 **[!UICONTROL 변경 내용 저장]**.

## 회사 멤버십 관리

기존 회사의 멤버십 관리에 대한 자세한 내용은 [회사 멤버십 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 청구 요금 관리

회사 수준에서 청구 요율 재정의에 대한 자세한 내용은 다음을 참조하십시오. [회사 수준에서 작업 역할 청구 요금 재정의](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## 회사와의 오브젝트 공유 개요

특정 권한은 섹션에 설명된 대로 회사와 연결된 사용자에게 제공됩니다 [회사에 사용자를 추가하면 얻을 수 있는 이점](#benefits-of-adding-users-to-a-company). 이러한 권한 외에도 사용자가에서 개체를 보거나, 기여하거나, 편집할 수 있는 권한을 허용할 수 있습니다 [!DNL Workfront] 개체를 회사와 공유함으로써.

한 번에 한 명의 개별 사용자와 오브젝트를 공유하지 않고 전체 회사와 공유할 수 있습니다. 회사의 각 사용자는 해당 객체에 대해 동일한 권한을 갖습니다.

개체 공유에 대한 자세한 내용은 [오브젝트에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 그룹 관리자 및 회사 {#group-administrators-and-companies}

다음과 같은 경우 [!DNL Workfront] 관리자가 그룹에 그룹을 할당하면 그룹 관리자는 해당 그룹을 얻을 수 있습니다 [!UICONTROL 관리] 에서 회사에 대한 액세스 [!UICONTROL 설정]. 여기에는 다음에 대한 액세스 권한이 포함됩니다. [!UICONTROL 회사] 페이지 위치 [!UICONTROL 설정]- 그룹과 연결된 회사를 확인하고 관리할 수 있습니다.

에 대한 이 액세스 권한을 사용하여 [!UICONTROL 회사] 페이지 그룹 관리자는 회사에 그룹을 할당할 수 있지만 그룹 관리자가 만든 회사여야 합니다. 그룹 관리자의 액세스 수준이 회사에 대한 관리 액세스 권한으로 구성되지 않은 경우 [!UICONTROL 그룹] 필드는 그룹 관리자가 회사를 만들 때 필요합니다. 굵게 표시된 제목은 다음을 나타냅니다.

![회사 편집](assets/group-admin-add-company.png)

사용자가 액세스 수준에서 회사에 대한 관리 액세스 권한을 얻는 방법에 대한 자세한 내용은 [사용자에게 특정 영역에 대한 관리 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

에서 회사 관리에 대한 자세한 내용 [!UICONTROL 설정] 영역, 참조 [에서 회사 만들기 또는 편집 [!DNL Workfront]](#create-or-edit-a-company-in-workfront) 이 문서에서.
