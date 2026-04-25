---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 파일 시스템에서 Adobe Workfront에 문서 추가
description: You can add documents to projects, tasks, or issues in multiple areas in Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 2%

---

# 파일 시스템에서 Adobe Workfront에 문서 추가

Workfront에는 현재 기존 문서 영역과 새 문서 영역의 두 가지 버전이 있습니다. 조직에서 사용하는 버전은 조직이 기존 Workfront 스토리지를 사용하는지 아니면 엔터프라이즈 스토리지를 사용하는지에 따라 다릅니다. 이러한 저장소 유형에 대한 자세한 내용은 [Adobe 엔터프라이즈 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

Adding documents to Workfront differs depending on which version of the documents area your organization uses.

* [Add documents to from your file system in the legacy documents area](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Add documents to Workfront in the new documents area](#add-documents-to-workfront-in-the-new-documents-area)



## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>기존 Workfront 스토리지를 사용하여 문서를 관리하는 모든 Workfront 패키지</p>
<p>Adobe 엔터프라이즈 스토리지를 사용하여 문서를 관리하는 모든 워크플로 패키지</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Legacy Workfront Storage: Edit access to Documents</p> 
   <p>Enterprise storage: Edit access to Documents is enabled by default and cannot be changed</p>
   </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Add documents from your file system in the legacy documents area

If your organization is on legacy Workfront Storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront Storage, see [Differences between Adobe enterprise storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

You can add documents to projects, tasks, or issues in the following areas in Adobe Workfront:

* The global Documents area
* The Documents area for a Workfront object
* A connected card on a Workfront board

새 버전의 문서를 업로드하고 Google 드라이브, Dropbox 및 Microsoft OneDrive와 같은 서드파티 클라우드 공급업체의 문서에 대한 링크를 추가할 수도 있습니다. 새 문서 버전 추가에 대한 자세한 내용은 [새 문서 버전 업로드](../../documents/managing-documents/upload-new-document-version.md)를 참조하십시오. 타사 클라우드 공급업체의 문서를 추가하는 방법에 대한 자세한 내용은 [외부 응용 프로그램에서 문서 연결](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)을 참조하십시오.

Workfront에 업로드할 수 있는 파일의 유형과 크기에는 제한이 없습니다. 그러나 업로드가 성공하려면 5분 이내에 완료되어야 하며 사용 가능한 저장 공간이 충분해야 합니다.

새 버전의 문서를 Workfront에 업로드하는 방법에 대한 자세한 내용은 [새 버전의 문서 업로드](../../documents/managing-documents/upload-new-document-version.md)를 참조하십시오.


### 기존 문서 영역에서 Workfront에 문서 추가

워크스테이션의 파일 시스템에서 Workfront에 새 문서를 추가할 수 있습니다. Google 드라이브 및 SharePoint과 같은 서드파티 애플리케이션에서 문서를 연결할 수도 있습니다.

>[!IMPORTANT]
>
>* 한 번에 최대 150개의 문서를 업로드할 수 있습니다.
>* 파일 크기에는 제한이 없습니다.
>* 문서 다운로드는 4GB로 제한됩니다.

문서를 추가하려면 다음 작업을 수행하십시오.

1. 새 문서를 추가할 프로젝트, 작업 또는 문제로 이동합니다.
1. **문서** 탭을 클릭한 다음 **새로 추가** 드롭다운 메뉴를 클릭합니다.

   ![새 문서 추가](assets/add-new-doc.png)

1. 추가할 문서의 유형에 따라 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">워크스테이션의 파일 시스템에서 문서 업로드</td> 
      <td> 
       <ol> 
        <li value="1"><strong>새로 추가</strong> 드롭다운 메뉴에서 <strong>문서</strong>를 선택합니다.</li> 
        <li value="2"> <p>워크스테이션의 파일 시스템에서 추가할 문서를 찾아 선택합니다.<br></p> <p>추가 파일을 선택할 때 Shift 키를 누르면 여러 문서를 선택할 수 있습니다.</p> </li> 
        <li value="3"><strong>열기를 클릭합니다</strong>.</li> 
       </ol> 
       <p><b>참고</b>: 파일 관리자에서 문서 목록으로 직접 파일을 끌어다 놓을 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Google 드라이브 또는 SharePoint과 같은 서드파티 애플리케이션에서 문서 업로드</td> 
      <td> 
       <ol> 
        <li value="1"> <p><strong>새로 추가</strong> 드롭다운 메뉴에서 <strong>From &lt;name_of_third-party_application&gt;</strong>을(를) 선택합니다.</p> <p>예를 들어 Google 드라이브에서 문서를 업로드하려면 <strong>Google 드라이브에서</strong>을(를) 클릭합니다.</p> </li> 
        <li value="2"> <p>화면의 지침에 따라 서드파티 애플리케이션에서 문서를 선택합니다.<br></p> <p>연결된 문서에 대한 자세한 내용은 <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">외부 응용 프로그램에서 문서 연결</a>을 참조하세요.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">다른 Workfront 사용자로부터 문서 요청</td> 
      <td> 
       <ol> 
        <li value="1"><strong>새로 추가</strong> 드롭다운 메뉴에서 <strong>문서 요청</strong>을 선택합니다.</li> 
        <li value="2"><strong>요청한 사용자 이름</strong> 상자에 문서를 요청한 사용자의 이름을 입력합니다.</li> 
        <li value="3"><strong>요청한 내용 전달</strong> 상자에 문서 이름을 입력합니다.</li> 
        <li value="4"> <p><strong>요청 보내기</strong>를 클릭합니다.</p> <p>요청이 문서 탭에 표시됩니다.</p> <p>문서 요청에 대한 자세한 내용은 <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">문서 요청</a>을 참조하십시오.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>


## 새 문서 영역에서 Workfront에 문서 추가

엔터프라이즈 스토리지 모델을 사용하여 프로젝트, 작업 또는 문제에 문서를 추가할 수 있습니다. 엔터프라이즈 스토리지에 대한 자세한 내용은 [Adobe 엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

새 문서 영역에서 현재 지원되지 않는 기능:

* 글로벌 문서 영역에 문서 업로드
* Google 드라이브, Dropbox 및 Microsoft OneDrive와 같은 서드파티 클라우드 공급업체의 문서에 대한 링크를 추가합니다.
* 문서 요청 중
* 폴더에 링크 복사
* 문서 체크 아웃
* 클립보드에서 이미지 붙여넣기
* 스마트 폴더 추가


### 새 문서 영역에서 Workfront에 문서 추가

조직에서 엔터프라이즈 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. 엔터프라이즈 스토리지에 대한 자세한 내용은 [Adobe 엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

<!--
>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.
-->

문서를 추가하려면 다음 작업을 수행하십시오.

1. 새 문서를 추가할 프로젝트, 작업 또는 문제로 이동합니다.
1. Click the **Documents** in the left panel.
1. Click **New** on the right side of the page or drag and drop the file into the drop zone that appears. You can add multiple documents at one time.

   ![Add a new document](assets/add-new-doc-new-doc.png)

새 버전의 문서를 Workfront에 업로드하는 방법에 대한 자세한 내용은 [새 버전의 문서 업로드](../../documents/managing-documents/upload-new-document-version.md)를 참조하십시오.

## Document security for enterprise storage

Workfront prevents viruses and other malicious content from entering the site via documents in the following ways:

**How Workfront detects corrupted files**

Document scanning is automatically enabled for objects using the enterprise storage model.

All files under 500 MB are scanned when they are uploaded. Files over 500 MB are not scanned. If Workfront detects a corrupted document, it is automatically removed.

**File name restrictions**

Because this integration is built using Adobe enterprise storage, there are some enforced structure and naming conventions to be aware of when managing projects and documents.

* Object names must be unique and can&#39;t be duplicated
* Adobe enterprise storage requires unique names for peer objects with the same parent in the hierarchy tree
* Documents can&#39;t have the same name if they belong to the same project
* Document names can&#39;t contain any of the following special characters: `\ / : * ? " | < >`
* Document names are limited to 255 characters maximum

With these limitations in mind, Workfront automatically renames objects or documents as needed to prevent conflicts.


## Document security for legacy Workfront storage

Workfront site prevents viruses and other malicious content from entering the site via documents in the following ways:

**How Workfront detects corrupted files**

Document scanning is enabled for your organization only upon request.

If document scanning is enabled, files under 25 MB are scanned when they are uploaded. Files over 25 MB are not scanned.

If Workfront detects a corrupted document, a message appears indicating that the file is corrupt. You also receive an email notification when Workfront detects potentially malicious content and the file is slated for removal.

Corrupted files are removed within 24 hours of detection unless you remove it manually. If you delete a corrupted file, Workfront tracks this action as an update. If you allow Workfront to remove it, then no updates are recorded.

**File name restrictions**

Files that are uploaded to Workfront cannot contain certain characters in file names. If a file contains any of the following characters in the file name, the characters are removed from the file name when the file is uploaded: `! # % * \ | ' " / ? < > { } [ ]`.
