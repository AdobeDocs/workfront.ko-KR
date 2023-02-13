---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 증명 설정 편집
description: 증명을 만든 후 언제든지 증명 설정을 편집할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 2%

---

# 증명 설정 편집

증명을 만든 후 언제든지 증명 설정을 편집할 수 있습니다.

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
   <td role="rowheader">증명 역할</td> 
   <td>작성자 또는 중재자</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 증명 설정 편집

일부 설정은 Workfront 관리자가 계정 수준에서 비활성화한 경우 잠길 수 있습니다.

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 탭.
1. 증명 위로 마우스를 가져간 다음 **문서 세부 정보**.
1. 왼쪽 패널에서 **언어 교정 뷰어 설정**.
1. 다음 설정을 조정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">로그인 필요. 게스트 사용자와 이 증명을 공유할 수 없습니다.</td> 
      <td> <p>검토 및 승인 프로세스에 더 높은 수준의 보안이 필요한 경우, 증명에 로그인해야 할 수 있습니다. 즉, Workfront 사용자만 증표에 추가할 수 있습니다. 전자 메일 및 암호를 입력해야 액세스할 수 있습니다.</p> <p>참고: <em style="font-style: normal;">로그인 필요 를 활성화하면 가입을 활성화할 수 없습니다.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정 시 전자 서명 필요</td> 
      <td> <p>증명의 결정을 내리는 검토자의 전자 서명이 필요할 수 있습니다. 검토자가 결정을 내리면 이메일과 암호를 입력하고 결정을 확인하라는 메시지가 나타납니다. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">필요한 모든 결정을 내릴 때 증명 잠금</td> 
      <td> <p>최종 승인자가 결정을 내릴 때 잠그도록 증명 상태를 설정할 수 있습니다. 이 기능은 검토자가 증명으로 돌아가서 추가 주석을 추가하거나 결정을 변경할 수 없도록 하려면 유용합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">원본 파일 다운로드 허용</td> 
      <td> <p>증명의 검토자가 증명을 만든 원본 파일을 다운로드하도록 허용할 수 있습니다. 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통해 증명 공유 허용</td> 
      <td>사용자가 공개 URL 또는 포함 코드와 증명을 공유할 수 있도록 허용할 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">공개 URL 또는 포함 코드를 통해 증명 구독 허용</td> 
      <td> <p>증명에 구독을 활성화하면 증명에 명시적으로 추가되지 않은 사람이 증명에 자신을 구독(예: 증명에 추가)할 수 있습니다. 그러면 가입 설정에서 해당 역할에 대해 선택하는 역할 및 이메일 경고가 할당됩니다.</p> <p>증명에서 구독을 활성화하면 아래 필드가 활성화됩니다.</p> 
       <ul> 
        <li><strong>구독자 유효성 검사 필요</strong> - 가입자는 이메일의 링크를 클릭해야 증명 정보에 액세스할 수 있습니다<br>이 옵션을 선택하면 구독하는 사람이 증명을 즉시 액세스할 수 없지만 이메일에 있는 증명에 대한 링크를 받게 됩니다. 가입자 유효성 검사의 목적은 사용자가 액세스할 수 있는 올바른 이메일 주소를 입력했는지 확인하는 것입니다.</li> 
        <li><strong>새 구독자에 대한 기본 역할 -</strong> 이는 증명에 구독하는 모든 검토자에게 할당되는 기본 증명 역할입니다.</li> 
        <li><strong>새 구독자에 대한 기본 이메일 경고</strong> - 이 경고는 증명에 가입하는 모든 검토자에게 할당되는 기본 이메일 경고입니다.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

 
