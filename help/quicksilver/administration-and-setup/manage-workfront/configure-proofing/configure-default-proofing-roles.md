---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 기본 언어 교정 역할 구성
description: Adobe Workfront 관리자는 Workfront에서 만든 증명에 액세스하는 사용자와 게스트 사용자에 대한 기본 교정 역할을 구성할 수 있습니다. 증명에 사용자를 추가하는 사람은 누구나 이러한 역할을 조정할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# 기본 언어 교정 역할 구성

Adobe Workfront 관리자는 Workfront에서 만든 증명에 액세스하는 사용자와 게스트 사용자에 대한 기본 교정 역할을 구성할 수 있습니다. 증명에 사용자를 추가하는 사람은 누구나 이러한 역할을 조정할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 기본 언어 교정 역할 구성

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. 클릭 **검토 및 승인** 왼쪽에 표시되는 목록의 맨 아래 근처에 있습니다.
1. 에서 **문서 증명 수신자의 역할** 섹션에서 증명의 워크플로우에 추가된 사용자와 게스트 사용자에 대한 기본 역할을 선택합니다.

   자세한 내용은 [언어 교정 역할과 관련된 권한](#rights-associated-with-proofing-roles) 아래에 각 교정 역할 및 이와 관련된 권한 목록이 표시됩니다.

   >[!NOTE]
   >
   >* 이 설정은 역할이 설정된 후 Workfront 시스템에서 생성된 사용자만 적용됩니다. 기존 사용자가 아님.
   >* 증명에 사용자를 추가하는 사람은 다음에 설명된 대로 이 역할을 조정할 수 있습니다. [증명에 사용자 추가](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Adobe Workfront에서 증명 공유](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. 에서 **문서 증명을 여는 비수신자를 위한 역할** 섹션에서 증명을 액세스할 수 있지만 증명의 워크플로우에 추가되지 않는 사용자 및 게스트 사용자에 대한 기본 역할을 선택합니다.

   이러한 상황은 사용자와 게스트가 증명서가 작성된 문서에 액세스할 때 발생합니다. 증명의 워크플로우에 추가되지 않았더라도 증명을 열 수 있습니다.

   **예:** 다음은 이 설정을 사용할 수 있는 방법의 예입니다.

   * 다음을 선택합니다 **읽기 전용** 댓글 추가 및 의사결정처럼 모든 증명 활동을 제한하는 것이 좋습니다.
   * 다음을 선택합니다 **검토자** 팀의 모든 구성원이 증명에 마크업과 주석을 추가할 수 있도록 하기 때문입니다.

1. **저장**&#x200B;을 클릭합니다.

## 언어 교정 역할과 관련된 권한 {#rights-associated-with-proofing-roles}

다음 표에는 각 역할 및 해당 역할과 연관된 권한이 표시됩니다.

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
   <th> <p><strong>답글이 없는 경우 댓글 편집</strong> </p> </th> 
   <th> <p><strong>결정</strong> </p> </th> 
   <th> <p><strong>다른 사람이 작성한 댓글 삭제</strong> </p> </th> 
   <th>댓글 해결</th> 
   <th>주석에 작업 적용</th> 
   <th> <p><strong>증명 편집</strong> </p> </th> 
   <th>다른 사람과 증명 공유</th> 
   <th>새 버전 만들기</th> 
   <th> <p><strong>홈 영역에서 승인 요청 보기</strong> </p> </th> 
   <th>새 검토자 추가</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>읽기 전용</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>검토자</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>승인자</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>검토자 및 승인자</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>작성자</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>중재자</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>새 Workfront 계획의 사용자는 시스템의 모든 사용자에게 작성자 또는 중재자 역할을 부여할 수 있습니다. 레거시 플랜의 사용자는 시스템에서 증명 라이센스를 가진 사용자에게 작성자 또는 중재자 역할을 부여할 수 있습니다.
