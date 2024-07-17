---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 블루프린트 구성
description: 블루프린트를 설치하기 전에 프로젝트 템플릿 또는 조직 구조의 세부 사항을 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1826'
ht-degree: 0%

---

# 블루프린트 구성

블루프린트를 설치하기 전에 블루프린트의 세부 사항을 구성할 수 있습니다. 프로젝트 템플릿 및 조직 구조 블루프린트 유형은 일반적으로 일부 환경 설정을 설정하고 일부 속성을 매핑해야 합니다. 다른 블루프린트 유형은 구성이 필요하지 않을 수 있으며 그대로 설치합니다. 설치에 대한 자세한 내용은 [블루프린트 설치](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md)를 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td>
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 라이선스</strong></td>
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td>
   <td> <p>[!UICONTROL 시스템 관리자]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 프로젝트 템플릿 블루프린트 구성

1. 사용할 블루프린트를 찾습니다.
1. **[!UICONTROL 설치]**&#x200B;를 클릭한 다음 환경을 선택하십시오.

   <table style="table-layout:auto">
        <tr>
        <td><strong>프로덕션</strong></td>
        <td>프로덕션은 라이브 환경입니다.</td>
    </tr>
    <tr>
        <td><strong>샌드박스 미리보기</strong></td>
        <td>샌드박스 미리보기는 라이브 환경의 복제본 역할을 하는 테스트 환경이며 Workfront에서 매주 주말에 새로 고칩니다.</td>
    </tr>
    <tr>
        <td><strong>샌드박스 1 및 2</strong></td>
        <td>사용자 지정 새로 고침 샌드박스는 사용자가 수동으로 새로 고치는 별도의 테스트 환경입니다. 사용자 지정 새로 고침 샌드박스를 얻는 데 추가 비용이 있습니다.</td>
    </tr>
   </table>

1. 다음 섹션을 계속합니다.

   * [[!UICONTROL 템플릿 환경 설정]](#template-preferences)
   * [[!UICONTROL 역할 매핑]](#role-mapping)
   * [[!UICONTROL 팀 매핑]](#team-mapping)
   * [[!UICONTROL 회사 매핑]g](#company-mapping)
   * [[!UICONTROL 그룹 매핑]](#group-mapping)

## [!UICONTROL 템플릿 환경 설정] {#template-preferences}

템플릿 설치 방법을 선택합니다.

블루프린트를 설치하기 전에 템플릿 소유권을 지정할 수도 있습니다. 템플릿을 설치한 후 이러한 필드를 변경할 수 있습니다. 자세한 내용은 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하세요.

![[!UICONTROL 템플릿 환경 설정] 섹션](assets/Blueprints_TemplatePreferences.png)

1. [!UICONTROL 템플릿 환경 설정] 섹션에서 새 템플릿 이름을 지정하십시오.
1. 다음을 지정합니다.

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 템플릿 소유자]<strong></td>
        <td>이 사람은 템플릿에 대한 [!UICONTROL 관리] 권한을 받으며, 템플릿을 사용하여 프로젝트를 만들 때 프로젝트 소유자가 됩니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 템플릿 스폰서]</strong></td>
        <td>이 사람은 일반적으로 프로젝트의 진행 상황을 알아야 하는 관리자, 경영진 또는 이해 당사자입니다. 프로젝트 스폰서는 프로젝트에 대한 추가 액세스 권한을 획득하지 않지만 프로젝트에 대한 이메일 알림에 추가됩니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>이는 프로젝트가 생성될 때 속할 포트폴리오입니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 프로그램]</strong></td>
        <td>이는 프로젝트가 생성될 때 속할 프로그램입니다.</td>
    </tr>
   </table>

1. 템플릿이 활성으로 설치되었는지 아니면 비활성으로 설치되었는지 선택합니다.
1. 환경 설정이 있는 경우 정의된 새 문제 환경 설정을 사용할지 여부를 선택합니다.

   **[!UICONTROL 문제 환경 설정 보기]**&#x200B;를 클릭하여 블루프린트와 함께 설치할 특정 환경 설정을 검토합니다. 가져온 템플릿에서 만든 프로젝트는 [!UICONTROL 문제] 섹션에 추가된 새 문제에 대해 이 환경 설정을 사용합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>대기열 주제 그룹</strong></td> 
      <td> <p>대기열 주제 그룹은 문제 또는 요청에 대한 가장 높은 수준의 범주를 정의합니다. 요청을 제출할 위치를 선택할 때 주제 그룹을 메뉴 옵션으로 봅니다. 주제 그룹에는 여러 개의 대기열 주제가 포함될 수 있습니다. 자세한 내용은 <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">주제 그룹 만들기</a>를 참조하십시오. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>대기열 주제</strong></td> 
      <td> <p>대기열 주제는 라우팅 규칙과 함께 작동하여 문제 또는 요청을 할당합니다. 사용자가 주제 그룹을 선택한 후 문제 또는 요청을 입력할 때 선택하는 메뉴 옵션입니다. 자세한 내용은 <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">대기열 주제 만들기</a>를 참조하십시오. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>라우팅 규칙</strong></td> 
      <td>라우팅 규칙은 특정 작업 역할 , 사용자 또는 팀에 문제 또는 요청을 보냅니다. 또한 요청 대기열과 연관된 프로젝트가 아닌 특정 프로젝트에 요청을 전송할 수도 있습니다. 자세한 내용은 <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a>를 참조하세요. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**예:** 이 블루프린트의 새 문제 환경 설정에서 4개의 대기열 주제를 제공합니다. 사용자는 문제를 생성할 때 다음 항목 중 하나를 선택합니다. (주제 그룹이 하나만 있으므로 자동으로 적용되며 사용자가 선택할 필요가 없습니다.) 사용자가 문제를 완료하고 제출하면 라우팅 규칙에 따라 할당된 작업 역할이나 팀이 결정됩니다.
   >![새 문제 환경 설정 예제](assets/Blueprints_IssuePrefsDetails.png)
   >![새 문제에 대한 대기열 주제](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![작업 역할로 전달된 문제](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* 문제 환경 설정을 사용하면 프로젝트에서 새로운 문제 또는 요청을 캡처하는 방식으로 일관성을 유지하는 데 도움이 됩니다.
   >* 이러한 환경 설정을 지정해도 템플릿에서 만든 프로젝트가 요청 대기열로 자동 만들어지지 않습니다. 요청 대기열 설정에 대한 자세한 내용은 [요청 대기열 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.
   >* 일부 블루프린트에 새 문제 환경 설정이 포함되어 있지 않습니다.


## [!UICONTROL 역할 매핑] {#role-mapping}

>[!NOTE]
>
>이 섹션은 일부 블루프린트에 표시되지 않을 수 있습니다.

일부 템플릿에는 규정된 작업 역할이 포함됩니다. 작업 역할은 템플릿을 프로젝트로 전환할 때 적합한 인력을 할당하는 데 도움이 됩니다. 블루프린트를 설치하기 전에 역할을 매핑하는 방법을 사용자 지정할 수 있습니다. 블루프린트에서 사용할 수 있는 역할에 대한 자세한 내용을 보려면 **[!UICONTROL 역할 설명 보기]**&#x200B;를 클릭하십시오.

블루프린트는 역할 이름별로 검색하여 일치하는 기존 역할이 있는지 확인합니다. 검색은 대/소문자를 구분하므로 이름은 정확히 일치해야 합니다. 일치하는 기존 역할이 없는 경우 블루프린트에서 자동으로 생성하도록 할 수 있습니다.

![[!UICONTROL 역할 매핑] 섹션](assets/Blueprints_RoleMapping.png)

1. 역할이 있는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 다른 이름으로 새 역할을 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 기존 역할을 사용한 다음 선택 상자에서 역할을 선택합니다.
   1. 매핑된 역할을 사용하지 마십시오. 일부 작업에는 역할이 할당되지 않으므로 이 옵션은 권장되지 않습니다.

1. 역할이 없는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 새 역할을 만듭니다. 이 옵션은 블루프린트에서 권장하는 역할을 만듭니다.
   1. 다른 이름으로 새 역할을 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 기존 역할을 사용한 다음 선택 상자에서 역할을 선택합니다.
   1. 매핑된 역할을 사용하지 마십시오. 일부 작업에는 역할이 할당되지 않으므로 이 옵션은 권장되지 않습니다.

>[!NOTE]
>
>설치 프로세스는 특정 사용자에게는 역할을 적용하지 않습니다. 블루프린트 솔루션을 설치한 후 이러한 역할의 직원을 확인하고 필요한 경우 직원을 할당해야 합니다. 자세한 내용은 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md)을 참조하세요.

[!DNL Workfront]의 작업 역할에 대한 자세한 내용은 [작업 역할 만들기 및 관리](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.

## [!UICONTROL 팀 매핑] {#team-mapping}

>[!NOTE]
>
>이 섹션은 일부 블루프린트에 표시되지 않을 수 있습니다.

일부 템플릿에는 처방된 팀이 포함됩니다. 팀에 할당된 작업은 팀원 누구나 완료할 수 있습니다. 블루프린트를 설치하기 전에 팀을 매핑하는 방법을 사용자 지정할 수 있습니다. 블루프린트에서 사용 가능한 팀에 대한 자세한 내용을 보려면 **[!UICONTROL 팀 설명 보기]**&#x200B;를 클릭하십시오.

블루프린트는 팀 이름별로 검색하여 일치하는 기존 팀이 있는지 확인합니다. 검색은 대/소문자를 구분하므로 이름은 정확히 일치해야 합니다. 일치하는 기존 팀이 없는 경우 블루프린트로 팀을 생성하도록 할 수 있습니다.

![[!UICONTROL 팀 매핑] 섹션](assets/Blueprints_TeamMapping.png)

1. 팀이 있는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 다른 이름으로 새 팀을 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. [!UICONTROL 기존 팀]을 사용한 다음 선택 상자에서 팀을 선택하십시오.
   1. 매핑된 팀을 사용하지 마십시오. 일부 작업에는 팀이 할당되지 않으므로 이 옵션은 권장되지 않습니다.

1. 팀이 없는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 새 팀을 만듭니다. 이 옵션은 블루프린트가 권장하는 팀을 만듭니다.
   1. 다른 이름으로 새 팀을 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. [!UICONTROL 기존 팀]을 사용한 다음 선택 상자에서 팀을 선택하십시오.
   1. 매핑된 팀을 사용하지 마십시오. 일부 작업에는 팀이 할당되지 않으므로 이 옵션은 권장되지 않습니다.

>[!NOTE]
>
>설치 프로세스는 팀에 사람을 추가하지 않습니다. 블루프린트 솔루션을 설치한 후 팀의 직원을 확인하고 필요한 경우 직원을 할당해야 합니다. 자세한 내용은 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md)을 참조하세요.

[!DNL Workfront]에서 팀이 작동하는 방법에 대한 자세한 내용은 [팀 만들기 및 관리](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md)를 참조하십시오.

## 회사 매핑 {#company-mapping}

>[!NOTE]
>
>이 섹션은 일부 블루프린트에 표시되지 않을 수 있습니다.

일부 청사진에는 처방받은 업체가 포함되어 있다. 회사는 조직, 조직 내 부서 또는 함께 일하는 고객을 대표할 수 있는 조직 단위입니다. 블루프린트를 설치하기 전에 회사가 매핑되는 방법을 사용자 지정할 수 있습니다. 블루프린트에서 사용할 수 있는 회사에 대한 자세한 내용을 보려면 **[!UICONTROL 회사 설명 보기]**&#x200B;를 클릭하십시오.

블루프린트는 회사 이름별로 검색하여 일치하는 기존 회사가 있는지 확인합니다. 검색은 대/소문자를 구분하므로 이름은 정확히 일치해야 합니다. 일치하는 기존 회사가 없는 경우 블루프린트에서 해당 회사를 생성하도록 할 수 있습니다. 블루프린트의 기본 회사는 동일한 이름이 없어도 환경의 기본 회사에 매핑됩니다.

![[!UICONTROL 회사 매핑] 섹션](assets/Blueprints_CompanyMapping.png)

1. 회사가 존재하는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 다른 이름으로 새 회사를 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 기존 회사를 사용한 다음 선택 상자에서 회사를 선택합니다.\

      블루프린트의 기본 회사는 동일한 이름이 없어도 환경의 기본 회사에 매핑됩니다.
   1. 매핑된 회사를 사용하지 마십시오. 다른 개체에 있는 회사 참조가 비어 있으므로 이 옵션은 권장되지 않습니다.

1. 회사가 없는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 새 회사를 만듭니다. 이 옵션은 블루프린트가 권장하는 회사를 만듭니다.
   1. 다른 이름으로 새 회사를 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 기존 회사를 사용한 다음 선택 상자에서 회사를 선택합니다.
   1. 매핑된 회사를 사용하지 마십시오. 다른 개체에 있는 회사 참조가 비어 있으므로 이 옵션은 권장되지 않습니다.

>[!NOTE]
>
>블루프린트를 설치한 후 회사를 구성하려면 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md)을 참조하십시오.

템플릿을 회사와 연결하는 방법에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md)을 참조하십시오.

[!DNL Workfront]에서 회사가 작동하는 방식에 대한 자세한 내용은 [회사 만들기 및 편집](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하십시오.

## [!UICONTROL 그룹 매핑] {#group-mapping}

>[!NOTE]
>
>이 섹션은 일부 블루프린트에 표시되지 않을 수 있습니다.

일부 청사진에는 처방된 그룹이 포함되어 있습니다. 그룹은 부서 구조와 일치하는 사용자 그룹입니다. 그룹은 Workfront의 팀 및 회사와 유사하지만 다릅니다. 블루프린트를 설치하기 전에 그룹을 매핑하는 방법을 사용자 지정할 수 있습니다. 블루프린트에서 사용할 수 있는 그룹에 대한 자세한 내용을 보려면 **[!UICONTROL 그룹 설명 보기]**&#x200B;를 클릭하십시오.

블루프린트는 그룹 이름별로 검색하여 일치하는 기존 그룹이 있는지 확인합니다. 검색은 대/소문자를 구분하므로 이름은 정확히 일치해야 합니다. 일치하는 기존 그룹이 없는 경우 블루프린트로 해당 그룹을 생성하도록 할 수 있습니다.

![[!UICONTROL 그룹 매핑] 섹션](assets/Blueprints_GroupMapping.png)

1. 그룹이 있으면 **[!UICONTROL 그룹 다시 매핑]**&#x200B;을 선택하고 다음 옵션 중 하나를 선택할 수 있습니다.

   1. **[!UICONTROL 다른 이름으로 새 그룹을 만든 다음]** 이 그룹에 할당할 이름을 입력하십시오. 블루프린트 정의의 그룹에 대한 참조는 대신 이 새 그룹에 연결됩니다.
   1. **[!UICONTROL 기존 그룹으로 바꾸기]**&#x200B;한 다음 선택 상자에서 그룹을 검색하고 선택합니다.

      >[!NOTE]
      >
      >기존 그룹의 이름은 변경할 수 없습니다.

1. 그룹이 없는 경우 다음을 수행할 수 있습니다.

   1. 텍스트 상자에 제안된 그룹 이름을 입력하여 변경합니다.
   1. **[!UICONTROL 그룹 다시 매핑]**&#x200B;을 선택하고 [!UICONTROL 기존 그룹으로 바꾸기]를 선택한 다음 선택 상자에서 그룹을 검색하고 선택합니다.
   1. **[!UICONTROL 그룹 다시 매핑]**&#x200B;을 선택하고 **[!UICONTROL 기존 그룹에 삽입]**&#x200B;을 선택한 다음 선택 상자에서 그룹을 검색하여 선택하십시오. 이 옵션은 기존 그룹 아래에 새 하위 그룹을 만듭니다.

>[!NOTE]
>
>블루프린트를 설치한 후 그룹을 구성하려면 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md)을 참조하십시오.

[!DNL Workfront]에서 그룹을 사용하는 방법에 대한 자세한 내용은 [그룹 개요](../../administration-and-setup/manage-groups/groups-overview/groups.md)를 참조하십시오.
