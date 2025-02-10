---
title: 작업 공유
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 작업을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 작업에 대한 액세스 권한 부여에 대한 자세한 내용은 작업에 대한 액세스 권한 부여를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: b4e90918c5f499638d0cf5355dc75c3ceca48293
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 2%

---

# 작업 공유

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>


Adobe Workfront 관리자는 사용자가 액세스 수준을 할당할 때 작업을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 작업에 대한 액세스 권한 부여에 대한 자세한 내용은 [작업에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)를 참조하십시오.

사용자에게 부여된 액세스 수준과 함께 공유할 액세스 권한이 있는 특정 작업을 보거나, Contribute 또는 관리할 수 있는 권한을 부여할 수도 있습니다.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

## 작업 공유 시 고려 사항

아래 고려 사항 외에 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

* 작업 작성자는 기본적으로 작업에 대한 관리 권한을 가집니다.
* 작업을 개별적으로 공유하거나 여러 작업을 한 번에 일괄적으로 공유할 수 있습니다.\
  작업 공유는 다른 오브젝트 공유와 동일합니다. Workfront에서 항목을 공유하는 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.

* 작업에 다음 권한을 부여할 수 있습니다. 

   * 보기
   * 관리
   * 참여\
     ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

     <span class="preview">미리 보기 중:
     ![](assets/task-permissons.png)
  </span>

* 작업을 공유할 때 기본적으로 사용자는 작업과 연결된 모든 하위 개체에 대해 동일한 권한을 상속합니다. 예를 들어, 하위 작업, 문제 및 작업에 첨부된 문서에 대한 동일한 권한을 상속합니다.\
  Workfront의 개체 계층 구조에 대한 자세한 내용은  [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Workfront 관리자는 문서가 사용자 액세스 수준의 상위 개체에서 권한을 상속해야 하는지 여부를 지정할 수 있습니다. 문서에 대해 상속된 사용 권한을 제한하는 방법에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하십시오.

* 작업에서 상속된 권한을 제거할 수 있습니다.\
  오브젝트에서 상속된 권한을 제거하는 방법에 대한 자세한 내용은  [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 작업 공유 방법

다음과 같은 방법으로 작업을 공유할 수 있습니다.

* 수동으로 개별적으로 또는 대량으로 수동으로 작업을 공유하는 것은 Workfront의 다른 개체를 공유하는 것과 비슷합니다.

  Workfront에서의 개체 공유에 대한 자세한 내용은  [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 다음을 수행하여 자동으로:

   * 작업의 상위 개체(프로젝트, 프로그램 또는 포트폴리오)에 대한 권한을 지정합니다. 작업은 상위 개체에서 권한을 상속합니다. 개체에 상속된 사용 권한을 보는 방법에 대한 자세한 내용은 [개체에 상속된 사용 권한 보기](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)를 참조하십시오.
   * 작업이 있는 프로젝트를 만드는 데 사용되는 템플릿에 대한 프로젝트 공유에 엔티티를 추가합니다. 템플릿에서 프로젝트를 공유하는 방법에 대한 자세한 내용은 [템플릿 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)를 참조하십시오.

   * 프로젝트를 편집할 때 프로젝트의 모든 작업에 대한 권한을 지정합니다. 프로젝트에 대한 사용자의 권한에 따라 프로젝트의 작업에 대한 액세스를 관리하는 방법에 대한 자세한 내용은 문서 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md)의 [](../../manage-work/projects/manage-projects/edit-projects.md#access) 섹션을 참조하십시오.

  >[!TIP]
  >
  >사용자가 프로젝트의 작업에 할당되었을 때 사용자에게 부여할 작업 권한을 지정하지 않으면 기본적으로 해당 사용자에게는 프로젝트에서 부여한 권한과 동일한 권한이 부여됩니다.

## 작업 권한

다음 표에는 사용자에게 작업을 보기, Contribute 또는 관리할 수 있도록 허용할 때 부여할 수 있는 권한이 표시됩니다.

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>작업</strong> </th> 
   <th><strong>관리</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>보기</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">작업 추가</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">전임 작업 추가</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">문제 추가</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">작업 삭제</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>일반 작업 편집<br></p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 상태 변경</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 제한 사항 편집</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 보기</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">문서 추가</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">작업 복사*</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">작업 이동*</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">시간 기록</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">계획된 일자 수정</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">할당 수락</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">할당하기</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 양식 첨부</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 필드 편집</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">승인 프로세스 만들기</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 승인</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">재무 편집*</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">경비 추가/편집</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">재무 보기</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">업데이트/주석</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">공유</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">시스템 전체 공유</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ 덧신</td> 
  </tr> 
 </tbody> 
</table>

&#42;액세스 수준 및 프로젝트에 대한 권한으로 제어됩니다.
