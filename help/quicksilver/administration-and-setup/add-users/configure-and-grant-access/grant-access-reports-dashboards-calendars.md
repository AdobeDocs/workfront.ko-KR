---
title: 보고서, 대시보드 및 캘린더에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront에서 보고서, 대시보드 및 캘린더에 대한 사용자의 액세스 권한을 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# 보고서, 대시보드 및 캘린더에 대한 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 액세스 수준을 사용하여 보고서, 대시보드 및 캘린더에 대한 사용자의 액세스 권한을 정의할 수 있습니다.

이 액세스에는 외부 페이지에 대한 액세스도 포함됩니다. 외부 페이지에 대한 자세한 내용은 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)를 참조하십시오.

>[!NOTE]
>
>* 사용자에게 보고서, 대시보드 및 캘린더에 대한 액세스 권한을 부여하려면 해당 사용자에게 필터, 보기 및 그룹화에도 액세스 권한을 부여해야 합니다. 지침은 [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)를 참조하십시오.
>* 누군가 다른 사용자와 보고서, 대시보드 또는 캘린더를 공유할 때 이에 대한 받는 사람의 권한은 두 가지 사항의 조합으로 결정됩니다. 보고서, 대시보드 및 캘린더에 대한 받는 사람의 액세스 수준 설정 _및_ 공유자가 보고서, 대시보드 또는 캘린더에 대해 부여한 모든 권한
>
>사용자가 보고서, 대시보드 또는 캘린더를 공유할 때 부여할 수 있는 권한에 대한 자세한 내용은 [보고서, 대시보드 및 캘린더 공유](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)를 참조하십시오.

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 정의 액세스 수준을 사용하여 보고서, 대시보드 및 달력에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 보고서 오른쪽의 **보기** 또는 **편집** 단추에서 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 클릭한 다음 **설정을 미세 조정**&#x200B;에서 부여할 기능을 선택합니다.

   ![reports_access.png](assets/reports-access.png)

   기본적으로 다음 옵션이 활성화되어 있습니다.

   * **만들기**
   * **삭제**
   * **기본 제공 보고서 보기**: Workfront에서 빌드한 보고서를 보려면 이 항목을 선택해야 합니다.
   * **공유**
   * **공개적으로 보고서 공유**: Workfront 계정이 없는 사용자와 보고서에 대한 공개 링크를 공유하여 보고서를 공개적으로 공유할 수 있습니다. 이 수준의 공유를 허용하려면 이 옵션을 선택해야 합니다.
   * **시스템 전체 공유**: Workfront 라이선스가 있는 시스템의 모든 사용자와 보고서를 공유할 수 있습니다. 이 수준의 공유를 허용하려면 이 옵션을 선택해야 합니다.

     보고서, 대시보드 및 캘린더 공유에 대한 자세한 내용은 [보고서, 대시보드 및 캘린더 공유](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)를 참조하십시오.

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나를 계속 사용하십시오(예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)).
1. 완료되면 **저장**&#x200B;을 클릭하세요.

   액세스 수준이 만들어지면 사용자에게 이를 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

## 라이선스 유형별 보고서, 대시보드 및 달력에 액세스

각 액세스 수준의 사용자가 문제에 대해 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)의 [보고서](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) 섹션을 참조하십시오.

## 공유 보고서, 대시보드 및 캘린더에 액세스

보고서, 대시보드 또는 캘린더의 소유자 또는 작성자는 [보고서, 대시보드 및 캘린더 공유](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)에 설명된 대로 보고서, 대시보드 또는 캘린더에 대한 권한을 부여하여 다른 사용자와 공유할 수 있습니다.

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
