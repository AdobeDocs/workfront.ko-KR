---
product-area: projects
navigation-topic: approvals
title: Workfront에서 문서 승인
description: 문서의 승인자로 할당된 경우 여러 가지 방법으로 승인 결정을 내릴 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 1%

---

# Workfront에서 문서 승인

문서의 승인자로 할당된 경우 여러 가지 방법으로 승인 결정을 내릴 수 있습니다.

새 문서 승인 만들기에 대한 자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

>[!IMPORTANT]
>
>이 문서의 내용은 특정 계정에만 사용할 수 있는 업데이트된 문서 승인 기능에 적용됩니다. 표준 승인 프로세스에 대한 자세한 내용은 [작업 승인](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)에 나열된 문서를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>기존 Workfront 스토리지를 사용하여 승인을 관리하는 모든 Workfront 패키지</p>
<p>Adobe 엔터프라이즈 스토리지를 사용하여 승인을 관리하는 모든 워크플로우 패키지</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p>
   <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>승인과 연관된 객체에 대한 보기 이상의 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>승인과 연관된 오브젝트에 대한 이상 권한 보기</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 홈에서 문서 승인

1. Adobe Workfront의 왼쪽 위 모서리에 있는 **홈** 아이콘 ![홈 아이콘](../assets/home-icon-30x29.png)을 클릭합니다.

   >[!NOTE]
   >
   >Workfront 관리자는 사용자 환경의 홈 아이콘을 다음과 같이 변경할 수 있습니다.
   >
   >* 조직 설명을 위해 사용자 지정된 이미지로 대체합니다. 이 경우 아이콘은 이 문서에 표시된 것과 다르게 표시됩니다.
   >
   >* 연결된 페이지를 다른 페이지로 바꿉니다. 이 경우 페이지의 오른쪽 상단에 있는 **주 메뉴** ![주 메뉴 아이콘](../assets/main-menu-icon.png)을 클릭한 다음 **홈**&#x200B;을 클릭합니다.

1. 페이지 왼쪽 상단의 **필터**&#x200B;를 클릭하고 **승인**&#x200B;이 선택되어 있는지 확인하십시오.

   All work items that require your approval are displayed in the list.

   >[!NOTE]
   >
   >* Approvals assigned to Job Roles or Groups aren&#39;t listed in Home.
   >* Approvals assigned to Teams display in each individual team member&#39;s My Approvals widget in Home.

1. Click on the document approval in the list for which you want to make an approval decision. Information regarding the approval will appear on the right side of the page.

1. Click one of the following two approval options in the top-right corner of the page:

   * The **Approve** dropdown contains two options:

      * **Approve** indicates that no changes are needed for this version of the document and that approval is given.

      * **Approve with changes** indicates that some small changes are still required on the document, but approval is given on the condition that those changes are made. If you select this option, a window will appear that contains a text box named **Next steps** where you can specify what changes are needed for the document to be approved. You may either enter that information and click **Add message**, or you may click **Skip** to send the approval decision without additional information.

   * **Needs work** indicates that the document version is not approved and requires significant changes.

   Consider the following when viewing document approvals in Home:

   * The name of the user who requested the approval is displayed above the document name in Home with the text &quot;*User A* would like your approval on...&quot;, as well as under **Submitted By** in the approval information that displays on the right once an approval is selected.

   * After a decision is made on an approval, the approval remains in the My Approvals tab with the text &quot;Decision Made&quot; until you click the **Refresh** button, or until you refresh the browser page.

## Approve a document from the document page

1. 문서 이름을 클릭하여 문서 페이지로 이동합니다.

1. Select the version of the document that is pending your approval in the version dropdown next to the document&#39;s name. 기본적으로 최신 버전이 선택됩니다.

   If the currently selected version of the document has a pending approval for you, the approval decision buttons are displayed in the top-right corner of the page; if other versions of the document have pending approvals for you, the version dropdown menu displays a red dot.

   <!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Click one of the following two approval options in the top-right corner of the page:

   * The **Approve** dropdown contains two options:

      * **Approve** indicates that no changes are needed for this version of the document and that approval is given.

      * **Approve with changes** indicates that some small changes are still required on the document, but approval is given on the condition that those changes are made. If you select this option, a window will appear that contains a text box named **Next steps** where you can specify what changes are needed for the document to be approved. 해당 정보를 입력하고 **메시지 추가**&#x200B;를 클릭하거나 **건너뛰기**&#x200B;를 클릭하여 추가 정보 없이 승인 결정을 보낼 수 있습니다.

   * **작업 필요**&#x200B;는 문서 버전이 승인되지 않았으며 중요한 변경이 필요함을 나타냅니다.

## 문서 요약 패널에서 문서 승인

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.

1. 승인이 필요한 문서를 클릭하면 문서 요약 패널이 열립니다.

1. 버전 드롭다운에서 검토할 문서의 버전을 선택합니다. 기본적으로 최신 버전이 선택됩니다.

   현재 선택한 문서 버전에 대기 중인 승인이 있는 경우 문서 요약 패널의 오른쪽 상단 모서리에 승인 결정 버튼이 표시됩니다. 다른 문서 버전에 대기 중인 승인이 있는 경우 버전 드롭다운 메뉴에 빨간색 점이 표시됩니다.
<!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
 -->
1. 문서 요약 패널의 오른쪽 상단 모서리에서 다음 두 가지 승인 옵션 중 하나를 클릭합니다.

   * **승인** 드롭다운에는 다음 두 가지 옵션이 있습니다.

      * **승인**&#x200B;은(는) 이 문서 버전에 변경이 필요하지 않으며 승인이 있음을 나타냅니다.

      * **변경 사항과 함께 승인**&#x200B;은(는) 문서에 일부 작은 변경 내용이 여전히 필요함을 나타내지만, 이러한 변경 내용이 적용되는 조건으로 승인이 제공됩니다. 이 옵션을 선택하면 문서를 승인하는 데 필요한 변경 내용을 지정할 수 있는 **다음 단계**&#x200B;라는 텍스트 상자가 포함된 창이 나타납니다. 해당 정보를 입력하고 **메시지 추가**&#x200B;를 클릭하거나 **건너뛰기**&#x200B;를 클릭하여 추가 정보 없이 승인 결정을 보낼 수 있습니다.

   * **작업 필요**&#x200B;는 문서 버전이 승인되지 않았으며 중요한 변경이 필요함을 나타냅니다.


## 증명 뷰어에서 문서 승인

문서를 검토하고 승인하려면 다음과 같이 하십시오.

1. 리뷰 전자 메일 알림으로 이동한 다음 **리뷰로 이동**&#x200B;을 클릭합니다.

1. Workfront에 있으면 **증명으로 이동**&#x200B;을 클릭하세요.

1. 콘텐츠를 검토하고 주석 또는 마크업을 추가합니다. 증명 뷰어를 사용하는 방법에 대한 자세한 내용은 [Adobe Workfront에서 증명 검토: 문서 인덱스](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)를 참조하십시오.

1. 다음 결정 중 하나를 선택합니다.

   * **승인**: 문서를 변경할 필요가 없으며 사용할 준비가 되었습니다.
   * **변경 사항과 함께 승인**: 문서를 변경해야 하며, 문서를 사용할 준비가 되었습니다. 추가 승인이 필요하지 않습니다.
   * **작업 필요**: 문서를 변경해야 하며 사용할 준비가 되지 않았습니다. 지정된 변경 사항이 적용되면 문서를 새 버전으로 업로드하고 다른 승인을 거쳐야 합니다. 새 버전 업로드에 대한 자세한 내용은 [새 문서 버전 업로드 및 승인 요청](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)을 참조하십시오.

결정을 내리면 문서 소유자에게 이메일을 통해 알림이 전송됩니다.


