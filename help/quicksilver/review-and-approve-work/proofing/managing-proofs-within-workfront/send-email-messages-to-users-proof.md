---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명 시 검토자에게 이메일 메시지 보내기
description: 검토 및 승인 프로세스 중에 한 명 또는 모든 검토자에게 증명으로 메시지를 보낼 수 있습니다. 메시지는 검토자에게 증명 검토를 완료하거나 증명과 관련된 기타 정보를 제공하도록 알리는 쉬운 방법입니다.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# 증명 시 검토자에게 이메일 메시지 보내기

검토 및 승인 프로세스 중에 한 명 또는 모든 검토자에게 증명으로 메시지를 보낼 수 있습니다. 메시지는 검토자에게 증명 검토를 완료하거나 증명과 관련된 기타 정보를 제공하도록 알리는 쉬운 방법입니다.

일반 미리 알림 전자 메일을 보내거나 지정된 스테이지와 연결된 사용자 중 하나 또는 모든 사용자에게 사용자 지정 메시지를 보내도록 선택할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Select 또는 Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
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

## 증명으로 사용자에게 이메일 메시지 보내기

1. 메시지를 표시할 사용자가 포함된 증명의 문서를 찾습니다.
1. 문서 위로 마우스를 가져간 다음 **교정 워크플로**.

   ![](assets/proof-workflow-doc-list-350x92.png)

1. 스테이지의 모든 사용자에게 메시지를 보내려면 **자세히** 스테이지의 메뉴 및 선택 **모두 메시지**.

   ![](assets/message-stage-350x122.png)

1. 개별 사용자에게 메시지를 보내려면 **자세히** 사용자 옆에 있는 메뉴를 선택하고 **메시지**.

   ![](assets/message-user-350x121.png)

1. 에서 **메시지 세부 사항** 섹션에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">전자 메일로 사람들에게 알림</td> 
      <td>이 옵션은 선택 취소할 수 없습니다. 모든 사용자는 이메일을 통해 메시지를 수신합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 지정 메시지 취소</td> 
      <td> <p>클릭 <strong>사용자 지정 메시지 취소</strong> 기본 이메일 콘텐츠만 포함하려는 경우.</p> <p>기본 미리 알림 전자 메일에는 다음 정보가 포함됩니다.</p> 
       <ul> 
        <li>증명에 대한 개인 링크<br>증명 이미지의 축소판<br></li> 
        <li>다음 증명 세부 정보: 증명 이름, 버전 번호, 폴더 이름(해당되는 경우) 및 검토자 목록과 증명 진행 상황.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">주제</td> 
      <td>메시지 제목을 입력합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">메시지</td> 
      <td>메시지 콘텐츠를 입력합니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **전송.**
