---
title: 레이아웃 템플릿에 사용자 할당
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Adobe Workfront 관리자는 사용자가 만든 레이아웃 템플릿을 사용해야 하는 사용자, 작업 역할, 팀 또는 그룹에 할당할 수 있습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# 레이아웃 템플릿에 사용자 할당

만든 레이아웃 템플릿을 사용해야 하는 사용자, 작업 역할, 팀 또는 그룹에 할당할 수 있습니다.

사용자에게 레이아웃 템플릿이 할당되지 않은 사용자의 경우 기본 레이아웃이 사용됩니다. 기본 레이아웃에 대한 자세한 내용은 [기본 Adobe Workfront 레이아웃 정보](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)를 참조하세요.

레이아웃 템플릿을 사용하여 내 작업 및 작업 요청 영역 변경에서 설명한 대로 사용자가 레이아웃 템플릿을 자신에게 할당할 수도 있습니다.

동일한 이름에 여러 다른 레이아웃 템플릿을 할당할 수 있습니다. 사용자, 역할, 그룹 또는 팀에 적용되는 레이아웃 템플릿에 대한 자세한 내용은 이 문서의 뒷부분에서 [레이아웃 템플릿 할당 우선 순위](#layout-template-assignment-priority)를 참조하십시오.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)을 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자에게 레이아웃 템플릿 할당

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.

   >[!TIP]
   >
   >레이아웃 템플릿이 만족스러우면 [새 레이아웃 템플릿 테스트](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)에 설명된 대로 테스트하는 것이 좋습니다.

1. 페이지 상단 섹션에서 **할당 대상**&#x200B;을 클릭합니다.
1. 표시되는 상자에서 **사용자, 작업 역할, 팀 또는 그룹 추가**&#x200B;를 클릭하고 사용자, 작업 역할, 팀 또는 그룹의 이름을 입력한 다음 드롭다운에 표시될 때 이름을 클릭합니다.

   최근에 추가된 이름이 파란색 배경과 함께 표시됩니다. 이 기능은 방금 추가한 이름과 이미 목록에 있는 이름을 구분할 수 있으므로 기존 레이아웃 템플릿을 편집할 때 유용합니다.

   다른 레이아웃 템플릿에 이미 할당된 사용자, 작업 역할, 팀 또는 그룹의 이름 오른쪽에 정보 아이콘 ![](assets/info-icon.png)이(가) 표시됩니다. 아이콘 위로 마우스를 가져가면 해당 레이아웃 템플릿의 이름을 볼 수 있으며 기존 할당을 재정의할지 여부를 결정할 수 있습니다.

1. 필요에 따라 레이아웃 템플릿을 다른 사용자, 작업 역할, 팀 또는 그룹에 할당하려면 앞의 두 단계를 반복합니다.

   한 번에 최대 100명의 사용자를 할당할 수 있습니다.

1. **완료**&#x200B;를 클릭한 다음 왼쪽 하단의 **저장**&#x200B;을 클릭합니다.

   이 단계에서는 레이아웃 템플릿을 만들고 할당하는 프로세스를 완료합니다.

## 레이아웃 템플릿 할당 우선 순위 {#layout-template-assignment-priority}

사용자와 다른 Workfront 관리자는 다음 네 가지 방법으로 동일한 사용자에게 서로 다른 여러 레이아웃 템플릿을 할당할 수 있습니다.

* 개별 사용자에게
* 사용자가 가지고 있는 특정 작업 역할에
* 사용자가 속한 특정 팀에게
* 사용자가 속한 특정 그룹에게

그러나 레이아웃 템플릿은 사용자가 언제든지 한 개만 볼 수 있습니다. 표시되는 템플릿은 다음 우선순위 계층에 의해 결정됩니다.

* **개별 사용자**: 개별 사용자로 사용자에게 할당된 레이아웃 템플릿이 다른 모든 사용자를 재정의합니다. 새 할당을 수행하여 개별 사용자가 수행한 이전 할당을 재정의할 수 있습니다. 가장 최근 할당이 우선합니다.
* **기본 작업 역할**: 사용자에게 단일 사용자로 레이아웃 템플릿이 할당되지 않은 경우 기본 작업 역할에 할당된 템플릿이 표시됩니다.

  사용자의 기본 작업 역할에 할당된 레이아웃 템플릿만 사용자에게 표시됩니다. 사용자가 보유한 보조 작업 역할에 할당된 템플릿이 표시되지 않습니다.

* **홈 팀**: 개인 사용자 또는 기본 작업 역할이 있는 사용자로 레이아웃 템플릿이 할당되지 않은 경우 홈 팀에 할당된 템플릿이 표시됩니다.

  사용자의 홈 팀에 할당된 템플릿만 사용자에게 표시됩니다. 사용자가 멤버인 다른 팀에 할당된 템플릿은 표시되지 않습니다.

* **홈 그룹**: 개인 사용자, 기본 작업 역할이 있는 사용자 또는 홈 팀의 구성원으로 레이아웃 템플릿이 할당되지 않은 경우 홈 그룹에 할당된 템플릿이 표시됩니다.

  사용자의 홈 그룹에 할당된 템플릿만 사용자에게 표시됩니다. 다른 그룹에 할당된 템플릿이 표시되지 않습니다.

## 많은 사용자가 레이아웃 템플릿에 할당됨

2000명 이상의 사용자에게 할당된 레이아웃 템플릿을 편집하고 변경하면 처음 2000명의 사용자만 레이아웃 템플릿에 유지되고 수행한 변경 사항이 표시됩니다. 레이아웃 템플릿이 다른 모든 템플릿에서 제거됩니다.

레이아웃 템플릿에 할당할 사용자가 2000명을 초과하는 경우 다음 중 하나를 수행하는 것이 좋습니다.

* 사용자를 그룹 또는 팀으로 구성하고 해당 그룹 또는 팀에 레이아웃 템플릿을 할당합니다. 자세한 내용은 [그룹 만들기](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 및 [팀 만들기 및 관리](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md)를 참조하세요.

* 사용자에게 작업 역할을 할당하고 기본 작업 역할에 레이아웃 템플릿을 할당합니다. 자세한 내용은 [작업 역할 만들기 및 관리](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)를 참조하십시오.
