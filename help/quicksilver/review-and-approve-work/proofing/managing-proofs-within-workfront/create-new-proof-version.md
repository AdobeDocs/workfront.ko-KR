---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 증명의 새 버전 만들기
description: 한 작업의 여러 버전 또는 수정 버전에서 피드백을 관리하는 것은 큰 문제가 될 수 있습니다. Workfront에서는 증명의 여러 버전을 만들고 비교할 수 있으므로 이 프로세스를 간소화합니다.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 0%

---

# 증명의 새 버전 만들기

한 작업의 여러 버전 또는 수정 버전에서 피드백을 관리하는 것은 큰 문제가 될 수 있습니다. Workfront에서는 증명의 여러 버전을 만들고 비교할 수 있으므로 이 프로세스를 간소화합니다.

증명의 새 버전을 만들 때는 다음 정보를 고려하십시오.

* 사용자에게 한 버전은 볼 수 있지만 다른 버전은 볼 수 없는 권한을 부여할 수 있습니다. 반대로 사용자와 최신 버전을 공유하는 경우, 이전 버전으로 돌아가 해당 이전 버전에 대한 액세스 권한을 명시적으로 부여하지 않으면 해당 사용자는 이전 버전을 볼 수 없습니다.
* 증명의 새 버전을 생성하려면 증명에 대한 편집 권한이 있어야 합니다.

  증명에 대한 편집 권한이 있는 사용자에 대한 자세한 내용은 [Workfront Proof에서 증명 역할 관리](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 및 [Workfront Proof에서 증명 권한 프로필](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)을 참조하십시오.

  증명 버전 공유에 대한 자세한 내용은  [Workfront Proof에서 증명 공유](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>증명이 Adobe Workfront 내에서 생성된 경우 해당 증명에 대해 생성된 모든 새 버전은 Workfront 내에서도 생성되어야 합니다. Workfront 내에서 증명을 만든 경우 해당 증명은 Workfront Proof 내에서 새 버전을 만들 수 없습니다.

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
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서에 대한 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 역할 또는 증명 권한 프로필을 확인하려면 Workfront 또는 Workfront Proof 관리자에게 문의하십시오.

+++

## Workfront에서 증명의 새 버전 만들기

Workfront에서 새 증명 버전을 업로드하는 방법에는 몇 가지가 있습니다. 기본 증명 설정은 선택한 방법에 따라 이전 버전에서 이전되거나 이전되지 않을 수 있습니다.

* **문서를 업로드할 때 증명을 자동으로 생성**: 기본 증명 설정이 이월되지 않습니다. 사용자 프로필에서 이 설정을 활성화한 경우 새 버전을 끌어서 놓을 때 기본 증명 설정이 이월되지 않습니다.
* **증명 만들기 > 단순**: 기본 증명 설정이 이월되지 않습니다. 새 증명 버전을 만들 때 단순을 선택하면 이전 버전에서 기본 증명 설정이 이월되지 않습니다.
* **새로 추가 > 버전 > 증명**: 기본 증명 설정이 이전 버전에서 이월됩니다.
* **증명 만들기 > 고급**: 기본 증명 설정이 이전 버전에서 이월됩니다.

  <table>
  <tbody>
  <tr>
  <td>문서 업로드 시 자동으로 증명 생성</td>
  <td>기본 증명 설정이 이월되지 않습니다. 사용자 프로필에서 이 설정을 활성화한 경우 새 버전을 끌어서 놓을 때 기본 증명 설정이 이월되지 않습니다.</td>
  </tr>
  <tr>
  <td>증명 만들기 &gt; 단순</td>
  <td>기본 증명 설정이 이월되지 않습니다. 새 증명 버전을 만들 때 단순을 선택하면 이전 버전에서 기본 증명 설정이 이월되지 않습니다.</td>
  </tr>
  <tr>
  <td>새로 추가 &gt; 버전 &gt; 증명</td>
  <td>기본 증명 설정이 이전 버전에서 이월됩니다.</td>
  </tr>
  <tr>
  <td>증명 만들기 &gt; 고급</td>
  <td>기본 증명 설정이 이전 버전에서 이월됩니다.</td>
  </tr>
  </tbody>
  </table>




증명의 새 버전을 생성하려면:

1. 증명이 포함된 문서 목록을 엽니다.
1. 컴퓨터의 파일 시스템에서 새 파일을 증명 위로 끌어서 놓습니다.

   또는

   증명이 나열된 행을 선택하고 **새로 추가** > **버전**&#x200B;을 클릭한 다음 새 증명 버전을 추가하는 데 사용할 옵션을 클릭합니다.

   ![](assets/add-new-version-350x185.png)

## 증명 뷰어에서 증명의 새 버전 만들기(Workfront Proof만 해당)

독립형 Workfront Proof을 사용하는 경우 단일 파일 또는 웹 캡처가 포함된 새 증명 버전을 만들 수 있습니다. 

>[!NOTE]
>
>계정이 Enterprise 플랜에 있고 여러 파일 또는 웹 캡처를 업로드하는 경우 새 단일 버전에 자동으로 결합됩니다. 자세한 내용은 [다중 페이지 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)를 참조하십시오.

Workfront Proof에서 증명의 새 버전을 생성하려면 다음을 수행하십시오.

1. 증명을 엽니다.
1. 왼쪽 상단 모서리에서 **버전** 드롭다운 메뉴를 클릭한 다음 나타나는 상자에서 **+ 새 버전**&#x200B;을 클릭합니다.

   표시되는 **새 증명 버전** 페이지에서 역할 및 전자 메일 알림 설정을 포함하여 이전 버전의 모든 검토자를 볼 수 있습니다. 이 페이지에서 기존 검토자의 역할과 알림을 쉽게 편집하거나 새 버전에서 기존 검토자를 제거할 수 있습니다.

1. **파일 추가**&#x200B;에서 컴퓨터에서 드래그 앤 드롭하거나 **찾아보기**&#x200B;를 클릭하고 원하는 파일을 선택하여 파일을 새 증명 버전으로 업로드하십시오. 버전에 대해 **증명 이름**&#x200B;을 입력하거나 이 상자를 비워 두면 끝에 버전 번호가 추가된 동일한 파일 이름을 사용할 수 있습니다.

   또는

   URL을 입력하여 웹 페이지를 증명의 새 버전으로 캡처합니다.

   >[!NOTE]
   >
   >드래그 앤 드롭은 HTML5를 완전히 지원하는 브라우저에서만 사용할 수 있습니다. 여기에는 Internet Explorer 7~9와 Safari가 제외됩니다.

1. **워크플로**&#x200B;에서 다음 중 하나를 변경하여 이 증명 버전에 대한 검토자를 지정하십시오.

   이전 버전의 검토자는 사용자가 추가한 검토자로 대체됩니다.

   * 버전의 **소유자**&#x200B;를 계정의 다른 사용자로 변경합니다.\
     소유자 권한에 대한 자세한 내용은 [Workfront Proof의 증명 권한 프로필](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)을 참조하십시오.

   * **연락처 이름 또는 전자 메일 주소를 입력하여 받는 사람 상자를 추가**&#x200B;하면 검토자를 버전에 추가하십시오. 각 받는 사람에 대해 **증명 역할** 및 **전자 메일 경고** 유형을 지정할 수 있습니다.

     증명에 그룹 추가에 대한 자세한 내용은  [증명에 그룹 추가](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). 역할에 대한 자세한 내용은 [Workfront Proof에서 증명 역할 관리](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)를 참조하십시오.

     >[!NOTE]
     >
     >의 작성자 또는 소유자인 경우  증명에 기본적으로 [증명 전자 메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)이(가) 비활성화되어 있습니다(개인 설정에서). 새 증명 페이지에서 전자 메일로 사람들에게 알림 상자를 선택해도 증명 전자 메일 또는 새 증명 전자 메일이 수신되지 않습니다. 전자 메일 알림에 대한 자세한 내용은 [Workfront Proof에서 전자 메일 알림 설정 구성](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)을 참조하십시오. [증명 메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 및 [새 증명 메일](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)도 참조하세요.

   * 버전에 대한 증명 기한을 설정합니다.
   * 검토자의 이름 위로 마우스를 가져가면 이전 버전에 대해 수행한 모든 결정을 볼 수 있습니다.

1. **전자 메일 알림**&#x200B;에서 다음 중 하나를 실행하십시오.

   * 검토자에게 새 버전을 알리는지 여부를 지정합니다.\
     선택 내용은 증명 세부 정보 페이지의 활동 섹션에 기록됩니다. 자세한 내용은 [Workfront Proof에서 증명 세부 정보 관리](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)를 참조하십시오.

   * 사용자 정의 제목과 메시지를 추가합니다.

1. **조직** 섹션에서 다음 중 하나를 수행합니다. 

   * 증명에 태그를 하나 이상 적용합니다. 자세한 내용은 [Workfront Proof에서 태그 만들기 및 관리](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md)를 참조하십시오.\
     태그는 증명의 이전 버전에서도 상속됩니다. 새 버전에 새 태그를 추가하면 이전 버전에도 태그가 지정됩니다.

   * 폴더에 버전을 추가합니다. 자세한 내용은 [Workfront Proof에서 폴더 관리](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)를 참조하십시오. 이전 버전의 증명에서 폴더가 복사됩니다. 다른 폴더를 선택하면 전체 증명(모든 버전)이 이동됩니다.

   * 청구 관리자 및 관리자는 설정 탭에서 폴더 필드를 전체 계정에서 필수로 설정할 수 있습니다. 자세한 내용은 를 참조하십시오.

1. 증명 설정에서 아래의 변경 내용을 적용합니다.

   * 증명에 로그인 필요
   * 증명에 전자 서명 필요(엔터프라이즈 플랜만 해당)
   * 모든 결정이 내려지면 증명 잠금
   * 원본 파일의 다운로드 허용 또는 차단
   * 공개 공유 설정을 포함하여 증명에 대한 공개 공유
   * 증명 구독\
     이 섹션에서 선택한 항목은 증명 세부 정보 페이지에 표시됩니다(일부 필드는 편집할 수 있음). 자세한 내용은 [Workfront Proof에서 증명 세부 정보 관리](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)를 참조하십시오.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## 새 버전 메시지 정보

이전 버전의 증명에 사용자 정의 주제/메시지가 포함된 경우 새 버전 페이지에 기본적으로 표시됩니다. 다음을 수행할 수 있습니다.

* 제목과 메시지를 편집합니다.
* 사람들에게 이메일로 알림 상자를 선택 취소합니다. 즉, 검토자에게 검토할 새 버전이 있음을 알리는 이메일이 전송되지 않습니다.

  >[!NOTE]
  >
  >개인 설정에 저장된 기본 사용자 정의 제목/메시지의 영향을 받지 않습니다.

기본 제목과 메시지가 개인 설정에 저장된 경우 새 버전 페이지에 기본적으로 표시되는 메시지에 영향을 줍니다.

* 표준 이메일을 사용하여 이전 버전의 증명에 대해 검토자에게 이메일로 알리도록 선택한 경우(예: 사용자 정의 제목/메시지가 없음) 기본 사용자 정의 제목/메시지(개인 설정)가 새 버전 페이지에 표시됩니다. 그런 다음 사용자 정의 제목과 메시지를 편집하거나 이메일로 사용자에게 알림 상자를 선택 취소할 수 있습니다(검토자에게 검토할 새 버전이 있음을 알리는 이메일이 전송되지 않음).
* 이전 버전의 증명에 대해 검토자에게 이메일로 알리지 않도록 선택한 경우(예: 표준 또는 사용자 정의 이메일 없음) 새 버전 페이지에는 기본적으로 메시지가 포함되지 않습니다. 검토자에게 새 버전을 알리려면 메시지 보내기 링크를 클릭합니다. 그러면 개인 설정에 따라 기본 사용자 지정 제목/메시지가 표시됩니다. 그런 다음 필요한 경우 사용자 정의 제목과 메시지를 편집할 수 있습니다.

개인 설정에 기본 제목과 메시지가 저장되지 않은 경우 새 버전 페이지에 다음이 표시됩니다.

* 표준 이메일을 사용하여 이전 버전의 증명에 대해 검토자에게 이메일로 알리도록 선택한 경우(예: 사용자 정의 제목/메시지가 없음) 새 버전 페이지에서 기본적으로 사람에게 이메일로 알림 옵션이 선택됩니다. 사용자 지정 메시지를 추가하려면 링크를 클릭합니다.
* 이전 버전의 증명에 대해 검토자에게 이메일로 알리지 않도록 선택한 경우(예: 표준 또는 사용자 정의 이메일 없음) 새 버전 페이지에는 기본적으로 메시지가 포함되지 않습니다. 검토자에게 새 버전을 알리려면 메시지 보내기 링크를 클릭합니다. 그런 다음 사용자 정의 메시지 추가 링크를 클릭하여 사용자 정의 제목과 메시지를 추가할 수 있습니다.
