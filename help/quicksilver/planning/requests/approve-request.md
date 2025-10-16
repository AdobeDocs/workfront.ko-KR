---
title: Adobe Workfront Planning에서 요청 승인
description: 사용자가 Adobe Workfront Planning의 승인과 연결된 요청 양식에 요청을 제출하면 승인자는 보류 중인 승인에 대한 알림 및 이메일을 수신합니다. Workfront Planning에서 개체를 만들기 전에 요청을 승인해야 합니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 1%

---

# Adobe Workfront Planning에서 요청 승인

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

사용자가 Adobe Workfront Planning의 승인과 연결된 요청 양식에 요청을 제출하면 승인자는 보류 중인 승인에 대한 알림 및 이메일을 수신합니다. Workfront Planning에서 개체를 만들기 전에 요청을 승인해야 합니다.

이 문서에서는 작업 영역 관리자가 레코드를 만들기 위해 Workfront Planning에 제출된 요청을 승인하는 방법에 대해 설명합니다.

다음 문서도 보는 것이 좋습니다.

* [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)
* [Adobe Workfront Planning 요청을 제출하여 레코드 생성](/help/quicksilver/planning/requests/submit-requests.md)
* [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## 요청 승인에 대한 고려 사항

* 제출된 요청은 Workfront의 요청 영역에서 제출된 섹션의 계획 탭에 다음 요청 상태 중 하나로 표시됩니다.

   * **검토 보류 중**: 승인자가 요청 개체를 열지 않은 경우 이 상태가 표시됩니다.
   * **검토 중**: 하나 이상의 승인자가 요청 개체를 열면 **검토 보류 중** 상태가 **검토 중**(으)로 변경됩니다. 모든 승인자가 요청을 승인할 때까지 요청의 상태가 **검토 중** 상태로 유지됩니다.
   * **승인됨**: 승인자가 요청 개체를 승인하면 개별 상태는 **승인됨**&#x200B;이 되지만, 전체 요청 개체 상태는 모든 승인자가 결정을 내릴 때까지 **검토 중**&#x200B;으로 유지됩니다. 모든 승인자가 요청을 승인하면 요청 상태는 **승인됨**&#x200B;이 됩니다.
   * **완료**: 모든 승인자가 요청 개체를 승인하면 상태가 **완료**(으)로 변경되거나 요청에 승인이 필요하지 않은 경우.
   * **거부됨**: 승인자가 요청 개체를 거부하면 상태는 **거부됨**&#x200B;이 됩니다. 레코드가 만들어지지 않으며 레코드를 만들려면 새 요청을 제출해야 합니다.

* 승인자 및 승인 일자 필드에 요청 양식을 실행하여 생성된 레코드에 승인 정보를 표시할 수 있습니다. 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul><li><p>모든 Workfront 패키지</p></li>
And
<li><p>모든 Planning 패키지</p></li></ul>
또는
<ul><li><p>모든 워크플로우 패키지</p></li>
And
<li><p>모든 Planning 패키지</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 및 레코드 종류</a>에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 만들기 요청 승인

사용자가 승인과 연결된 레코드 유형 요청 양식에 요청을 추가하면 요청이 승인자에게 전송됩니다.

승인자는 승인 보류 중인 요청에 대해 다음 알림을 받습니다.

* 인앱 알림
* 이메일 알림

>[!NOTE]
>
>사용자가 이메일 및 인앱 알림을 수신할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.

요청을 승인하려면:

1. 다음 중 하나를 수행하십시오.

   * Workfront Planning에 액세스하여 하나 이상의 작업 영역을 볼 수 있는 경우 화면 오른쪽 상단의 **주 메뉴** ![점 주 메뉴](assets/dots-menu.png) 또는 사용 가능한 경우 왼쪽 상단의 **주 메뉴** ![선 주 메뉴](assets/lines-menu.png)를 클릭한 다음 **요청** > **제출됨** > **계획**&#x200B;을 클릭하고 **검토 보류 중** 또는 **검토 중** 상태의 요청을 클릭합니다.

     >[!TIP]
     >
     >Workfront Planning에 대한 액세스 권한이 없거나 작업 영역을 볼 수 있는 액세스 권한이 없는 경우 이메일 또는 인앱 알림을 사용하는 승인 요청에만 액세스할 수 있습니다.

   * 화면 오른쪽 상단에 있는 **알림** 영역 아이콘 ![통합 셸의 알림 영역 아이콘](assets/notifications-area-icon-unified-shell.png)을 클릭하고 승인 보류 중인 요청에 대한 알림을 클릭하여 요청을 엽니다.
   * 승인 보류 중인 요청을 알리는 전자 메일의 전자 메일 알림으로 이동한 다음 **요청 열기**&#x200B;를 클릭하여 요청을 엽니다. <!--add the name of the button here, from the email-->

   요청 페이지가 읽기 전용 모드로 열립니다.

   ![검토 상태의 읽기 전용 요청 페이지](assets/read-only-reqeust-page-in-review-status.png)

1. (선택 사항) 승인자를 보려면 요청의 오른쪽 상단에 있는 **승인** 아이콘 ![승인 아이콘](assets/approvals-icon.png)을 클릭합니다.
1. **검토 및 승인**&#x200B;을 클릭한 후 다음 중 하나를 선택하십시오.

   * **승인**: 요청을 승인합니다. 모든 승인자가 요청을 승인한 후 요청 양식과 연결된 레코드 유형에 대해 레코드가 즉시 만들어집니다.
   * **거부**: 사용자가 요청을 거부하는 유일한 승인자인 경우에도 이 요청은 거부됩니다. 요청 양식과 연결된 레코드 유형에 대해 만들어진 레코드가 없습니다.

   요청을 제출한 사용자는 요청이 승인되거나 거부되면 이메일 및 인앱 알림을 받게 됩니다.

   승인 결정에 따라 요청의 상태가 다음으로 변경됩니다.

   * **완료**: 요청이 승인되었습니다.
   * **거부됨**: 요청이 거부되었습니다.

   요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭에 남아 있습니다.
