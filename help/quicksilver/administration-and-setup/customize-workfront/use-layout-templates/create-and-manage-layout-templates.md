---
title: 레이아웃 템플릿 만들기 및 관리
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 만들고 수정하여 사용자를 위해 Workfront의 레이아웃 요소를 사용자 정의할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 2%

---

# 레이아웃 템플릿 만들기 및 관리

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 만들고 수정하여 사용자를 위해 Workfront에서 다음 레이아웃 요소를 사용자 정의할 수 있습니다.

* 메인 메뉴
* 왼쪽 탐색 패널
* 홈 영역
* 요약 패널
* 목록 및 보고서에서 사람들이 사용하는 보기, 필터 및 그룹입니다.
* 화면 용어
* 프로젝트, 작업 및 문제 헤더

레이아웃 템플릿을 만들거나 수정한 후에는 개별 사용자, 팀, 그룹 또는 작업 역할에 할당할 수 있습니다.

모든 사용자의 기본 Workfront 레이아웃은 액세스 수준 및 라이선스 유형에 따라 다릅니다. 예를 들어, 일부 사용자는 기본 메뉴에 일부 영역이 표시되지 않을 수 있습니다. 자세한 내용은 [기본 Adobe Workfront 레이아웃 정보](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)를 참조하세요.

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
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.</p>
        <p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레이아웃 템플릿 만들기 및 관리에 대한 고려 사항

* 사용자는 자신의 레이아웃의 몇 가지 영역을 사용자 정의할 수 있습니다. 레이아웃 템플릿을 변경하면 덮어쓰거나 재설정하지 않고 변경 사항이 사용자 정의된 모든 항목과 병합됩니다. 새 레이아웃 템플릿에 사용자를 할당하는 경우에도 마찬가지입니다.
* 그룹 관리자와 다른 사용자를 편집할 수 있는 플랜 라이선스가 있는 사용자는 프로필을 편집할 때 관리할 수 있는 사용자에게 시스템 수준 및 그룹 수준 레이아웃 템플릿을 추가할 수 있습니다.
* 그룹 관리자는 작업 역할 또는 팀에 레이아웃 템플릿을 할당할 수 없습니다.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)을 참조하십시오.

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## 레이아웃 템플릿 만들기 또는 수정

{{step-1-to-setup}}

1. 왼쪽 패널에서 **인터페이스** > **레이아웃 템플릿**&#x200B;을 클릭합니다.

1. **새 레이아웃 템플릿**&#x200B;을 클릭합니다.

   또는

   수정할 레이아웃 템플릿의 이름을 클릭합니다.

1. 새 레이아웃 템플릿을 만드는 경우 **레이아웃 템플릿 이름**&#x200B;을(를) 입력하고 **설명**&#x200B;을(를) 입력하십시오.

1. 다음 문서에 설명된 대로 사용자 인터페이스의 영역을 사용자 정의합니다.

   * [레이아웃 템플릿을 사용하여 기본 메뉴 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [레이아웃 템플릿을 사용하여 고정된 페이지 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [레이아웃 템플릿을 사용하여 요약 패널 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [레이아웃 템플릿을 사용하여 홈 맞춤화](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   * [레이아웃 템플릿을 사용하여 랜딩 페이지 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [레이아웃 템플릿을 사용하여 사용자 인터페이스 용어 맞춤화](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 아래 문서에 설명된 대로 레이아웃 템플릿을 계속 테스트하고 사용자가 사용할 수 있도록 합니다.

   * [새 레이아웃 템플릿 테스트](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [레이아웃 템플릿에 대한 관리자 액세스 권한 부여](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [레이아웃 템플릿에 사용자 할당](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>레이아웃 템플릿을 복사하고 복사본을 변경하여 만들 수도 있습니다. 자세한 내용은 [레이아웃 템플릿 복사](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md)를 참조하십시오.

