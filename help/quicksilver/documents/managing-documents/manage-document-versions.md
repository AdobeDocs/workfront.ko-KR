---
product-area: documents
navigation-topic: manage-documents
title: 문서 버전 관리
description: Workfront에서 여러 버전의 문서를 관리할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 문서 버전 관리

Workfront에서 여러 버전의 문서를 관리할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p> 임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 보기</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서에 대한 액세스 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 전제 조건

* 이 문서에서는 문서에 여러 버전이 있다고 가정합니다.

  새 버전의 문서를 Workfront에 업로드하는 방법에 대한 자세한 내용은 [새 버전의 문서 업로드](../../documents/managing-documents/upload-new-document-version.md)를 참조하십시오.

## 문서의 모든 버전 목록 보기

1. 요약에서 **모든 버전** 섹션으로 스크롤합니다. 여기에서 문서의 모든 버전을 볼 수 있습니다.

## 이전 문서 버전에 대한 세부 정보 보기 및 관리

1. 문서 세부 정보 페이지 상단에서 이름 옆에 있는 드롭다운 메뉴를 클릭한 다음 보고 관리할 버전의 이름을 클릭합니다.

   문서 세부 정보의 ![버전 드롭다운](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   버전의 세부 사항 보기와 함께 버전 이름, 메타데이터 및 증명 설정(문서 증명인 경우)과 같은 버전을 변경할 수 있습니다.

## 단일 문서 버전 다운로드

1. 요약의 **버전**&#x200B;에서 버전 오른쪽에 있는 기타 메뉴 ![기타 메뉴](assets/more-icon.png)를 클릭한 다음 표시되는 드롭다운 목록에서 **다운로드**&#x200B;를 클릭합니다.

   ![단일 문서 다운로드](assets/more-versions-350x143.png)

## 문서의 모든 버전 다운로드

1. **문서 세부 정보**&#x200B;를 클릭한 다음 왼쪽 패널에서 **모든 버전**&#x200B;을 선택합니다.

1. 목록 맨 위에서 **모두 다운로드**&#x200B;를 클릭합니다.

## 문서 버전 삭제

실수로 문서 버전을 업로드하거나 더 이상 버전이 필요하지 않으면 버전을 삭제하고 원본 문서를 유지할 수 있습니다.

>[!IMPORTANT]
>
>개별적으로 삭제한 문서 버전은 복구할 수 없습니다.

문서 버전을 삭제할 때는 다음 사항을 염두에 두십시오.

* 한 번에 하나의 버전만 삭제할 수 있습니다. 버전을 삭제하면 이 작업은 문서의 **업데이트**&#x200B;에 나타납니다.
* 버전을 삭제한 후 새 버전을 업로드하면 새 버전이 다음 일련 번호를 받습니다. 예를 들어, 문서의 버전이 3개인 경우 버전 3을 삭제하면 업로드되는 다음 문서는 버전 4가 됩니다.
* 버전에 대한 시스템 업데이트 및 주석은 버전이 삭제된 후 Workfront에 유지됩니다.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

문서 버전을 삭제하려면 다음을 수행합니다.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.필요한 문서를 찾습니다.
1. 요약의 **버전** 영역에서 버전을 클릭한 다음 나타나는 드롭다운 목록에서 **삭제**&#x200B;를 클릭합니다. **삭제** 옵션은 버전이 두 개 이상인 경우에만 표시됩니다.

   문서가 외부 소스에 연결된 경우 해당 링크가 삭제되고 Workfront을 통해 문서에 더 이상 액세스할 수 없습니다.

   ![문서 버전 삭제](assets/more-versions-350x143.png)
