---
title: 시스템 프로젝트 상태 목록 액세스
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 사용자는 다른 사용자가 주어진 시간에 프로젝트의 현재 개발 단계를 볼 수 있도록 프로젝트 상태를 지정할 수 있습니다.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# 시스템 프로젝트 상태 목록 액세스

사용자는 다른 사용자가 주어진 시간에 프로젝트의 현재 개발 단계를 볼 수 있도록 프로젝트 상태를 지정할 수 있습니다.

Workfront에는 9개의 시스템 프로젝트 상태가 있습니다. 이러한 상태의 이름은 변경할 수 있지만 삭제할 수는 없습니다.

조직의 요구 사항에 맞게 사용자 정의 프로젝트 상태를 추가할 수도 있습니다.

Workfront 관리자는 시스템의 모든 새 프로젝트에 대한 기본 상태를 구성합니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

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
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>시스템 관리자</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 상태 액세스

Workfront 관리자는 시스템 수준 프로젝트 상태 목록에 액세스할 수 있습니다.

시스템 상태를 편집하고 사용자 지정 상태를 만드는 방법에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.

{{step-1-to-setup}}

1. **프로젝트 환경 설정** > **상태**&#x200B;를 클릭합니다.

1. **프로젝트** 탭을 클릭합니다.

   Workfront에서 사용할 수 있는 프로젝트 상태가 이 탭에 나열됩니다.

   ![프로젝트 상태](assets/project-status.png)

   각 기본 제공 시스템 프로젝트 상태에 대한 자세한 내용은 [시스템 프로젝트 상태 개요](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md)를 참조하십시오.

## 사용자 정의 프로젝트 상태 만들기 및 시스템 상태 사용자 정의

Workfront 관리자는 Workfront에 시스템 프로젝트 상태를 추가할 수 있습니다. 그룹 소유자는 한 그룹에 고유한 사용자 지정 상태를 추가할 수 있습니다. 사용자 지정 상태를 만들거나 시스템 상태를 편집하는 방법에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.

사용자 지정 프로젝트 상태를 만들 때 항상 새 상태와 기존 시스템 상태를 동일시해야 합니다. 사용자 지정 상태와 동일시하기 적합한 상태를 알려면 시스템 상태의 동작을 이해해야 합니다. 동등한 상태를 선택한 후에는 이 선택을 변경할 수 없습니다. 시스템 프로젝트 상태에 대한 자세한 내용은 [시스템 프로젝트 상태 개요](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md)를 참조하십시오.
