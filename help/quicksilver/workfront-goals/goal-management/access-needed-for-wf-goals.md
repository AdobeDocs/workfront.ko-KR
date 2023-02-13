---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Workfront 목표 사용 요구 사항
description: Adobe Workfront 목표에 액세스할 수 있으려면 먼저 Adobe Workfront 관리자가 특정 조건이 충족되는지 확인해야 합니다.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 4298659c6eaf7c0370d8d88454e54aeba70f48cf
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# Workfront 목표 사용 요구 사항

Adobe Workfront 목표에 액세스할 수 있으려면 먼저 Adobe Workfront 관리자가 다음 조건을 모두 충족하는지 확인해야 합니다.

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* 조직은 Workfront 목표에 대한 올바른 라이센스를 구매해야 합니다. 자세한 내용은 섹션을 참조하십시오 [Workfront 목표 조직 액세스 권한 얻기](#obtain-workfront-goals-organization-access)참조하십시오.

* 올바른 유형의 Workfront 라이센스를 지정합니다. 라이선스 유형 및 액세스 수준 지정에 대한 자세한 내용은 섹션을 참조하십시오 [라이선스 유형 및 액세스 수준 설정 업데이트](#update-license-types-and-access-level-settings) 참조하십시오.

>[!NOTE]
>
>외부 라이선스 유형이 있는 사용자는 Workfront 목표에 액세스할 수 없습니다.

* 액세스 수준에서 목표에 액세스할 수 있도록 합니다. 자세한 내용은 [Adobe Workfront 목표에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* 기본 메뉴의 목표 영역을 포함하는 레이아웃 템플릿을 지정합니다.

   자세한 내용은 섹션을 참조하십시오. [레이아웃 템플릿에 Workfront 목표 추가](#add-workfront-goals-to-a-layout-template) 참조하십시오.

* 직접 만들지 않은 목표를 수정해야 하는 경우, 목표 작성자가 사용자와 목표를 공유하고 목표에 대한 관리 권한을 제공해야 합니다.

   자세한 내용은 섹션을 참조하십시오 [다른 사용자와 개별 목표 공유](#share-individual-goals-with-other-users) 참조하십시오.

## Workfront 목표 조직 액세스 권한 얻기 {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

사용자가 Workfront 목표에 액세스할 수 있도록 하려면 조직에서 Workfront 라이선스 외에도 추가 라이선스를 구매해야 합니다. 조직에서 추가 라이선스를 구입한 후 Workfront에서 계정에 대해 Workfront 목표를 사용할 수 있습니다. Workfront 목표용 라이센스 구매에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오.

## 라이선스 유형 및 액세스 수준 설정 업데이트  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

Workfront 관리자는 Workfront 목표에 액세스할 수 있도록 다음 Workfront 라이선스 유형 중 하나를 부여해야 합니다.

* 플랜
* 작업
* 검토
* 요청

Workfront 관리자가 이러한 라이선스 유형 중 하나를 부여하면 액세스 수준에서 목표에 대한 액세스 권한도 부여해야 합니다. 목표 액세스에 대한 자세한 내용은 [Adobe Workfront 목표에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Workfront 관리자는 시스템의 Workfront 목표 라이선스 수를 검토하고 현재 활성화된 라이선스 수를 파악할 수 있습니다. 자세한 내용은 [시스템에서 사용 가능한 라이센스 관리](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront을 사용하면 구입한 Workfront 목표 라이센스를 더 많이 할당할 수 있습니다. 그러나 Workfront 목표 계약에 허용된 것보다 더 많은 라이선스를 할당하면 Workfront 계정 관리자가 사용자에게 연락하여 계약 번호를 초과했음을 알려줍니다.

## 레이아웃 템플릿에 Workfront 목표 추가 {#add-workfront-goals-to-a-layout-template}

Workfront 목표에 액세스할 수 있도록 Workfront 또는 그룹 관리자가 기본 메뉴에서 목표 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다.

![](assets/layout-template-align-highlighted-350x220.png)

Workfront 관리자나 그룹 관리자는 레이아웃 템플릿에 다음을 추가하여 Workfront 목표에 쉽게 액세스할 수 있습니다.

* 고정된 탭
* 목표 영역을 랜딩 페이지로 만들기

레이아웃 템플릿 업데이트에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [레이아웃 템플릿 만들기 및 관리](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [레이아웃 템플릿을 사용하여 기본 메뉴 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [레이아웃 템플릿을 사용하여 고정된 페이지 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [레이아웃 템플릿을 사용하여 랜딩 페이지 사용자 지정](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [레이아웃 템플릿에 사용자 할당](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## 다른 사용자와 개별 목표 공유 {#share-individual-goals-with-other-users}

기본적으로 액세스 수준에서 목표에 대한 보기 액세스 권한이 있는 모든 사용자는 Workfront에서 모든 목표를 볼 수 있습니다.

목표에 대한 편집 액세스 권한을 가진 모든 사용자는 목표를 만들 수 있으며, 사용자가 만든 목표에 대한 액세스 권한을 자동으로 관리합니다. 다른 사용자의 목표를 편집해야 하는 경우, 해당 목표에 대한 관리 권한이 있는 사람은 사용자가 만들지 않은 목표를 자신과 공유해야 합니다.

사용자와 목표를 공유하고 사용자에게 관리 권한을 제공하는 방법에 대한 자세한 내용은 [Workfront 목표에서 목표 공유](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
