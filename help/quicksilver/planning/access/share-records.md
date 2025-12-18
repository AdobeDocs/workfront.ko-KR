---
title: 레코드 공유
description: 공유 버튼을 사용하여 레코드를 공유하면 Adobe Workfront Planning에서 공동 작업을 향상시킬 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1772'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# 레코드 공유

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

레코드 종류의 개별 레코드에 대한 사용자의 권한을 조정할 수 있습니다.

다음과 같은 방법으로 Adobe Workfront Planning 레코드를 공유할 수 있습니다.

* 레코드에 대한 링크를 공유합니다.

  자세한 내용은 [링크를 사용하여 레코드 공유](/help/quicksilver/planning/records/share-records.md)를 참조하십시오.

* 작업 영역과 레코드 유형을 공유하여 작업 영역의 모든 레코드를 다른 사용자와 공유합니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [작업 영역 공유](/help/quicksilver/planning/access/share-workspaces.md)

   * [레코드 유형 공유](/help/quicksilver/planning/access/share-record-types.md)

* **공유** 옵션을 사용하여 레코드를 공유합니다.

  이 문서에서는 **공유** 옵션을 사용하여 다른 사용자와 레코드를 공유하는 방법에 대해 설명합니다.

>[!IMPORTANT]
>
>작업 영역에 대한 액세스 권한이 있는 사용자는 작업 영역의 모든 레코드에 대한 최소 보기 권한을 자동으로 부여받습니다.
>보기를 공유해도 사용자에게 레코드에 대한 권한이 부여되지 않습니다. 공유 작업 영역만 사용자에게 레코드 종류 및 레코드에 대한 권한을 부여할 수 있습니다.
>
>Workfront Planning에서 개체 공유에 대한 일반적인 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.


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
<p>모든 Workfront 및 Planning 패키지</p> 
또는
<p>모든 워크플로우 및 계획 패키지</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>임의</p> 
   <p><b>메모</b></p>
   <p>Standard 라이선스가 있는 사람에게만 레코드에 대한 관리 권한을 부여할 수 있습니다. 다른 모든 라이센스는 보기 권한만 가질 수 있으며, 해당 라이센스에 대한 관리 옵션은 흐리게 표시됩니다.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>  <p>작업 공간, 레코드 유형 및 레코드에 대한 권한 관리</p>  
   <p><b>중요</b></p>
   <p>작업 영역에 대한 관리 권한이 있는 사용자만 레코드를 공유할 수 있습니다.</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> 라이트 또는 기여자 라이선스가 있는 사용자에게 Planning이 포함된 레이아웃 템플릿을 할당해야 합니다.
   <p>표준 사용자 및 시스템 관리자에게는 기본적으로 계획 영역이 활성화되어 있습니다.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 공유 시 고려 사항

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* 사람, 그룹, 팀, 회사 또는 작업 역할과 같은 엔티티와 레코드를 공유할 수 있습니다.
* 레코드에 다음 수준의 권한을 부여할 수 있습니다.

   * 보기
   * 관리
* 사용자와 작업 공간 및 레코드 유형을 공유하면 기본적으로 작업 공간의 레코드에 대해 동일한 권한을 받습니다.
사용자가 작업 영역 또는 레코드 유형에 대한 기여 권한을 가지고 있으면 해당 레코드 유형의 레코드에 대한 관리 권한을 받습니다.
* 작업 영역에서 엔티티를 제거하면 모든 공유 권한이 레코드 유형 및 그 안의 모든 레코드에서 제거됩니다.
* 사용자의 레코드에 대한 액세스는 다음 3가지 설정의 조합을 통해 결정됩니다.

   * 레코드 유형 및 작업 영역에서 상속된 권한
   * 레코드 공유 대화 상자에서 개별적으로 추가된 권한
   * 다음 권한:

      * **작업 영역의 모든 사용자가 볼 수 있음**: 이 경우 작업 영역의 모든 사용자가 레코드를 볼 수 있습니다. <!-- is this OK to say "workspace? should it be "record"??-->
      * **초대된 사람만 액세스할 수 있습니다**: 이 옵션은 기본적으로 선택되어 있으며 특정 사람에게 레코드에 대한 액세스를 제한할 수 있습니다.

     >[!NOTE]
     >
     >**작업 영역의 모든 사용자에게 레코드 종류 또는 레코드에 대한 사용 권한 보기**&#x200B;를 부여하도록 선택하면 작업 영역 사용 권한의 공유 목록에 나열된 모든 사용자에게 레코드 종류 및 레코드에 대한 동일한 사용 권한이 부여됩니다. 이는 상속된 사용 권한이 비활성화된 경우에도 마찬가지입니다.


* 사용자와 레코드를 공유하면 기본적으로 레코드 유형에 있는 권한과 동일한 권한으로 추가됩니다.

  예:

   * 레코드 유형에 대한 보기 권한이 있는 경우 레코드에 대한 보기 권한을 갖게 됩니다
   * 레코드 유형에 대한 기여 또는 관리 권한이 있는 경우 레코드에 대한 관리 권한을 얻습니다

* 작업 영역 관리자는 레코드 유형 또는 작업 영역에 대한 권한이 없는 사용자와 레코드를 공유할 수 있습니다. 이 경우 추가된 엔티티 옆에 작업 영역 또는 레코드 유형에 액세스할 수 없음을 알리는 경고가 있습니다. <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> 레코드 종류 및 작업 영역에 사용자를 추가하거나 공유를 취소할 레코드에 사용자를 계속 추가할 수 있습니다.

* 사용자가 작업 공간 및 레코드 유형에 대한 관리 또는 기여 권한을 가지고 있고 이를 레코드 권한에 추가하면 보기 권한이 흐리게 표시됩니다. 레코드 유형에 대한 권한과 동일한 권한을 보유하며, 레코드에 대해 더 낮은 권한을 부여할 수 없습니다. <!--Lilit is checking on this, it is not working correctly-->

  작업 영역 또는 레코드 유형에 대한 보기 권한이 있는 경우 레코드에 대한 보기 권한은 그대로 유지됩니다. 상속된 권한을 비활성화하고 초대된 사용자만 액세스할 수 있음 설정을 선택하여 레코드에 대한 관리 권한을 부여할 수 있습니다. <!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* 단일 레코드에 대해 상속된 사용 권한을 비활성화할 수 있습니다. 이 경우 개별 레코드에 사용 권한을 부여하거나 **작업 영역의 모든 사용자가 볼 수 있음** 옵션에 속하는 경우 사용 권한을 얻을 수 있습니다.

* 동일한 사용자에 대해 여러 공유 권한이 적용되는 경우 해당 권한 중 가장 높은 권한을 받습니다.

  예를 들어 레코드가 보기 권한이 있는 사용자와 공유되고 해당 그룹이 관리 액세스 권한이 있는 경우 레코드에 대한 관리 권한을 받습니다.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* 연결된 레코드의 수식 필드 또는 조회 필드가 사용 권한이 없는 레코드의 필드를 기반으로 하는 경우 다른 방법으로 액세스할 수 없는 레코드의 요소를 올바르게 계산할 수 있습니다.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## 레코드 권한 공유

작업 영역 관리자는 개별 레코드에 대한 권한을 조정할 수 있습니다.

{{step1-to-planning}}

1. 공유할 레코드가 있는 작업 영역을 엽니다.
1. 공유할 레코드의 레코드 유형을 클릭합니다.

1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **공유**&#x200B;를 클릭합니다.
   * 표 보기에서 레코드를 선택한 다음 목록 하단의 파란색 도구 모음에서 **공유**&#x200B;를 클릭합니다.
   * 보기에서 레코드 이름을 클릭한 다음 레코드 세부 정보 페이지의 오른쪽 상단에 있는 **공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.

   ![에서 상속된 사용 권한을 가진 레코드에 대한 &#x200B;](assets/permissions-for-records-with-inherited-permissions-on.png)사용 권한

1. (선택 사항) **액세스 권한이 있는 사용자** 영역에서 **작업 영역의 모든 사용자가 볼 수 있음** 옵션이 기본적으로 선택됩니다.  작업 영역 및 레코드 유형에 대해 **보기** 이상의 권한이 있는 모든 사용자는 레코드에 대해 동일한 권한을 가집니다.

1. (선택 사항) 작업 영역에서 권한을 상속하는 사용자, 팀, 그룹, 회사 또는 작업 역할을 보려면 **상속된 권한** 옵션 아래의 사용자 수를 클릭합니다.

   >[!TIP]
   >
   >상속된 권한 목록에서 개별 엔티티를 제거할 수 없습니다.

1. (선택 사항 및 조건부) 특정 엔티티와 레코드를 공유하고 작업 공간에 이미 있는 것과 다른 레코드 유형에 대한 액세스 권한을 부여하려면 다음을 수행합니다.

   1. **상속된 권한** 드롭다운 메뉴에서 **사용 안 함**&#x200B;을(를) 선택합니다.

   >[!TIP]
   >
   >Workspace 관리자는 레코드 유형 및 레코드에 대한 관리 권한을 계속 가집니다.

   1. (선택 사항) **액세스 권한이 있는 사용자** 영역에서 **초대된 사용자만 액세스할 수 있음**&#x200B;을(를) 선택합니다.

   1. **이 레코드 형식에 대한 액세스 권한 부여** 필드에서 작업 영역 또는 레코드 형식에 대해 다른 권한 수준을 부여할 사용자, 팀, 그룹, 회사 또는 작업 역할을 추가합니다.
   1. 다음 권한 수준 중 하나를 선택합니다.

      * 보기
      * 관리

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* 팀, 그룹, 회사 및 작업 역할 외에도 Adobe Admin Console에 추가된 사용자와만 공유할 수 있습니다. Workfront 전용 사용자는 추가할 수 없습니다. 자세한 내용은 [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)를 참조하십시오.
   >* 사용자가 작업 공간 및 레코드 유형에 대한 기여 또는 관리 권한을 가지고 있는 경우 레코드에 대한 관리 권한을 유지합니다. 보기 권한이 흐리게 표시됩니다. <!--this is not dimmed at this time, Lilit to check-->
   >* 사용자에게 레코드 유형에 대한 Contribute 이상이 있으면 레코드에 대한 권한을 줄일 수 없습니다.
   > 자세한 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.

1. 작업 영역에 대한 권한이 없는 사용자에게 레코드를 볼 수 있는 액세스 권한을 부여하려면 **이 보기에 대한 액세스 권한 부여** 필드에 사용자, 그룹, 팀, 회사 또는 작업 역할의 이름을 입력한 다음 목록에 표시될 때 클릭합니다.

   선택한 엔터티는 레코드와 레코드 종류 및 **보기** 권한이 있는 작업 영역에 추가됩니다.

   시스템 관리자는 항상 공유 레코드에 대한 관리 권한을 받으며, 사용자가 시스템 관리자임을 나타냅니다.

1. (선택 사항) **링크 복사**&#x200B;를 클릭하여 레코드에 대한 링크를 클립보드에 복사하고 다른 사용자와 공유합니다. 이 링크를 클릭하면 레코드의 세부 정보 페이지가 열립니다.
1. **저장**&#x200B;을 클릭합니다.

   이제 레코드가 다른 사용자와 공유됩니다.

   레코드를 공유한 사용자는 다음 엔티티에 대한 권한이 부여되었다는 내용의 인앱 및 이메일 알림을 모두 수신하게 됩니다.

   * 레코드
   * 레코드 종류(이전에 권한이 없는 경우)
   * 작업 공간(레코드가 공유되기 전에 작업 공간에 대한 권한이 없는 경우).

   자세한 내용은 [Adobe Workfront Planning 알림: 문서 색인](/help/quicksilver/planning/notifications/notifications-information.md)을 참조하십시오.

1. 복사한 링크를 다른 사용자와 공유합니다. 링크를 받은 사용자는 활성 사용자여야 하며 레코드 유형 페이지에 액세스하여 선택한 보기에 표시할 수 있도록 Workfront에 로그인해야 합니다. 레코드 유형을 볼 수 있으려면 레코드 유형에 대한 권한이 있어야 합니다. 자세한 내용은 [링크를 사용하여 레코드 공유](/help/quicksilver/planning/records/share-records.md)도 참조하세요.

## 레코드에 대한 권한 제거

레코드에서 사용자의 권한을 제거할 수 있습니다. 그러나 레코드 유형에 대해 적어도 보기 권한을 제공하는 작업 영역에 대해 적어도 보기 권한은 유지됩니다. 작업 영역의 레코드 유형 또는 레코드에 대한 권한이 없도록 하려면 작업 영역에서 해당 액세스 권한을 제거해야 합니다.

{{step1-to-planning}}

1. 공유를 중지할 레코드가 있는 작업 영역을 연 다음 레코드 유형 카드를 클릭합니다. 그러면 레코드 유형 페이지가 열립니다.
1. 다음 중 하나를 수행하십시오.

   * 테이블 보기에서 레코드 이름 위로 마우스를 가져간 후 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **공유**&#x200B;를 클릭합니다.
   * 표 보기에서 레코드를 선택한 다음 목록 하단의 파란색 도구 모음에서 **공유**&#x200B;를 클릭합니다.
   * 보기에서 레코드 이름을 클릭한 다음 레코드 세부 정보 페이지의 오른쪽 상단에 있는 **공유**&#x200B;를 클릭합니다.

   **공유** 상자가 열립니다.
1. 권한을 제거할 사용자, 그룹, 팀, 회사 또는 작업 역할을 찾은 다음 이름 오른쪽에 있는 권한 드롭다운 메뉴를 확장한 다음 **제거**&#x200B;를 클릭합니다. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![레코드에 대한 권한 제거](assets/remove-option-on-record-sharing-drop-down.png)

1. **저장**&#x200B;을 클릭합니다.

   직원들에게 더 이상 레코드에 대한 표시된 권한이 없습니다. 그러나 레코드 유형 및 작업 영역도 해당 권한에서 제거하지 않는 한 해당 권한에 대한 권한이 남아 있습니다.

   더 이상 이러한 권한이 없다는 알림이 레코드에 액세스할 수 없도록 제거된 사용자에게 없습니다.
