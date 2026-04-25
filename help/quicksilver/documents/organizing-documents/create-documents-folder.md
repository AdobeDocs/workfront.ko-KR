---
product-area: documents
navigation-topic: organize-documents
title: 문서 폴더 만들기
description: 문서를 폴더로 구성할 수 있습니다. 개인 문서 영역에 개인 폴더를 만들 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 41974d6b-fb00-49b7-9db2-36519994e0fd
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 2%

---

# 문서 폴더 만들기

문서를 폴더로 구성할 수 있습니다. Workfront에는 현재 기존 문서 영역과 새 문서 영역의 두 가지 버전이 있습니다. 조직에서 사용하는 버전은 조직이 기존 Workfront 스토리지를 사용하는지 아니면 엔터프라이즈 스토리지를 사용하는지에 따라 다릅니다. 이러한 저장소 유형에 대한 자세한 내용은 [Adobe 엔터프라이즈 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>기존 Workfront 스토리지를 사용하여 문서를 관리하는 모든 Workfront 패키지</p>
<p>Adobe 엔터프라이즈 스토리지를 사용하여 문서를 관리하는 모든 워크플로 패키지</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p>
   <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기존 문서 영역에 문서 폴더 만들기

조직이 기존 Workfront 스토리지에 있는 경우 Workfront의 문서에 액세스할 때 기존 문서 영역이 표시됩니다. 기존 Workfront 스토리지에 대한 자세한 내용은 [Adobe 엔터프라이즈 스토리지와 기존 Workfront 스토리지의 차이점](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage)을 참조하십시오.

>[!NOTE]
>
>문서를 구성하면 문서와 연결된 객체 사이에 링크가 만들어집니다. 시스템에 재배치하지 않습니다.

### 폴더 표시

폴더를 축소판, 표준 또는 목록 보기로 표시할 수 있습니다. 뷰를 변경하려면 오른쪽 상단의 뷰 옵션을 사용합니다.

{{step1-to-documents}}

또는

Workfront 개체를 연 상태에서 왼쪽 패널에서 **문서**&#x200B;를 클릭합니다.

1. Click the view options above the right panel to change how the documents are displayed.

   ![Document view options](assets/screenshot-2016-07-07-12.46.54.png)

### Create folders and subfolders

Create folders to better organize your documents. You can create up to 2,000 folders on an object and up to 50 subfolders within each folder. Subfolders count towards the 2,000 folder maximum.

{{step1-to-documents}}

또는

Workfront 개체를 연 상태에서 왼쪽 패널에서 **문서**&#x200B;를 클릭합니다.

1. To create a top-level folder, ensure that nothing is selected, then click **Add New** > **Folder**.

   또는

   To create a sub-folder, select the folder where you want to create the sub-folder, then click **Add New** > **Folder**.

### Sharing folders

For information about sharing folders, see [Share a document folder](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Create document folders in the new documents area

조직에서 엔터프라이즈 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. 엔터프라이즈 스토리지에 대한 자세한 내용은 [Adobe 엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

### System-generated folders

When you upload a document to a task or issue, Workfront automatically creates a system-generated folder named after the task or issue. This folder is linked to the task or issue and inherits its permissions. System-generated folders are visible in the project-level documents area.

For more information about folder permissions, see [How document permissions work](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

### Create subfolders

You can create subfolders within a system-generated folder to organize documents further. All subfolders inherit permissions from the parent folder.

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.
1. Click into the folder you want to create a subfolder in, then click the **Add folder** ![add folder icon](assets/add-folder-icon.png) icon.
   ![add subfolder](assets/add-subfolder.png)
1. 하위 폴더 이름을 입력한 다음 **만들기**&#x200B;를 클릭합니다.

### 폴더 이름 바꾸기

시스템에서 생성한 폴더는 작업 또는 문제의 이름을 자동으로 상속합니다. 폴더 이름을 클릭하고 편집하여 이름을 변경할 수 있습니다.

폴더 이름을 변경하려면:

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.
1. 이름을 바꿀 폴더를 찾은 다음 **자세히** ![추가 아이콘](assets/more-icon.png) 아이콘을 클릭합니다.
1. **이름 바꾸기**&#x200B;를 클릭한 다음 폴더의 새 이름을 입력합니다.

   ![폴더 이름 바꾸기](assets/rename-folder.png)

1. **이름 바꾸기**&#x200B;를 클릭합니다.

### 폴더 이동

시스템에서 생성한 폴더를 다른 프로젝트, 작업 또는 문제로 이동할 수 있습니다. 시스템에서 생성한 폴더를 다른 위치로 이동하면 연결된 객체가 새 객체로 업데이트되고 권한은 새 상위 객체에서 상속됩니다. 하위 폴더를 다른 프로젝트, 작업 또는 문제로 이동할 수도 있습니다.

>[!NOTE]
>
>이동 대화 상자에서는 동일한 스토리지 유형을 사용하는 프로젝트, 작업 및 문제만 사용할 수 있습니다. 예를 들어 엔터프라이즈 스토리지 프로젝트에서 폴더를 이동하는 경우 엔터프라이즈 스토리지를 사용하는 프로젝트, 작업 및 문제만 이동할 수 있습니다.


폴더를 이동하려면 다음 작업을 수행하십시오.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.
1. 이동할 폴더를 찾은 다음 **자세히** ![추가 아이콘](assets/more-icon.png) 아이콘을 클릭합니다.
1. **이동**&#x200B;을 클릭한 다음 폴더를 이동할 프로젝트, 작업 또는 문제를 선택하십시오.


   ![폴더 이동](assets/rename-folder.png)

<!-- STEPS PLACEHOLDER: Add steps for moving a folder in the new documents area -->

### 폴더 삭제

폴더를 삭제하려면:

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.
1. 삭제할 폴더를 찾은 다음 **자세히** ![추가 아이콘](assets/more-icon.png) 아이콘을 클릭합니다.
1. **삭제**&#x200B;를 클릭합니다.

   ![delete folder](assets/rename-folder.png)
