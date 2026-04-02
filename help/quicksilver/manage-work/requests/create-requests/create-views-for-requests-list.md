---
product-area: requests
navigation-topic: create-requests
title: 요청 영역에서 보기 만들기 및 관리
description: 새 요청 경험을 사용하는 경우 요청 영역에 대한 보기를 만들고 저장할 수 있습니다.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ff87e425389f30dfaa1a178ea2b548d1c41179bb
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 3%

---


# 요청 영역에서 보기 만들기 및 관리

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


Adobe Workfront에서 새로운 요청 경험을 사용하는 경우 요청 영역에 대한 보기를 만들고 저장할 수 있습니다. 이러한 보기에는 필터, 열 배열 <span class="preview"> 및 그룹화가 포함됩니다.</span>


>[!IMPORTANT]
>
>* 이 기능은 요청 영역의 새 요청 경험에서만 사용할 수 있습니다.
>* 보기 설정은 홈의 내 요청 위젯에서도 사용할 수 있습니다. 하지만 요청 영역의 보기는 내 요청 위젯의 보기와 별개입니다.
>* 요청 영역 및 내 작업 위젯의 요청 목록은 Workfront의 향상된 목록을 사용합니다. 자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>모든 Workfront 또는 워크플로우 패키지</p>
   <p>요청 목록에서 Workfront Planning 요청을 보기 위한 모든 Worfront Planning 라이선스</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p>  <p>레이아웃 템플릿에 보기를 추가하려면 Workfront 관리자여야 합니다.</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<div class="preview">

## 요청에 대한 시스템 보기

Workfront에서는 직접 만들 수 있는 보기 외에도 홈의 요청 영역 및 내 요청 위젯에 대해 다음과 같은 시스템 보기를 제공합니다.

* **모든 요청**: 귀하 또는 다른 사람이 대기열이나 작업 공간에서 제출한 모든 요청을 볼 수 있는 권한이 있습니다. 내 요청 위젯에서는 사용할 수 없습니다.
* **내 요청**: 상태에 관계없이 제출한 요청입니다.
* **내 진행 중 요청**: 제출했으며 아직 열려 있습니다.
* **내 초안**: 아직 제출되지 않은 퀘스트의 초안입니다.
* **요청 열기**: 사용자 또는 다른 사람이 큐에 제출했거나 아직 열려 있는 작업 영역을 볼 수 있는 권한이 있는 요청에 대한 요청입니다. 내 요청 위젯에서는 사용할 수 없습니다.

시스템 보기는 편집할 수 없습니다. 요소를 수정한 다음 보기를 복사하고 복사본을 편집하거나 공유할 수 있습니다.

</div>

## 요청에 대한 보기 만들기

새 요청 경험을 사용할 때 Workfront의 요청 영역에서 보기를 만들 수 있습니다. 및 새 요청 경험을 활성화한 후 홈에서 내 요청 위젯에 대한 보기를 만들 수도 있습니다.

1. **요청** 목록에 액세스하려면:

   {{step1-to-requests}}

   1. **새 경험 사용** 설정이 켜져 있는지 확인하십시오.

1. 홈에서 **내 요청** 위젯에 액세스하려면:

   {{step1-to-home}}

   1. **내 요청** 위젯을 추가하거나 이동합니다.

1. 요청 목록에서 **보기** 드롭다운 메뉴 ![보기 드롭다운](assets/view-icon-requests.png)을 클릭하고 **새 보기**&#x200B;를 클릭합니다.

   ![새 보기](assets/create-new-view.png)

1. 새 보기의 이름을 입력하고 **만들기**&#x200B;를 클릭합니다.
1. [요청 보기 편집](#edit-a-view-for-requests)을 계속합니다.

## 요청에 대한 보기 편집

요청 영역에서 방금 만든 보기 또는 홈의 내 요청 위젯을 포함하여 기존 보기를 편집할 수 있습니다.

뷰를 편집하여 뷰의 다음 요소를 변경할 수 있습니다.

* 이름
* 필터
* 열

<div class="preview">

* 그룹화
* 셀 서식 지정
* 행 높이

</div>

자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요.

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * 보기에 대한 변경 사항은 자동으로 저장됩니다.
> * 보기에 대한 변경 내용은 <span class="preview"> 보기를 변경한 후 새 복사본을 공유하는 경우에만 해당 보기를 사용하는 모든 사용자에게 표시됩니다.</span>
> * 사용자가 값으로 있는 모든 필드에서 **내(로그인한 사용자)** 필터 와일드카드를 사용하십시오.

## 레이아웃 템플릿에 요청 보기 추가

Workfront 관리자는 요청 영역에 대한 레이아웃 템플릿에 새 보기를 추가할 수 있습니다.

자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

## 보기 공유

만든 보기를 다른 사용자, 팀, 그룹 또는 회사와 공유할 수 있습니다.

보기를 공유하면 다른 사용자는 공유하기 전에 해당 보기에 대해 편집한 업데이트된 보기 요소를 볼 수 있습니다.

<span class="preview">보기를 업데이트하면 같은 보기의 복사본을 만들어 복사본을 공유하기 전에 변경 내용을 보존하지 않으면 변경 내용이 다른 사용자에게 표시되지 않습니다.

자세한 내용은 [향상된 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하세요. </span>

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->