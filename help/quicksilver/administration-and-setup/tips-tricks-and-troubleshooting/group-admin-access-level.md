---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 그룹 관리자는 자신이 관리하는 사용자보다 높은 액세스 권한을 가져야 합니다.
description: 그룹 관리자의 액세스 권한이 관리하는 액세스 수준보다 낮은 경우 낮은 액세스 수준을 보거나 수정하거나 할당할 수 없습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# 그룹 관리자는 자신이 관리하는 사용자보다 높은 액세스 권한을 가져야 합니다.

그룹 관리자의 액세스 권한이 관리하는 액세스 수준보다 낮은 경우 낮은 액세스 수준을 보거나 수정하거나 할당할 수 없습니다.

## 문제

그룹 관리자에게 팀에 대한 보기 권한이 있는 수정된 계획자 액세스 수준이 할당되지만 특정 사용자에게 팀에 대한 편집 권한이 있는 작업자 액세스 수준이 할당되면 그룹 관리자는 수정된 작업자 액세스 수준과 상호 작용할 수 없습니다.

![그룹 관리자 수정 액세스](assets/group-admin-modified-access.png)


>[!NOTE]
>
>이 논리는 설정 세부 조정 드롭다운 메뉴에도 적용됩니다. 두 액세스 수준 모두 편집 액세스 권한을 가질 수 있지만 그룹 관리자의 경우 설정 세부 조정 드롭다운 메뉴의 설정이 더 높아야 합니다.
> ![설정 미세 조정](assets/fine-tune-your-settings.png)

## 솔루션

그룹 관리자는 액세스 수준의 모든 영역에서 자신이 관리하는 영역보다 더 높은 권한을 가져야 합니다.
