---
title: 문서 공유
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 관리자는 문서에 대한 액세스 권한 부여에 설명된 대로 액세스 수준을 할당할 때 사용자에게 문서를 보거나 편집할 수 있는 액세스 권한을 부여합니다.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# 문서 공유

Adobe Workfront 관리자는 [문서에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)에 설명된 대로 액세스 수준을 할당할 때 사용자에게 문서를 보거나 편집할 수 있는 액세스 권한을 부여합니다.

Workfront 관리자가 사용자에게 부여하는 액세스 수준으로 문서를 보거나 편집할 수 있습니다. 이 외에도 다른 사용자는 자신이 업로드했거나 공유할 수 있는 액세스 권한이 있는 특정 문서를 보거나 관리할 수 있는 권한을 다른 사용자에게 부여할 수도 있습니다.

권한은 Workfront의 한 항목에 한정되며, 해당 항목에 대해 수행할 수 있는 작업을 정의합니다. 개체 사용 권한에 대한 자세한 내용은 [개체에 대한 공유 사용 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

Workfront에 문서를 업로드하는 사용자에게는 기본적으로 관리 권한이 있습니다.

전체 문서 폴더 공유에 대한 자세한 내용은 [문서 폴더 공유](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)를 참조하십시오.

## 문서 공유에 대한 고려 사항

아래 고려 사항 외에 [개체에 대한 공유 권한 개요](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

>[!NOTE]
>
>Workfront 관리자는 해당 항목의 소유자가 아닌 모든 사용자에 대해 시스템의 모든 항목에 대한 권한을 추가하거나 제거할 수 있습니다.

* 문서를 공유하는 것은 Workfront의 다른 개체를 공유하는 것과 비슷합니다. Workfront에서 문서를 공유하는 방법에 대한 자세한 내용은 [개체 공유](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)를 참조하십시오.
* 문서에 다음 권한을 부여할 수 있습니다.

   * 보기
   * 관리

* 문서를 공개적으로 공유하거나 시스템 전체에서 공유할 수도 있습니다.

  >[!CAUTION]
  >
  >외부 사용자와 기밀 정보가 포함된 오브젝트를 공유할 때는 주의하는 것이 좋습니다. 이를 통해 Workfront 사용자 또는 조직의 일부가 아니더라도 정보를 볼 수 있습니다.

* Workfront 계정이 없는 사람과 문서 액세스 권한 부여 대상 필드에 전자 메일 주소를 추가하여 문서를 공유할 수 있습니다.
* 문서를 공유할 때 사용자는 모든 문서 버전과 모든 문서 증명에 대해 동일한 액세스 권한을 갖습니다.\
  Workfront의 증명에 대한 자세한 내용은 [증명](../../review-and-approve-work/proofing/proofing.md) 섹션을 참조하십시오.

* 문서와 연관된 개체에서 문서에 대한 권한을 상속할 수 있습니다. Workfront 관리자는 액세스 수준의 문서에 대한 권한 상속을 제한할 수 있습니다.

  문서에 대해 상속된 사용 권한을 제한하는 방법에 대한 자세한 내용은 [사용자 지정 액세스 수준 만들기 또는 수정](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하십시오.

  문서에 대해 상속된 권한을 수동으로 제거할 수 있습니다. 자세한 내용은 [개체에서 권한 제거](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)를 참조하십시오.

* 첨부된 문서는 첨부된 객체에서만 권한을 상속합니다. 개체에서 폴더를 만들고 문서를 폴더로 이동하면 해당 폴더의 권한이 상속됩니다. 그러나 상위 또는 최상위 개체에 폴더를 만들어 해당 폴더로 문서를 이동하면 해당 폴더의 권한이 상속되지 않습니다.

## 문서 권한

다음 표에는 사용자가 문서를 보거나 관리할 수 있도록 허용할 때 부여할 수 있는 권한이 표시됩니다.

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>작업</strong> </p> </th> 
   <th> <p><strong>관리</strong> </p> </th> 
   <th> <p><strong>보기</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">만들기</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">문서 세부 정보 편집</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">삭제*</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">다운로드</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">체크아웃</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">승인자 추가</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">문서 승인</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 양식 첨부</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">사용자 정의 필드 편집</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">(오브젝트)로 이동</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">전송 대상(통합)</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">업데이트/주석</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">새 버전 업로드</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">버전 삭제</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">문서 보기</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">미리보기</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">증명**</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">증명 생성**</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">증명 제거**</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">공유*</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">시스템 전체 공유*</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">공개적으로 문서 공유*</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">외부 이메일 주소와 공유</td> 
   <td> </td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">추가/제거</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">이름 바꾸기</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">링크(통합 사용)</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td scope="row">연결 해제(통합 사용)</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 작업이 문서 폴더와 문서 폴더 모두에서 공유됩니다.

&#42;&#42; 문서를 증명하려면 Workfront 계정과 연결된 별도의 증명 라이선스가 있어야 합니다. 증명 라이선스 취득에 대해서는 계정 관리자에게 문의하십시오. Workfront의 증명에 대한 자세한 내용은 [증명](../../review-and-approve-work/proofing/proofing.md)을 참조하세요.
