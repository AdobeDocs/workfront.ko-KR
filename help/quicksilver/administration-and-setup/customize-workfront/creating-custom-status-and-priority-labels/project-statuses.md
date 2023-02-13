---
title: 시스템 프로젝트 상태 목록에 액세스합니다
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 사용자는 다른 사용자가 프로젝트의 현재 개발 단계를 지정된 시간에 볼 수 있도록 프로젝트 상태를 지정할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# 시스템 프로젝트 상태 목록에 액세스합니다

사용자는 다른 사용자가 프로젝트의 현재 개발 단계를 지정된 시간에 볼 수 있도록 프로젝트 상태를 지정할 수 있습니다.

Workfront에는 9개의 시스템 프로젝트 상태가 포함되어 있습니다. 이러한 상태의 이름을 변경할 수 있지만 삭제할 수는 없습니다.

조직의 요구 사항에 맞게 사용자 지정 프로젝트 상태를 추가할 수도 있습니다.

Workfront 관리자는 시스템의 모든 새 프로젝트에 대한 기본 상태를 구성합니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 프로젝트 상태에 액세스

Workfront 관리자는 시스템 수준 프로젝트 상태 목록에 액세스할 수 있습니다.

시스템 상태 편집 및 사용자 지정 상태 만들기에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

1. 클릭 **프로젝트 환경 설정** > **상태**.

1. 을(를) 클릭합니다. **프로젝트** 탭.

   Workfront에서 사용할 수 있는 프로젝트 상태가 이 탭에 나열됩니다.

   ![](assets/project-status.png)

   기본 제공 시스템 프로젝트 상태에 대한 자세한 내용은 [시스템 프로젝트 상태](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## 사용자 정의 프로젝트 상태 만들기 및 시스템 상태 사용자 정의

Workfront 관리자는 시스템 프로젝트 상태를 Workfront에 추가할 수 있습니다. 그룹 소유자는 하나의 그룹에 해당하는 사용자 지정 상태를 추가할 수 있습니다. 사용자 지정 상태를 만들거나 시스템 상태를 편집하는 방법에 대한 자세한 내용은 다음을 참조하십시오 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

사용자 지정 프로젝트 상태를 생성할 때 항상 새 상태와 기존 시스템 상태가 같아야 합니다. 사용자 지정 상태와 동일한 상태를 확인하려면 시스템 상태의 동작을 이해해야 합니다. 동일한 상태를 선택한 후에는 이 선택을 변경할 수 없습니다. 시스템 프로젝트 상태에 대한 자세한 내용은 [시스템 프로젝트 상태](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
