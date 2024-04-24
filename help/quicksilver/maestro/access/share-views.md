---
title: 보기 공유
description: 보기를 다른 사용자와 공유하여 Adobe Workfront Planning 사용 시 공동 작업을 보장할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# 보기 공유

{{maestro-important-intro}}

보기를 다른 사용자와 공유하여 Adobe Workfront Planning에서 레코드 작업 시 공동 작업을 보장할 수 있습니다.

작업 영역에 권한을 부여해도 다른 사용자에게 레코드 유형 페이지의 보기에 대한 권한이 부여되지 않습니다. 다른 사용자와 공유하려면 레코드 유형 페이지에서 개별 보기에 대한 권한을 부여해야 합니다.

<!--
You can share a view with the following entities: 

* Workfront users
* Workfront groups
* Publicly, with users outside Workfront
-->

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Workfront Planning 마감된 Beta 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> Adobe Workfront Planning에 대한 액세스 제어가 없습니다. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td> <p>보기에 대한 권한 관리</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p> <p>자세한 내용은 <a href="/help/quicksilver/maestro/access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 보기에 대한 권한 공유 <!--internally-->

만든 보기 또는 관리 권한이 있는 보기를 공유할 수 있습니다. <!--with users or groups in Workfront-->.

>[!NOTE]
>
>시스템 관리자는 자신이 만들지 않은 보기를 보거나 공유할 수 없습니다. 공유된 보기에만 액세스하거나 공유할 수 있습니다.
>
>시스템 관리자는 보기에 대한 관리 권한만 가질 수 있습니다.

{{step1-to-maestro}}

1. 보기를 공유할 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다.

   그러면 레코드 유형 페이지가 열립니다.

1. 보기 탭에서 공유할 보기를 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png) 뷰 이름의 오른쪽에 있는 **공유**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. 다음에서 **보기 액세스 권한 부여 대상** 필드에서 사용자 또는 그룹 이름을 입력한 다음 목록에 표시될 때 클릭합니다.  <!--replace screen shot below-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 드롭다운 메뉴에서 다음 권한 수준 중 하나를 선택합니다.
   * 보기
   * 관리

     권한 수준 및 사용자가 각 수준에 대해 수행할 수 있는 작업에 대한 자세한 내용은 [Adobe Workfront Planning의 공유 권한 개요](../access/sharing-permissions-overview.md).

     시스템 관리자는 항상 공유 보기에 대한 관리 권한을 받습니다.

1. 클릭 **링크 복사** 를 클릭하여 보기에 대한 링크를 클립보드에 복사합니다.
1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자는 활성 사용자여야 하며 레코드 유형 페이지에 액세스하여 선택한 보기에 표시할 수 있도록 Workfront에 로그인해야 합니다.
1. **저장**&#x200B;을 클릭합니다.

<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## 보기에 대한 권한 제거

{{step1-to-maestro}}

1. 공유를 중지할 보기를 가진 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다. 그러면 레코드 유형 페이지가 열립니다.
1. 공유를 제거할 보기의 탭 이름 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **공유**.
1. 제거할 사용자 또는 그룹을 찾은 다음 **제거** 사용 권한 드롭다운 메뉴에서 사용자 또는 그룹 이름 오른쪽에 있는 권한
1. 클릭 **저장**.
제거된 그룹에 속한 사용자 또는 사용자는 더 이상 보기에 액세스할 수 없습니다. 보기에 액세스하지 못하도록 제거된 사용자에게 이 액세스 권한을 잃었다는 알림이 없습니다.

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->