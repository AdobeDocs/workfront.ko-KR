---
title: 작업 공유
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 작업을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 작업에 대한 액세스 권한 부여에 대한 자세한 내용은 작업에 대한 액세스 권한 부여를 참조하십시오.
author: Courtney
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 7%

---

# 작업 공유

Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 작업을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 작업에 대한 액세스 권한 부여에 대한 자세한 내용은 [작업에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)를 참조하십시오.

사용자에게 부여된 액세스 수준과 함께 공유할 액세스 권한이 있는 특정 작업을 보거나, 기여하거나, 관리할 수 있는 권한을 부여할 수도 있습니다.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.


## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p> 
   <p>작업 이상</p> 
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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 공유 시 고려 사항

아래 고려 사항 외에 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

* 작업 작성자는 기본적으로 해당 작업에 대한 관리 권한을 가집니다.
* 작업을 개별적으로 공유하거나 여러 작업을 한 번에 일괄적으로 공유할 수 있습니다.\
  작업 공유는 다른 오브젝트 공유와 동일합니다. Workfront에서 항목을 공유하는 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.

* 작업에 다음 권한을 부여할 수 있습니다.

   * 보기
   * 관리
   * 참여
* 작업을 공유할 때 기본적으로 사용자는 작업과 연결된 모든 하위 개체에 대해 동일한 권한을 상속합니다. 예를 들어, 하위 작업, 문제 및 작업에 첨부된 문서에 대한 동일한 권한을 상속합니다.\
  Workfront의 개체 계층 구조에 대한 자세한 내용은   [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Workfront 관리자는 문서가 사용자 액세스 수준의 상위 개체에서 권한을 상속해야 하는지 여부를 지정할 수 있습니다. 문서에 대해 상속된 사용 권한을 제한하는 방법에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하십시오.

* 작업에서 상속된 권한을 제거할 수 있습니다.\
  오브젝트에서 상속된 권한을 제거하는 방법에 대한 자세한 내용은   [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 작업 공유 방법

다음과 같은 방법으로 작업을 공유할 수 있습니다.

* 수동으로 개별적으로 또는 대량으로

* 다음을 수행하여 자동으로:

   * 작업의 상위 개체(프로젝트, 프로그램 또는 포트폴리오)에 대한 권한을 지정합니다. 작업은 상위 개체에서 권한을 상속합니다. 개체에 상속된 사용 권한을 보는 방법에 대한 자세한 내용은 [개체에 상속된 사용 권한 보기](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)를 참조하십시오.
   * 작업이 있는 프로젝트를 만드는 데 사용되는 템플릿에 대한 프로젝트 공유에 엔티티를 추가합니다. 템플릿에서 프로젝트를 공유하는 방법에 대한 자세한 내용은 [템플릿 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)를 참조하십시오.

   * 프로젝트를 편집할 때 프로젝트의 모든 작업에 대한 권한을 지정합니다.  프로젝트에 대한 사용자의 권한에 따라 프로젝트의 작업에 대한 액세스를 관리하는 방법에 대한 자세한 내용은 문서 [](../../manage-work/projects/manage-projects/edit-projects.md#access)프로젝트 편집[의 ](../../manage-work/projects/manage-projects/edit-projects.md) 섹션을 참조하십시오.

  >[!TIP]
  >
  >사용자가 프로젝트의 작업에 할당되었을 때 사용자에게 부여할 작업 권한을 지정하지 않으면 기본적으로 해당 사용자에게는 프로젝트에서 가지고 있는 권한과 동일한 권한이 부여됩니다.

## 작업 공유

1. 공유할 작업으로 이동합니다.

1. 작업 이름 오른쪽에서 **공유**&#x200B;를 클릭합니다. **작업 이름 [공유]** 대화 상자가 열립니다.

   ![작업 공유 단추](assets/share-task-button.png)

1. **작업 액세스 권한 부여** 필드에서 작업을 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 해당 이름을 클릭합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 작업을 공유할 수 있습니다.


1. (선택 사항) **액세스 권한이 있는 사용자** 드롭다운을 선택하고 작업의 액세스 수준을 선택합니다.

   * **초대된 사용자만 액세스할 수 있습니다.** 작업에 초대된 사용자만 액세스할 수 있습니다(기본값).
   * **시스템의 모든 사용자가 볼 수 있습니다**: 시스템의 모든 사용자는 초대장 없이 작업을 볼 수 있습니다.

1. 사용자 이름 오른쪽에 있는 드롭다운을 클릭하고 이 작업에 대한 권한 수준을 선택합니다.

   * **보기**: 사용자가 작업을 검토하고 공유할 수 있습니다.
   * **참여**: 사용자는 업데이트를 수행하고, 정보를 기록하며, 약간의 편집을 수행하고, 작업을 공유할 수 있습니다(모든 보기 권한도 포함).
   * **관리**: 사용자가 액세스 수준에서 부여된 관리 권한 없이 작업에 대한 전체 액세스 권한을 가지고 있습니다(모든 보기 및 기여 권한도 포함).

1. (선택 사항) 작업에 대한 특정 권한을 구성하기 위해 부여한 권한 수준 옆에 있는 고급 옵션 아이콘을 클릭합니다.

   ![구성된 고급 권한 옵션](assets/advanced-permission-options.png)

1. (선택 사항) 작업의 자식 개체에 대해 상속된 사용 권한을 끄려면 **상속된 사용 권한**&#x200B;과(와) 함께 **끄기** 인라인을 클릭합니다.

1. (선택 사항) 링크를 사용하여 작업을 빠르게 공유하려면 **링크 복사**&#x200B;를 클릭한 다음 받는 사람에게 전달하십시오.

1. **저장**&#x200B;을 클릭합니다.


## 일괄 작업 공유

1. 공유할 작업이 포함된 프로젝트로 이동합니다.

1. 프로젝트 페이지의 **작업** 탭에서 공유할 각 작업의 왼쪽에 있는 상자를 선택한 다음 페이지 상단에 있는 **공유** 아이콘 ![공유 아이콘](assets/share-icon.png)을 클릭합니다. 공유 모달이 열립니다.

   ![일괄 공유 작업](assets/bulk-share-tasks.png)

1. **작업 액세스 권한 부여** 필드에서 작업을 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 해당 이름을 클릭합니다.

   >[!TIP]
   >
   >활성 사용자, 팀, 역할 또는 회사와만 작업을 공유할 수 있습니다.


1. (선택 사항) **액세스 권한이 있는 사용자** 드롭다운을 선택하고 작업의 액세스 수준을 선택합니다.

   * **초대된 사용자만 액세스할 수 있습니다.** 작업에 초대된 사용자만 액세스할 수 있습니다(기본값).
   * **시스템의 모든 사용자가 볼 수 있습니다**: 시스템의 모든 사용자는 초대장 없이 작업을 볼 수 있습니다.


1. 사용자 이름 오른쪽에 있는 드롭다운을 클릭하고 작업에 대한 권한 수준을 선택합니다.

   * **보기**: 사용자가 작업을 검토하고 공유할 수 있습니다.
   * **참여**: 사용자는 업데이트를 수행하고, 정보를 기록하며, 약간의 편집을 수행하고, 작업을 공유할 수 있습니다(모든 보기 권한도 포함).
   * **관리**: 사용자는 액세스 수준에서 부여된 관리 권한 없이 작업에 대한 전체 액세스 권한을 가집니다(모든 보기 및 기여 권한도 포함).

1. (선택 사항) 작업에 대한 특정 권한을 구성하기 위해 부여한 권한 수준 옆에 있는 고급 옵션 아이콘을 클릭합니다.

   ![구성된 고급 권한 옵션](assets/advanced-permission-options.png)

1. **저장**&#x200B;을 클릭합니다.

## 작업 권한

다음 표에는 사용자에게 작업을 보기, 기여 또는 관리할 수 있도록 허용할 때 부여할 수 있는 권한이 표시됩니다.

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>작업</strong> </th> 
   <th><strong>관리</strong> </th> 
   <th><strong>참여</strong> </th> 
   <th><strong>보기</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">작업 추가</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">전임 작업 추가</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">문제 추가</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">작업 삭제</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>일반 작업 편집<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 상태 변경</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 제한 사항 편집</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">문서 추가</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">작업 복사*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">작업 이동*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">시간 기록</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">계획된 일자 수정</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">할당 수락</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">할당하기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 양식 첨부</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 필드 편집</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">승인 프로세스 만들기</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 승인</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">재무 편집*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">경비 추가/편집</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td scope="row">재무 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">업데이트/주석</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">공유</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">시스템 전체 공유</td> 
   <td>  </td> 
   <td>  </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;액세스 수준 및 프로젝트에 대한 권한으로 제어됩니다.
