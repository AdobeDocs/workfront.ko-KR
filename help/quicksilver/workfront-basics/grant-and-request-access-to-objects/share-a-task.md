---
title: 작업 공유
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 액세스 수준을 할당할 때 작업을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 작업에 대한 액세스 권한 부여에 대한 자세한 내용은 작업에 대한 액세스 권한 부여 를 참조하십시오.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 4%

---

# 작업 공유

Adobe Workfront 관리자는 액세스 수준을 할당할 때 작업을 보거나 편집할 수 있는 액세스 권한을 부여할 수 있습니다. 작업에 대한 액세스 권한 부여에 대한 자세한 내용은 [작업에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

사용자에게 부여된 액세스 레벨과 함께 사용자에게 공유 액세스 권한이 있는 특정 작업을 보기, 기여 또는 관리할 권한을 부여할 수도 있습니다.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다.

## 작업 공유 시 고려 사항

아래 고려 사항 외에 다음을 참조하십시오 [개체에 대한 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* 작업 작성자는 기본적으로 이 작업에 대한 관리 권한이 있습니다.
* 개별적으로 작업을 공유하거나 여러 작업을 한꺼번에 일괄적으로 공유할 수 있습니다.\
   작업 공유는 다른 개체 공유와 동일합니다. Workfront에서 항목 공유에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 작업에 다음 권한을 부여할 수 있습니다. 

   * 보기
   * 관리
   * 참여\
      ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* 작업을 공유하면 사용자는 기본적으로 작업과 연관된 모든 하위 객체에 대해 동일한 권한을 상속합니다. 예를 들어 하위 작업, 문제 및 작업에 첨부된 문서에 대해 동일한 권한을 상속합니다.\
   Workfront에서 개체의 계층 구조에 대한 자세한 내용은  [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   Workfront 관리자는 문서가 사용자의 액세스 수준에서 상위 개체에서 권한을 상속해야 하는지 여부를 지정할 수 있습니다. 문서에 대한 상속된 권한 제한에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 작업에서 상속된 권한을 제거할 수 있습니다.\
   개체에서 상속된 사용 권한을 제거하는 방법에 대한 자세한 내용은  [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 작업 공유 방법

다음과 같은 방법으로 작업을 공유할 수 있습니다.

* 수동으로, 개별적으로 또는 대량으로 수동으로 작업을 공유하는 것은 Workfront에서 다른 개체를 공유하는 것과 비슷합니다.

   Workfront에서 개체 공유에 대한 자세한 내용은  [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 다음을 수행하여 자동으로 다음을 수행합니다.

   * 작업의 상위 개체에 대한 권한을 지정합니다. 프로젝트, 프로그램 또는 포트폴리오 작업은 상위 개체에서 권한을 상속합니다. 객체에 대한 상속된 권한 보기에 대한 자세한 내용은 [객체에 대한 상속된 권한 보기](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * 작업이 있는 프로젝트를 만드는 데 사용되는 템플릿의 프로젝트 공유에 엔티티를 추가합니다. 템플릿에서 프로젝트 공유에 대한 자세한 내용은 [템플릿 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * 프로젝트를 편집할 때 프로젝트의 모든 작업에 대한 권한을 지정합니다. 프로젝트에 대한 사용자의 권한에 따라 프로젝트의 작업에 대한 액세스 관리를 위한 자세한 내용은 [](../../manage-work/projects/manage-projects/edit-projects.md#access) 문서의 섹션 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md).
   >[!TIP]
   >
   >사용자가 프로젝트의 작업에 할당될 때 어떤 작업 권한을 가질 것인지 지정하지 않으면 기본적으로 프로젝트에 대해 가지고 있는 것과 동일한 권한을 사용자에게 받습니다.

## 작업 권한

다음 표에는 사용자에게 작업 보기, 기여 또는 관리를 허용할 때 사용자에게 부여할 수 있는 권한이 표시됩니다.

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>개 액션</strong> </th> 
   <th><strong>관리</strong> </th> 
   <th><strong>참여</strong> </th> 
   <th><strong></strong> 보기 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">작업 추가</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">선행 작업 추가</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>일반 작업 편집<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 상태 변경</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">작업 제약 조건 편집</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">시간 기록</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">계획 일자 수정</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">할당 수락</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">할당 만들기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 양식 첨부</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 지정 필드 편집</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">승인 프로세스 만들기</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">비용 추가/편집</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">재무 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">업데이트/댓글</td> 
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
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;프로젝트에 대한 액세스 수준 및 권한에 의해 제어됩니다.
