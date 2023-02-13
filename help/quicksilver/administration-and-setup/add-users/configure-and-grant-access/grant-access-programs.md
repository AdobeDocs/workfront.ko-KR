---
title: 프로그램에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront의 프로그램에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 169f6357-1fbb-43e0-83af-1c4be682ddbf
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# 프로그램에 대한 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

사용자 지정 액세스 수준을 사용하여 Workfront의 다른 개체 유형에 대한 사용자의 액세스를 관리하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 정의 액세스 수준을 사용하여 프로그램에 대한 사용자 액세스 구성

1. 액세스 수준 만들기 또는 편집을 시작합니다. [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 톱니바퀴 아이콘을 클릭합니다 ![](assets/gear-icon-settings.png) on **보기** 또는 **편집** 프로그램 오른쪽의 버튼을 클릭한 다음 아래에서 부여할 기능을 선택합니다 **설정 세부 조정**.

   각 액세스 수준의 사용자가 프로그램으로 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [프로그램](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) 기사 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

   >[!NOTE]
   >
   >특정 유형의 객체에 대한 액세스 레벨 설정을 구성해도 해당 구성은 낮은 등급을 가진 객체에 대한 사용자의 액세스에 영향을 주지 않습니다. 예를 들어 사용자가 액세스 수준에서 프로그램을 삭제하지 못하도록 제한할 수 있지만 프로그램보다 낮은 순위를 갖는 프로젝트를 삭제하지 못하도록 제한하지는 않습니다.객체 계층에 대한 자세한 내용은 섹션을 참조하십시오 [개체의 상호 종속성 및 계층](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 기사 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 다음 문서에 나열된 문서 중 하나를 계속 사용합니다. [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), 예 [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 완료되면 를 클릭합니다 **저장**.

   액세스 수준이 만들어지면 사용자에게 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 라이선스 유형별 프로그램 액세스

각 액세스 수준의 사용자가 프로그램으로 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [프로그램](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) 기사 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 공유 프로그램 액세스

프로그램의 소유자 또는 작성자는 다음에 설명된 대로 다른 사용자에게 권한을 부여하여 다른 사용자와 공유할 수 있습니다 [프로그램 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

개체를 다른 사용자와 공유할 때 개체에 대한 수신자의 권한은 두 가지 항목을 조합하여 결정됩니다.

* 객체에 대해 수신자에게 부여하는 권한
* 개체 유형에 대한 수신자의 액세스 수준 설정입니다
