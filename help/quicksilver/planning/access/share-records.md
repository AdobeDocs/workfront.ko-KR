---
title: 레코드 공유
description: 공유 버튼을 사용하여 레코드를 공유하면 Adobe Workfront Planning에서 공동 작업을 향상시킬 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/NTytTWD-zq3PVhXn4n-GHinvQxna1wfnAXjaeYBgTEY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 95859f692efbd6ce12238cc03e23e1cecbd99956
workflow-type: tm+mt
source-wordcount: 1713
ht-degree: 2%

---

<!--update metadata with real information at release-->

# 레코드 공유

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>\
<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


{{planning-important-intro}}

Adobe Workfront Planning에서 레코드 유형의 개별 레코드에 대한 사람들의 권한을 조정할 수 있습니다.

다음과 같은 방법으로 Adobe Workfront Planning 레코드를 공유할 수 있습니다.

* 레코드에 대한 링크를 공유합니다.

  자세한 내용은 [링크를 사용하여 레코드 공유](/help/quicksilver/planning/records/share-records.md)를 참조하십시오.

* 작업 영역과 레코드 유형을 공유하여 작업 영역의 모든 레코드를 다른 사용자와 공유합니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [작업 영역 공유](/help/quicksilver/planning/access/share-workspaces.md)

   * [레코드 유형 공유](/help/quicksilver/planning/access/share-record-types.md)

* **공유** 옵션을 사용하여 개별 레코드를 공유하거나 여러 레코드를 일괄적으로 공유합니다.

  이 문서에서는 **공유** 옵션을 사용하여 다른 사용자와 레코드를 공유하는 방법에 대해 설명합니다.

>[!IMPORTANT]
>
>* 작업 영역에 대한 액세스 권한이 있는 사용자는 작업 영역의 모든 레코드에 대한 최소 보기 권한을 자동으로 부여받습니다.
>* 보기를 공유해도 사용자에게 레코드에 대한 권한이 부여되지 않습니다. 공유 작업 영역만 사용자에게 레코드 종류 및 레코드에 대한 권한을 부여할 수 있습니다.
>
>Workfront Planning에서 개체 공유에 대한 일반적인 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Workfront 및 Planning 패키지</p> 
또는
<p>모든 워크플로우 및 계획 패키지</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>Any</p> 
   <p><b>메모</b></p>
   <p>Standard 라이선스가 있는 사람에게만 레코드에 대한 관리 권한을 부여할 수 있습니다. 다른 모든 라이센스는 보기 권한만 가질 수 있으며, 해당 라이센스에 대한 관리 옵션은 흐리게 표시됩니다.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>  <p>작업 공간, 레코드 유형 및 레코드에 대한 권한 관리</p>  
   <p><b>중요</b></p>
   <p>작업 영역에 대한 관리 권한이 있는 사용자만 레코드를 공유할 수 있습니다.</p></td> 
  </tr>
</tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 공유 시 고려 사항

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* 사람, 그룹, 팀, 회사 또는 작업 역할과 같은 엔티티와 레코드를 공유할 수 있습니다.
* 다음과 같은 제한 사항이 있습니다.

   * 한 번에 100개 이상의 레코드를 공유할 수 없습니다.
   * 100개 이상의 엔터티와 레코드를 공유할 수 없습니다.
* 레코드에 대한 권한을 제한하면 사용자는 더 이상 해당 레코드가 표시되는 시스템의 어느 곳에서든 해당 레코드와 조회 필드 값을 볼 수 없습니다.
* Workfront은 최대 5개의 레코드 깊이에 있는 연결에서 레코드 권한을 확인하므로 사용자가 공유된 레코드만 볼 수 있습니다.
* 레코드에 다음 수준의 권한을 부여할 수 있습니다.

   * 보기
   * 관리
* 사용자와 작업 공간 및 레코드 유형을 공유하면 기본적으로 작업 공간의 레코드에 대해 동일한 권한을 받습니다.
사용자가 작업 영역 또는 레코드 유형에 대한 기여 권한을 가지고 있으면 해당 레코드 유형의 레코드에 대한 관리 권한을 받습니다.
* 작업 영역에서 엔티티를 제거하면 모든 공유 권한이 레코드 유형 및 그 안의 모든 레코드에서 제거됩니다.
* 작업 영역 또는 레코드 유형에 대한 권한이 없는 사용자와 레코드를 공유할 수 없습니다.

  작업 영역에 없는 사람과 레코드를 공유하는 경우 해당 레코드가 작업 영역에 자동으로 추가됩니다.
* 사용자의 레코드에 대한 액세스는 다음 3가지 설정의 조합을 통해 결정됩니다.

   * 레코드 유형 및 작업 영역에서 상속된 권한
   * 레코드 공유 상자에 개별적으로 추가된 권한
   * 작업 영역의 모든 사용자가 볼 수 있음&#x200B;**설정.**

     이렇게 하면 작업 공간의 모든 사용자가 레코드를 볼 수 있습니다

     <!--
      Cannot do this on a record: 
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 
      -->

* 사용자와 레코드를 공유하면 기본적으로 레코드 유형에 있는 권한과 동일한 권한으로 추가됩니다.

  예:

   * 레코드 유형에 대한 보기 권한이 있는 경우 레코드에 대한 보기 권한을 갖게 됩니다
   * 레코드 유형에 대한 기여 또는 관리 권한이 있는 경우 레코드에 대한 관리 권한을 얻습니다

* 사용자가 작업 공간 및 레코드 유형에 대한 관리 또는 기여 권한을 가지고 있고 이를 레코드 권한에 추가하면 보기 권한이 흐리게 표시됩니다. 레코드 유형에 대한 권한과 동일한 권한을 보유하며, 레코드에 대해 더 낮은 권한을 부여할 수 없습니다.

* 단일 레코드에 대해 상속된 권한을 비활성화할 수 있습니다. 이 경우 개별 레코드에 대한 권한을 선택한 사용자에게 부여할 수 있습니다. 또는 **작업 영역의 모든 사람이 볼 수 있음** 옵션으로 인해 작업 영역에 속하는 경우 권한을 획득할 수 있습니다.

* 동일한 사용자에 대해 여러 공유 권한이 적용되는 경우 해당 권한은 가장 높은 수준으로 제공됩니다.

  예를 들어 레코드가 보기 권한이 있는 사용자와 공유되고 해당 그룹이 관리 액세스 권한이 있는 경우, 해당 사용자는 레코드에 대한 관리 권한을 받습니다.

* 연결된 레코드의 수식 필드 또는 조회 필드가 사용 권한이 없는 레코드의 필드를 기반으로 하는 경우 다른 방법으로 액세스할 수 없는 레코드의 요소를 올바르게 계산할 수 있습니다.

  <!--
   Not possible: 
   * As a workspace manager, you can share a record with a user that does not have permissions to the record type or the workspace. In this case, there is a warning next to the added entity notifying you that they don't have access to the workspace or the record type.  You can continue adding the user to the record which will also add them to the record type and workspace, or cancel the sharing.
   -->

  <!--
   ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
   -->

<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

<!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

<!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## 레코드 공유

작업 영역 관리자는 개별 레코드에 대한 권한을 조정할 수 있습니다.

{{step1-to-planning}}

1. 작업 영역을 연 다음 공유할 레코드의 레코드 유형을 엽니다.

1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **공유**&#x200B;를 클릭합니다.
   * 표 보기에서 레코드를 하나 이상 선택한 다음 목록 하단의 파란색 도구 모음에서 **공유**&#x200B;를 클릭합니다.
   * 보기에서 레코드 이름을 클릭한 다음 레코드 세부 정보 페이지의 오른쪽 상단에 있는 **공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.

   ![&#128279;](assets/permissions-for-records-with-inherited-permissions-on.png)에서 상속된 사용 권한을 가진 레코드에 대한 사용 권한

   >[!WARNING]
   >
   >다른 작업 공간에 추가된 레코드에 대한 권한을 공유할 수 없습니다. 레코드를 대량으로 공유할 때는 모든 레코드가 동일한 작업 영역에서 생성되어야 합니다.

1. (선택 사항) **액세스 권한이 있는 사용자** 영역에서 **작업 영역의 모든 사용자가 볼 수 있음** 옵션이 기본적으로 선택됩니다.  작업 영역 및 레코드 유형에 대해 **보기** 이상의 권한이 있는 모든 사용자는 레코드에 대해 동일한 권한을 가집니다.

1. (선택 사항) 작업 영역에서 권한을 상속하는 사용자, 팀, 그룹, 회사 또는 작업 역할을 보려면 **다음에서 상속된 권한** 옵션 아래의 사용자 아바타를 클릭합니다. <!--logged bug to move "Permissions" to lowercase-->

   레코드 유형에 대한 사용자의 권한은 상속된 권한을 확장할 때 표시됩니다.

   >[!TIP]
   >
   >상속된 권한 목록에서 개별 엔티티를 제거할 수 없습니다. 작업 공간 및 레코드 유형이 공유될 때 연관된 엔티티 대신 팀, 그룹, 회사 또는 작업 역할의 사용자가 나열됩니다.

1. (선택 사항 및 조건부) 특정 엔티티와 레코드를 공유하고 작업 공간에 이미 있는 것과 다른 레코드 유형에 대한 액세스 권한을 부여하려면 다음을 수행합니다.

   1. **상속된 사용 권한**&#x200B;에서 **켜짐** 옵션을 선택 취소합니다. 기본적으로 선택되어 있습니다.

      옵션이 **꺼짐**(으)로 변경됩니다.

      >[!TIP]
      >
      >Workspace 관리자 및 레코드 작성자는 레코드 유형 및 레코드에 대한 관리 권한을 계속 갖게 됩니다.

      <!-- 
      This is no longer possible for a record: 
      (Optional) Select **Only invited people can access** from the **Who has access** area. You must indicate individual users, groups, teams, or companies to share the records with. 
      >[!TIP]
      >
      >You cannot disable or enable Inherited permissions when this setting is selected.
      -->

   1. **이 레코드에 대한 액세스 권한 부여** 필드에서 작업 영역 또는 레코드 형식에 대해 부여한 권한 수준과 다른 권한 수준을 부여할 사용자, 팀, 그룹, 회사 또는 작업 역할을 추가합니다.

      사용자와 레코드를 공유하면 기본 작업 역할과 이메일도 필드에 표시됩니다. 사용자 이메일을 보려면 액세스 수준의 사용자 개체에 대해 연락처 정보 보기 설정을 활성화해야 합니다.

   1. 다음 권한 수준 중 하나를 선택합니다.

      * 보기
      * 관리

      >[!IMPORTANT]
      >
      >* 사용자가 작업 공간 및 레코드 유형에 대한 기여 또는 관리 권한이 있는 경우 해당 사용자에게 레코드에 대한 관리 권한을 부여할 수 있습니다. 보기 권한이 흐리게 표시됩니다.
      >* 사용자에게 레코드 유형에 대한 Contribute 이상이 있으면 레코드에 대한 권한을 줄일 수 없습니다.
      >자세한 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.
      >* 작업 영역에 없는 사용자에게는 권한을 부여할 수 없습니다. 작업 공간 및 레코드 유형에 대한 권한이 없는 사용자는 레코드에 액세스할 수 없습니다.

   <!--   
   Not possible:
   1. To give users who do not have permissions to the workspace access to view a record, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 
      The entity you selected is added to the record and also to the record type and the workspace with **View** permissions. 
      System administrators always receive Manage permissions to records shared with them, and there is an indication that a user is a System administrator.
   -->

1. (선택 사항) **링크 복사**&#x200B;를 클릭하여 레코드에 대한 링크를 클립보드에 복사하고 다른 사용자와 공유합니다. 이 링크를 클릭하면 레코드의 세부 정보 페이지가 열립니다.
1. **저장**&#x200B;을 클릭합니다.

   이제 레코드가 다른 사용자와 공유됩니다.

   레코드를 공유한 사용자는 레코드에 대한 권한이 부여되었다는 인앱과 이메일 알림을 모두 수신합니다.

   <!--
   not possible anymore: 
   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them.
   -->

   자세한 내용은 [Adobe Workfront Planning 알림: 문서 색인](/help/quicksilver/planning/notifications/notifications-information.md)을 참조하십시오.


1. (선택 사항) 복사한 링크를 다른 사용자와 공유합니다.

   링크를 받은 사용자는 활성 사용자여야 하며 레코드 유형 페이지에 액세스하여 선택한 보기에 표시할 수 있도록 Workfront에 로그인해야 합니다.

   레코드 유형을 볼 수 있으려면 레코드 유형에 대한 권한이 있어야 합니다.

   자세한 내용은 [링크를 사용하여 레코드 공유](/help/quicksilver/planning/records/share-records.md)도 참조하세요.


## 레코드에 대한 권한 제거

레코드에서 사용자의 권한을 제거할 수 있습니다. 그러나 레코드 유형에 대해 적어도 보기 권한을 제공하는 작업 영역에 대해 적어도 보기 권한은 유지됩니다.

작업 영역의 레코드 유형 또는 레코드에 대한 권한이 없도록 하려면 작업 영역에서 해당 액세스 권한을 제거해야 합니다.

상속된 권한에서는 사용자를 제거할 수 없습니다.

{{step1-to-planning}}

1. 공유를 중지할 레코드가 있는 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다. 그러면 레코드 유형 페이지가 열립니다.
1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **공유**&#x200B;를 클릭합니다.
   * 표 보기에서 레코드를 하나 또는 여러 개 선택한 다음 목록 하단의 파란색 도구 모음에서 **공유**&#x200B;를 클릭합니다.

     동일한 작업 영역에서 생성된 레코드를 선택해야 합니다.
   * 보기에서 레코드 이름을 클릭한 다음 레코드 세부 정보 페이지의 오른쪽 상단에 있는 **공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.
1. 권한을 제거할 사용자, 그룹, 팀, 회사 또는 작업 역할을 찾은 다음 이름 오른쪽에 있는 권한 드롭다운 메뉴를 확장한 다음 **제거**&#x200B;를 클릭합니다.

   ![레코드에 대한 권한 제거](assets/remove-option-on-record-sharing-drop-down.png)

1. **저장**&#x200B;을 클릭합니다.

   직원들에게 더 이상 레코드에 대한 표시된 권한이 없습니다. 그러나 레코드 유형 및 작업 영역도 해당 권한에서 제거하지 않는 한 해당 권한에 대한 권한이 남아 있습니다.

   더 이상 이러한 권한이 없다는 알림이 레코드에 액세스할 수 없도록 제거된 사용자에게 없습니다.
