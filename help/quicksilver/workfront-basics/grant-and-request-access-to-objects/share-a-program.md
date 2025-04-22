---
title: 프로그램 공유
product-area: projects
keywords: 공유,프로그램,권한
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 액세스 수준을 할당할 때 사용자에게 프로그램을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 프로그램 편집에 액세스하려면 플랜 라이선스가 있어야 합니다.
author: Courtney
feature: Get Started with Workfront
exl-id: bfa6ce97-24ad-44b3-9c2f-7fac6b748f94
source-git-commit: fcf6165c9c641316c701d92af2e39294a9fe0123
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# 프로그램 공유


Adobe Workfront 관리자는 액세스 수준을 할당할 때 사용자에게 프로그램을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 프로그램 편집에 액세스하려면 플랜 라이선스가 있어야 합니다. 자세한 내용은 [프로그램에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)를 참조하십시오.

귀하에게 부여된 액세스 수준과 함께, 귀하와 특정 프로그램을 공유할 수 있는 사용자로부터 특정 프로그램을 보거나 관리할 수 있는 권한을 받을 수도 있습니다. 액세스 수준 및 사용 권한에 대한 자세한 내용은 [액세스 수준 및 사용 권한이 함께 작동하는 방법](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)을 참조하세요.

권한은 Workfront의 각 항목에 따라 다르며, 사용자가 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.


## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

객체를 공유하려면 다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>새로운 기능: 표준</p> 
   또는
   <p>현재: 작업 시간 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>공유할 개체에 대한 액세스 이상의 보기</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>공유할 개체에 대한 권한 이상 보기</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로그램 공유에 대한 고려 사항

아래 고려 사항 외에 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아닌 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

* 프로그램 작성자는 기본적으로 프로그램에 대한 관리 권한을 가집니다.

* 프로그램을 개별적으로 공유하거나 여러 프로그램을 한 번에 공유할 수 있습니다.

  Workfront에서 항목을 공유하는 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.

* 프로그램에 대한 보기 또는 관리 권한만 부여할 수 있습니다.

* 프로그램을 공유하면 기본적으로 사용자는 프로그램과 연결된 모든 자식 개체에 대해 동일한 권한을 상속합니다.

  Workfront의 개체 계층 구조에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)를 참조하십시오.

* 프로그램에서 상속된 권한을 제거할 수 있습니다. 개체에서 권한을 제거하는 방법에 대한 자세한 내용은  [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 프로그램 공유

{{step1-to-programs}}

1. **프로그램** 페이지에서 공유할 프로그램을 선택합니다. 프로그램 페이지가 열립니다.

1. 프로그램 이름 오른쪽에서 **공유**&#x200B;를 클릭합니다. **[프로그램 이름 공유]** 대화 상자가 열립니다.

   ![프로그램 공유 단추](assets/share-program-button.png)

1. **프로그램 액세스 권한 부여** 필드에서 프로그램을 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 해당 이름을 클릭합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 프로그램을 공유할 수 있습니다.


1. (선택 사항) **액세스 권한이 있는 사용자** 드롭다운을 선택하고 프로그램의 액세스 수준을 선택합니다.

   * **초대된 사용자만 액세스할 수 있습니다.** 프로그램에 초대된 사용자만 액세스할 수 있습니다(기본값).
   * **시스템의 모든 사용자가 볼 수 있습니다**: 시스템의 모든 사용자는 초대장 없이 프로그램을 볼 수 있습니다.


1. 사용자 이름 오른쪽에 있는 드롭다운을 클릭하고 이 프로그램에 대한 권한 수준을 선택합니다.

   * **보기**: 사용자가 프로그램을 검토하고 공유할 수 있습니다.
   * **관리**: 사용자가 액세스 수준에서 부여된 관리 권한 없이 프로그램에 대한 전체 액세스 권한을 가지고 있습니다(모든 보기 권한도 포함).

1. (선택 사항) 프로그램에 대한 특정 권한을 구성하기 위해 부여한 권한 수준 옆에 있는 고급 옵션 아이콘을 클릭합니다.

   ![구성된 고급 권한 옵션](assets/advanced-options-icon.png)

1. (선택 사항) 프로그램의 자식 개체에 대해 상속된 사용 권한을 해제하려면 **상속된 사용 권한**&#x200B;과(와) 함께 **해제**&#x200B;를 클릭하십시오.

1. (선택 사항) 링크를 사용하여 프로그램을 빠르게 공유하려면 **링크 복사**&#x200B;를 클릭한 다음 받는 사람에게 전달하십시오.

1. **저장**&#x200B;을 클릭합니다.

## 프로그램 일괄 공유

{{step1-to-programs}}

1. **프로그램** 페이지에서 공유할 각 프로그램의 왼쪽에 있는 상자를 선택한 다음 페이지 상단의 **공유** 아이콘 ![공유 아이콘](assets/share-icon.png)을 클릭합니다. 공유 모달이 열립니다.

   ![프로그램 일괄 공유](assets/bulk-share-programs.png)

1. **프로그램 액세스 권한 부여** 필드에서 프로그램을 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 해당 이름을 클릭합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 프로그램을 공유할 수 있습니다.


1. (선택 사항) **액세스 권한이 있는 사용자** 드롭다운을 선택하고 프로그램의 액세스 수준을 선택합니다.

   * **초대된 사용자만 액세스할 수 있습니다.** 프로그램에 초대된 사용자만 액세스할 수 있습니다(기본값).
   * **시스템의 모든 사용자가 볼 수 있습니다**: 시스템의 모든 사용자는 초대장 없이 프로그램을 볼 수 있습니다.


1. 사용자 이름 오른쪽에 있는 드롭다운을 클릭하고 프로그램에 대한 권한 수준을 선택합니다.

   * **보기**: 사용자가 프로그램을 검토하고 공유할 수 있습니다.
   * **관리**: 사용자가 액세스 수준에서 부여된 관리 권한 없이 프로그램에 대한 전체 액세스 권한을 가지고 있습니다(모든 보기 권한도 포함).

1. (선택 사항) 프로그램에 대한 특정 권한을 구성하기 위해 부여한 권한 수준 옆에 있는 고급 옵션 아이콘을 클릭합니다.

   ![구성된 고급 권한 옵션](assets/advanced-options-icon.png)

1. **저장**&#x200B;을 클릭합니다.

## 프로그램 권한

다음 표에는 사용자가 프로그램을 보거나 관리할 수 있도록 허용할 때 부여할 수 있는 권한이 표시됩니다.

| **작업** | **관리** | **보기** |
|---|---|---|
| 프로그램 세부 정보 편집 | ✓ |   |
| 프로그램 보기 | ✓ | ✓ |
| 프로그램 삭제 | ✓ |   |
| 사용자 정의 양식 첨부 | ✓ |   |
| 사용자 정의 필드 편집 | ✓ |   |
| 프로젝트 추가 또는 제거&#42; | ✓ |   |
| 프로젝트 승인 | ✓ |   |
| 문서 폴더 추가&#42; | ✓ | ✓ |
| 문서 추가 | ✓ | ✓ |
| 업데이트/주석 추가 | ✓ | ✓ |
| 공유 | ✓ | ✓ |
| 시스템 전체 공유 |   | ✓ |

*이러한 권한은 액세스 수준 및 프로젝트와 같은 다른 오브젝트에 대한 권한에 의해 제어됩니다.


