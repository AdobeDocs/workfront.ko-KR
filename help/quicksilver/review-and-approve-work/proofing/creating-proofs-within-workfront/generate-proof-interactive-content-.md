---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: ZIP 파일에서 대화형 컨텐츠에 대한 증명 만들기
description: ZIP 파일에 저장된 웹 사이트가 아닌 대화형 컨텐츠에 대한 증명을 생성할 수 있습니다. 이러한 유형의 웹 콘텐츠의 예로는 스트리밍 비디오 또는 오디오가 포함된 광고, HTML 애니메이션, 대화형 배너 등이 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# ZIP 파일에서 대화형 컨텐츠에 대한 증명 만들기

ZIP 파일에 저장된 웹 사이트가 아닌 대화형 컨텐츠에 대한 증명을 생성할 수 있습니다. 이러한 유형의 웹 콘텐츠의 예로는 스트리밍 비디오 또는 오디오가 포함된 광고, HTML 애니메이션, 대화형 배너 등이 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">증명 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## ZIP 파일에서 대화형 컨텐츠에 대한 증명 만들기

ZIP 파일에 대화형 컨텐츠를 증표에 추가하면 Adobe Workfront은 압축된 문서의 증명을 만듭니다. 파일 크기에 따라 업로드 로드 시간이 달라질 수 있습니다. 더 큰 파일을 만드는 데 시간이 더 오래 걸립니다. 페이지에서 멀리 이동할 수 있으며 Workfront에서 계속해서 파일을 생성합니다. 최대 파일 업로드 크기는 4GB입니다. 

1. ZIP 번들 파일을 만들어 컨텐츠를 준비합니다.

   ZIP 파일은 다음 요구 사항을 충족해야 합니다.

   * CSS, JavaScript, 비디오, 사운드 및 이미지와 같은 모든 자산은 번들 파일에 포함되어야 합니다.
   * 기본 파일(예: index.html, index.htm)이 루트 폴더에 있고 이 파일이 폴더에 저장된 유일한 .html/.htm 파일인지 확인하십시오.

      기본 파일이 루트 폴더에 없는 경우 Workfront은 폴더를 검색하여 기본 파일을 찾습니다.

   * 최대 번들 크기는 500MB입니다.
   * iOS에서 만든 ZIP 파일의 경우, 도구는 컨텐츠가 배치되는 올바른 폴더를 자동으로 식별합니다.

1. ZIP 파일을 업로드할 프로젝트, 작업 또는 문제로 이동합니다.
1. 클릭 **문서** 왼쪽 패널에서 을 클릭합니다.
1. 클릭 **새로 추가**&#x200B;를 클릭한 다음&#x200B;**증명** 나타납니다.
1. 에서 **파일 추가** 섹션에서 필요한 ZIP 파일을 끌어다 놓거나 찾습니다.
1. 클릭 **증명 만들기** 검토 프로세스 없이 간단한 증명을 만들 수 있습니다.\
   또는\
   고급 증명을 구성하여 계속합니다.

   * [기본 워크플로우를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [자동화된 워크플로우를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
