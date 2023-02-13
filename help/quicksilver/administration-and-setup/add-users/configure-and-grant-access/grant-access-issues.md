---
title: 문제에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront에서 문제에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 문제에 대한 액세스 권한 부여

Adobe Workfront 관리자는 다음과 같이 액세스 수준을 사용하여 문제에 대한 사용자의 액세스를 정의할 수 있습니다. [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## 사용자 지정 액세스 수준을 사용하여 문제에 대한 사용자 액세스 권한 부여

1. 액세스 수준 만들기 또는 편집을 시작합니다. [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 톱니바퀴 아이콘을 클릭합니다 ![](assets/gear-icon-settings.png) on **보기** 또는 **편집** 문제 오른쪽에 있는 버튼을 선택한 다음 아래에서 부여할 기능을 선택합니다 **설정 세부 조정**.

1. (선택 사항) 상위 순위 개체에서 문제에 대해 상속된 권한을 제한하려면 **추가 제한 설정**&#x200B;를 선택하고 을 선택합니다. **프로젝트, 작업, 문제 등에서 문서 액세스를 상속하지 마십시오**.

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 다음 문서에 나열된 문서 중 하나를 계속 사용합니다. [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), 예 [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 완료되면 를 클릭합니다 **저장**.

   액세스 수준이 만들어지면 사용자에게 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 라이선스 유형별 문제에 대한 액세스

각 액세스 수준의 사용자가 문제에 대해 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [문제](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues) 기사 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 공유 문제에 대한 액세스

문제의 소유자 또는 작성자는 다음에 설명된 대로 다른 사용자에게 권한을 부여하여 다른 사용자와 공유할 수 있습니다 [문제 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

개체를 다른 사용자와 공유할 때 개체에 대한 수신자의 권한은 두 가지 항목을 조합하여 결정됩니다.

* 객체에 대해 수신자에게 부여하는 권한
* 개체 유형에 대한 수신자의 액세스 수준 설정입니다

또한 액세스 수준에서 허용되는 경우 개체 계층 구조를 통해 문제에 액세스할 수 있습니다. 사용자에게 이미 문제의 상위 프로젝트 또는 작업에 대한 권한이 있는 경우 해당 문제에 대한 권한도 있습니다(위의 3단계 참조). 문제를 공유할 때 권한을 상속한 사용자 목록을 볼 수 있습니다.

![](assets/inherited-permissions.png)
