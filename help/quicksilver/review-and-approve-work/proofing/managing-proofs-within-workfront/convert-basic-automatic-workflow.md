---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 기본 워크플로우를 증명의 자동화된 워크플로우로 변환합니다
description: 증명 소유자인 경우 기존 증명의 기본 워크플로우를 자동화된 워크플로우로 변환할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: c676c696-ab7d-415b-bf5e-5d0335a3920f
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 3%

---

# 기본 워크플로우를 증명의 자동화된 워크플로우로 변환합니다

증명 소유자인 경우 기존 증명의 기본 워크플로우를 자동화된 워크플로우로 변환할 수 있습니다.

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

## 기본 워크플로우를 자동화된 워크플로우로 변환

1. 문서 목록에서 문서 위로 마우스를 가져간 다음 **교정 워크플로** 표시됩니다.
1. Adobe Workfront의 오른쪽 위 모서리 근처에 있는 **자동화된 워크플로우로 변환**.
1. 클릭 **새 단계** 화면 오른쪽 상단 모서리에서 을(를) 클릭합니다.
1. 다음을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>이름</strong> </td> 
      <td>스테이지의 이름을 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>마감</strong> </td> 
      <td>마감일 날짜를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p><strong>단계 활성화</strong> </p> </td> 
      <td>스테이지를 활성화할 시기를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>최종 기한 옵션</strong> </td> 
      <td>마감일이 트리거되는 방식을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>스테이지 잠금</strong> </td> 
      <td>스테이지를 잠가야 할지 여부를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>주요 의사 결정자</strong> </td> 
      <td>기본 의사 결정자를 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>결정</strong> </td> 
      <td>하나의 결정만 필요한 경우 선택합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>개인 정보 보호</strong> </td> 
      <td>스테이지가 비공개 상태인지 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 추가</strong> </td> 
      <td>연락처 이름 또는 전자 메일 주소를 입력하고 증명 역할을 선택한 다음 전자 메일 경고를 구성합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **단계 추가**.
1. (선택 사항) 워크플로우가 만족될 때까지 3단계와 4단계를 반복합니다.
