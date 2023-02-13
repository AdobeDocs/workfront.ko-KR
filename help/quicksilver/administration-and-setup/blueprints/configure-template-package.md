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
source-wordcount: '1824'
ht-degree: 0%

---

# 블루프린트 구성

블루프린트를 설치하기 전에 블루프린트의 세부 사항을 구성할 수 있습니다. 프로젝트 템플릿 및 조직 구조 블루프린트 유형에는 일반적으로 일부 환경 설정을 설정하고 일부 속성을 매핑해야 합니다. 다른 블루프린트 유형은 구성이 필요하지 않을 수 있으며, 있는 그대로 설치합니다. 설치에 대한 자세한 내용은 [블루프린트 설치](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td>
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 라이선스</strong></td>
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td>
   <td> <p>[!UICONTROL System 관리자]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 프로젝트 템플릿 블루프린트 구성

1. 사용할 블루프린트를 찾습니다.
1. 클릭 **[!UICONTROL 설치]**&#x200B;를 선택한 다음 환경을 선택합니다.

   <table style="table-layout:auto">
        <tr>
        <td><strong>프로덕션</strong></td>
        <td>프로덕션은 라이브 환경입니다.</td>
    </tr>
    <tr>
        <td><strong>샌드박스 미리보기</strong></td>
        <td>샌드박스 미리 보기는 라이브 환경의 복제본 역할을 하며 Workfront에서 매주 새로 고침되는 테스트 환경입니다.</td>
    </tr>
    <tr>
        <td><strong>샌드박스 1 및 2</strong></td>
        <td>사용자 지정 새로 고침 샌드박스는 사용자가 수동으로 새로 고치는 별도의 테스트 환경입니다. 사용자 지정 새로 고침 샌드박스를 얻는 데 추가 비용이 있습니다.</td>
    </tr>
   </table>

1. 다음 섹션을 계속 진행합니다.

   * [[!UICONTROL 템플릿 기본 설정]](#template-preferences)
   * [[!UICONTROL 역할 매핑]](#role-mapping)
   * [[!UICONTROL 팀 매핑]](#team-mapping)
   * [[!UICONTROL 회사 매핑]g](#company-mapping)
   * [[!UICONTROL 그룹 매핑]](#group-mapping)

## [!UICONTROL 템플릿 기본 설정] {#template-preferences}

템플릿을 설치할 방법을 선택합니다.

블루프린트를 설치하기 전에 템플릿 소유권을 지정할 수도 있습니다. 템플릿을 설치한 후 이러한 필드를 변경할 수 있습니다. 자세한 내용은 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL 템플릿 기본 설정] 섹션](assets/Blueprints_TemplatePreferences.png)

1. 에서 [!UICONTROL 템플릿 기본 설정] 섹션에서 새 템플릿 이름을 지정합니다.
1. 다음을 지정합니다.

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 템플릿 소유자]<strong></td>
        <td>이 사람은 템플릿에 대한 [!UICONTROL 관리] 권한을 받고 템플릿을 사용하여 프로젝트를 만들 때 프로젝트 소유자가 됩니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Template Sponsor]</strong></td>
        <td>일반적으로 이 사람은 프로젝트의 진행 상황을 알고 있어야 하는 관리자, 경영진 또는 이해 당사자입니다. 프로젝트 스폰서는 프로젝트에 대한 추가 액세스 권한을 받지 않지만, 프로젝트에 대한 이메일 알림에 추가됩니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>프로젝트가 생성될 때 프로젝트가 속할 포트폴리오입니다.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>프로젝트가 생성될 때 프로젝트가 속해 있는 프로그램입니다.</td>
    </tr>
   </table>

1. 템플릿이 활성 또는 비활성 상태로 설치되는지 여부를 선택합니다.
1. 기본 설정을 사용할 수 있는 경우 정의된 새 문제 기본 설정을 사용할지 여부를 선택합니다.

   클릭 **[!UICONTROL 문제 환경 설정 을 참조하십시오]** 를 클릭하여 블루프린트와 함께 설치할 특정 환경 설정을 검토합니다. 가져온 템플릿에서 만든 프로젝트에서는 이러한 환경 설정을 [!UICONTROL 문제] 섹션을 참조하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>대기열 주제 그룹</strong></td> 
      <td> <p>큐 항목 그룹은 문제 또는 요청에 대한 가장 높은 카테고리 수준을 정의합니다. 사용자는 요청을 제출할 위치를 선택할 때 항목 그룹을 메뉴 옵션으로 봅니다. 항목 그룹에는 여러 큐 주제가 포함될 수 있습니다. 자세한 내용은 <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">주제 그룹 만들기</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>대기열 주제</strong></td> 
      <td> <p>대기열 항목은 공정순서 규칙과 함께 작동하여 문제나 요청을 지정합니다. 이는 사용자가 주제 그룹을 선택한 후 문제 또는 요청을 입력할 때 선택하는 메뉴 옵션입니다. 자세한 내용은 <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">큐 항목 만들기</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>라우팅 규칙</strong></td> 
      <td>라우팅 규칙은 문제나 요청을 특정 작업 역할, 사용자 또는 팀에 보냅니다. 또한 요청 큐와 연결된 프로젝트 이외의 특정 프로젝트에 요청을 보낼 수도 있습니다. 자세한 내용은 <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**예:** 이 블루프린트의 새 문제 환경 설정은 4개의 큐 주제를 제공합니다. 사용자는 문제를 만들 때 이러한 항목 중 하나를 선택합니다. (주제 그룹은 하나만 있으므로 자동으로 적용되며 사용자가 선택할 필요가 없습니다.) 사용자가 문제를 완료하고 제출하면, 라우팅 규칙은 사용자에게 할당된 작업 역할 또는 팀을 결정합니다.
   >![새 문제 환경 설정 샘플](assets/Blueprints_IssuePrefsDetails.png)
   >![새 문제에 대한 큐 항목](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![작업 역할로 라우팅된 문제](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* 문제 환경 설정을 사용하면 프로젝트에서 새로운 문제 또는 요청을 캡처하는 방식으로 일관성을 만들 수 있습니다.
   >* 이러한 환경 설정을 설정해도 템플릿에서 만든 프로젝트가 요청 큐로 자동으로 만들어지지 않습니다. 요청 큐 설정에 대한 자세한 내용은 [요청 큐 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* 모든 청사진에는 새 문제 환경 설정이 포함되어 있지 않습니다.



## [!UICONTROL 역할 매핑] {#role-mapping}

>[!NOTE]
>
>이 섹션이 일부 청사진에는 나타나지 않을 수 있습니다.

일부 템플릿에는 지정된 작업 역할이 포함됩니다. 작업 역할은 템플릿을 프로젝트로 변환할 때 적합한 사람을 할당하는 데 도움이 됩니다. 블루프린트를 설치하기 전에 역할 매핑 방법을 사용자 지정할 수 있습니다. 클릭 **[!UICONTROL 역할 설명 을 참조하십시오]** 블루프린트에서 사용할 수 있는 역할에 대해 자세히 알아보십시오.

블루프린트는 역할 이름으로 검색하여 기존 역할이 일치하는지 확인합니다. 검색은 대/소문자를 구분하므로 이름이 정확히 일치해야 합니다. 일치하는 기존 역할이 없는 경우 블루프린트에서 자동으로 만들 수 있습니다.

![[!UICONTROL 역할 매핑] 섹션](assets/Blueprints_RoleMapping.png)

1. 역할이 있을 경우 다음 옵션 중 하나를 선택할 수 있습니다.

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
>설치 프로세스는 특정 사용자에게 역할을 적용하지 않습니다. 블루프린트 솔루션을 설치한 후 해당 역할의 사람을 확인하고 필요한 경우 사람을 할당해야 합니다. 자세한 내용은 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

의 작업 역할에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오. [작업 역할 만들기 및 관리](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL 팀 매핑] {#team-mapping}

>[!NOTE]
>
>이 섹션이 일부 청사진에는 나타나지 않을 수 있습니다.

일부 템플릿에는 지정된 팀이 포함됩니다. 팀에 할당된 작업은 팀의 모든 구성원이 완료할 수 있습니다. 블루프린트를 설치하기 전에 팀 매핑 방법을 사용자 지정할 수 있습니다. 클릭 **[!UICONTROL 팀 설명 참조]** 를 참조하십시오.

블루프린트는 팀 이름으로 검색하여 기존 팀이 일치하는지 확인합니다. 검색은 대/소문자를 구분하므로 이름이 정확히 일치해야 합니다. 일치하는 기존 팀이 없으면 블루프린트에서 자동으로 만들 수 있습니다.

![[!UICONTROL 팀 매핑] 섹션](assets/Blueprints_TeamMapping.png)

1. 팀이 있는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 다른 이름으로 새 팀을 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 사용 [!UICONTROL 기존 팀]을 선택한 다음 선택 상자에서 팀을 선택합니다.
   1. 매핑된 팀을 사용하지 마십시오. 일부 작업에는 팀이 할당되지 않으므로 이 옵션은 권장되지 않습니다.

1. 팀이 없으면 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 새 팀을 만듭니다. 이 옵션은 블루프린트에서 권장하는 팀을 만듭니다.
   1. 다른 이름으로 새 팀을 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 사용 [!UICONTROL 기존 팀]을 선택한 다음 선택 상자에서 팀을 선택합니다.
   1. 매핑된 팀을 사용하지 마십시오. 일부 작업에는 팀이 할당되지 않으므로 이 옵션은 권장되지 않습니다.

>[!NOTE]
>
>설치 프로세스에서 팀에 사람을 추가하지 않습니다. 블루프린트 솔루션을 설치한 후 팀의 사람을 확인하고 필요한 경우 사람을 할당해야 합니다. 자세한 내용은 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

에서 팀이 작동하는 방식에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오. [팀 만들기 및 관리](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## 회사 매핑 {#company-mapping}

>[!NOTE]
>
>이 섹션이 일부 청사진에는 나타나지 않을 수 있습니다.

일부 청사진에는 처방된 회사가 포함됩니다. 회사는 조직, 조직 내 부서 또는 함께 일하는 클라이언트를 나타낼 수 있는 조직 단위입니다. 블루프린트를 설치하기 전에 회사 매핑 방법을 사용자 지정할 수 있습니다. 클릭 **[!UICONTROL 회사 설명 참조]** 블루프린트에서 사용할 수 있는 회사에 대해 자세히 알아보십시오.

블루프린트는 회사 이름으로 검색하여 기존 회사가 일치하는지 확인합니다. 검색은 대/소문자를 구분하므로 이름이 정확히 일치해야 합니다. 일치하는 기존 회사가 없으면 블루프린트에서 자동으로 만들 수 있습니다. 블루프린트의 기본 회사는 이름이 동일하지 않더라도 환경의 기본 회사에 매핑됩니다.

![[!UICONTROL 회사 매핑] 섹션](assets/Blueprints_CompanyMapping.png)

1. 회사가 존재하는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 다른 이름으로 새 회사를 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 기존 회사를 사용한 다음 선택 상자에서 회사를 선택합니다.\

      블루프린트의 기본 회사는 이름이 동일하지 않더라도 환경의 기본 회사에 매핑됩니다.
   1. 매핑된 회사를 사용하지 마십시오. 다른 개체의 회사 참조가 비어 있으므로 이 옵션은 사용하지 않는 것이 좋습니다.

1. 회사가 없는 경우 다음 옵션 중 하나를 선택할 수 있습니다.

   1. 새 회사 만들기. 이 옵션은 블루프린트에서 권장하는 회사를 만듭니다.
   1. 다른 이름으로 새 회사를 만든 다음 텍스트 상자에 이름을 입력합니다.
   1. 기존 회사를 사용한 다음 선택 상자에서 회사를 선택합니다.
   1. 매핑된 회사를 사용하지 마십시오. 다른 개체의 회사 참조가 비어 있으므로 이 옵션은 사용하지 않는 것이 좋습니다.

>[!NOTE]
>
>블루프린트를 설치한 후 회사를 구성하려면 를 참조하십시오 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

템플릿과 회사 연결에 대한 자세한 내용은 [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

에서 회사가 작동하는 방식에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오. [회사 만들기 및 편집](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL 그룹 매핑] {#group-mapping}

>[!NOTE]
>
>이 섹션이 일부 청사진에는 나타나지 않을 수 있습니다.

몇몇 청사진에는 처방된 그룹이 포함되어 있습니다. 그룹은 부서 구조와 일치하는 사용자 그룹입니다. 그룹은 Workfront의 팀 및 회사와 유사하지만 구별됩니다. 블루프린트를 설치하기 전에 그룹 매핑 방법을 사용자 지정할 수 있습니다. 클릭 **[!UICONTROL 그룹 설명 을 참조하십시오]** 블루프린트에서 사용할 수 있는 그룹에 대해 자세히 알아보십시오.

블루프린트는 그룹 이름으로 검색하여 기존 그룹이 일치하는지 확인합니다. 검색은 대/소문자를 구분하므로 이름이 정확히 일치해야 합니다. 일치하는 기존 그룹이 없으면 블루프린트에서 자동으로 만들 수 있습니다.

![[!UICONTROL 그룹 매핑] 섹션](assets/Blueprints_GroupMapping.png)

1. 그룹이 있으면 **[!UICONTROL 그룹 다시 매핑]** 다음 옵션 중 하나를 선택합니다.

   1. **[!UICONTROL 다른 이름으로 새 그룹 만들기]**&#x200B;그런 다음 이 그룹에 지정할 이름을 입력합니다. 블루프린트 정의에서 그룹에 대한 참조가 이 새 그룹에 대신 연결됩니다.
   1. **[!UICONTROL 기존 그룹으로 바꾸기]**&#x200B;그런 다음 선택 상자에서 그룹을 검색하고 선택합니다.

      >[!NOTE]
      >
      >기존 그룹의 이름은 변경할 수 없습니다.

1. 그룹이 없으면 다음을 수행할 수 있습니다.

   1. 텍스트 상자에 입력하여 추천 그룹 이름을 변경합니다.
   1. 선택 **[!UICONTROL 그룹 다시 매핑]** 및 [!UICONTROL 기존 그룹으로 바꾸기]그런 다음 선택 상자에서 그룹을 검색하고 선택합니다.
   1. 선택 **[!UICONTROL 그룹 다시 매핑]** 및 **[!UICONTROL 기존 그룹 아래에 삽입]**&#x200B;그런 다음 선택 상자에서 그룹을 검색하고 선택합니다. 이 옵션은 기존 그룹 아래에 새 하위 그룹을 만듭니다.

>[!NOTE]
>
>블루프린트를 설치한 후 그룹을 구성하려면 다음을 참조하십시오 [블루프린트 설치 후 수행할 작업](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

에서 그룹 사용에 대한 자세한 내용 [!DNL Workfront]를 참조하십시오. [그룹 개요](../../administration-and-setup/manage-groups/groups-overview/groups.md).
