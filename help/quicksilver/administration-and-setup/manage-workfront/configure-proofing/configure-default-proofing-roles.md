---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 기본 증명 역할 구성
description: Adobe Workfront 관리자는 Workfront에서 생성된 증명에 액세스하는 사용자 및 게스트 사용자에 대한 기본 증명 역할을 구성할 수 있습니다. 증명에 사용자를 추가하는 모든 사람은 이러한 역할을 조정할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 2%

---

# 기본 교정 역할 구성하기

Adobe Workfront 관리자는 Workfront에서 생성된 증명에 액세스하는 사용자 및 게스트 사용자에 대한 기본 증명 역할을 구성할 수 있습니다. 증명에 사용자를 추가하는 모든 사람은 이러한 역할을 조정할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 기본 교정 역할 구성하기

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. 왼쪽에 표시되는 목록의 맨 아래에 있는 **검토 및 승인**&#x200B;을 클릭합니다.
1. **문서 증명의 지정된 수신자를 위한 역할** 섹션에서 증명의 워크플로에 추가된 사용자 및 게스트 사용자에 대한 기본 역할을 선택하십시오.

   각 증명 역할과 관련된 권한 목록을 보려면 아래의 [증명 역할과 관련된 권한](#rights-associated-with-proofing-roles)을 참조하십시오.

   >[!NOTE]
   >
   >* 이 설정은 역할이 설정된 후 Workfront 시스템에서 생성된 사용자에게만 적용되며 기존 사용자에게는 적용되지 않습니다.
   >* 증명에 사용자를 추가하는 사용자는 [Adobe Workfront 내에서 증명 공유](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)의 [증명에 사용자 추가](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add)에 설명된 대로 이 역할을 조정할 수 있습니다.

1. **문서 증명을 여는 수신자가 아닌 사용자를 위한 역할** 섹션에서 증명에 액세스할 수 있지만 증명의 워크플로에 추가되지 않은 사용자 및 게스트 사용자에 대한 기본 역할을 선택합니다.

   이 상황은 사용자와 게스트가 증명을 만든 문서에 액세스할 때 발생합니다. 증명의 워크플로에 추가되지 않았더라도 증명을 열 수 있습니다.

   **예:** 이 설정을 사용하는 방법에 대한 예는 다음과 같습니다.

   * 댓글 추가 및 의사 결정과 같은 모든 증명 활동을 제한하려면 **읽기 전용**&#x200B;을 선택합니다.
   * 팀의 모든 구성원이 증명에 마크업과 주석을 추가할 수 있도록 하려면 **검토자**&#x200B;를 선택합니다.

1. **저장**&#x200B;을 클릭합니다.

## 증명 역할과 관련된 권한 {#rights-associated-with-proofing-roles}

다음 표는 각 역할과 그에 연결된 권한을 보여 줍니다.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>증명 보기</strong> </p> </th> 
   <th> <p><strong>마크업 추가</strong> </p> </th> 
   <th> <p><strong>댓글 추가</strong> </p> </th> 
   <th> <p><strong>답글이 없으면 댓글 편집</strong> </p> </th> 
   <th> <p><strong>결정</strong> </p> </th> 
   <th> <p><strong>다른 사용자가 작성한 댓글 삭제</strong> </p> </th> 
   <th>댓글 확인</th> 
   <th>댓글에 작업 적용</th> 
   <th> <p><strong>증명 편집</strong> </p> </th> 
   <th>다른 사용자와 증명 공유</th> 
   <th>새 버전 만들기</th> 
   <th> <p><strong>홈 영역에서 승인 요청 보기</strong> </p> </th> 
   <th>새 검토자 추가</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>읽기 전용</strong> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ 덧신</td> 
   <td> <p> </p> </td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>검토자</strong> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ 덧신</td> 
   <td> <p> </p> </td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>승인자</strong> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ 덧신</td> 
   <td> <p> </p> </td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>검토자 및 승인자</strong> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓ 덧신</td> 
   <td> <p> </p> </td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>작성자</strong> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p> </p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> <p>✓ 덧신</p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> </td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td> <p><strong>중재자</strong> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ <strong>개</strong> </p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> </td> 
   <td> <p>✓ 덧신</p> <p> </p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td> <p>✓ 덧신</p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>새 Workfront 플랜의 사용자는 시스템의 모든 사용자에게 작성자 또는 중재자 역할을 부여할 수 있습니다. 기존 플랜의 사용자는 시스템에서 증명 라이선스가 있는 모든 사용자에게 작성자 또는 중재자 역할을 부여할 수 있습니다.
