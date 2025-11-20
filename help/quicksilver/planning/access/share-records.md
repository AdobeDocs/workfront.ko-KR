---
title: 레코드 공유
description: 공유 버튼을 사용하여 레코드를 공유하면 Adobe Workfront Planning에서 공동 작업을 향상시킬 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# 레코드 공유

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


{{planning-important-intro}}

레코드 종류의 개별 레코드에 대한 사용자의 권한을 조정할 수 있습니다. O

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
   <p><b>중요 사항</b></p>
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

* 사람, 그룹, 팀, 회사 또는 작업 역할과 같은 엔티티와 레코드를 공유할 수 있습니다.
* 사용자와 작업 영역을 공유하면 기본적으로 작업 영역의 레코드에 대해 동일한 권한을 받습니다.
* 작업 영역에서 엔티티를 제거하면 모든 공유 권한이 레코드 유형 및 그 안의 모든 레코드에서 제거됩니다.
* 사용자의 레코드에 대한 액세스는 다음 3가지 설정의 조합을 통해 결정됩니다.

   * 레코드 유형 및 작업 영역에서 상속된 권한
   * 레코드 공유 대화 상자에서 개별적으로 추가된 권한
   * 다음 권한:

      * **작업 영역의 모든 사용자가 볼 수 있음**: 이 경우 작업 영역의 모든 사용자가 레코드를 볼 수 있습니다. <!-- is this OK to say "workspace? should it be "record"??-->
      * **초대된 사람만 액세스할 수 있습니다**: 이 옵션은 기본적으로 선택되어 있으며 특정 사람에게 레코드에 대한 액세스를 제한할 수 있습니다.

* 레코드에 다음 수준의 권한을 부여할 수 있습니다.

   * 보기
   * 관리

* 사용자와 레코드를 공유하면 기본적으로 레코드 유형에 있는 권한과 동일한 권한으로 추가됩니다.

  For example:

   * 레코드 유형에 대한 보기 권한이 있는 경우 레코드에 대한 보기 권한을 갖게 됩니다
   * 레코드 유형에 대한 기여 또는 관리 권한이 있는 경우 레코드에 대한 관리 권한을 얻습니다

* 작업 영역 관리자는 작업 영역에 속하지 않는 사용자와 레코드를 공유할 수 있습니다. 이 경우 추가된 엔티티 옆에 작업 영역에 액세스할 수 없다는 경고가 표시됩니다. 를 수락하여 레코드와 작업 공간 모두에 사용자를 추가하거나, 작업 공간에 사용자 추가를 거부하여 레코드에서도 사용자를 제거할 수 있습니다.

* 작업 영역에 대한 관리 권한이 있는 사용자와 레코드를 공유할 때 기본적으로 해당 사용자는 레코드에 대한 관리 권한도 갖게 됩니다. 보기 권한이 흐리게 표시됩니다.

* 작업 영역에 사람을 추가할 수 있는 권한이 없는 경우 작업 영역에 이미 추가된 사용자, 팀, 그룹, 역할 및 회사만 보고 추가할 수 있습니다. 아직 작업 공간에 속하지 않은 다른 엔티티를 추가할 수 없습니다.

* 단일 레코드에 대해 상속된 권한을 비활성화할 수 있습니다. 이 경우 상속된 권한에 대해 개별적으로 권한을 부여하거나 상속된 권한이 &quot;작업 공간의 모든 사용자&quot; 옵션에 속하는 경우 권한을 얻을 수 있습니다. <!-- is this OK to say "workspace? should it be "record"??-->

* 동일한 사용자에 대해 여러 공유 권한이 적용되는 경우 해당 권한 중 가장 높은 권한을 받습니다.

  예를 들어 레코드가 보기 권한이 있는 사용자와 공유되고 해당 그룹이 관리 액세스 권한이 있는 경우 레코드에 대한 관리 권한을 받습니다.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* 연결된 레코드의 수식 필드 또는 조회 필드가 사용 권한이 없는 레코드의 필드를 기반으로 하는 경우 다른 방법으로 액세스할 수 없는 레코드의 요소를 올바르게 계산할 수 있습니다.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## 레코드 권한 공유

