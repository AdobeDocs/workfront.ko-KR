---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 조직에 대한 증명 설정 구성
description: Adobe Workfront 관리자 또는 Workfront Proof 관리자는 조직의 기본 증명 설정을 사용자 지정할 수 있습니다. 이러한 설정에는 기본 공유 옵션, 브랜딩 등이 포함됩니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# 조직에 대한 증명 설정 구성

Adobe Workfront 관리자 또는 Workfront Proof 관리자는 조직의 기본 증명 설정을 사용자 지정할 수 있습니다. 이러한 설정에는 기본 공유 옵션, 브랜딩 등이 포함됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 플랜: Pro 이상</p> <p>또는</p> <p>기존 플랜: Premium 또는 선택</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>를 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>증명 권한 프로필에서 관리자를 선택해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">사용자의 증명 액세스 구성</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 작업 구성

증명 뷰어에서 작업을 사용하는 방법에 대한 자세한 내용은 [증명 댓글에 작업 사용](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)을 참조하십시오.

다음 방법으로 조직에 대한 작업을 구성할 수 있습니다.

* [작업 추가 또는 이름 바꾸기](#add-or-rename-an-action)
* [작업 비활성화 또는 다시 활성화](#deactivate-or-reactivate-an-action)
* [작업 순서 바꾸기](#reorder-actions)

### 작업 추가 또는 이름 바꾸기 {#add-or-rename-an-action}

{{step1-to-proofing}}

1. Workfront Proof 인터페이스의 오른쪽 상단에서 **설정** > **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 새 작업을 만들려면 **작업** 섹션에서 **새 작업**&#x200B;을 클릭하세요.

     계정에서 설정할 수 있는 작업 수에는 제한이 없습니다.

   * 기존 작업의 이름을 바꾸려면 작업 옆에 있는 **설정**&#x200B;을 클릭합니다.

1. 작업의 이름을 입력한 다음 **저장**&#x200B;을 클릭합니다.
1. **저장**&#x200B;을 클릭합니다.

### 작업 비활성화 또는 재활성화 {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}}

1. Workfront Proof 인터페이스의 오른쪽 상단에서 **설정** > **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.

1. 비활성화하거나 다시 활성화할 작업 옆에 있는 **설정**&#x200B;을 클릭합니다.
1. **활성화** 또는 **비활성화**&#x200B;를 선택한 다음 **저장**&#x200B;을 클릭합니다.

### 작업 순서 바꾸기 {#reorder-actions}

{{step1-to-proofing}}

1. Workfront Proof 인터페이스의 오른쪽 상단에서 **설정** > **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.

1. **설정** 옆에 있는 파란색 위쪽 및 아래쪽 화살표를 클릭하여 작업 순서를 변경합니다.

   ![Re-order_actions.png](assets/re-order-actions-350x103.png)

## 증명을 위한 맞춤형 디바이스 구성

사용자 정의 장치를 시스템에 추가하여 사용자가 대화형 콘텐츠를 검토하고 콘텐츠가 특정 장치에 표시되는 방식을 시뮬레이션할 수 있습니다.

사용자가 대화형 콘텐츠를 검토할 때 장치를 선택하는 방법에 대한 자세한 내용은 [증명 뷰어에서 대화형 증명 해상도 변경](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)을 참조하십시오.

사용자 지정 장치를 추가하려면:

{{step1-to-proofing}}

1. Workfront Proof 인터페이스의 오른쪽 상단에서 **설정** > **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.

1. **증명을 위한 사용자 지정 장치** 섹션에서 **새 장치 추가**&#x200B;를 클릭합니다.

1. 표시되는 **새 장치 추가** 상자에서 다음 정보를 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td><a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">증명 뷰어에서 대화형 증명 해상도 변경</a>에 설명된 대로 사용자가 데스크톱 증명 뷰어에서 장치를 선택할 때 표시되는 이름입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">차원</td> 
      <td>이 장치에 사용할 차원을 지정하십시오. 장치 이름 아래에 표시되는 차원이 사용자에게 표시됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">비율</td> 
      <td>장치의 비율을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">유형</td> 
      <td>장치가 모바일, 태블릿 또는 데스크톱인지 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 에이전트 문자열</td> 
      <td>장치에 대한 사용자 에이전트를 입력하여 소프트웨어를 장치에 맞게 실행하고 표시할 수 있도록 하는 정보를 제공합니다.<p>장치에서 <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a>로 이동하여 사용자 에이전트를 가져올 수 있습니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">비활성화됨</td> 
      <td>이 옵션을 선택하면 사용자가 대화형 증명을 검토할 때 장치를 선택할 수 없습니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Create**.

## 증명에 대한 팝업 메시지 구성

증명에 대한 팝업 메시지를 구성하여 조직의 모든 검토자에게 일반 정보를 전달할 수 있습니다.

다음과 같은 상황에서 메시지가 나타나도록 구성할 수 있습니다.

* **메시지 로드 시**: 증명을 처음 열 때 표시됩니다. 증명 검토 또는 면책조항 또는 기타 법적 고지 사항 제공 방법을 사용자에게 설명하는 데 유용합니다.
* **결정 메시지**: 사용자가 증명에서 결정을 선택할 때 표시됩니다. 브랜드 또는 규정 준수와 같은 항목에 대한 체크리스트를 사용자에게 제공하는 데 유용합니다. 결정에 대한 자세한 내용은 [증명 뷰어에서 증명 결정](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)을 참조하십시오.

* **단추 텍스트 확인**: 위에서 설명한 로드 시 팝업 메시지의 단추에 표시되는 레이블입니다.

증명에 대한 팝업 메시지를 만들려면 다음을 수행하십시오.

1. 사용자 지정할 메시지 오른쪽의 **편집**&#x200B;을 클릭합니다.
1. 메시지를 지정하고 적절한 서식을 포함한 다음 **저장**&#x200B;을 클릭합니다.
1. (선택 사항) [로드 시] 메시지를 사용자 지정하고 확인 단추 레이블도 사용자 지정하려면 **확인 단추 텍스트** 오른쪽에 있는 **편집**&#x200B;을 클릭하고 레이블을 지정한 다음 **저장**&#x200B;을 클릭합니다.

## 증명 기본값 구성

조직의 증명 기본값을 구성하는 방법에 대한 자세한 내용은 [기본 증명 설정 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)을 참조하십시오.


## 공유 기본값 구성

조직의 증명을 공유할 수 있는 사용자, 검토자가 사용할 수 있는 버전 및 자동화된 워크플로의 증명이 지정된 단계와 연결된 사용자에게 표시되는 시기를 지정할 수 있습니다.

Workfront Proof 내의 공유 설정에 대한 자세한 내용은 [사용자에 대한 공유 설정 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md)을 참조하십시오.

## Workfront Proof 사이트 브랜딩

Workfront Proof을 사용하는 경우 사이트의 다음 영역에 대한 브랜딩을 설정할 수 있습니다.

* 증명이 로드될 때 표시되는 스플래시 페이지
* 로그인 및 로그아웃 화면
* 이메일 알림

Workfront Proof 사이트를 브랜딩하는 방법에 대한 자세한 내용은 [Workfront Proof 사이트 브랜딩](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)을 참조하십시오.

## 고급 암호 설정 구성

>[!IMPORTANT]
>
>이 옵션은 레거시 Workfront 플랜에만 사용할 수 있습니다. Pro, Business 또는 Enterprise Workfront 플랜을 사용하는 경우 고급 암호 설정을 더 이상 구성할 수 없습니다.

**고급 암호 설정**&#x200B;에서 사용자의 암호 보안을 강화할 수 있습니다.

1. 구성할 설정 오른쪽의 **설정**&#x200B;을 클릭합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">최소 암호 길이</td> 
      <td>기본 Workfront Proof 암호 길이는 6자입니다. 조직의 정책에 따라 숫자를 늘릴 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>문자 혼합</strong> </td> 
      <td>사용자가 암호에 소문자, 대문자, 숫자 및 기호를 혼합하여 사용하도록 할 수 있습니다. 암호에 포함할 문자 수를 결정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>최대 문자 반복</strong> </td> 
      <td>각 사용자의 암호에 반복할 수 있는 문자 수를 지정할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">자동 암호 에이징</td> 
      <td>사용자가 암호를 정기적으로 변경하도록 강제합니다. 당신은 그들이 얼마나 자주 그렇게 할 것인지를 결정한다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>암호 반복 허용 안 됨</strong> </td> 
      <td>계정에서 허용되지 않는 암호 반복 횟수를 구성합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>프로필 잠금</strong> </td> 
      <td>지정한 로그인 시도 실패 횟수가 많으면 사용자를 계정에서 잠급니다. 또한 계정에 다시 액세스할 수 있을 때까지 기다려야 하는 시간을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">30일 후에도 암호가 재설정되지 않는 경우 사용자 잠금</td> 
      <td>사용자가 프로필 활성화 후 30일 이내에 초기 암호를 변경하지 않으면 계정이 잠깁니다.<br><p>계정 관리자는 시스템에서 자동으로 잠기는 사용자의 잠금을 해제(재활성화)할 수 있습니다. 이렇게 하면 암호를 변경하는 데 7일이 추가로 소요됩니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">120일 동안 비활성 상태인 경우 사용자 계정 잠금</td> 
      <td>사용자가 Workfront Proof 또는 로그인 필수 증명에 120일 동안 로그인하지 않으면 계정에서 잠깁니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>처음 로그인한 후 암호 변경</strong> </td> 
      <td>사용자가 처음 로그인한 후 임시 암호를 변경해야 합니다.<p>계정 관리자는 시스템에 의해 자동으로 잠긴 사용자의 잠금을 해제(재활성화)할 수 있습니다.</p><p>자세한 암호 정보는 <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Workfront Proof 로그인 및 암호 변경</a>을 참조하십시오.</p></td> 
     </tr> 
    </tbody> 
   </table>
