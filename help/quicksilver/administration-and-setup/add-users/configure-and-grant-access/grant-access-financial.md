---
title: 재무 데이터에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 통해 Workfront의 재무 데이터에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 재무 데이터에 대한 액세스 권한 부여

{{highlighted-preview}}

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 사용자의 액세스 수준을 통해 다음에 대한 사용자의 액세스 권한을 정의할 수 있습니다.

* Workfront의 프로젝트에 대한 재무 정보
* 리소스 계획 도구의 리소스 예산 정보

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

## 재무 데이터에 대한 액세스 권한 부여에 대한 고려 사항

사용자에게 Workfront의 재무 데이터에 대한 액세스 권한을 부여할 때 다음 사항을 고려하십시오.

* 액세스 수준이 재무 데이터에 대한 액세스를 허용하지 않는 사용자는 프로젝트에 대한 위험을 만들 수 없습니다. 자세한 내용은 [프로젝트에 대한 위험 만들기 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)을 참조하세요.
* 또한 액세스 레벨을 사용하여 사용자가 자원 할당을 예산 책정하거나 조회하기 위해 사용할 수 있는 자원 관리 활동을 결정할 수 있습니다. 자세한 내용은 [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)를 참조하십시오.

## 사용자 정의 액세스 수준을 사용하여 재무 데이터에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 재무 데이터 오른쪽의 **보기** 또는 **편집** 단추에서 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 클릭한 다음 **설정을 미세 조정**&#x200B;에서 부여할 기능을 선택합니다.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (선택 사항) **관리 액세스 허용** 영역에서 다음 옵션을 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">환율</td> 
      <td> <p>Workfront에서 새 통화를 추가합니다.</p> <p>이 액세스 권한이 없으면 사용자는 자신이 만드는 프로젝트에 기존 통화만 추가할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td> <p>Workfront의 개체에 대한 모든 비용을 봅니다.</p> <p>사용자가 새 경비 유형을 만들 수 없습니다.</p> <p>이 액세스 권한이 없으면 사용자는 다음만 볼 수 있습니다.</p> 
       <ul> 
        <li>관리하는 프로젝트, 작업 또는 문제의 경비</li> 
        <li>자신의 경비</li> 
        <li>부하 직원의 비용</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나(예: [작업에 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md))를 계속 사용하십시오.
1. 완료되면 **저장**&#x200B;을 클릭하세요.

   액세스 수준이 만들어지면 사용자에게 이를 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

## 공유 재무 정보에 대한 액세스

[개체에 대한 재무 권한 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)에 설명된 대로 프로젝트, 작업 또는 문제에 대한 재무 정보를 다른 사용자에게 부여하여 공유할 수 있습니다.

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

다른 사용자와 객체를 공유할 때 객체에 대한 수신자의 권한은 다음 두 가지 사항의 조합으로 결정됩니다.

* 객체에 대해 수신자에게 부여하는 권한
* 개체 유형에 대한 수신자의 액세스 수준 설정입니다.

## 라이선스 유형별 재무 정보 액세스

각 액세스 수준의 사용자가 재무 정보로 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)의 [재무 데이터](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) 섹션을 참조하십시오.

## 다음을 설정하여 재무 정보에 액세스

다음 정보는 액세스 수준 설정을 사용하여 사용자의 재무 데이터에 대한 액세스를 제어하는 방법을 이해하는 데 도움이 됩니다.

### 액세스 권한 없음

재무 데이터에 대한 액세스 권한이 없는 사용자에게는 다음에 대한 액세스 권한이 없습니다.

* 프로젝트 및 작업 객체 아래의 재무 섹션
* 비즈니스 사례
* 청구 요금 및 청구 기록
* <span class="preview">카드 평가</span>
* 사용자 환경 설정의 시간당 비용 및 시간당 청구

  위의 4단계에서 보기 단추의 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 사용하여 구성할 수 있습니다.

* 작업 역할의 시간당 비용 및 시간당 청구

  위의 4단계에서 보기 단추의 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 사용하여 구성할 수 있습니다.

### 액세스 권한 보기

재무 데이터에 대한 보기 액세스 권한이 있는 사용자는 다음을 볼 수 있습니다(편집할 수 없음).

* 프로젝트 및 작업 객체 아래의 재무 섹션
* 비즈니스 사례
* 청구 요금 및 청구 기록
* 사용자 환경 설정의 시간당 비용 및 시간당 청구

  위의 4단계에서 보기 단추의 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 사용하여 구성할 수 있습니다.

* 작업 역할의 시간당 비용 및 시간당 청구

  위의 4단계에서 보기 단추의 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 사용하여 구성할 수 있습니다.

### 액세스 권한 편집

재무 데이터에 대한 편집 액세스 권한이 있는 사용자는 다음을 보고 편집할 수 있습니다.

* 프로젝트 및 작업 객체 아래의 재무 섹션
* 비즈니스 사례
* 청구 요금 및 청구 기록
* <span class="preview">카드 평가</span>
* 사용자 환경 설정의 시간당 비용 및 시간당 청구

  위의 4단계에서 편집 단추의 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 사용하여 구성할 수 있습니다.

* 작업 역할의 시간당 비용 및 시간당 청구

  위의 4단계에서 편집 단추의 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 사용하여 구성할 수 있습니다.
