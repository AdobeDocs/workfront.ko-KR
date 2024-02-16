---
title: 포트폴리오 액세스 권한 부여
user-type: administrator
product-area: system-administration;portfolios
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront의 포트폴리오에 대한 사용자의 액세스 권한을 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f4a9c4f3-8ed4-4629-aced-9cc09b8acd3f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# 포트폴리오 액세스 권한 부여

Adobe Workfront 관리자는에 설명된 대로 액세스 수준을 사용하여 포트폴리오에 대한 사용자의 액세스를 정의할 수 있습니다 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 정의 액세스 수준을 사용하여 포트폴리오에 대한 사용자 액세스 구성

1. 에 설명된 대로 액세스 수준 만들기 또는 편집을 시작합니다. [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 톱니바퀴 아이콘 클릭 ![](assets/gear-icon-settings.png) 다음에 있음 **보기** 또는 **편집** Portfolio 오른쪽에 있는 버튼을 클릭한 다음 아래에 부여할 기능을 선택합니다 **설정 미세 조정**.

   ![](assets/fine-tune-portfolios.png)

   >[!NOTE]
   >
   >특정 객체 유형에 대한 액세스 수준 설정을 구성할 때 해당 구성은 하위 등급 객체에 대한 사용자의 액세스 권한에 영향을 주지 않습니다. 예를 들어 사용자가 자신의 액세스 수준에서 포트폴리오를 삭제하지 못하도록 제한할 수 있지만 그렇다고 해서 포트폴리오보다 순위가 낮은 프로젝트를 삭제하는 것은 제한하지 않습니다.객체 계층에 대한 자세한 내용은 섹션을 참조하십시오 [객체의 상호 의존성 및 계층](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 이 문서에서 [Adobe Workfront의 오브젝트 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (선택 사항) 작업 중인 액세스 수준의 다른 오브젝트 및 영역에 대한 액세스 설정을 구성하려면 다음 문서 중 하나를 사용하여 계속합니다. [Adobe Workfront 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), 예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 작업을 마치면 를 클릭합니다. **저장**.

   액세스 수준이 만들어지면 사용자에게 이를 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 라이선스 유형별 포트폴리오 액세스

각 액세스 수준의 사용자가 포트폴리오를 사용하여 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [Portfolio](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#portfoli) 이 문서에서 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 공유 포트폴리오에 액세스

포트폴리오의 소유자 또는 작성자는에 설명된 대로 다른 사용자에게 권한을 부여하여 다른 사용자와 공유할 수 있습니다 [포트폴리오 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

다른 사용자와 객체를 공유할 때 객체에 대한 수신자의 권한은 다음 두 가지 사항의 조합으로 결정됩니다.

* 객체에 대해 수신자에게 부여하는 권한
* 개체 유형에 대한 수신자의 액세스 수준 설정입니다.

사용자가 포트폴리오를 공유할 때 포트폴리오에 부여할 수 있는 권한에 대한 자세한 내용은 [포트폴리오 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).
