---
product-area: documents
navigation-topic: manage-documents
title: 문서 체크 아웃
description: 문서를 체크 아웃하여 다른 사용자가 문서를 삭제하거나 새 버전을 업로드하지 못하도록 할 수 있습니다. 한 번에 한 명의 사용자만 문서를 체크 아웃할 수 있습니다. Adobe Workfront에 업로드된 모든 문서와 타사 문서 공급자(Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint 또는 기타 사용자 정의 공급자)에 연결된 문서를 체크 아웃할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 문서 체크 아웃

문서를 체크 아웃하여 다른 사용자가 문서를 삭제하거나 새 버전을 업로드하지 못하도록 할 수 있습니다. 한 번에 한 명의 사용자만 문서를 체크 아웃할 수 있습니다. Adobe Workfront에 업로드된 모든 문서와 타사 문서 공급자(Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint 또는 기타 사용자 정의 공급자)에 연결된 문서를 체크 아웃할 수 있습니다. 

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서에 대한 액세스 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 체크 아웃된 문서에서 허용되는 작업

문서에 대한 액세스 권한을 관리하는 사용자는 다음을 수행할 수 있습니다.

* 문서(문서 이름, 설명, 사용자 정의 데이터) 편집
* 문서 이동
* 문서 공유
* 문서 미리 보기
* 문서 다운로드

   >[!TIP]
   >
   > 다른 사용자가 문서를 체크 아웃할 때 문서를 다운로드할 수 있지만 문서를 다운로드하기 전에 사용자가 문서를 다시 체크 인할 때까지 기다리는 것이 좋습니다. 문서를 체크 아웃하면 문서에 작업이 계속 수행되고 있음을 나타냅니다. 문서가 다시 체크 인될 때까지 기다리면 최신 버전이 제공됩니다.

* 문서를 승인하거나 문서에 승인을 적용합니다.
* 교정 뷰어에서 문서를 검토합니다

   교수에 대한 자세한 내용은 [교정](../../review-and-approve-work/proofing/proofing.md)

## 문서 체크 아웃

문서에 대한 관리 권한이 있는 경우 체크 아웃하여 문서에 대한 특정 작업을 금지할 수 있습니다. 

1. 문서가 저장된 영역으로 이동한 다음 문서를 선택합니다. 

   문서 추가에 대한 자세한 내용은 [파일 시스템에서 Adobe Workfront에 문서 추가](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. 을(를) 클릭합니다. **체크 아웃** 아이콘 ![](assets/check-out-25x23.png).

1. 잠금 아이콘 ![](assets/lock-icon-locked-qs.png) 문서 이름의 오른쪽에 표시됩니다. Workfront에서 로그아웃한 후에도 문서가 체크 아웃되지 않은 상태로 유지됩니다.
1. 문서를 체크 아웃한 사용자 또는 Workfront 관리자만 문서를 체크 인할 수 있습니다.

## 체크 아웃된 문서 관리

체크 아웃된 문서에 대해 다음 사항을 고려하십시오.

* 체크 아웃된 문서가 저장된 객체를 삭제하려면 먼저 문서를 다시 체크 인해야 합니다. 
* Workfront 관리자가 소유하지 않은 문서를 체크 아웃한 사용자를 삭제하면 Workfront에서 자동으로 문서를 체크 인합니다.
* Workfront 관리자가 자신이 소유한 문서를 체크 아웃한 사용자를 삭제하고 문서가 객체에 업로드된 경우 문서가 체크 아웃된 상태로 유지됩니다. Workfront 관리자만 다시 체크 인할 수 있습니다.
* Workfront 관리자가 자신이 소유한 문서를 체크 아웃한 사용자를 삭제하고 문서가 객체 이외의 문서 영역에만 업로드되는 경우 해당 문서는 사용자와 함께 삭제됩니다.

   사용자 삭제에 대한 자세한 내용은 [사용자 삭제](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Workfront 관리자가 사용자를 비활성화하면 사용자가 체크 아웃한 모든 문서는 체크 아웃된 상태로 유지됩니다. Workfront 관리자만 다시 체크 인할 수 있습니다. 

## 문서 체크 인

새 버전을 업로드하거나 삭제하려면 먼저 문서를 다시 체크 인해야 합니다. 

문서를 체크 인하려면

1. 문서가 저장된 영역으로 이동하여 문서를 선택합니다. 

   잠금 아이콘 ![](assets/lock-icon-locked-qs.png) 문서 이름의 오른쪽에 표시됩니다.

1. 을(를) 클릭합니다. **체크인** 아이콘 ![](assets/check-in-25x22.png).
