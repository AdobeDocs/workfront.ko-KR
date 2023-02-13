---
title: Adobe Workfront 라이선스 개요
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 라이선스,유형
navigation-topic: access-levels
description: 조직은 Adobe Workfront을 인수할 때 특정 수의 라이선스를 구매했습니다. Workfront 관리자는 사용자에게 액세스 수준을 할당할 때 4가지 유형의 유료 Workfront 라이센스 중 하나를 각 사용자에게 제공합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f30e2d8-f5c3-4811-b780-49a2b0d058e7
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 2%

---

# Adobe Workfront 라이선스 개요

조직은 Adobe Workfront을 인수할 때 특정 수의 라이선스를 구매했습니다. Workfront 관리자는 사용자에게 액세스 수준을 할당할 때 4가지 유형의 유료 Workfront 라이센스 중 하나를 각 사용자에게 제공합니다.

## Workfront 라이선스 및 액세스 수준 연결 방법

4가지 유형의 유료 Workfront 라이센스를 통해 Workfront에 대한 다양한 수준의 액세스를 사용할 수 있습니다. 각 액세스 수준은 이러한 라이센스 중 하나에 연결됩니다.

Workfront 관리자는 사용자에게 라이센스를 할당하는 대신 해당 라이센스에 첨부된 액세스 수준을 사용자에게 할당합니다.

이 테이블 및 다이어그램은 Workfront에 대한 기본 액세스 수준을 보여줍니다.

| 라이선스 | 연결된 액세스 수준 |
|--- |--- |
| 플랜 | 시스템 관리자, 계획자 |
| 작업 | 보조 |
| 검토 | 검토자 |
| 외부* | 외부 사용자 |

>[!NOTE]
>
>외부 라이센스는 유료 라이센스가 아닙니다. 주로 Workfront을 사용하지 않는 공동 작업자와 문서를 공유하도록 설계되었습니다. 자세한 내용은 [Adobe Workfront의 내장된 액세스 수준](default-access-levels-in-workfront.md).

![](assets/licenses-and-access-levels.png)

## 라이센스에서 액세스 수준을 정의하는 방법

액세스 수준에 첨부된 라이센스는 액세스 수준에서 사용할 수 있는 기능의 전체 범위를 결정합니다.

기본 액세스 수준을 복사하고 필요에 따라 복사본을 사용자 지정할 수 있습니다. 복사된 액세스 수준에 대해 라이센스에서 허용하는 기능 범위 내에서 사용자의 요구 사항에 맞게 액세스 설정을 조정할 수 있습니다.

자세한 내용은 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) 및 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 라이선스 수

사용자에게 액세스 수준을 지정하면 사용 가능한 라이선스 수가 1씩 줄어듭니다.

예를 들어, 사용자에게 계획자 액세스 레벨을 지정하면 사용 가능한 계획 라이센스의 수가 1씩 줄어듭니다.

사용자에게 할당된 라이선스 및 액세스 수준을 볼 수 있습니다. 자세한 내용은 [사용자의 액세스 수준 및 라이선스 나열](../../../administration-and-setup/add-users/access-levels-and-object-permissions/list-access-levels-and-licenses-for-your-users.md).

라이선스 관리에 대한 자세한 내용은 [시스템에서 사용 가능한 라이센스 관리](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
