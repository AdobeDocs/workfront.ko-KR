---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials에 대해 연결된 자산 증명
description: Experience Manager Assets Essentials의 에셋을 연결한 후에는 증명을 생성하고 에셋에 주석을 추가할 사용자를 할당할 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 1%

---

# Experience Manager Assets 또는 Assets Essentials에 대해 연결된 자산 증명

Experience Manager Assets Essentials의 에셋을 연결한 후에는 증명을 생성하고 에셋에 주석을 추가할 사용자를 할당할 수 있습니다.

## 액세스 요구 사항

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
   <td> <p>작업 이상</p>
   <p>사용자에 대한 증명이 활성화되어 있어야 합니다.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials이 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에,

* Workfront 관리자는 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

## 교정쇄 만들기

정적 증명, 비디오 증명 또는 대화형 증명을 만들 수 있습니다.

증명을 만들려면 다음 작업을 수행하십시오.

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
      <td role="rowheader"><strong>단순 증명</strong></td> 
      <td>이 옵션은 워크플로가 첨부되지 않은 증명을 만들고 기본 증명 설정을 적용합니다. 기본 증명 설정을 업데이트하거나 증명을 만든 후 워크플로우를 추가할 수 있습니다. 증명 설정에 대한 자세한 내용은 <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">증명 설정 편집</a>을 참조하세요.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>고급 증명</strong></td> 
      <td> <p>이 옵션을 사용하면 기본 또는 고급 워크플로를 구성하고 만든 증명에 대한 증명 설정을 수정할 수 있습니다. 자세한 내용은 </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">기본 워크플로를 사용하여 고급 증명 만들기</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">자동화된 워크플로로 고급 증명 만들기</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 기존 증명 관리

증명을 만든 후에는 다음과 같은 작업을 수행할 수 있습니다.

* 현재 스테이지 활동 보기
* 검토자 및 기한 업데이트
* 워크플로우 편집

기존 증명을 관리하는 방법에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 관리](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md)를 참조하십시오.

## 증명 검토

할당된 검토자는 다음과 같은 작업을 수행할 수 있습니다.

* 에셋 보기 및 주석 달기
* 댓글에 작업 추가
* 버전 비교
* 증명 승인 또는 거부

증명 도구를 사용하여 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront에서 증명 검토](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)를 참조하십시오.
