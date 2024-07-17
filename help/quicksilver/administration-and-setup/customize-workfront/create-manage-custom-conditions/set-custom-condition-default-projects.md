---
title: 사용자 지정 조건을 프로젝트의 기본값으로 설정
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 프로젝트의 상태 유형이 수동 대신 진행 상태로 설정되어 있는 경우 프로젝트 상태 및 상태 유형 개요에 설명된 대로 Adobe Workfront은 프로젝트 진행 시 프로젝트에 내장된 세 가지 기본 상태(목표 달성, 위험 또는 문제 발생) 중 하나를 자동으로 표시합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 사용자 지정 조건을 프로젝트의 기본값으로 설정

프로젝트의 상태 유형이 [수동]이 아닌 [진행 상태]로 설정되어 있으면 [프로젝트 상태 및 상태 유형 개요](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)에 설명된 대로 Adobe Workfront은 진행할 때 프로젝트에 내장된 세 가지 기본 조건(대상, 위험 또는 문제 발생) 중 하나를 자동으로 표시합니다.

![](assets/condition-in-project-header-nwe.png)

이러한 세 가지 기본 조건을 사용하는 대신 사용자 지정 조건을 기본 조건으로 설정할 수 있습니다. 예를 들어 모든 프로젝트에서 추적 웰 (Tracking Well)로 표시되도록 타겟 상(On Target) 기본 조건을 변경할 수 있습니다.

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 사용자 지정 조건을 모든 프로젝트에 대한 기본 조건으로 설정합니다.

1. Adobe Workfront 오른쪽 상단의 **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **설정** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. **프로젝트 환경 설정** > **조건**&#x200B;을 클릭합니다.

1. **프로젝트** 탭을 클릭합니다.
1. **기본 조건 설정**&#x200B;을 클릭합니다.
1. 변경할 기본 조건 옆에 있는 드롭다운 메뉴에서 대신 사용할 사용자 지정 조건을 클릭합니다.
1. 변경할 다른 기본 조건에 대해 이전 단계를 반복합니다.
1. **저장**&#x200B;을 클릭합니다.

사용자 지정 조건을 작업 및 문제의 기본 조건으로 설정하는 방법에 대한 자세한 내용은 [사용자 지정 조건을 작업 및 문제의 기본값으로 설정](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)을 참조하십시오.

사용자가 수동으로 상태를 업데이트할 수 있도록 프로젝트를 설정하는 방법에 대한 자세한 내용은 [작업 및 문제에 대한 상태 업데이트](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)를 참조하십시오.

사용자 지정 조건에 대한 자세한 내용은 [사용자 지정 조건](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)을 참조하세요.
