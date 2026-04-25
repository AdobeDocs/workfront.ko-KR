---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials에 대해 연결된 에셋 증명
description: Experience Manager Assets Essentials의 에셋을 연결한 후에는 증명을 생성하고 에셋에 주석을 추가할 사용자를 할당할 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 6%

---

# Experience Manager Assets 또는 Assets Essentials에 대해 연결된 에셋 증명

Experience Manager Assets Essentials의 에셋을 연결한 후에는 증명을 생성하고 에셋에 주석을 추가할 사용자를 할당할 수 있습니다.

>[!NOTE]
>
>이 기능은 새 문서 영역에서 사용할 수 없습니다.<br>
>조직에서 엔터프라이즈 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. 거기에서 Experience Manager Assets의 에셋을 추가하고 Frame.io 뷰어로 검토하고 승인할 수 있습니다. 자세한 내용은 [Frame.io 통합에 Adobe Experience Manager 사용](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)을 참조하십시오.

## 액세스 요구 사항

<!-- Audited: 4/2025 -->

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>표준</p>
   <p>작업 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">추가 제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials가 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

시작하기 전에:

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

## 교정쇄 만들기

정적 증명, 비디오 증명 또는 대화형 증명을 만들 수 있습니다.

증명을 만들려면 다음 작업을 수행하십시오.

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 섹션을 클릭합니다.
1. 문서 위로 마우스를 가져간 다음 문서 이름 아래에 나타나는 **증명 만들기** 링크를 클릭합니다.

   >[!NOTE]
   >
   >사용자 프로필에 **문서를 업로드할 때 자동으로 증명 생성**&#x200B;이 활성화되어 있으면 간단한 증명이 자동으로 만들어집니다.

1. 드롭다운에서 다음 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>단순 증명</strong></td> 
      <td>This option creates a proof with no workflow attached and applies the default proof settings. You can update the default proof settings or add a workflow after you've created the proof. For more information on proof settings, see <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Edit proof settings</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Advanced Proof</strong></td> 
      <td> <p>This option allows you to configure a Basic or Advanced workflow and modify proof settings for the proof you create. 자세한 내용은 다음 문서를 참조하십시오. </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Create an advanced proof with a Basic workflow</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Create an advanced proof with an Automated workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Manage an existing proof

Once you&#39;ve created a proof, you can do the following:

* View current stage activity
* Update reviewers and deadlines
* Edit the workflow

For more information about how to manage an existing proof, see [Manage proofs within Adobe Workfront: article index](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## 교정쇄 검토

Assigned reviewers can do the following:

* View the asset and make comments
* Add actions to comments
* Compare versions
* Approve or reject the proof

For more information about what you can do with the proofing tool, see [Review proofs within Adobe Workfront: article index](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
