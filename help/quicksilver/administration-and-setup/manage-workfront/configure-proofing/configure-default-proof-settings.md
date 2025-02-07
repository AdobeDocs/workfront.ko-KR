---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 기본 증명 설정 구성
description: 이 설정을 사용하면 사용자가 만든 모든 새 증명에 적용되는 기본값을 설정할 수 있습니다. 그러나 사용자는 증명을 만들 때 이러한 설정 대부분을 무시할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 7%

---

# 기본 증명 설정 구성

이 설정을 사용하면 사용자가 만든 모든 새 증명에 적용되는 기본값을 설정할 수 있습니다. 그러나 사용자는 증명을 만들 때 이러한 설정 대부분을 무시할 수 있습니다.

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
   <td>
   <p>새로운 기능: 표준</p>
   또는
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>Workfront 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 새 증명 기본 설정 구성

{{step-1-to-setup}}

1. 왼쪽 패널에서 **증명** > **증명 설정**&#x200B;을 클릭합니다.
1. **새 증명 기본값** 섹션에서 다음 설정을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>수신자</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">로그인 필요</td> 
      <td> <p>검토자는 조직의 계정에서 만든 증명을 볼 수 있으려면 먼저 전자 메일과 암호를 사용하여 로그인해야 합니다. 활성화되면 사용자는 게스트 검토자와 증명을 공유할 수 없습니다.</p> <p><b>중요</b>: 활성화되면 새로 만든 모든 증명에 로그인해야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">새 버전의 원본 교정쇄에서 소유자 복사</td> 
      <td> <p>첫 번째 증명 버전의 소유자는 해당 증명 버전의 작성자에 관계없이 모든 연속 증명 버전의 소유자이기도 합니다. 이 설정은 기본적으로 활성화되어 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자가 증명 주석을 삭제할 수 있도록 허용</td> 
      <td>사용자는 자신의 주석을 삭제할 수 있습니다. 이 설정은 기본적으로 활성화되어 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">결정 시 전자 서명 필요 </td> 
      <td> <p>의사 결정자는 증명을 결정할 때 Workfront 로그인 자격 증명을 입력하라는 메시지가 표시됩니다.</p> <p><b>중요</b>: 활성화되면 사용자는 로그인 자격 증명이 없는 게스트 검토자와 증명을 공유할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>마감</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 기한 설정</td> 
      <td> <p>시스템은 자동화된 워크플로가 없는 계정의 모든 새 증명에 이 기한을 적용합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">증명이 위험 상태가 되기 전에 수신자에게 알림</td> 
      <td>위에 지정된 기한에 따라 증명이 위험 상태로 간주되기 전에 수신자에게 이메일을 통해 알립니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>이메일 알림</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">증명에 추가될 때 수신자에게 알림</td> 
      <td>수신자가 증명에 추가되면 이메일을 통해 알림을 받습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

## 증명 결정 구성

사용자는 검토 후 증명 결정을 사용하여 증명의 상태를 표시할 수 있습니다.

>[!NOTE]
>
>증명 결정 이면의 논리는 다양한 수준의 결정이 여러 개 있는 경우 증명 워크플로의 전체 상태를 계산하는 데 사용됩니다. &quot;승인됨&quot; 및 &quot;변경 사항과 함께 승인됨&quot; 결정은 자동 워크플로우의 다음 단계를 트리거합니다.

증명 결정을 구성하려면:

{{step-1-to-setup}}

1. 왼쪽 패널에서 **증명** > **증명 설정**&#x200B;을 클릭합니다.
1. **결정** 섹션에서 다음을 수행할 수 있습니다.

   1. **결정 이름 바꾸기**: 결정 상자 안의 텍스트를 클릭하고 새 결정 레이블을 입력하십시오.

      >[!TIP]
      >
      >결정의 이름을 바꿀 때 결정의 논리를 유지합니다. 예를 들어, 기본 [거부됨] 결정은 *새 버전이 필요합니다*(으)로 변경할 수 있지만 *프린터로 보내기*(으)로 변경하면 안 됩니다.

      ![결정 이름 바꾸기](assets/rename-decision-350x109.png)

   1. **결정 순서 다시 정렬**: 증명 뷰어에 표시하려는 순서대로 결정 상자를 드래그합니다.

      ![결정 이동](assets/move-decision-350x110.png)

   1. **결정 숨기기**: 결정 상자 위로 마우스를 가져간 후 오른쪽 상단의 숨기기 아이콘을 클릭합니다.

      ![결정 숨기기](assets/hide-decision-350x109.png)

1. (선택 사항) Workfront 기본값으로 돌아가려면 **기본값 복원**&#x200B;을 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.
