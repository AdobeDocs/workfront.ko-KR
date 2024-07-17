---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 문서에 대한 증명 만들기
description: Workfront에 업로드할 때 문서에 대한 증명을 생성할 수 있습니다. Adobe Workfront에 이미 업로드된 문서 또는 Workfront에 이미 있는 새 증명 버전에 대한 증명을 생성할 수도 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# 문서에 대한 증명 만들기

<!-- Audited: 1/2024 -->

Workfront에 업로드할 때 문서에 대한 증명을 생성할 수 있습니다.

Adobe Workfront에 이미 업로드된 문서 또는 Workfront에 이미 있는 새 증명 버전에 대한 증명을 생성할 수도 있습니다.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> 
   <p>새로 만들기: 모두 </p>
   <p>현재: Pro 이상</p> <p>기존 플랜: Select 또는 Premium</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>새로운 기능: 표준</p>
   <p>현재 : 작업 또는 계획</p> <p>기존 계획: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 문서 업로드 및 증명 만들기

1. 새 증명을 만들 프로젝트, 작업 또는 문제로 이동합니다.
1. **문서** 탭을 클릭합니다.
1. 왼쪽 패널에서 문서 ![](assets/document-icon.png)을(를) 클릭합니다.
1. **새로 추가**&#x200B;를 클릭한 다음 표시되는 메뉴에서 **증명**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >이 프로세스를 자동화하려면 사용자 프로필에서 **문서를 업로드할 때 증명을 자동으로 생성** 설정을 활성화할 수 있습니다. 자세한 내용은 [내 설정 구성](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) 을 참조하십시오.

1. 표시되는 **새 증명** 페이지에서 다음을 수행할 수 있습니다.

   * [기본 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [자동화된 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 문서 업로드 및 새 증명 버전 만들기

1. 기존 증명의 새 버전을 만들 프로젝트, 작업 또는 문제로 이동합니다.
1. **문서** 탭을 클릭합니다.
1. 새 버전을 추가할 문서를 선택합니다.
1. **새로 추가** > **버전** > **증명**&#x200B;을 클릭합니다.
1. 표시되는 **새 증명 버전** 페이지에서 다음을 수행할 수 있습니다.

   * [기본 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [자동화된 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 드래그 앤 드롭을 사용하여 새 버전에 대한 간단한 증명 생성

파일 시스템(예: 데스크탑)에서 문서를 드래그 앤 드롭하여 새 증명 또는 기존 증명의 새 버전을 만들 수 있습니다. 증명에는 새 증명을 만드는지 아니면 새 버전을 만드는지에 따라 다음 설정이 포함됩니다.

* **새 증명:** 귀하와만 공유되는 간단한 증명을 만듭니다. [증명 설정 편집](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md)에 설명된 대로 증명을 만든 후 공유 설정을 수정할 수 있습니다.

* **기존 증명의 새 버전:** 이전 버전과 동일한 증명 설정으로 새 버전을 만듭니다.

드래그 앤 드롭을 사용하여 새 증명 또는 새 증명 버전을 생성하려면 다음을 수행하십시오.

1. 에 설명된 대로 증명이 자동으로 생성되도록 구성되었는지 확인합니다.
1. 계속  [파일 시스템에서 Adobe Workfront에 문서를 추가](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)합니다. 여기에서는 문서를 추가하는 드래그 앤 드롭 방법에 대해 설명합니다. 

## 기존 문서에 대한 증명 만들기

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 섹션을 클릭합니다.
1. 문서 위로 마우스를 가져간 다음 문서 이름 아래에 나타나는 **증명 만들기** 링크를 클릭합니다.

   >[!NOTE]
   >
   >사용자 프로필에 **문서를 업로드할 때 자동으로 증명 생성**&#x200B;이 활성화되어 있으면 간단한 증명이 자동으로 만들어집니다.

1. 다음 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">단순 증명</td> 
      <td>이 옵션은 워크플로가 첨부되지 않은 증명을 만들고 기본 증명 설정을 적용합니다. 기본 증명 설정을 업데이트하거나 증명을 만든 후 워크플로우를 추가할 수 있습니다. 증명 설정에 대한 자세한 내용은 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">증명 설정 편집</a>을 참조하세요.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">고급 증명</td> 
      <td> <p>이 옵션을 사용하면 기본 또는 고급 워크플로를 구성하고 만든 증명에 대한 증명 설정을 수정할 수 있습니다. 자세한 내용은 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">기본 워크플로를 사용하여 고급 증명 만들기</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">자동화된 워크플로로 고급 증명 만들기</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
