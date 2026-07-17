---
title: 레코드에 대한 기본 권한 설정
description: 레코드 유형 또는 작업 공간 설정을 수정할 때 레코드에 대한 기본 권한을 설정할 수 있습니다. 레코드 유형에 추가될 모든 레코드에 대해 열기 또는 제한된 권한을 부여할 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 9ef64f5a39c94426b2158c6504b913c8cb749c8e
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 3%

---


# 레코드에 대한 기본 권한 설정

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}


레코드 유형 또는 작업 공간 설정을 수정할 때 레코드에 대한 기본 권한을 설정할 수 있습니다.

레코드 유형에 추가될 모든 레코드에 대해 열기 또는 제한된 권한을 부여할 수 있습니다.


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
<p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p> 
또는
<p>모든 Workfront Planning을 독립 실행형 제품 패키지로</p>

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
   <td>  <p>작업 공간 및 레코드 유형에 대한 권한 관리</p>  
   <p><b>중요</b></p>
   <p>작업 영역에 대한 관리 권한이 있는 사용자만 레코드를 공유할 수 있습니다.</p></td> 
  </tr>
</tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기본 레코드 권한 설정에 대한 고려 사항

기본 레코드 권한을 구성할 때 다음 사항을 고려하십시오.

* 레코드 유형당 한 번에 하나의 기본 권한 규칙만 활성화할 수 있습니다.
* 규칙을 변경하면 변경 후에 생성된 레코드에만 영향을 줍니다. 기존 레코드는 현재 권한을 유지합니다.
* 시스템 관리자 및 작업 공간 관리자는 규칙에 관계없이 모든 레코드에 대한 관리 액세스 권한을 항상 유지합니다.
* 레코드가 만들어지면 기본 규칙에 영향을 주지 않고 공유 대화 상자에서 해당 권한을 독립적으로 변경할 수 있습니다.
* 글로벌 레코드 유형의 경우 각 작업 영역(기본 및 보조)은 자체 기본 규칙을 구성할 수 있으며 새 레코드는 해당 레코드를 만든 작업 영역의 규칙을 사용합니다.

## 작업 공간에 대한 기본 레코드 권한 구성

1. 작업 영역 > **기타** 메뉴 ![기타 메뉴](assets/more-menu.png) > **설정** > **레코드 종류**&#x200B;로 이동합니다.

   ![Workspace 레코드 종류 설정 영역](assets/workspace-record-types-settings-area.png)

1. (선택 사항) **레코드 종류**&#x200B;의 셀 내부를 클릭하여 레코드 종류 이름을 편집합니다.

1. **새 레코드 권한 기본값** 열에서 업데이트할 권한을 가진 레코드 종류의 셀을 클릭합니다.

1. 다음 선택 사항 중 하나를 선택합니다.

   * **열기**: 모든 작업 영역 기여자는 새로 만든 레코드를 관리할 수 있습니다. 기존 및 새 레코드 유형의 현재 기본 동작입니다.
   * **제한됨**: 레코드 작성자와 명시적으로 추가한 모든 사용자만 새로 만든 레코드를 편집할 수 있습니다. 다른 모든 사용자는 보기 전용 액세스 권한을 받습니다.

1. (조건부) 기본 권한을 **제한됨**&#x200B;에서 **열기**(으)로 변경하는 경우 **열기로 전환** 상자에서 **전환**&#x200B;을 클릭하여 선택을 확인합니다.
1. (조건부) **제한됨**&#x200B;을(를) 선택한 경우 **레코드를 편집할 수 있는 사용자** 열에 편집기를 추가하십시오. 사용자, 그룹, 팀, 역할 또는 회사를 추가할 수 있습니다.

   >[!NOTE]
   >
   >* 레코드 생성자는 항상 포함되며 제거할 수 없습니다.
   >* 레코드 유형에 대한 기여 또는 관리 권한이 이미 있는 항목만 선택할 수 있습니다.

   변경 사항은 자동으로 저장됩니다. 저장되면 규칙은 즉시 적용되며 향후 해당 레코드 유형에 대해 생성된 모든 레코드에 자동으로 적용됩니다.

## 레코드 유형에 대한 기본 레코드 권한 구성

1. 레코드 종류 > **기타** 메뉴 ![기타 메뉴](assets/more-menu.png) > **설정** > **레코드 설정**&#x200B;으로 이동합니다.

   ![레코드 종류 설정 영역의 레코드 설정 탭](assets/record-settings-tab-in-record-type-settings-area.png)

1. **레코드 권한 형식** 필드에서 다음 옵션 중 하나를 클릭합니다.

   * **열기**: 모든 작업 영역 기여자는 새로 만든 레코드를 관리할 수 있습니다. 기존 및 새 레코드 유형의 현재 기본 동작입니다.
   * **제한됨**: 레코드 작성자와 명시적으로 추가한 모든 사용자만 새로 만든 레코드를 편집할 수 있습니다. 다른 모든 사용자는 보기 전용 액세스 권한을 받습니다.
1. (조건부) 기본 권한을 **제한됨**&#x200B;에서 **열기**(으)로 변경하는 경우 **열기로 전환** 상자에서 **전환**&#x200B;을 클릭하여 선택을 확인합니다.
1. (조건부) **제한됨**&#x200B;을(를) 선택한 경우 **레코드를 편집할 수 있는 사용자** 필드에 편집자를 추가하십시오. 사용자, 그룹, 팀, 역할 또는 회사를 추가할 수 있습니다.

   >[!NOTE]
   >
   >* 레코드 생성자는 항상 포함되며 제거할 수 없습니다.
   >* 레코드 유형에 대한 기여 또는 관리 권한이 이미 있는 항목만 선택할 수 있습니다.

   변경 사항은 자동으로 저장됩니다. 저장되면 규칙은 즉시 적용되며 향후 해당 레코드 유형에 대해 생성된 모든 레코드에 자동으로 적용됩니다.