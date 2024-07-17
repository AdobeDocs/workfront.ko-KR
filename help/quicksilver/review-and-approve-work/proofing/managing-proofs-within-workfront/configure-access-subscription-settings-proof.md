---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: 증명에 대한 액세스 및 구독 설정 구성
description: 사용자 로그인 필요 여부, 사용자 증명 구독 허용 여부 등 개별 증명에 대한 특정 액세스 및 구독 설정을 구성할 수 있습니다. 증명을 만드는 동안 증명에 대한 액세스 및 구독 설정을 설정하거나 Workfront에 이미 존재하는 증명에 대해 설정할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# 증명에 대한 액세스 및 구독 설정 구성

사용자 로그인 필요 여부, 사용자 증명 구독 허용 여부 등 개별 증명에 대한 특정 액세스 및 구독 설정을 구성할 수 있습니다. 증명을 만드는 동안 증명에 대한 액세스 및 구독 설정을 설정하거나 Workfront에 이미 존재하는 증명에 대해 설정할 수 있습니다.

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

## 증명을 만드는 동안 액세스 및 구독 설정 구성

증명을 만드는 동안 증명에 대한 액세스 및 구독 설정을 설정하려면 다음을 수행하십시오.

1. 증명을 원하는 프로젝트, 작업 또는 문제로 이동한 다음 **문서** 섹션을 클릭합니다.
1. 오른쪽 상단에서 **새로 추가**&#x200B;를 클릭합니다.
1. **새 증명** 페이지의 오른쪽 아래 모서리에 있는 **증명 설정** 섹션으로 스크롤합니다.

1. 다음 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>공개 URL 또는 포함 코드를 통한 증명 공유 허용</strong> </td> 
      <td>이 옵션을 선택하면 공용 URL 또는 포함 코드를 통해 증명을 공유할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>공개 URL 또는 포함 코드를 통한 증명 구독 허용</strong> </td> 
      <td>이 옵션을 선택하면 증명에 명시적으로 추가되지 않은 사람도 증명에 가입할 수 있습니다. 증명을 구독하는 사용자에게는 다음 설정에서 정의한 역할 및 이메일이 부여됩니다.
       <ul>
        <li><p><strong>구독자 역할:</strong> 증명을 구독하는 모든 검토자에게 할당된 기본 증명 역할입니다. </p><p>중요: <strong>공유 허용</strong>이(가) Workfront Proof 설정에서 <strong>모든 사용자</strong> 이외의 값으로 설정된 경우 구독은 조직 내 사용자에 대해서만 작동합니다. 자세한 내용은 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof에서 증명 설정 구성</a>을 참조하십시오.</p></li>
        <li><strong>구독자에 대한 전자 메일 경고 설정:</strong> 증명을 구독하는 모든 검토자에게 할당되는 기본 전자 메일 경고입니다.</li>
       </ul><p>
        <ul>
         <li><strong>전자 메일 링크를 통한 증명 액세스 필요:</strong> 구독자가 증명에 대한 링크가 포함된 전자 메일을 받는지 여부를 구성합니다. <strong>전자 메일 없음</strong>(증명에 액세스하는 데 전자 메일 링크가 필요하지 않음), <strong>증명 알림 전자 메일 전용</strong>(구독자가 확인 없이 전자 메일을 통해 증명에 대한 링크를 받음) 또는 <strong>확인 및 증명 알림 전자 메일</strong>(구독자가 전자 메일을 통해 증명에 대한 링크를 받고 증명에 액세스하려면 링크를 클릭해야 함)을 선택할 수 있습니다. 이 옵션의 목적은 해당 사용자가 액세스 권한이 있는 올바른 전자 메일 주소를 입력했는지 확인하는 것입니다.</li>
        </ul><p>참고:  증명에 자동화된 워크플로가 첨부된 경우 모든 구독은 증명 소유자에게 확인 이메일을 생성하므로 대상자를 추가해야 하는 단계를 결정할 수 있습니다.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 증명 만들기를 계속합니다.

## 기존 증명에 대한 액세스 및 구독 설정 구성

Workfront에 이미 존재하는 증명에 대한 액세스 및 구독 설정을 설정하려면:

1. 문서 영역에서 설정을 구성할 증명이 포함된 문서를 선택한 다음 **문서 세부 정보**&#x200B;를 클릭합니다.
1. 왼쪽 패널에서 **증명 뷰어 설정**&#x200B;을 클릭합니다.
1. 다음 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>공개 URL 또는 포함 코드를 통한 증명 공유 허용</strong><strong>e</strong> </td> 
      <td>이 옵션을 선택하면 공용 URL 또는 포함 코드를 통해 증명을 공유할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>공개 URL 또는 포함 코드를 통한 증명 구독 허용</strong> </td> 
      <td>이 옵션을 선택하면 증명에 명시적으로 추가되지 않은 사람도 증명에 가입할 수 있습니다. 증명을 구독하는 사용자에게는 다음 설정에서 정의한 역할 및 이메일이 부여됩니다.
       <ul>
        <li><p><strong>구독자 역할:</strong> 증명을 구독하는 모든 검토자에게 할당된 기본 증명 역할입니다. </p><p>중요: <strong>공유 허용</strong>이(가) Workfront Proof 설정에서 <strong>모든 사용자</strong> 이외의 값으로 설정된 경우 구독은 조직 내 사용자에 대해서만 작동합니다. 자세한 내용은 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof에서 증명 설정 구성</a>을 참조하십시오.</p></li>
        <li><strong>구독자에 대한 전자 메일 경고 설정:</strong> 증명을 구독하는 모든 검토자에게 할당되는 기본 전자 메일 경고입니다.</li>
       </ul><p>
        <ul>
         <li><strong>전자 메일 링크를 통한 증명 액세스 필요:</strong> 구독자가 증명에 대한 링크가 포함된 전자 메일을 받는지 여부를 구성합니다. <strong>전자 메일 없음</strong>(증명에 액세스하는 데 전자 메일 링크가 필요하지 않음), <strong>증명 알림 전자 메일 전용</strong>(구독자가 확인 없이 전자 메일을 통해 증명에 대한 링크를 받음) 또는 <strong>확인 및 증명 알림 전자 메일</strong>(구독자가 전자 메일을 통해 증명에 대한 링크를 받고 증명에 액세스하려면 링크를 클릭해야 함)을 선택할 수 있습니다. 이 옵션의 목적은 해당 사용자가 액세스 권한이 있는 올바른 전자 메일 주소를 입력했는지 확인하는 것입니다.</li>
        </ul><p>참고:  증명에 자동화된 워크플로가 첨부된 경우 모든 구독은 증명 소유자에게 확인 이메일을 생성하므로 대상자를 추가해야 하는 단계를 결정할 수 있습니다.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.
