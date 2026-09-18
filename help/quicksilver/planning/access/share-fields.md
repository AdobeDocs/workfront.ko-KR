---
title: Workfront 계획 필드 공유
description: Adobe Workfront Planning 레코드 필드를 다른 사용자와 공유하여 Workfront Planning 사용 시 공동 작업을 보장할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 2%
---

# Workfront Planning 필드 공유

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Adobe Workfront Planning 레코드 필드를 다른 사용자와 공유하여 Workfront Planning 사용 시 공동 작업을 보장할 수 있습니다.

필드 공유를 통해 작업 공간 관리자는 개별 필드에 대한 액세스를 제어할 수 있습니다. 레코드 유형의 각 필드에는 액세스 권한 없음, 필드 값 보기 또는 필드 값 관리로 액세스를 설정할 수 있는 자체 공유 대화 상자가 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



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
<p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p> 
또는
<p>모든 Workfront Planning을 독립 실행형 제품 패키지로</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>Any</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Planning 라이선스</p></td> 
   <td><p>Any</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가해야 합니다.</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td><p>필드에 대한 권한을 관리하여 필드 값 변경</p>  
   <p>레코드 유형에 대한 또는 그 이상의 권한을 기여하여 필드에 대한 관리 권한을 상속합니다.</p>  
   </td> 
  </tr>
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 필드 공유에 대한 고려 사항

* 사용자, 작업 역할, 그룹, 팀 또는 회사와 필드를 공유할 수 있습니다.
* 레코드 종류의 테이블 보기에서만 필드를 공유할 수 있습니다.
* 다음 유형의 필드는 공유할 수 없습니다.

  * 시스템 필드(예: 작성자, 레코드 ID)
  * 기본 필드
  * 조회 필드. 이 사용자는 항상 소스 오브젝트 필드의 권한을 상속합니다.
* 필드에 대한 액세스는 다음 설정을 결합하여 가져옵니다.

  * **상속된 사용 권한**: 기본적으로 필드는 다른 사람이 레코드 형식에 대해 가지고 있는 동일한 액세스 권한을 상속합니다. 상속된 권한을 끄고 사용자에게 레코드 유형에 대한 액세스 권한보다 낮은 수준의 필드 액세스 권한을 부여할 수 있습니다.
  * **작업 영역의 모든 사용자가 볼 수 있음** 또는 **초대된 사용자만 액세스**&#x200B;할 수 있습니다. 작업 영역에 대한 권한이 있는 모든 사람이 필드를 보도록 허용하거나 개별 엔터티에만 권한을 부여할 수 있습니다.

  동일한 사람에게 여러 개의 규칙이 적용되는 경우, 규칙 중 하나에서 사용자에게 사용 가능한 가장 높은 권한을 부여합니다.

* 레코드 유형 권한에 따라 사용자는 다음 필드 권한을 받을 수 있습니다.

  * 레코드 유형 보기 권한 사용자에게 필드 값을 볼 수 있는 권한 부여
  * 기여 또는 레코드 유형 관리 권한을 통해 사용자는 필드 값을 관리할 수 있습니다.

* 작업 영역 소유자 및 관리자만 필드 권한을 조정할 수 있습니다. Workspace 관리자는 항상 모든 필드에 대한 관리 액세스 권한을 유지하며 이를 낮출 수 없습니다.
* 필드 공유는 필드 설정이 아니라 값에 대한 액세스를 제어합니다. 작업 영역 관리자만 필드의 구성을 변경할 수 있습니다.
* 필드의 공유 목록에 사용자를 추가해도 작업 공간이나 레코드 유형 액세스 권한은 부여되지 않습니다. 액세스 권한이 없는 경우 경고 아이콘은 레코드 유형에 추가된 후에만 권한이 적용됨을 나타냅니다.
* 제한된 권한이 있는 필드는 필드가 표시되는 모든 곳에서 적용됩니다. 여기에는 모든 보기, 레코드 세부 사항 페이지, 요청 양식, 연결 및 조회 필드, 캔버스 대시보드, API 및 MCP 도구가 포함됩니다.
* 공개 보기는 액세스할 수 있는 모든 사람에게 완전히 표시되며 읽기 전용입니다.
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* 제한된 필드 값 변경 사항은 레코드 기록에 기록되지 않습니다.
* 필드에 대한 권한 변경이 알림을 트리거하지 않습니다.
* 글로벌 레코드 유형의 경우 필드 권한은 모든 보조 작업 영역에 적용되며 로컬로 조정할 수 없습니다.

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## 필드 공유

작업 영역 관리자는 개별 필드에 대한 권한을 조정할 수 있습니다.

{{step1-to-planning}}

1. 작업 영역을 연 다음 공유할 필드의 레코드 유형을 엽니다.

1. 테이블 보기에서 필드의 열 머리글 이름 위로 마우스를 가져간 후 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **필드 공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.

1. (선택 사항) **액세스 권한 부여** 영역에서 **작업 영역의 모든 사용자가 볼 수 있음** 옵션이 기본적으로 선택됩니다. 작업 영역 및 레코드 유형에 대해 **보기** 이상의 권한이 있는 모든 사용자는 필드에 대해 동일한 권한을 가집니다.

1. (선택 사항) 작업 영역에서 권한을 상속하는 사용자, 팀, 그룹, 회사 또는 작업 역할을 보려면 **다음에서 상속된 권한** 옵션 아래의 사용자 아바타를 클릭합니다.

   레코드 유형에 대한 사용자의 권한은 상속된 권한을 확장할 때 표시됩니다.

   >[!TIP]
   >
   >상속된 권한 목록에서 개별 엔티티를 제거할 수 없습니다. 작업 공간 및 레코드 유형이 공유될 때 연관된 엔티티 대신 팀, 그룹, 회사 또는 작업 역할의 사용자가 나열됩니다.

1. (선택 사항 및 조건부) 특정 엔티티와 필드를 공유하고 레코드 유형에 대해 기존 액세스 권한과 다른 필드 액세스 권한을 부여하려면 다음을 수행하십시오.

   1. **상속된 사용 권한**&#x200B;에서 **켜짐** 옵션을 선택 취소합니다. 기본적으로 선택되어 있습니다.

      옵션이 **꺼짐**(으)로 변경됩니다.

      >[!TIP]
      >
      >Workspace 관리자는 레코드 종류 및 필드에 대한 관리 권한을 계속 갖게 됩니다.

   1. **액세스 권한 부여** 상자에서 작업 영역 또는 레코드 형식에 대해 다른 권한 수준을 부여할 사용자, 팀, 그룹, 회사 또는 작업 역할을 추가합니다.

      사용자와 필드를 공유할 때 기본 작업 역할과 이메일도 필드에 표시됩니다. 사용자 이메일을 보려면 액세스 수준의 사용자 개체에 대해 연락처 정보 보기 설정을 활성화해야 합니다.

   1. 다음 권한 수준 중 하나를 선택합니다.

      * 필드 값 보기
      * 필드 값 관리

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* 레코드 유형에 대한 Contribute 이상이 있는 경우 사용자에게 필드에 대한 사용 권한을 적게 부여할 수 없습니다.
      >
      >* 작업 영역에 없는 사용자에게는 권한을 부여할 수 없습니다. 작업 공간 및 레코드 유형에 대한 권한이 없는 사용자는 필드에 액세스할 수 없습니다. 작업 영역 및 레코드 유형에 대한 권한을 얻으면 필드에 액세스할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

   이제 필드가 다른 사용자와 공유됩니다.

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## 필드에 대한 권한 제거

필드에서 사용자의 권한을 제거할 수 있습니다. 하지만 작업 영역에 대한 적어도 보기 권한은 유지되며 필드에 대한 적어도 보기 권한을 부여하는 레코드 유형도 유지됩니다.

작업 영역의 레코드 유형 또는 필드에 대한 권한이 없는 경우에는 작업 영역에서 해당 액세스 권한을 제거해야 합니다.

상속된 권한에서는 사용자를 제거할 수 없습니다.

{{step1-to-planning}}

1. 공유를 중지할 필드가 있는 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다. 그러면 레코드 유형 페이지가 열립니다.
1. 테이블 보기에서 필드의 열 머리글 이름 위로 마우스를 가져간 후 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **필드 공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.
1. 권한을 제거할 사용자, 그룹, 팀, 회사 또는 작업 역할을 찾은 다음 이름 오른쪽에 있는 권한 드롭다운 메뉴를 확장한 다음 **제거**&#x200B;를 클릭합니다.

1. **저장**&#x200B;을 클릭합니다.

   사용자에게는 더 이상 필드에 대해 표시된 권한이 없습니다. 그러나 레코드 유형 및 작업 영역도 해당 권한에서 제거하지 않는 한 해당 권한에 대한 권한이 계속 있습니다.

   필드 액세스에서 제거된 사용자에게 더 이상 이러한 권한이 없다는 알림이 없습니다.
