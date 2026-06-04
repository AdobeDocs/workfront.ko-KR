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
TQID: https://experienceleague.adobe.com/uxZXjgW85JgdyPJA5UEEfIvwU41hLWE-B3XLDh6D89w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 157
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
> ![설정을 미세 조정](assets/fine-tune-your-settings.png)

## 솔루션

그룹 관리자는 액세스 수준의 모든 영역에서 자신이 관리하는 영역보다 더 높은 권한을 가져야 합니다.
