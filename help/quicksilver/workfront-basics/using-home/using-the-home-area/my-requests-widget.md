---
product-area: projects
navigation-topic: use-the-home-area
title: 내 요청 위젯 사용
description: 내 요청 위젯에서 요청을 제출할 수 있습니다. 필터 및 열을 사용하여 위젯을 사용자 정의할 수도 있습니다.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 2%

---

# 내 요청 위젯 사용

>[!IMPORTANT]
>
>이 문서에서는 새로운 내 요청 위젯에 대해 설명합니다. 새 위젯을 보려면 새 요청 환경을 활성화해야 합니다.
>요청 영역에서 새 요청 경험을 활성화할 수 있습니다.

내 요청 위젯은 사용자가 제출한 요청을 표시합니다. 요청을 필터링하거나 특정 요청을 검색하거나 열 순서 및 가시성을 조정할 수 있습니다. 내 요청 위젯에서 새 요청을 만들 수도 있습니다.

>[!NOTE]
>
>* 내 요청 위젯이 로드되면 최대 50개의 요청이 표시됩니다. 요청을 더 표시하려면 목록을 아래로 스크롤합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>모든 Workfront 또는 워크플로우 패키지</p>
   <p>Workfront Planning 요청 및 생성된 객체에 액세스할 수 있는 모든 Workfront Planning 패키지</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>대화에서 태그 지정되었거나 승인을 해결해야 하는 오브젝트(프로젝트, 작업, 문제, 문서)에 대한 액세스 권한 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>대화에서 태그가 지정되었거나 승인을 해결해야 하는 프로젝트, 작업, 문제, 문서에 대한 [!UICONTROL 보기] 이상의 권한</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 만들기

내 요청 위젯에서 직접 요청을 만들 수 있습니다.

지침은 [홈 영역에서 작업 항목 및 프로젝트 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) 문서의 [요청 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) 섹션을 참조하십시오.

## 요청 복사

내 요청 위젯에서 요청을 복사하고 편집한 다음 새 요청으로 제출할 수 있습니다.

자세한 내용은 [요청 복사 및 제출](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)을 참조하십시오.

## 내 요청 위젯의 요청 목록에서 정보를 관리합니다.

<!--
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. 왼쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/lines-main-menu.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾은 다음 클릭하여 **Home**&#x200B;에 추가합니다.
1. (선택 사항) 정보가 요청 목록에 표시되는 방식을 관리하려면 목록에 대해 다음 보기 요소를 갱신합니다.

   * 보기
   * 필터
   * 열

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   요청 목록에서 정보를 관리하는 방법에 대한 자세한 내용은 [고급 목록 사용](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)을 참조하십시오.


<!-- Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.


The filter is saved automatically.

-->

>[!TIP]
>
>조직에서 Adobe Workfront 외에도 Workfront Planning을 구매한 경우 내 요청 위젯에 Workfront 및 Workfront Planning 요청이 모두 포함됩니다.
> 
>* Workfront 요청만 필터링하려면 필터를 **개체 유형** > **다음 중 하나가 있습니다** > **문제**(으)로 설정하십시오.
>* Workfront Planning 요청만 필터링하려면 필터를 **개체 유형** > **다음 항목 없음** > **문제**(으)로 설정하십시오.

<!--

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## 검색 요청

내 요청 위젯에서 특정 요청을 검색하려면 다음을 수행합니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾은 다음 클릭하여 **Home**&#x200B;에 추가합니다.
1. 내 요청 위젯의 오른쪽 상단 근처에 있는 검색 막대에서 검색할 용어를 입력합니다.

   용어가 포함된 요청은 주황색으로 강조 표시됩니다.

1. (선택 사항) 강조 표시된 요청으로 이동하려면 검색 막대에서 위쪽 또는 아래쪽 화살표를 클릭합니다.

## 요청에 의해 생성된 오브젝트로 이동

내 요청 위젯에서 요청에 의해 생성된 오브젝트를 찾을 수 있습니다.

>[!NOTE]
>
>생성된 객체에 대한 링크는 요청 자체가 객체를 생성한 경우 Planning 요청에 대해서만 새 요청 환경에서 사용할 수 있습니다. Workfront 요청이 프로젝트 또는 다른 오브젝트로 전환되는 경우 전환된 해당 오브젝트에 대한 링크를 새 요청 경험의 요청 목록에서 사용할 수 없습니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **내 요청** 위젯을 홈 화면에 추가합니다. **사용자 지정**&#x200B;을 클릭하고 **내 요청**&#x200B;을 찾은 다음 클릭하여 **Home**&#x200B;에 추가합니다.
1. 개체를 만든 요청을 찾습니다.
1. 해당 요청에 대한 **만들어진 개체** 열에서 개체 이름을 클릭합니다.

   객체의 페이지가 열립니다.

