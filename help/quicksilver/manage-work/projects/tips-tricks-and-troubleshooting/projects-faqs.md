---
title: 프로젝트 FAQ
description: 프로젝트 FAQ
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# 프로젝트 FAQ

프로젝트에 대한 FAQ는 다음과 같습니다.

## 작업 목록에서 작업을 마우스 오른쪽 단추로 클릭할 때 위에 작업 삽입/아래에 작업이 없는 이유는 무엇입니까?

### 답변

삽입 옵션을 사용하려면 작업 목록을 번호별로 정렬해야 합니다. 열을 번호별로 정렬하려면 **#** 의 왼쪽에 있는 열 헤더에서 **작업 이름** 번호를 기준으로 작업을 선택합니다.

## 실제 완료 날짜는 언제입니까?

### 답변

실제 완료 일자는 작업이 완료된 날짜와 시간을 나타냅니다. 자세한 내용은 [프로젝트 실제 완료 일자 개요](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## 들여쓰기/내어쓰기 단추가 없는 이유는 무엇입니까?

### 답변

들여쓰기/내어쓰기 단추를 사용하려면 작업이 작업 번호별로 정렬되며 적용된 그룹화가 없는지 확인합니다.

## 프로젝트 상태를 완료로 변경할 수 없는 이유는 무엇입니까?

프로젝트 완료로 표시하려고 하면 다음 오류 메시지가 표시됩니다.

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### 답변

프로젝트에 다음 중 하나가 있는 경우 프로젝트 상태를 완료로 변경할 수 없습니다.

* 완료되지 않은 작업 또는 문제
* 승인 보류 중인 상태의 작업 또는 문제

## 프로젝트 상태를 완료에서 현재로 변경할 수 없는 이유는 무엇입니까?

### 답변

프로젝트에 완료 모드가 자동으로 설정되어 있는 경우, 모든 작업과 문제가 완료되면 프로젝트의 상태가 자동으로 완료로 바뀌고 다른 상태로 수정할 수 없습니다. 전체 프로젝트를 현재(Current)로 전환하려면 프로젝트의 완료 모드(Completion Mode)를 수동(Manual)으로 설정해야 합니다. 자세한 내용은 [프로젝트 상태는 완료에서 현재 상태로 변경되지 않습니다](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## 올바른 권한이 있지만 Portfolio에 프로젝트를 추가할 수 없는 이유는 무엇입니까?

올바른 권한이 있지만 Portfolio의 프로젝트 탭에서 프로젝트 추가 단추가 누락됩니다.

### 답변

Portfolio 상태가 비활성으로 인해 발생합니다. Portfolio 상태를 변경하려면

1. 클릭 **Portfolio 세부 사항 > 개요**.
1. 변경 **상태** to **활성.**

1. **저장**&#x200B;을 클릭합니다.\
   다음 **프로젝트 추가** 이제 버튼이 **프로젝트** 탭.

## 프로젝트에 추가될 때 리소스 관리자가 받는 액세스 권한은 무엇입니까?

### 답변

리소스 관리자는 프로젝트에 대한 액세스 관리를 자동으로 받습니다. 리소스 관리자 역할에서 사용자를 제거해도 공유 관리 액세스가 제거되지 않습니다.

## 그룹을 추가할 때 프로젝트 상태가 변경되는 이유는 무엇입니까?

### 답변

그룹의 기본 상태 때문에 프로젝트 상태가 변경됩니다. 프로젝트에 그룹을 추가하면 상태 목록이 그룹에 대해 설정된 기본 상태로 변경됩니다.

자세한 내용은 문서를 참조하십시오 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## 예산 상태란 무엇입니까?

### 답변

예산 상태는 프로젝트가 현재 능력 계획자에 추가되었는지 여부 및 예산 계산이 완료되었는지 여부를 표시합니다.

다음은 예산 상태입니다.

* 포함되지 않음 - 프로젝트가 능력 계획자에 추가되지 않습니다.
* 포함되지만 계산되지 않음 - 프로젝트가 능력 계획자에 추가되지만 예산 계산에서 제외됩니다.
* 포함 및 계산 - 프로젝트가 능력 계획자에 추가되고 예산 계산에 포함됩니다.

## 내가 소유자이며 팀과 관리 권한이 있는 프로젝트를 공유할 수 없는 이유는 무엇입니까? 프로젝트의 공유 대화 상자에서 팀을 찾을 수 없습니다.

### 답변

Adobe Workfront 관리자는 액세스 수준에서 사용자가 속한 회사, 그룹 및 팀만 볼 수 있도록 제한했습니다. 찾고 있는 팀은 사용자가 속한 팀 중 하나가 아닙니다.

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

사용자가 시스템의 모든 팀을 볼 수 있도록 하는 방법에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
