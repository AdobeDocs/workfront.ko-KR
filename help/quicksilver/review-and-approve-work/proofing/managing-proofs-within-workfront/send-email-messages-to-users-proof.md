---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명에서 검토자에게 이메일 메시지 보내기
description: 검토 및 승인 프로세스 중에 증명에 대한 검토자 한 명 또는 모두에게 메시지를 보낼 수 있습니다. 메시지는 검토자에게 증명 검토를 완료하도록 알리거나 증명과 관련된 다른 정보를 제공하는 쉬운 방법입니다.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# 증명에서 검토자에게 이메일 메시지 보내기

검토 및 승인 프로세스 중에 증명에 대한 검토자 한 명 또는 모두에게 메시지를 보낼 수 있습니다. 메시지는 검토자에게 증명 검토를 완료하도록 알리거나 증명과 관련된 다른 정보를 제공하는 쉬운 방법입니다.

일반 미리 알림 이메일을 보내거나 사용자 지정된 메시지를 지정된 단계와 연관된 사용자 중 한 명 또는 모두에게 보낼 수 있습니다.

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
   <td role="rowheader">증명 역할</td> 
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

## 증명에서 사용자에게 이메일 메시지 보내기

1. 메시지를 보낼 사용자가 포함된 증명 문서를 찾습니다.
1. 문서 위로 마우스를 가져간 다음 **증명 워크플로**&#x200B;를 클릭합니다.

   ![증명 워크플로](assets/proof-workflow-doc-list-350x92.png)

1. 스테이지에 있는 모든 사용자에게 메시지를 보내려면 스테이지에서 **자세히** 메뉴를 클릭하고 **모두 메시지**&#x200B;를 선택하세요.

   ![스테이지에 있는 메시지](assets/message-stage-350x122.png)

1. 개별 사용자에게 메시지를 보내려면 사용자 옆에 있는 **자세히** 메뉴를 클릭하고 **메시지**&#x200B;를 선택하세요.

   ![메시지 사용자](assets/message-user-350x121.png)

1. **메시지 세부 정보** 섹션에서 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">사람들에게 이메일로 알림</td> 
      <td>이 옵션은 선택 취소할 수 없습니다. 모든 사용자는 이메일을 통해 메시지를 수신합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 지정 메시지 버리기</td> 
      <td> <p>기본 전자 메일 콘텐츠만 포함하려면 <strong>사용자 지정 메시지 버리기</strong>를 클릭하세요.</p> <p>기본 미리 알림 이메일에는 다음 정보가 포함됩니다.</p> 
       <ul> 
        <li>증명에 대한 개인 링크<br>증명 이미지의 썸네일<br></li> 
        <li>증명 이름, 버전 번호, 폴더 이름(해당하는 경우) 및 검토자 목록과 증명에 대한 진행 상황 등 증명 세부 정보.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">제목</td> 
      <td>메시지 제목을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">메시지</td> 
      <td>메시지 콘텐츠를 입력합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **보내기**&#x200B;를 클릭합니다.
