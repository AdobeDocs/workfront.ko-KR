---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 향상된 커넥터로 연결된 자산 증명
description: Experience Manager Assets에서 에셋을 연결한 후 증명을 생성하고 에셋에 주석을 검토하고 추가할 사용자를 할당할 수 있습니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 향상된 커넥터로 연결된 자산 증명

Experience Manager Assets에서 에셋을 연결한 후 증명을 생성하고 에셋에 주석을 검토하고 추가할 사용자를 할당할 수 있습니다. 연결된 자산에서 생성된 증명은 증명 저장소 할당량에 계산됩니다.

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
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>Experience Manager Assets Essentials가 있어야 합니다.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 권한 이상 보기</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다

* Workfront for Experience Manager 강화 커넥터 설치

## 증명 만들기

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

## 기존 증명 관리

증명을 만든 후에는 다음과 같은 작업을 수행할 수 있습니다.

* 현재 스테이지 활동 보기
* 검토자 및 기한 업데이트
* 워크플로우 편집

기존 증명을 관리하는 방법에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 관리](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md)를 참조하십시오.

## 증명 검토

할당된 검토자는 다음과 같은 작업을 수행할 수 있습니다.

* 에셋 보기 및 주석 달기
* 댓글에 작업 추가
* 버전 비교
* 증명 승인 또는 거부

증명 도구를 사용하여 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront에서 증명 검토](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)를 참조하십시오.
