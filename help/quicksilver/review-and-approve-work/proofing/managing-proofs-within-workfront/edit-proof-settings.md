---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 증명 설정 편집
description: 증명을 만든 후 언제든지 증명 설정을 편집할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 2%

---

# 증명 설정 편집

증명을 만든 후 언제든지 증명 설정을 편집할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td role="rowheader">교정쇄 역할</td> 
   <td>작성자 또는 중재자</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## 증명 설정 편집

Workfront 관리자가 계정 수준에서 일부 설정을 사용하지 않도록 설정한 경우 일부 설정이 잠길 수 있습니다.

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 탭을 클릭합니다.
1. 증명을 마우스로 가리킨 다음 **문서 세부 정보**&#x200B;를 클릭합니다.
1. 왼쪽 패널에서 **증명 뷰어 설정**&#x200B;을 클릭합니다.
1. 다음 설정을 조정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">로그인 필요. 이 증명은 게스트 사용자와 공유할 수 없습니다.</td> 
      <td> <p>검토 및 승인 프로세스에 더 높은 수준의 보안이 필요한 경우 를 사용하여 증명에 로그인 요구 를 사용할 수 있습니다. 즉, Workfront 사용자만 증명에 추가할 수 있습니다. 액세스하려면 먼저 이메일과 암호를 입력해야 합니다.</p> <p>참고: <em style="font-style: normal;">로그인 필요 기능이 활성화된 경우 구독을 활성화할 수 없습니다.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정 시 전자 서명 필요</td> 
      <td> <p>증명에 대해 결정을 내리는 모든 검토자의 전자 서명이 필요할 수 있습니다. 검토자가 결정을 내리면 이메일 및 암호를 입력하고 결정을 확인하라는 메시지가 나타납니다. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">필요한 모든 결정을 내릴 때 증명 잠금</td> 
      <td> <p>최종 승인자가 결정을 내리면 증명 상태를 잠글 수 있습니다. 이 기능은 검토자가 증명으로 돌아가 추가 댓글을 추가하거나 결정을 변경할 수 없도록 하려는 경우 유용합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">원본 파일 다운로드 허용</td> 
      <td> <p>증명에 대한 검토자가 증명을 만든 원본 파일을 다운로드하도록 허용할 수 있습니다. 이 기능은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통한 증명 공유 허용</td> 
      <td>사용자가 공개 URL 또는 포함 코드와 증명을 공유하도록 할 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통한 증명 구독 허용</td> 
      <td> <p>증명에 대한 구독을 활성화하면 증명에 명시적으로 추가되지 않은 사람도 증명에 구독(즉, 증명에 자신을 추가)할 수 있습니다. 그런 다음 구독 설정에서 선택한 역할 및 이메일 알림이 할당됩니다.</p> <p>증명에서 구독을 활성화한 경우 아래 필드가 활성화됩니다.</p> 
       <ul> 
        <li><strong>구독자 유효성 검사 필요</strong> - 구독자가 증명에 액세스하려면 전자 메일의 링크를 클릭해야 함<br>이 옵션을 선택하면 구독하는 사람이 즉시 증명에 액세스하지는 않지만 전자 메일의 증명에 대한 링크를 받게 됩니다. 구독자 유효성 검사의 목적은 해당 사용자가 액세스할 수 있는 올바른 이메일 주소를 입력했는지 확인하는 것입니다.</li> 
        <li><strong>새 구독자의 기본 역할 -</strong> 증명에 자신을 구독하는 모든 검토자에게 할당되는 기본 증명 역할입니다.</li> 
        <li><strong>새 구독자에 대한 기본 전자 메일 경고</strong> - 증명에 자신을 구독하는 모든 검토자에게 할당되는 기본 전자 메일 경고입니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

 
