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
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 3%
---
# 사용자의 증명 액세스 구성

Adobe Workfront 관리자 또는 Workfront Proof 관리자는 Workfront 및 Workfront Proof에서 증명을 만들고 보기 위한 사용자 액세스를 구성할 수 있습니다.

기본 및 통합 교정에 사용할 수 있는 증명 기능에 대한 자세한 내용은 [Workfront의 증명 기능에 액세스](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td>Any</td> 
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

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

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
