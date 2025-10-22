---
product-area: projects
navigation-topic: manage-issues
title: 목록에서 문제 편집
description: 개별 문제를 편집하거나 문제 목록 또는 보고서에서 문제를 편집할 수 있습니다. 이 문서에서는 목록에서 문제를 편집하는 방법에 대해 설명합니다.
author: Alina
feature: Work Management
exl-id: a3276d83-c08f-4480-9092-aa47ba76d794
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 1%

---

# 목록에서 문제 편집

<!--Audited: 08/2025-->

<!--Audited: 03/2025-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

개별 문제를 편집하거나 문제 목록 또는 보고서에서 문제를 편집할 수 있습니다. 이 문서에서는 목록에서 문제를 편집하는 방법에 대해 설명합니다.

개별 문제 편집에 대한 자세한 내용은 [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>

<ul><li><p>기여자 이상</p> </li>
   <li><p>프로젝트의 문제 섹션에서 문제를 편집할 수 있는 라이트 또는 상위 라이선스</p></li></ul> 
    또는
   <ul><li><p>요청자 이상</p> </li>
   <li><p>프로젝트의 문제 섹션에서 문제를 편집할 수 있는 검토자 이상의 라이선스</p></li></ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 기여 또는 더 높은 권한</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a>를 참조하십시오.</p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 권한 요청을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to edit issues in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the issue</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 인라인 편집 문제

목록 보기에 표시된 필드를 인라인 편집하여 문제 목록에서 문제 정보를 편집할 수 있습니다.

목록에서 문제를 편집할 때 다음 사항을 고려하십시오.

* 목록에 표시되고 업데이트할 권한이 있는 모든 문제 필드를 편집할 수 있습니다.
* 다음 목록에서 문제를 편집할 수 있습니다.

   * 프로젝트 또는 작업의 문제 섹션
   * 문제 보고서

문제를 인라인 편집하려면:

1. 프로젝트 또는 작업의 문제 목록으로 이동합니다.
1. 수동으로 업데이트할 권한이 있는 필드 내부를 클릭합니다. 필드는 편집 가능해지며 변경할 수 있습니다.

   ![인라인 문제 편집](assets/edit-issues-inline-350x34.png)

1. 변경 내용을 적용하려면 Enter 키를 누릅니다. 변경 사항이 즉시 저장됩니다.

   인라인 편집 개체에 대한 자세한 내용은 [Adobe Workfront의 목록에서 인라인 편집 항목](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)을 참조하십시오.

## 목록에서 문제 편집

1. 프로젝트 또는 작업의 문제 목록으로 이동합니다.
1. 다음 중 하나를 수행합니다

   * 목록에서 문제를 선택한 다음 도구 모음에서 **편집** 아이콘 ![편집 아이콘](assets/qs-edit-icon.png)을 클릭합니다.
   * 문제의 이름을 클릭한 다음 **편집**&#x200B;을 클릭합니다.

     이러한 작업을 수행하면 **문제 편집** 상자가 열립니다.

     **문제 편집** 상자에서 문제를 편집하는 방법에 대한 자세한 내용은 [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md)을 참조하십시오.

## 요약을 사용하여 문제 편집

요약 패널을 사용하여 목록에서 문제를 편집할 수 있습니다.

1. 문제를 편집할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **문제**&#x200B;를 클릭합니다.

   프로젝트의 문제 목록이 표시됩니다.

1. 편집할 문제를 선택한 다음 문제 목록의 오른쪽 상단에 있는 **요약 열기** 아이콘 ![요약 열기 아이콘](assets/qs-open-summary-icon-in-new-toolbar-small.png)을 클릭합니다.

   **요약**&#x200B;이 열립니다.

1. (선택 사항) **업데이트** 영역에서 문제에 대한 업데이트를 입력하십시오.
1. 다음 아이콘 또는 영역을 클릭하여 문제로 이동하고 문제 수준에서 정보를 편집합니다.

   | 아이콘 | 액션 |
   |---|---|
   | 문서 ![문서 아이콘](assets/documents-icon-in-summary.png) | 문제에 문서를 추가하려면 **여기를 클릭**&#x200B;하세요. |
   | 세부 정보 ![세부 정보 아이콘](assets/details-icon-in-summary.png) | 을(를) 클릭하여 문제에 대한 정보를 업데이트합니다. |
   | 시간 ![로그 시간](assets/log-time-icon-in-summary.png) | 클릭하여 시간을 기록합니다. |
   | 승인 ![승인 아이콘](assets/approvals-icon-in-summary.png) | 문제 승인을 추가하려면 클릭하십시오. |

1. (선택 사항) **요약 열기** 아이콘을 다시 클릭하거나 요약 오른쪽 상단의 **X 아이콘**&#x200B;을 클릭하여 패널을 닫고 문제를 인라인으로 편집합니다.

## 일괄 문제 편집

문제를 일괄적으로 편집하고 모든 정보를 동시에 업데이트할 수 있습니다.

문제를 일괄 편집하려면 다음을 수행하십시오.

1. **기본 메뉴**(으)로 이동합니다.
1. **프로젝트**&#x200B;를 클릭합니다.
1. 프로젝트 이름을 클릭하여 프로젝트에 액세스합니다.
1. 왼쪽 패널에서 **문제**&#x200B;를 클릭합니다.
1. 목록에서 몇 가지 문제를 선택하십시오.
1. **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

   **문제 편집** 대화 상자가 열립니다.

1. 선택한 모든 문제에 대한 정보를 지정합니다.

   모든 문제에 대한 정보를 편집하는 것은 다음 영역을 편집할 때 한 문제에 대한 정보를 편집하는 것과 동일합니다.

   * 개요
   * 설정
   * 할당
   * 댓글

   문제 편집에 대한 자세한 내용은 [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md)을 참조하세요.

   >[!NOTE]
   >
   >선택한 모든 문제에 대해 변경 중인 정보는 **할당** 필드를 제외한 개별 문제에 대한 기존 정보를 재정의합니다. 일괄 편집에서 새 피할당자를 추가하면 해당 피할당자가 선택한 모든 문제에 추가됩니다. 다른 피할당자가 선택한 문제에 할당되면 일괄 편집을 통해 추가된 문제와 함께 할당된 상태로 유지됩니다.

1. 선택한 모든 문제에 첨부된 사용자 정의 양식을 편집하려면 **사용자 정의 Forms**&#x200B;을(를) 클릭하십시오.

   선택한 문제에 일반적인 사용자 정의 양식이 없는 경우 이 섹션에 양식이 나열되지 않습니다.

   선택한 모든 문제에 첨부되고 편집 권한이 있는 양식의 필드만 편집할 수 있습니다.

   <!--1. (Optional and conditional) Depending what environment you use to edit the issues, do one of the following to recalculate custom expressions for all issues:
   1. In the Production environment, ADD THE SENTENCE FROM THE NEXT STEP HERE:-->

1. (선택 사항) **사용자 지정 Forms** 영역에서 **사용자 지정 표현식 다시 계산** 옵션을 선택하여 선택한 문제에 첨부된 사용자 지정 Forms에 있는 모든 계산된 사용자 지정 필드가 최신 상태인지 확인합니다.

   <!--  
   <div class="preview">

   1. In the Preview environment, with all the issues selected in the list, click the **More** menu ![More menu](assets/more-icon.png) at the top of the issue list, then click **Recalculate Expressions**.
   -->

   >[!IMPORTANT]
   >
   >사용자 정의 표현식을 다시 계산할 때 한 번에 500개 이상의 문제를 선택하지 않는 것이 좋습니다.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

   이제 선택한 모든 문제에서 변경한 사항이 모두 표시됩니다.
