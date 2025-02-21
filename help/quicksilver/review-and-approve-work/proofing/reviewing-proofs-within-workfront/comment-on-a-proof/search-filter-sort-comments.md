---
product-area: documents
navigation-topic: comment-on-a-proof
title: 증명 주석 검색, 필터링 및 정렬
description: 증명 주석을 검색, 필터링 및 정렬하여 콘텐츠에 대한 피드백을 쉽게 탐색할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 03edaa7e-08c3-4ab1-83ab-747694cf1c17
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# 증명 주석 검색, 필터링 및 정렬

증명 주석을 검색, 필터링 및 정렬하여 콘텐츠에 대한 피드백을 쉽게 탐색할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 플랜: Pro 이상</p> <p>또는</p> <p>기존 플랜: Select 또는 Premium</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## 댓글 목록 검색

주석 목록에서 주석 자체에 포함된 텍스트, 주석 번호 또는 주석을 작성한 사용자를 검색할 수 있습니다.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.
1. 필요한 증명을 찾은 다음 **증명 열기**&#x200B;를 클릭합니다.

1. (조건부) 댓글 영역이 열려 있지 않으면 오른쪽 상단의 **댓글 보기**&#x200B;를 클릭합니다.
1. **검색** 아이콘을 클릭하여 검색 상자를 표시합니다.

1. 다음 중 하나를 입력하십시오.

   * 검색할 텍스트입니다. 주석 목록은 사용자가 입력하는 첫 번째 문자부터 필터링됩니다.
   * 표시할 주석의 번호입니다.
   * 댓글을 작성한 사용자입니다.

1. (선택 사항) 설명을 증명 관련 영역에 연결하는 줄을 표시하려면 설명을 클릭합니다.
1. 검색을 마치고 모든 주석을 표시하려면 검색 상자 끝에 있는 X를 클릭합니다.

## 주석 목록 필터링

사용자, 작업, 읽지 않음 상태 등과 같은 필터 매개 변수를 정의하여 표시되는 주석을 필터링할 수 있습니다.

1. 댓글을 필터링할 증명을 엽니다.
1. (조건부) 댓글 영역이 열려 있지 않으면 오른쪽 상단의 **댓글 보기**&#x200B;를 클릭합니다.
1. 설명 영역에서 **필터** 아이콘을 클릭합니다.

   ![proof_comment_filter.png](assets/proof-comment-filter.png)

1. **필터** 아이콘 아래에 표시되는 옵션을 사용하여 다음 기준으로 주석을 필터링합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>작성자</strong> </td> 
      <td>지정한 사용자가 작성한 댓글 및 댓글 답장만 표시합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>작업</strong> </td> 
      <td>선택한 작업과 일치하는 주석만 표시합니다. 작업이 없습니다. 시스템에서 작업을 활성화해야 합니다. 자세한 내용은 를 참조하십시오.<!--
        &nbsp;
       --></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>일반 필터링 옵션</strong> </td> 
      <td> 
       <ul> 
        <li><strong>해결되지 않음</strong>: 아직 해결되지 않은 주석만 표시합니다. </li> 
        <li><strong>읽지 않음</strong>: 아직 읽지 않은 댓글만 표시합니다. </li> 
        <li><strong>첨부 파일 사용</strong>: 첨부 파일이 포함된 댓글이나 첨부 파일이 포함된 답글이 포함된 댓글만 표시합니다.</li> 
        <li><strong>현재 페이지만</strong>:현재 보고 있는 페이지의 주석만 표시합니다. 표시되는 페이지를 변경하면 댓글 목록이 새로 고침됩니다. 정적 및 대화형 증명에만 사용할 수 있습니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 필터 기준이 적용된 댓글 목록을 보려면 **적용**&#x200B;을 클릭하거나 **필터** 아이콘을 클릭하십시오. 필터 아이콘에 필터가 적용되었음을 나타내는 파란색 점이 표시됩니다.

1. 필터링을 마치고 모든 댓글을 보려면 **필터** 아이콘을 클릭하고 **재설정**&#x200B;을 클릭한 다음 **필터** 아이콘을 다시 클릭합니다.

## 주석 목록 정렬

주석 목록을 정렬할 때 선택한 정렬 옵션은 다음에 사용 중인 증명 뷰어에서 증명을 열 때 기억됩니다.

1. 댓글을 정렬할 증명을 엽니다.
1. 댓글 영역이 열려 있지 않으면 오른쪽 상단의 **댓글 보기**&#x200B;를 클릭합니다.

1. 정렬 메뉴를 클릭하여 엽니다.
1. ![정렬 메뉴](assets/mceclip3.png)

1. 다음 정렬 옵션 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">끝</td> 
      <td>주석 목록의 맨 위에 가장 최근 주석을 표시합니다.</td> 
      <td>모든 증명에 사용 가능</td> 
     </tr> 
     <tr> 
      <td role="rowheader">가장 오래된</td> 
      <td>주석 목록의 맨 위에 가장 오래된 주석을 표시합니다. 이것이 기본값입니다. </td> 
      <td>모든 증명에 사용 가능</td> 
     </tr> 
     <tr> 
      <td role="rowheader">크리에이터 A-Z</td> 
      <td>댓글을 작성한 사용자별로 그룹화된 댓글을 알파벳순으로 표시합니다.</td> 
      <td>모든 증명에 사용 가능</td> 
     </tr> 
     <tr> 
      <td role="rowheader">작성자 Z-A</td> 
      <td>댓글을 작성한 사용자별로 그룹화된 댓글을 알파벳 역순으로 표시합니다.</td> 
      <td>모든 증명에 사용 가능</td> 
     </tr> 
     <tr> 
      <td role="rowheader">페이지(아래로, 위로)</td> 
      <td>페이지 번호 또는 비디오 타임라인과 관련하여 댓글이 표시되는 순서대로 표시합니다. </td> 
      <td>정적 증명에만 사용할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임스탬프(작동 중지)</td> 
      <td>비디오 타임라인과 관련하여 댓글이 표시되는 순서대로 표시합니다. 타임라인에서 나중에 작성한 댓글이 먼저 표시됩니다. </td> 
      <td>비디오 증명에만 사용할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타임스탬프(위쪽)</td> 
      <td>비디오 타임라인과 관련하여 댓글이 표시되는 순서대로 표시합니다. 타임라인에서 이전에 만든 주석이 먼저 표시됩니다. </td> 
      <td>비디오 증명에만 사용할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">장치(위)</td> 
      <td>댓글이 작성되었을 때 선택한 장치에 따라 댓글을 순서대로 표시합니다. 낮은 해상도의 주석이 먼저 표시됩니다.</td> 
      <td>대화형 증명에만 사용할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">장치(작동 중지)</td> 
      <td> <p>(대화형 증명에만 사용할 수 있습니다.) 댓글이 작성되었을 때 선택한 해결 방법에 따라 댓글을 순서대로 표시합니다. 높은 해상도의 주석이 먼저 표시됩니다.</p> <p>대화형 증명에서 해상도를 변경하는 방법에 대한 자세한 내용은 <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">증명 뷰어에서 대화형 증명 해상도 변경</a>을 참조하십시오.</p> </td> 
      <td>대화형 증명에만 사용할 수 있습니다.</td> 
     </tr> 
    </tbody> 
   </table>
