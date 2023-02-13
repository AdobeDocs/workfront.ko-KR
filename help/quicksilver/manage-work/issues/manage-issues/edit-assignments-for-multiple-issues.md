---
product-area: projects
navigation-topic: manage-issues
title: 목록의 여러 문제에 대한 사용자 할당 수정
description: 목록의 여러 문제에 대한 사용자 할당 수정
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 목록의 여러 문제에 대한 사용자 할당 수정

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

여러 문제에 대한 사용자 지정을 동시에 수정할 수 있습니다. 문제를 편집하거나 한 번에 하나씩 지정하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [문제 편집](../../../manage-work/issues/manage-issues/edit-issues.md)
* [문제 할당](../../../manage-work/issues/manage-issues/assign-issues.md)

문제 지정에 대한 일반적인 정보는 [문제 지정 수정 개요](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>문제에 할당할 수 있으려면 Contribute 권한 이상이 있어야 합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 여러 문제에 대한 지정 수정

1. 수정할 할당이 있는 문제가 포함된 문제 목록으로 이동합니다.
1. (선택 사항) 수정할 할당자에게 할당된 문제만 표시하도록 필터를 만듭니다.

   예를 들어 할당자로 특정 역할이 있는 문제만 표시하도록 필터를 만들 수 있습니다. 그런 다음 역할을 특정 사용자로 대체할 수 있습니다. 다음을 수행합니다.

   1. 을(를) 클릭합니다. **필터** 드롭다운 목록을 클릭한 다음 **새 필터**.

      새 필터 대화 상자가 표시됩니다.

   1. 클릭 **필터 규칙을 추가합니다.**
   1. 특정 역할에 대해 필터링하려면 다음을 확장합니다. **할당 역할,** 을 클릭한 다음 **ID.**

      또는

      특정 사용자에 대해 필터링하려면 **할당 사용자,** 을 클릭한 다음 **ID.**

      >[!TIP]
      >
      >사용 안 함 **지정 대상** 이 필드는 문제 소유자만 참조하고 모든 담당자가 아닙니다.

   1. 드롭다운 목록에서 을(를) 선택합니다 **Equal** 을 필터 한정자로 사용하십시오.
   1. 필터링할 사용자 또는 역할의 이름을 입력하고 드롭다운 목록에 표시할 이름을 클릭합니다.
   1. 클릭 **필터 저장.**

1. 지정을 수정할 문제를 선택한 다음 **편집** 아이콘 ![](assets/qs-edit-icon.png).

   다음 **문제 편집** 표시됩니다. 편집된 항목은 페이지의 왼쪽 위 모서리에 표시됩니다.

1. 로 이동합니다. **지정** 섹션을 선택한 다음 **할당자**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. 다음 중 하나를 수행하십시오.

   1. 새 할당자를 추가하려면

      1. 사용자, 역할 또는 팀의 이름을 입력하고 목록에 표시될 때 선택합니다. 할당이 추가되고 선택한 문제에 대한 현재 할당이 대체되지 않습니다.

         >[!TIP]
         여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
         사용자, 작업 역할 또는 팀이 비활성화되기 전에 할당된 경우 작업 항목에 지정된 상태로 유지됩니다. 이 경우 다음을 권장합니다.
         * 작업 항목을 활성 자원에 재지정합니다.
         * 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


         선택한 모든 문제에 공통되는 정보가 표시됩니다. 예를 들어 동일한 사용자가 모든 문제에 할당되면 해당 사용자는 **할당자** 열. 선택한 문제 간에 정보가 일반적이지 않으면 정보가 표시되지 않습니다.
   1. 개별 할당을 제거하려면 다음을 수행합니다.

      1. 을(를) 클릭합니다. **X 아이콘** 할당자가 지정 목록에 표시되는 경우 제거할 할당자의 이름 옆에 있습니다.

         또는

         (조건부) 제거하려는 할당자가 선택한 문제 중 일부에만 할당되어 있기 때문에 지정 섹션에 표시되지 않는 경우 을 클릭합니다 **할당자 제거** 제거할 할당자의 이름을 입력하고 드롭다운 목록에 나타나면 이름을 클릭합니다.

      1. 클릭 **할당자 제거** 제거할 다른 담당자를 다시 추가합니다.
   1. 기존 담당자를 모두 제거하려면

      1. 클릭 **기존 할당 모두 제거**&#x200B;를 클릭한 다음 **예, 모든 담당자 삭제**.

         따라서 편집 대화 상자에 표시되는 할당자 뿐만 아니라 선택한 모든 문제에 대한 모든 지정자도 제거됩니다.



1. (선택 사항) 문제와 연결하도록 선택한 담당자에 대해 다음 옵션을 수정합니다.

   * **문제 소유자:** 라디오 단추를 선택하여 문제 소유자로 지정된 담당자를 표시합니다. 선택하지 않은 경우 Adobe Workfront은 첫 번째 할당자를 문제 소유자로 지정합니다. 팀 할당에는 사용할 수 없습니다.
   * **할당자의 역할**: 드롭다운 목록에서 역할을 선택합니다. 선택하지 않은 경우 Workfront은 자동으로 사용자의 기본 역할을 선택합니다.

1. 클릭 **변경 내용 저장**.
