---
title: 포트폴리오 공유
description: 포트폴리오에 액세스할 수 있는 권한이 있는 경우 다른 사용자와 포트폴리오를 공유할 수 있습니다.
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 포트폴리오 공유

Adobe Workfront 관리자는 액세스 수준을 할당할 때 포트폴리오를 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 포트폴리오를 편집하려면 액세스 권한이 있는 플랜 라이선스가 있어야 합니다. 자세한 내용은 [포트폴리오에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)를 참조하십시오.

권한이 부여된 액세스 수준과 함께 특정 포트폴리오를 사용자와 공유할 수 있는 사용자로부터 보거나 관리할 수 있는 권한을 받을 수도 있습니다. 액세스 수준 및 사용 권한에 대한 자세한 내용은 [액세스 수준 및 사용 권한이 함께 작동하는 방법](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)을 참조하세요.

권한은 Workfront의 한 항목에 한정되며 사용자가 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

## 포트폴리오 공유에 대한 고려 사항

아래 고려 사항 외에 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아닌 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

* 포트폴리오 작성자는 기본적으로 포트폴리오에 대한 관리 권한을 가집니다.
* 포트폴리오를 개별적으로 공유하거나 여러 포트폴리오를 동시에 공유할 수 있습니다. 포트폴리오를 공유하는 것은 Workfront에서 다른 개체를 공유하는 것과 동일합니다. 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.

* Portfolio에 대한 보기 또는 관리 권한만 부여할 수 있습니다.

  ![](assets/screen-shot-2014-01-23-at-12.45.15-pm.png)    ![](assets/screen-shot-2014-01-22-at-10.03.43-am-190x167.png)

* 포트폴리오를 공유하면 기본적으로 사용자는 포트폴리오와 연결된 모든 하위 개체에 대해 동일한 권한을 상속합니다.

  Workfront의 개체 계층 구조에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)를 참조하십시오.

* Portfolio에서 상속된 권한을 제거할 수 있습니다. 개체에서 권한을 제거하는 방법에 대한 자세한 내용은 [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)를 참조하십시오.

## Portfolio 권한

다음 표에는 사용자가 Portfolio을 보거나 관리할 수 있도록 허용할 때 부여할 수 있는 권한이 표시됩니다.

| **작업** | **관리** | **보기** |
|---|---|---|
| Portfolio 세부 정보 편집 | ✓ 덧신 |   |
| Portfolio 보기 | ✓ 덧신 | ✓ 덧신 |
| Portfolio 삭제 | ✓ 덧신 |   |
| 사용자 정의 양식 첨부 | ✓ 덧신 |   |
| 사용자 정의 필드 편집 | ✓ 덧신 |   |
| 프로그램 추가 또는 제거&#42; | ✓ 덧신 |   |
| 프로젝트 추가 또는 제거&#42; | ✓ 덧신 |   |
| 프로젝트 승인 | ✓ 덧신 |   |
| Portfolio 최적화&#42; | ✓ 덧신 |   |
| 문서 폴더 추가&#42; | ✓ 덧신 | ✓ 덧신 |
| 문서 추가 | ✓ 덧신 | ✓ 덧신 |
| 업데이트/주석 | ✓ 덧신 | ✓ 덧신 |
| 공유 | ✓ 덧신 | ✓ 덧신 |
| 시스템 전체 공유 |   | ✓ 덧신 |

*이러한 권한은 액세스 수준 및 프로젝트, 프로그램, 문서 등의 다른 개체에 대한 권한에 의해 제어됩니다.
