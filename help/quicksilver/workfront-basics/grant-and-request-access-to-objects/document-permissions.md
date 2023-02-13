---
title: 문서 공유
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 문서에 대한 액세스 권한 부여에 설명된 대로 액세스 수준을 할당할 때 문서를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# 문서 공유

Adobe Workfront 관리자는 다음과 같이 액세스 수준을 지정할 때 사용자에게 문서를 보거나 편집할 수 있는 액세스 권한을 부여합니다. [문서에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Workfront 관리자가 사용자에게 부여하는 액세스 수준에서는 문서를 보거나 편집할 수 있습니다. 이 외에도 다른 사용자는 다른 사용자에게 자신이 업로드한 특정 문서를 보거나 관리할 수 있는 권한 또는 공유 액세스 권한을 부여할 수 있습니다.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다. 개체 권한에 대한 자세한 내용은 [개체에 대한 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Workfront에 문서를 업로드하는 사용자에게는 기본적으로 관리 권한이 있습니다.

전체 문서 폴더 공유에 대한 자세한 내용은 [문서 폴더 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## 문서 공유에 대한 고려 사항

아래 고려 사항 외에 다음을 참조하십시오 [개체에 대한 권한 공유 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아니더라도 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

* 문서를 공유하는 것은 Workfront에서 다른 개체를 공유하는 것과 비슷합니다. Workfront에서 문서를 공유하는 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* 문서에 다음 권한을 부여할 수 있습니다.

   * 보기
   * 관리

* 공개 또는 시스템 전체에서 문서를 공유할 수도 있습니다.

   >[!CAUTION]
   >
   >외부 사용자와 기밀 정보가 포함된 개체를 공유할 때는 주의해야 합니다. 이를 통해 Workfront 사용자 또는 조직의 구성원이 아니더라도 정보를 볼 수 있습니다.

* 문서에 액세스할 수 있는 권한 부여 필드에 전자 메일 주소를 추가하여 Workfront 계정이 없는 사람과 문서를 공유할 수 있습니다.
* 문서를 공유하면 사용자는 모든 문서 버전 및 모든 문서 증명에 동일한 액세스 권한을 갖습니다.\
   Workfront에서 교정에 대한 자세한 내용은 [교정](../../review-and-approve-work/proofing/proofing.md) 섹션을 참조하십시오.

* 연관된 객체에서 문서에 대한 권한을 상속할 수 있습니다. Workfront 관리자는 액세스 수준에서 문서에 대한 권한 상속을 제한할 수 있습니다.

   문서에 대한 상속된 권한 제한에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   문서에 대한 상속된 권한을 수동으로 제거할 수 있습니다. 자세한 내용은 [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* 첨부된 문서는 첨부된 개체에서만 권한을 상속합니다. 객체에 폴더를 만들고 문서를 폴더로 이동하면 해당 폴더는 폴더의 권한을 상속합니다. 그러나 상위 또는 상위 개체에 폴더를 만들고 해당 폴더로 문서를 이동해도 해당 폴더의 권한은 상속되지 않습니다.

## 문서 권한

다음 표에는 사용자에게 문서를 보거나 관리할 수 있도록 허용할 수 있는 권한이 표시됩니다.

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>개 액션</strong> </p> </th> 
   <th> <p><strong>관리</strong> </p> </th> 
   <th> <p><strong></strong> 보기 </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">만들기</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">문서 세부 정보 편집</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">삭제*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">다운로드</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">체크아웃</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">승인자 추가</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">문서 승인</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 양식 첨부</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 지정 필드 편집</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">(개체)로 이동</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">보내기(통합)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">업데이트/댓글</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">새 버전 업로드</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">버전 삭제</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">문서 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">미리 보기</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">증명**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">증명 생성**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">증명 제거**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">공유*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">시스템 전체 공유*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">공개적으로 문서 공유*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">외부 전자 메일 주소와 공유</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">추가/제거</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">이름 바꾸기</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">링크(통합 포함)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">연결 해제(통합 사용)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 작업은 문서와 문서 폴더 모두에서 공유됩니다.

&#42;&#42; 문서를 증명하려면 Workfront 계정과 별도의 언어 교정 라이센스가 있어야 합니다. 교정 라이선스를 획득하는 방법은 계정 관리자에게 문의하십시오. Workfront에서 교정에 대한 자세한 내용은 [교정](../../review-and-approve-work/proofing/proofing.md).
