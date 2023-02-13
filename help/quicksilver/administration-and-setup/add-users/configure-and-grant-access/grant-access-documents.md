---
title: 문서에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront에서 문서에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# 문서에 대한 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

이 액세스는 문서 폴더에도 적용됩니다.

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
   <td> <p>Workfront 관리자여야 합니다.&gt;.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 정의 액세스 수준을 사용하여 문서에 대한 사용자 액세스 구성

1. 액세스 수준 만들기 또는 편집을 시작합니다. [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 톱니바퀴 아이콘을 클릭합니다 ![](assets/gear-icon-settings.png) on **보기** 또는 **편집** 문서 오른쪽에 있는 버튼을 선택한 다음 아래에서 부여할 기능을 선택합니다 **설정 세부 조정**.

   ![document_access.png](assets/document-access.png)

   사용자가 액세스 권한이 있는 프로젝트, 작업 및 문제에 대해 다음을 수행하도록 허용할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">만들기</td> 
      <td>문서를 업로드합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">삭제</td> 
      <td> <p>업로드된 문서를 제거합니다.</p> <p>다음 <b>만들기</b> 이 옵션을 활성화하면 옵션이 자동으로 활성화됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">공유</td> 
      <td>특정 사용자, 작업 역할, 팀과 문서를 공유합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개적으로 문서 공유</td> 
      <td>외부 사용자와 문서를 공유합니다(Workfront 라이센스가 없음).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시스템 전체 공유</td> 
      <td> <p>Workfront 인스턴스의 모든 사용자가 문서를 사용할 수 있도록 합니다.</p> <p>다음과 같은 경우 시스템의 모든 사용자가 이러한 방식으로 공유된 문서를 볼 수 있습니다.</p> 
       <ul> 
        <li> <p>업로드된 문서 페이지로 연결되는 링크를 보냅니다.</p> </li> 
        <li> <p>그들은 Workfront에서 그것을 검색합니다</p> </li> 
       </ul> <p>다음 <b>공유</b> 이 옵션을 활성화하면 옵션이 자동으로 활성화됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >특정 유형의 객체에 대한 액세스 레벨 설정을 구성해도 해당 구성은 낮은 등급을 가진 객체에 대한 사용자의 액세스에 영향을 주지 않습니다. 예를 들어, 사용자가 액세스 수준에서 프로젝트를 삭제하지 못하도록 제한할 수 있지만, 프로젝트 보다 순위가 낮은 문서의 삭제는 제한되지 않습니다.객체 계층에 대한 자세한 내용은 섹션을 참조하십시오 [개체의 상호 종속성 및 계층](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 기사 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (선택 사항) 상위 순위 객체에서 문서에 대한 상속된 권한을 제한하려면 **추가 제한 설정**&#x200B;를 선택하고 을 선택합니다. **프로젝트, 작업, 문제 등에서 문서 액세스를 상속하지 마십시오**.
1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 다음 문서에 나열된 문서 중 하나를 계속 사용합니다. [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), 예 [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 완료되면 를 클릭합니다 **저장**.

   액세스 수준이 만들어지면 사용자에게 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 라이선스 유형별 문서 액세스

각 액세스 수준의 사용자가 문서로 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [문서](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) 기사 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 공유 문서에 대한 액세스

Workfront에 문서를 업로드한 후에는 다음에 설명된 대로 다른 사용자에게 권한을 부여하여 다른 사용자와 문서를 공유할 수 있습니다 [문서 공유](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

개체를 다른 사용자와 공유할 때 개체에 대한 수신자의 권한은 두 가지 항목을 조합하여 결정됩니다.

* 객체에 대해 수신자에게 부여하는 권한
* 개체 유형에 대한 수신자의 액세스 수준 설정입니다
