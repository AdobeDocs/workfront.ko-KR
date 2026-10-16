---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 웹 링크를 문서로 추가
description: 웹 사이트를 Adobe Workfront에 웹 링크로 추가하고 승인을 요청할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 5e37582fe161e1a4689c35773cb1b3f6ead5a859
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 5%
---
# 웹 링크를 문서로 추가

새 문서 영역에서 웹 사이트를 Adobe Workfront에 웹 링크로 추가할 수 있습니다. 추가한 후에는 업로드된 파일에 대한 승인을 요청하는 것과 같은 방식으로 라이브 웹 페이지에서 승인을 요청할 수 있습니다.

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. Adobe 클라우드 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>기존 Workfront 스토리지를 사용하여 문서를 관리하는 모든 Workfront 패키지</p>
<p>Adobe 클라우드 스토리지를 사용하여 문서를 관리하는 모든 워크플로우 패키지</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>레거시 Workfront 스토리지: 문서에 대한 액세스 편집</p> 
   <p>Adobe 클라우드 스토리지: 문서에 대한 편집 액세스는 기본적으로 활성화되어 있으며 변경할 수 없습니다</p>
   </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 웹 링크를 문서로 추가

html 웹 페이지를 Workfront에 웹 링크로 업로드할 수 있습니다. 추가한 후에는 업로드된 파일에 대한 승인을 요청하는 것과 같은 방식으로 라이브 웹 페이지에서 승인을 요청할 수 있습니다. Frame.io에서 웹 링크를 처리하는 방법에 대한 자세한 내용은 [Frame.io 웹 링크](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links)를 참조하십시오.

<!--
>[!IMPORTANT]
>
>A web page behind single sign-on or a login page can't be displayed for review.
-->

웹 링크를 추가하려면:

1. 웹 사이트를 추가할 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;를 선택합니다.
1. **새로 만들기**&#x200B;를 클릭한 다음 **웹 링크**&#x200B;를 선택합니다.
1. **문서 이름** 필드에 이름을 입력한 다음 **URL** 필드에 웹 사이트 주소를 입력하십시오.
1. **추가를 클릭합니다**.
   ![웹 링크를 문서로 추가](assets/web-url.png)

웹 링크에서 승인을 요청하려면 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

## 알려진 제한 사항

* Frame.io에서 생성된 웹 링크 문서에 일시적인 문제가 있습니다. Frame.io에서 웹 링크를 만든 다음 Workfront에서 이에 대한 승인을 만들면 문서가 Frame.io에서 열리지 않습니다. Workfront에서 만든 웹 링크는 영향을 받지 않습니다. 이 문제가 해결될 때까지 승인을 시작하기 전에 Workfront에서 웹 링크 문서를 만드십시오.
* 현재 Frame.io에서는 웹 링크 문서의 새 버전을 만들 수 없습니다. 웹 링크 문서의 새 버전을 만들어야 하는 경우 Workfront에서 새 버전을 만듭니다.