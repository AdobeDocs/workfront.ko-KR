---
product-area: documents
navigation-topic: manage-documents
title: 문서 체크 아웃
description: 문서를 체크 아웃하여 다른 사용자가 해당 문서를 삭제하거나 새 버전의 문서를 업로드하지 못하도록 할 수 있습니다. 한 번에 한 명의 사용자만 문서를 체크 아웃할 수 있습니다. Adobe Workfront에 업로드된 모든 문서는 물론 서드파티 문서 공급자(Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint 또는 기타 모든 사용자 지정 공급자)에 연결된 문서를 체크 아웃할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# 문서 체크 아웃

문서를 체크 아웃하여 다른 사용자가 해당 문서를 삭제하거나 새 버전의 문서를 업로드하지 못하도록 할 수 있습니다. 한 번에 한 명의 사용자만 문서를 체크 아웃할 수 있습니다. Adobe Workfront에 업로드된 모든 문서는 물론 서드파티 문서 공급자(Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint 또는 기타 모든 사용자 지정 공급자)에 연결된 문서를 체크 아웃할 수 있습니다. 

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td> 
   <p>기여자 이상</p>
   <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서에 대한 액세스 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 체크 아웃된 문서에 대해 허용되는 작업

문서에 대한 관리 액세스 권한이 있는 사용자는 다음을 수행할 수 있습니다.

* 문서(문서 이름, 설명, 사용자 정의 데이터) 편집
* 문서 이동
* 문서 공유
* 문서 미리보기
* 문서 다운로드

  >[!TIP]
  >
  > 다른 사용자가 문서를 체크 아웃한 경우 사용자가 문서를 다운로드할 수 있지만 문서를 다운로드하기 전에 다시 체크 인할 때까지 기다리는 것이 좋습니다. 문서가 체크 아웃되면 문서에 대한 작업이 아직 진행 중임을 나타내는 경우가 많습니다. 문서가 다시 체크 인되어 다운로드될 때까지 기다리면 사용자가 최신 버전을 보유하게 됩니다.

* 문서를 승인하거나 문서에 승인을 적용합니다.
* 증명 뷰어에서 문서 검토

  교정에 대한 자세한 내용은 [교정](../../review-and-approve-work/proofing/proofing.md)을 참조하세요.

## 문서 체크 아웃

문서에 대한 관리 권한이 있는 경우 문서를 체크 아웃하여 문서에 대한 특정 작업을 금지할 수 있습니다. 

1. 문서가 저장된 영역으로 이동한 다음 문서를 선택합니다. 

   문서 추가에 대한 자세한 내용은 [파일 시스템에서 Adobe Workfront에 문서 추가](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)를 참조하십시오.

1. **체크 아웃** 아이콘 ![체크 아웃 아이콘](assets/check-out-25x23.png)을 클릭합니다.

1. 문서 이름 오른쪽에 잠금 아이콘 ![잠금 아이콘](assets/lock-icon-locked-qs.png)이 표시됩니다. Workfront에서 로그아웃한 후에도 문서가 체크 아웃된 상태로 유지됩니다.
1. 문서를 체크아웃한 사용자나 Workfront 관리자만 문서를 체크인할 수 있습니다.

## 체크 아웃된 문서 관리

체크 아웃된 문서에 대해 다음 사항을 고려하십시오.

* 체크 아웃된 문서가 저장된 객체를 삭제하려면 먼저 문서를 다시 체크 인해야 합니다. 
* Workfront 관리자가 소유하지 않은 문서를 체크아웃한 사용자를 삭제하는 경우 Workfront은 자동으로 문서를 체크인합니다.
* Workfront 관리자가 자신이 소유한 문서를 체크 아웃한 사용자를 삭제하고 문서가 오브젝트에 업로드되면 문서가 체크 아웃된 상태로 유지됩니다. Workfront 관리자만 다시 체크인할 수 있습니다.
* Workfront 관리자가 자신이 소유한 문서를 체크아웃한 사용자를 삭제하고 문서가 문서 영역(오브젝트가 아닌)에만 업로드되면 문서가 사용자와 함께 삭제됩니다.

  사용자 삭제에 대한 자세한 내용은 [사용자 삭제](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)를 참조하십시오.

* Workfront 관리자가 사용자를 비활성화하면 사용자가 체크 아웃한 모든 문서가 체크 아웃된 상태로 유지됩니다. Workfront 관리자만 다시 체크인할 수 있습니다. 

## 에서 문서 확인

새 버전을 업로드하거나 삭제하려면 먼저 문서를 다시 체크 인해야 합니다. 

문서를 체크 인하려면 다음과 같이 하십시오.

1. 문서가 저장된 영역으로 이동하여 문서를 선택합니다. 

   문서 이름 오른쪽에 잠금 아이콘 ![잠금 아이콘](assets/lock-icon-locked-qs.png)이 표시됩니다.

1. **체크 인** 아이콘 ![체크 인 아이콘](assets/check-in-25x22.png)을 클릭합니다.
