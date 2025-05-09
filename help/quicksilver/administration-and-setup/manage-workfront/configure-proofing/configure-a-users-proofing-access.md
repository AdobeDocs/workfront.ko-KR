---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: 사용자의 증명 액세스 구성
description: Adobe Workfront 관리자 또는 Workfront Proof 관리자는 Workfront 및 Workfront Proof에서 증명을 만들고 보기 위한 사용자 액세스를 구성할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# 사용자의 증명 액세스 구성

Adobe Workfront 관리자 또는 Workfront Proof 관리자는 Workfront 및 Workfront Proof에서 증명을 만들고 보기 위한 사용자 액세스를 구성할 수 있습니다.

기본 및 통합 교정에 사용할 수 있는 증명 기능에 대한 자세한 내용은 [Workfront의 증명 기능에 액세스](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)를 참조하십시오.

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
   <td> <p>Workfront 관리자 또는 Workfront Proof 관리자여야 합니다. Workfront 관리자에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 사용자에 대한 증명 활성화 및 비활성화(기존 계획만 해당) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

조직에서 Workfront 관리자로서 레거시 Select 또는 Premium Workfront 계획을 사용하는 경우 사용자에 대한 증명 기능을 활성화하거나 비활성화할 수 있습니다.

사용자에 대한 증명을 활성화하면 Workfront에서 사용자의 증명이 자동으로 생성되는 옵션을 활성화합니다.

사용자를 증명 사용자로 활성화할 수 있지만, Workfront 기본 메뉴에서 Workfront Proof 인터페이스로 직접 이동하려면 관리자 권한이 있어야 합니다. Workfront 시스템의 모든 증명 사용자에 대해 이 옵션을 활성화하는 방법에 대한 자세한 내용은 [모든 사용자에 대한 Workfront 주 메뉴를 통해 Workfront Proof 액세스 구성](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users)을 참조하십시오.

1. **기본 메뉴**&#x200B;에서 **사용자**&#x200B;를 선택합니다.

1. 사용자를 선택한 다음 **편집** 아이콘을 클릭합니다.
1. **액세스** 섹션에서 **사용자가 증명을 생성할 수 있음**&#x200B;을(를) 선택하거나 선택 취소합니다.

## 사용자의 증명 권한 프로필 구성

선택한 권한 프로필은 조직 내에 있는 각 증명에 대해 사용자에게 부여됩니다.

{{step-1-to-users}}

1. 사용자를 한 명 이상 선택한 다음 **편집**&#x200B;을 클릭합니다.

1. **액세스** 섹션에서 **증명 권한 프로필** 드롭다운 메뉴에서 다음 Workfront Proof 권한 옵션 중 하나를 클릭합니다.

   >[!NOTE]
   >
   >기존 Workfront 플랜을 사용하는 경우 [사용자에 대한 증명 활성화 및 비활성화(기존 플랜만 해당)](#enable-and-disable-proofing-for-a-user-legacy-plans-only) 섹션에 설명된 대로 **사용자가 증명을 생성할 수 있음** 옵션이 활성화되어 있는지 확인하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>감독자</strong> </td> 
      <td>사용자는 조직의 계정에서 만든 모든 증명을 관리하고 볼 수 있습니다. 또한 이러한 증명에 추가된 검토자를 편집할 수도 있습니다. 이 권한 프로필이 있는 사용자는 사용자를 관리하거나 Workfront Proof 설정을 편집할 수 없습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>관리자</strong> </td> 
      <td> <p> 사용자는 조직의 계정에서 만들거나 소유한 증명을 관리하고 볼 수 있습니다. 검토자로 추가된 경우에만 다른 사용자의 증명을 볼 수 있습니다. 기본 설정입니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>관리자</strong> </td> 
      <td> 사용자에게 Workfront Proof의 관리자 권한이 부여되고 계정 설정을 편집할 수 있습니다. 사용자는 조직의 계정에서 만든 모든 증명을 관리하고 볼 수 있습니다. 여기에는 검토자, 증명 및 주석 추가 및 제거가 포함됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>사용자 지정</strong> </td> 
      <td> <p>Workfront Proof 내에서 사용자 지정 권한 프로필을 구성한 경우에만 사용할 수 있습니다.</p> <p><b>참고</b>:  <p>여기서 부여하는 권한 프로필이 Workfront의 사용자 액세스 수준 설정보다 높은 액세스 권한을 제공하지 않는지 확인하십시오(<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a> 참조). 더 높은 액세스 권한을 제공하는 경우 사용자는 Workfront Proof 내에서 액세스할 수 없는 Workfront 내의 증명에 액세스할 수 있습니다.</p> <p><a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Adobe Workfront에서 Workfront Proof 액세스</a>에 설명된 대로 모든 Workfront 사용자가 Workfront에서 직접 Workfront Proof에 액세스할 수 있도록 허용하려는 경우 특히 중요합니다.</p> <p>기본적으로 Workfront 관리자만 Workfront 전역 탐색 모음에서 Workfront Proof 사이트로 연결되는 직접 링크에 액세스할 수 있습니다.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   선택한 권한 프로필은 조직 내에 있는 각 증명에 대해 사용자에게 부여됩니다.

1. 사용자 설정에 대한 업데이트를 완료하려면 **변경 내용 저장**&#x200B;을 클릭하세요.

   >[!NOTE]
   >
   >Workfront에서 사용자를 만들거나 업데이트하고 사용자의 Workfront 이메일 주소가 라이선스가 있는 Workfront Proof 사용자의 이메일 주소와 일치하면 Workfront 내에서 해당 사용자에 대한 증명이 활성화됩니다. 자세한 내용은 [Adobe Workfront과 Workfront Proof 간의 사용자 동기화](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md)를 참조하십시오.

### 고려 사항

권한을 설정할 때 다음 정보를 고려하십시오.

* 사용자의 권한 프로필을 사용 권한이 적은 프로필로 변경하면 사용자가 Workfront 내의 기존 증명을 볼 수 없게 됩니다. 이 문제는 누군가가 Workfront 내의 사용자와 작업을 공유하지만 작업에 첨부된 증명을 공유하지 않을 때 발생할 수 있습니다([Adobe Workfront 내에서 증명 공유](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)에서 [Adobe Workfront 내에서 증명 공유](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) 참조).
* Workfront 환경이 Workfront Proof Premium 계정과 통합된 경우에만 Workfront에서 Workfront Proof 권한을 설정할 수 있습니다. 이 섹션에서 설명한 대로 증명을 사용할 수 없는 경우 Workfront 관리자에게 문의하십시오.
* 증명을 위해서는 Workfront 환경에서 최소한 한 명 이상의 사용자에게 관리자 권한이 있어야 합니다. 모든 사용자의 증명에 대한 관리자 권한을 제거하려고 하면 오류 메시지가 표시됩니다.
* 사용자의 Workfront 액세스 수준을 시스템 관리자가 아닌 다른 수준으로 변경하면 사용자의 Workfront Proof 권한 프로필의 기본값이 관리자로 설정됩니다.

* Workfront 액세스 수준을 시스템 관리자로 변경하면 증명 권한 프로필이 관리자로 변경됩니다.

## 모든 사용자를 위한 Workfront 메인 메뉴를 통해 Workfront Proof 액세스 구성 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

기본적으로 Workfront 내의 관리 권한이 있는 사용자만 [Adobe Workfront에서 Workfront Proof 액세스](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)에 설명된 대로 Workfront Proof에 액세스할 수 있습니다.

Workfront 지원에 문의하고 요청을 제출하여 모든 사용자에게 Workfront 기본 메뉴 내의 Workfront Proof 버튼에 대한 액세스 권한을 부여할 수 있습니다.

>[!IMPORTANT]
>
> 모든 Workfront 사용자가 Workfront 전역 탐색 모음에서 Workfront Proof에 직접 액세스할 수 있도록 하려면 각 사용자에 대한 권한 프로필이 Workfront 내에서 사용자의 액세스 수준보다 더 많은 액세스 권한을 제공하지 않도록 하십시오. 이렇게 하면 사용자가 Workfront Proof 내에서 액세스할 수 없는 Workfront 내의 증명에 액세스할 수 없습니다. 자세한 내용은 [사용자에 대한 증명 사용 및 사용 안 함(기존 계획만 해당)](#enable-and-disable-proofing-for-a-user-legacy-plans-only)을 참조하십시오.

## Desktop Proofing Viewer에 대한 사용자 액세스 구성

조직의 사용자가 대화형 내용을 검토하기 위해 웹 증명 뷰어 대신 데스크톱 증명 뷰어를 사용하고자 하는 경우, 사용자가 대화형 내용 증명을 열 때 데스크톱 증명 뷰어가 자동으로 시작되도록 구성할 수 있습니다. 이 데스크톱 증명 뷰어와 웹 증명 뷰어의 차이점에 대한 자세한 내용은 [데스크톱 증명 뷰어 이해](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) 및 [웹 증명 뷰어와 데스크톱 증명 뷰어의 차이점](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)을 참조하십시오.

1. Workfront에서 전역 탐색 막대에 있는 Workfront Proof 아이콘을 클릭하여 Workfront Proof에 액세스합니다.

   ![증명 아이콘](assets/proof-access-proofhq-350x39.png)

1. Workfront Proof의 오른쪽 상단 모서리에서 **계정 설정**&#x200B;을 클릭한 다음, **설정** 탭을 클릭합니다.

1. **증명 기본값**&#x200B;에서 **대화형 증명을 위한 데스크톱 증명 뷰어** 행 끝에 있는 **설정**&#x200B;을 클릭합니다.

1. [조직에 대한 증명 설정 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) 문서의 [데스크톱 증명 뷰어](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)에 설명된 대로 데스크톱 증명 뷰어 설정을 수정합니다.

1. **저장**&#x200B;을 클릭합니다.

## 대화형 증명에 대한 사용자 정의 장치 구성

사용자 정의 장치를 시스템에 추가하여 사용자가 Desktop Proofing Viewer를 사용할 때 대화형 콘텐츠를 검토하고 콘텐츠가 특정 장치에 표시되는 방식을 시뮬레이션할 수 있습니다. (이 기능은 사용자가 대화형 콘텐츠를 검토할 수 있는 웹 증명 뷰어에서 사용할 수 없지만, 다양한 장치가 아닌 다양한 해상도에서만 표시됩니다.)

자세한 내용은 증명 뷰어에서 [대화형 증명 해상도 변경](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)을 참조하십시오.

1. [Workfront에서 Workfront Proof 액세스](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)에 설명된 대로 Adobe Workfront에서 Workfront Proof 인터페이스에 액세스합니다.
1. [조직에 대한 증명 설정 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) 문서의 [증명에 대한 사용자 지정 장치 구성](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs)에 설명된 대로 데스크톱 증명 뷰어 설정을 수정합니다.
