---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: ZIP 파일에 대화형 컨텐츠에 대한 증명 만들기
description: ZIP 파일에 저장된 비 웹 사이트 대화형 컨텐츠에 대한 증명을 생성할 수 있습니다. 이러한 유형의 웹 콘텐츠의 예에는 스트리밍 비디오 또는 오디오가 있는 광고, HTML 애니메이션 및 대화형 배너가 포함됩니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# ZIP 파일에 대화형 컨텐츠에 대한 증명 만들기

ZIP 파일에 저장된 비 웹 사이트 대화형 컨텐츠에 대한 증명을 생성할 수 있습니다. 이러한 유형의 웹 콘텐츠의 예에는 스트리밍 비디오 또는 오디오가 있는 광고, HTML 애니메이션 및 대화형 배너가 포함됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>표준</p>
   <p>작업 또는 계획</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## ZIP 파일에 대화형 컨텐츠에 대한 증명 만들기

ZIP 파일의 대화형 컨텐츠를 증명에 추가하면 Adobe Workfront에서 압축 문서의 증명을 만듭니다. 파일 크기에 따라 업로드 로드 시간이 달라질 수 있습니다. 파일이 클수록 만드는 데 시간이 오래 걸립니다. 페이지에서 멀리 탐색할 수 있으며 Workfront에서 파일을 계속 만듭니다. 최대 파일 업로드 크기는 4GB입니다. 

1. ZIP 번들 파일을 만들어 콘텐츠를 준비합니다.

   ZIP 파일은 다음 요구 사항을 충족해야 합니다.

   * CSS, JavaScript, 비디오, 사운드 및 이미지와 같은 모든 자산이 번들 파일에 포함되어야 합니다.
   * 기본 파일(예: index.html, index.htm)이 루트 폴더에 있고 .html/.htm 파일만 저장되어 있는지 확인합니다.

     주 파일이 루트 폴더에 배치되지 않은 경우 Workfront은 폴더를 검색하여 주 파일을 찾습니다.

   * 최대 번들 크기는 500MB입니다.
   * iOS에서 만든 ZIP 파일의 경우, 이 도구는 콘텐츠가 배치된 올바른 폴더를 자동으로 식별합니다.

1. ZIP 파일을 업로드할 프로젝트, 작업 또는 문제로 이동합니다.
1. 왼쪽 패널에서 **문서**&#x200B;를 클릭합니다.
1. 표시되는 메뉴에서 **새로 추가**&#x200B;를 클릭한 다음&#x200B;**증명**&#x200B;을 클릭합니다.
1. **파일 추가** 섹션에서 필요한 ZIP 파일을 끌어서 놓거나 찾아봅니다.
1. 검토 프로세스가 없는 간단한 증명을 만들려면 **증명 만들기**&#x200B;를 클릭하십시오.\
   또는\
   고급 증명을 구성하여 계속합니다.

   * [기본 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [자동화된 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
