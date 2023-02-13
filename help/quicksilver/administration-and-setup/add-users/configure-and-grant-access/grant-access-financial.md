---
title: 재무 데이터에 대한 액세스 권한 부여
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 관리자는 액세스 수준을 통해 Workfront에서 재무 데이터에 대한 사용자의 액세스를 정의할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# 재무 데이터에 대한 액세스 권한 부여

Adobe Workfront 관리자는 다음에 설명된 대로 사용자의 액세스 수준을 통해 다음에 대한 사용자의 액세스를 정의할 수 있습니다. [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Workfront의 프로젝트 재무 정보
* Resource Planning 도구의 자원 예산 책정 정보

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

## 재무 데이터에 대한 액세스 권한을 부여하기 위한 고려 사항

Workfront에서 재무 데이터에 대한 액세스 권한을 사용자에게 부여할 때 다음 사항을 고려하십시오.

* 액세스 수준이 재무 데이터에 대한 액세스를 허용하지 않는 사용자는 프로젝트에 대한 위험을 만들 수 없습니다. 자세한 내용은 [프로젝트에서 위험 요소 생성 및 편집](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* 액세스 레벨을 사용하여 사용자가 자원 할당을 예산 또는 조회하기 위해 사용할 수 있는 자원 관리 활동을 결정할 수도 있습니다. 자세한 내용은 [리소스 관리에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## 사용자 지정 액세스 수준을 사용하여 재무 데이터에 대한 사용자 액세스 구성

1. 액세스 수준 만들기 또는 편집을 시작합니다. [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 톱니바퀴 아이콘을 클릭합니다 ![](assets/gear-icon-settings.png) on **보기** 또는 **편집** 재무 데이터 오른쪽의 버튼을 선택한 다음, **설정 세부 조정**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (선택 사항)에서 **에 대한 관리자 액세스 허용** 영역에서 다음 옵션을 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">환율</td> 
      <td> <p>Workfront에서 새 통화를 추가합니다.</p> <p>이 액세스 권한이 없으면 사용자는 기존 통화를 자신이 만드는 프로젝트에만 추가할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">경비</td> 
      <td> <p>Workfront의 개체에 대한 모든 비용을 봅니다.</p> <p>사용자가 새 비용 유형을 생성할 수 없습니다.</p> <p>이 액세스 권한이 없으면 사용자는 다음을 볼 수만 있습니다.</p> 
       <ul> 
        <li>관리하는 프로젝트, 작업 또는 문제에 대한 비용</li> 
        <li>그들 자신의 비용</li> 
        <li>부하의 경비</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 다음 문서에 나열된 문서 중 하나를 계속 사용합니다. [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) 예 [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. 완료되면 를 클릭합니다 **저장**.

   액세스 수준이 만들어지면 사용자에게 할당할 수 있습니다. 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 공유 재무 정보에 대한 액세스

에 설명된 대로 프로젝트, 작업 또는 다른 사용자에게 권한을 부여하여 프로젝트, 작업 또는 문제에 대한 재무 정보를 공유할 수 있습니다. [개체에 대한 재무 권한 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

개체를 다른 사용자와 공유할 때 개체에 대한 수신자의 권한은 두 가지 항목을 조합하여 결정됩니다.

* 객체에 대해 수신자에게 부여하는 권한
* 개체 유형에 대한 수신자의 액세스 수준 설정입니다

## 라이선스 유형별 재무 정보 액세스

각 액세스 수준의 사용자가 재무 정보로 수행할 수 있는 작업에 대한 자세한 내용은 섹션을 참조하십시오 [재무 데이터](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) 기사 [각 객체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 다음을 설정하여 재무 정보에 액세스

다음 정보는 액세스 수준 설정을 사용하여 사용자의 재무 데이터 액세스를 제어하는 방법을 이해하는 데 도움이 될 수 있습니다.

### 액세스 권한 없음

재무 데이터에 액세스할 수 없는 사용자는 다음에 액세스할 수 없습니다.

* 프로젝트 및 작업 객체의 재무 섹션
* 비즈니스 사례
* 청구 비율 및 청구 레코드
* 사용자 환경 설정에 따른 시간당 비용 및 시간당 청구

   톱니바퀴 아이콘을 사용하여 구성할 수 있습니다 ![](assets/gear-icon-settings.png) 를 클릭합니다.

* Job 역할에 대한 시간당 비용 및 시간당 청구

   톱니바퀴 아이콘을 사용하여 구성할 수 있습니다 ![](assets/gear-icon-settings.png) 를 클릭합니다.

### 액세스 권한 보기

재무 데이터에 대한 보기 액세스 권한이 있는 사용자는 다음을 보고(편집할 수 없음)

* 프로젝트 및 작업 객체의 재무 섹션
* 비즈니스 사례
* 청구 비율 및 청구 레코드
* 사용자 환경 설정에 따른 시간당 비용 및 시간당 청구

   톱니바퀴 아이콘을 사용하여 구성할 수 있습니다 ![](assets/gear-icon-settings.png) 를 클릭합니다.

* Job 역할에 대한 시간당 비용 및 시간당 청구

   톱니바퀴 아이콘을 사용하여 구성할 수 있습니다 ![](assets/gear-icon-settings.png) 를 클릭합니다.

### 액세스 편집

재무 데이터에 대한 편집 액세스 권한이 있는 사용자는 다음을 보고 편집할 수 있습니다.

* 프로젝트 및 작업 객체의 재무 섹션
* 비즈니스 사례
* 청구 비율 및 청구 레코드
* 사용자 환경 설정에 따른 시간당 비용 및 시간당 청구

   톱니바퀴 아이콘을 사용하여 구성할 수 있습니다 ![](assets/gear-icon-settings.png) 위의 4단계에서 편집 단추를 클릭합니다.

* Job 역할에 대한 시간당 비용 및 시간당 청구

   톱니바퀴 아이콘을 사용하여 구성할 수 있습니다 ![](assets/gear-icon-settings.png) 위의 4단계에서 편집 단추를 클릭합니다.
