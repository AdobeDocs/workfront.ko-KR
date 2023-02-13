---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets 또는 Assets Essentials에 연결된 자산 증명
description: Experience Manager Assets Essentials에서 자산을 연결한 후 증명을 만들고 사용자에게 검토를 할당하고 자산에 주석을 추가할 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Experience Manager Assets 또는 Assets Essentials에 연결된 자산 증명

Experience Manager Assets Essentials에서 자산을 연결한 후 증명을 만들고 사용자에게 검토를 할당하고 자산에 주석을 추가할 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p> 모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>작업 이상</p>
   <p>사용자에 대해 언어 교정이 활성화되어 있어야 합니다.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager as a Cloud Service 또는 Assets Essentials이 있어야 하며 Admin Console에서 사용자로 제품에 추가되어야 합니다. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에

* Workfront 관리자가 Experience Manager 통합을 구성해야 합니다. 자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 또는 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 증명 만들기

정적, 비디오 또는 대화형 증명을 만들 수 있습니다.

증명을 작성하려면:

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 섹션을 참조하십시오.
1. 문서 위로 마우스를 가져간 다음 **증명 만들기** 문서 이름 아래에 표시되는 링크입니다.

   >[!NOTE]
   >
   >만약 **문서를 업로드할 때 증명을 자동으로 생성합니다** 사용자 프로필에서 활성화하면 시스템이 자동으로 간단한 증명을 만듭니다.

1. 다음 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>단순 증명</strong></td> 
      <td>이 옵션은 연결된 워크플로우가 없는 증명을 만들고 기본 증명 설정을 적용합니다. 증명을 만든 후 기본 교정 설정을 업데이트하거나 워크플로우를 추가할 수 있습니다. 증명 설정에 대한 자세한 내용은 <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">증명 설정 편집</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>고급 증명</strong></td> 
      <td> <p>이 옵션을 사용하면 기본 또는 고급 워크플로우를 구성하고 만든 증명의 증명 설정을 수정할 수 있습니다. 자세한 내용은 </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">기본 워크플로우를 사용하여 고급 증명 만들기</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">자동화된 워크플로우를 사용하여 고급 증명 만들기</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 기존 증명 관리

증명을 만들면 다음과 같은 작업을 수행할 수 있습니다

* 현재 단계 활동 보기
* 검토자 및 마감일 업데이트
* 워크플로우 편집

기존 증명을 관리하는 방법에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 관리](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## 증명 검토

지정된 검토자는 다음과 같은 작업을 수행할 수 있습니다

* 자산 보기 및 주석 만들기
* 주석에 작업 추가
* 버전 비교
* 증명 승인 또는 거부

교정 도구로 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 검토](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
