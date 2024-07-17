---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명에서 기본 워크플로를 자동화된 워크플로로 변환
description: 증명 소유자인 경우 기존 증명의 기본 워크플로를 자동화된 워크플로로 변환할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: c676c696-ab7d-415b-bf5e-5d0335a3920f
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 1%

---

# 증명에서 기본 워크플로를 자동화된 워크플로로 변환

증명 소유자인 경우 기존 증명의 기본 워크플로를 자동화된 워크플로로 변환할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 플랜: Pro 이상</p> <p>또는</p> <p>레거시 플랜: Premium</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
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
   <td> <p>문서에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

## 기본 워크플로우를 자동화된 워크플로우로 변환

1. 문서 목록에서 문서 위로 마우스를 가져간 다음 표시될 때 **증명 워크플로**&#x200B;를 클릭합니다.
1. Adobe Workfront의 오른쪽 상단 모서리에서 **자동 워크플로우로 전환**&#x200B;을 클릭합니다.
1. 화면 오른쪽 상단에서 **새 단계**&#x200B;를 클릭합니다.
1. 다음을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>이름</strong> </td> 
      <td>단계 이름을 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기한</strong> </td> 
      <td>마감일의 날짜를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p><strong>단계 활성화</strong> </p> </td> 
      <td>스테이지를 활성화할 시기를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기한 옵션</strong> </td> 
      <td>기한이 트리거되는 방식을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>단계 잠금</strong> </td> 
      <td>단계를 잠글지 여부를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 의사 결정자</strong> </td> 
      <td>기본 의사 결정자를 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>결정</strong> </td> 
      <td>하나의 결정만 필요한 경우 선택합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>개인 정보</strong> </td> 
      <td>스테이지가 비공개인 경우 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 추가</strong> </td> 
      <td>연락처 이름 또는 이메일 주소를 입력하고 증명 역할을 선택한 다음 이메일 경고를 구성합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **단계 추가**&#x200B;를 클릭합니다.
1. (선택 사항) 워크플로우가 만족스러울 때까지 3단계와 4단계를 반복합니다.
