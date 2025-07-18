---
title: 레코드 유형 공유
description: Adobe Workfront Planning 사용 시 공동 작업을 보장하기 위해 다른 사용자와 레코드 유형을 공유할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 58d2bf9f14b9a3adf4bacfad58f1b9862aeaf247
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# 레코드 유형 공유

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning에서 레코드 작업을 할 때 공동 작업을 보장하기 위해 다른 사용자와 레코드 유형을 공유할 수 있습니다.

>[!IMPORTANT]
>
>작업 영역에 대한 액세스 권한이 있는 사용자는 작업 영역의 모든 레코드 유형에 대해 적어도 보기 권한을 자동으로 부여받습니다.
>>보기를 공유해도 사용자에게 레코드 유형에 대한 권한이 부여되지 않습니다. 공유 작업 영역만 사용자에게 레코드 유형에 대한 권한을 부여할 수 있습니다.
>
>* Workfront Planning에서 개체 공유에 대한 일반적인 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.
>* 자세한 내용은 이 문서의 [레코드 종류 공유 시 고려 사항](#considerations-when-sharing-record-types) 섹션을 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>Workfront Planning 보기에 대한 권한을 얻으려면 Adobe Admin Console에 사용자를 추가해야 합니다.</p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>  <p>레코드 유형에 대한 권한 관리</p>  
   <p>작업 영역에 대한 관리 권한이 있는 사용자만 레코드 유형에 대한 관리 권한을 공유할 수 있습니다.</p></td> 
  </tr>

</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 유형 공유 시 고려 사항

* 작업 영역에 권한을 부여하면 기본적으로 작업 영역의 레코드 유형에 대해 동일한 권한이 사용자에게 부여됩니다.

  또한 개별 레코드 유형에 대한 권한을 조정할 수 있습니다.

  그러나 작업 영역에 대해 가지고 있는 권한보다 레코드 유형에 대해 더 높은 권한을 부여할 수는 없습니다.
* 작업 영역에서 사용자에게 기록 유형에 대한 사용 권한을 보다 낮게 부여할 수 있습니다. 예를 들어 작업 공간에 대한 기여 권한 및 레코드 유형에 대한 보기 권한이 있을 수 있습니다.
* 작업 영역에 대한 관리 권한이 있는 직원은 항상 작업 영역의 모든 레코드 유형에 대한 관리 액세스 권한을 유지합니다. 상속된 권한이 꺼져 있더라도 레코드 유형에서 해당 권한을 낮출 수 없습니다.

* 현재 레코드 유형을 공유할 때 다음을 수행할 수 있습니다.

   * 기록 유형을 처음 공유하지만 작업 공간에 대한 권한이 없는 경우, 사용자에게 작업 공간에 대한 보기 권한을 부여합니다.

     또한 작업 영역의 모든 레코드 유형에 대해 보기 권한을 부여합니다.

     레코드 유형에 대한 권한을 부여하면 공유 상자에 해당 레코드 또한 작업 공간에 추가된다는 표시가 나타납니다.
   * 상속된 권한을 비활성화할 때는 작업 영역의 모든 사용자(작업 영역 관리자는 제외)에 대해 레코드 유형을 보기 전용으로 만듭니다.

     작업 영역에 대한 관리 권한이 있는 사람은 레코드 유형에 대해 상속된 권한을 해제할 때에도 항상 레코드 유형에 대한 관리 권한을 갖습니다.
   * 레코드 유형에 대한 사용자의 사용 권한을 낮춥니다. 작업 공간에 있는 레코드 유형에서 다른 사람의 레코드 유형 권한을 늘릴 수 없습니다.

     예를 들어 작업 영역에 대한 기여 권한이 있는 사용자가 자신의 권한을 특정 레코드 유형으로 [보기]로 변경할 수 있습니다. 그러나 작업 영역에 대한 보기 권한이 있는 경우 레코드 유형에 Contribute 권한을 부여할 수 없습니다.

* 작업 영역의 사용자에 대한 레코드 종류에 대한 액세스 권한을 제거할 수 없습니다. 작업 영역에 대해 적어도 보기 권한이 있는 경우 모든 사용자는 항상 모든 레코드 유형에 대해 적어도 보기 권한을 갖습니다.

* 다음 엔티티와 내부적으로 레코드 유형을 공유할 수 있습니다.

  Workfront 사용자, 그룹, 팀, 회사 및 작업 역할
* 레코드 유형은 Workfront 외부의 사용자와 외부에서 공유할 수 없습니다.
* 작업 공간 권한이 보기 권한보다 높지 않은 사용자에게 레코드 유형에 대한 권한을 부여하려면 먼저 보기 권한보다 높은 권한을 가진 사용자와 작업 공간을 공유해야 합니다. 그러면 레코드 유형에 작업 공간에 대한 더 높은 권한이 적용됩니다.

## 레코드 종류에 대한 권한 공유

작업 공간에 대한 관리 권한이 있는 경우 작업 공간의 개별 레코드 유형에 대한 권한을 조정할 수 있습니다.

{{step1-to-planning}}

1. 레코드 유형을 공유할 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다.

   그러면 레코드 유형 페이지가 열립니다.

1. 보기의 탭에서 레코드 종류의 오른쪽 상단의 **공유**&#x200B;를 클릭합니다.
1. **레코드 종류 공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.

   ![에서 상속된 사용 권한을 가진 레코드 형식에 대한 ](assets/permissions-for-record-types-with-inherited-permissions-on.png)사용 권한

1. (선택 사항) **액세스 권한이 있는 사용자** 영역에서 **작업 영역의 모든 사용자가 볼 수 있음** 옵션이 기본적으로 선택됩니다.  작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자는 레코드 유형을 볼 수 있습니다.

1. (선택 사항) 작업 영역에서 권한을 상속하는 사용자, 팀, 그룹, 회사 또는 작업 역할을 보려면 **상속된 권한** 옵션 아래의 사용자 수를 클릭합니다.

   >[!TIP]
   >
   >상속된 권한 목록에서 개별 엔티티를 제거할 수 없습니다.


1. (선택 사항 및 조건부) 특정 엔티티와 레코드 유형을 공유하고 작업 공간에 이미 있는 것과 다른 레코드 유형에 대한 액세스 권한을 부여하려면 다음을 수행합니다.

   1. **상속된 권한** 드롭다운 메뉴에서 **사용 안 함**&#x200B;을(를) 선택합니다.

   >[!TIP]
   >
   >Workspace 관리자는 레코드 유형에 대한 관리 권한을 계속 보유합니다.

   1. **이 레코드 형식에 대한 액세스 권한 부여** 필드에서 작업 영역에 대해 부여한 권한 수준과 다른 권한 수준을 부여할 사용자, 팀, 그룹, 회사 또는 작업 역할을 추가합니다.
   1. 권한 수준을 선택합니다.

   >[!IMPORTANT]
   >
   >* 팀, 그룹, 회사 및 작업 역할 외에도 Adobe Admin Console에 추가된 사용자와만 공유할 수 있습니다. Workfront 전용 사용자는 추가할 수 없습니다. 자세한 내용은 [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)를 참조하십시오.
   >* 작업 영역에서 사용자에게 기록 유형에 대한 권한보다 더 큰 권한을 부여할 수 없습니다.
   >* 작업 영역에 대한 관리 권한이 있는 경우 사용자에게 레코드 유형에 대한 관리 권한보다 적은 권한을 부여할 수 없습니다.
   >* 작업 영역에 대한 기여 권한이 있는 경우 사용자에게 레코드 유형에 대한 권한을 덜 부여할 수 있습니다.
   > 자세한 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.

1. 작업 영역에 대한 액세스 권한이 없는 사용자에게 레코드 종류를 볼 수 있는 액세스 권한을 부여하려면 **이 보기에 대한 액세스 권한 부여** 필드에 사용자, 그룹, 팀, 회사 또는 작업 역할의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   선택한 엔터티가 레코드 종류 및 **보기** 권한이 있는 작업 영역에 추가됩니다.

   시스템 관리자는 항상 공유 레코드 유형에 대한 관리 권한을 받으며, 사용자가 시스템 관리자임을 나타냅니다.

1. (선택 사항) **링크 복사**&#x200B;를 클릭하여 레코드 종류에 대한 링크를 클립보드에 복사하고 다른 사용자와 공유합니다.
1. **저장**&#x200B;을 클릭합니다.

   이제 레코드 유형이 다른 사용자와 공유됩니다.
와 레코드 유형을 공유한 사용자는 다음 엔티티에 대한 권한 부여에 대한 인앱 및 이메일 알림을 모두 수신합니다.

   * 레코드 유형
   * 기록 유형을 작업 영역과 공유하기 전에 작업 영역에 대한 권한이 없었던 경우 작업 영역입니다.

1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자는 활성 사용자여야 하며 레코드 유형 페이지에 액세스하여 선택한 보기에 표시할 수 있도록 Workfront에 로그인해야 합니다. 레코드 유형을 볼 수 있으려면 레코드 유형에 대한 권한이 있어야 합니다.

## 레코드 유형에 대한 권한 제거

레코드 유형에서 사용자의 권한을 제거할 수 있습니다. 그러나 레코드 유형에 대해 적어도 보기 권한을 제공하는 작업 영역에 대해 적어도 보기 권한은 유지됩니다. 작업 영역의 레코드 유형에 대한 권한이 없도록 하려면 작업 영역에서 해당 액세스 권한을 제거해야 합니다.

{{step1-to-planning}}

1. 공유를 중지할 레코드 종류가 있는 작업 영역을 연 다음 레코드 종류 카드를 클릭합니다. 그러면 레코드 유형 페이지가 열립니다.

1. 보기의 탭에서 레코드 종류의 오른쪽 상단의 **공유**&#x200B;를 클릭합니다.
1. **레코드 종류 공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.
1. 권한을 제거할 사용자, 그룹, 팀, 회사 또는 작업 역할을 찾은 다음 이름 오른쪽에 있는 권한 드롭다운 메뉴를 확장한 다음 **제거**&#x200B;를 클릭합니다. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![레코드 형식 공유 드롭다운에서 옵션 제거](assets/remove-option-on-record-type-sharing-drop-down.png)

1. **저장**&#x200B;을 클릭합니다.

   직원들에게 더 이상 레코드 종류에 대해 표시된 권한이 없습니다. 하지만 작업 영역 권한에서도 제거하지 않는 한 해당 작업공간에 대한 권한은 계속 있습니다.

   보기에 액세스하지 못하도록 제거된 사용자에게 더 이상 이 액세스 권한이 없다는 알림이 없습니다.

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

