---
title: Workfront 계획 필드 공유
description: Adobe Workfront Planning 레코드 필드를 다른 사용자와 공유하여 Workfront Planning 사용 시 공동 작업을 보장할 수 있습니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
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
* 필드에 대한 액세스는 다음 설정을 결합하여 가져옵니다.

  * **상속된 권한**: 기본적으로 필드는 다른 사람이 레코드 형식에 대해 가지고 있는 동일한 액세스 권한을 상속합니다(레코드 형식 보기 사용 권한은 사용자에게 필드 값을 볼 수 있는 권한을 부여하고, Contribute 또는 레코드 형식 관리 사용 권한은 사용자에게 필드 값을 관리할 수 있는 권한을 부여합니다). 상속된 권한을 끄고 사용자에게 레코드 유형에 대한 액세스 권한보다 낮은 수준의 필드 액세스 권한을 부여할 수 있습니다.
  * **작업 영역의 모든 사용자가 볼 수 있음** 또는 **초대된 사용자만 액세스**&#x200B;할 수 있습니다. 작업 영역에 대한 권한이 있는 모든 사람이 필드를 보도록 허용하거나 개별 엔터티에만 권한을 부여할 수 있습니다.

  동일한 사람에게 여러 개의 규칙이 적용되는 경우, 규칙 중 하나에서 사용자에게 사용 가능한 가장 높은 권한을 부여합니다.

* 작업 영역 소유자와 관리자만 필드 권한을 조정할 수 있습니다. 작업 영역 관리자는 항상 모든 필드에 대한 관리 액세스 권한을 유지하며 이를 낮출 수 없습니다.
* 필드 공유는 필드 설정이 아니라 값에 대한 액세스를 제어합니다. 작업 영역 관리자만 필드의 구성을 변경할 수 있습니다.
* 필드의 공유 목록에 사용자를 추가해도 작업 공간이나 레코드 유형 액세스 권한은 부여되지 않습니다. 액세스 권한이 없는 경우 경고 아이콘은 레코드 유형에 추가된 후에만 권한이 적용됨을 나타냅니다.
* 시스템 필드(예: 작성자, 레코드 ID) 및 기본 필드는 제한된 공유를 가질 수 없습니다.
* 제한된 필드는 필드가 표시되는 모든 곳에서 적용됩니다. 여기에는 모든 보기, 레코드 세부 사항 페이지, 요청 양식, 연결 및 조회 필드, 캔버스 대시보드, API 및 MCP 도구가 포함됩니다.
* 조회 필드는 소스 필드의 권한을 상속합니다.
* 공개 보기는 액세스할 수 있는 모든 사람에게 완전히 표시되며 읽기 전용입니다.
* 레코드를 복제하면 제한된 값이 새 레코드에 복사되지 않습니다.
* 제한된 필드 값 변경 사항은 레코드 기록에 기록되지 않습니다.
* 필드에 대한 권한 변경이 알림을 트리거하지 않습니다.
* 글로벌 레코드 유형의 경우 필드 권한은 모든 보조 작업 영역에 적용되며 로컬로 조정할 수 없습니다.


클로드에서:
필드에 대한 추가 권한 - 모든 공유에 대한 개요 문서에 이 권한을 추가할 수 있습니다?? - help/quicksilver/planning/access/sharing-permissions-overview.md

다음은 문서의 레코드 유형/작업 영역 액세스를 필드 수준 액세스에 매핑하는 방법입니다.

필드 권한 수준(2개 + 없음):

액세스 권한 없음 - 필드가 완전히 숨겨짐
필드 값 보기 - 값을 볼 수 있고 편집할 수 없음
필드 값 관리 - 보고 편집할 수 있음

레코드 유형 역할의 기본 상속

레코드 유형/작업 영역 액세스 기본 필드 권한
보기 필드 값 보기
Contribute 필드 값 관리
관리(작업 공간 관리자) 필드 값 관리(잠김 — 줄일 수 없음)

따라서 기본적으로 필드는 레코드 유형에서 어떤 역할이든 미러링합니다. 뷰어는 읽기 전용이 되고 기여자 및 관리자는 편집 권한을 받습니다. Workspace 관리자는 특별한 경우가 있습니다. 필드의 공유 목록에 추가될 때마다 &quot;필드 값 관리&quot;가 미리 선택되고 &quot;필드 값 보기&quot; 옵션이 비활성화됩니다. 이는 편집 액세스 권한을 제거할 수 없기 때문입니다.

와일드카드(대체) 설정
상속과 별도로 각 필드에는 와일드카드 기본값이 있습니다.

작업 영역의 모든 사용자가 볼 수 있음(기본값)
초대된 사용자만 액세스 가능

최종 권한 계산 방법

상속된 권한이 활성화된 경우: 개인의 액세스 = 가장 높음 (레코드 유형, 와일드카드, 개별적으로 부여된 권한에서 상속됨).
상속된 권한이 비활성화된 경우: 개인의 액세스 = 가장 높음(와일드카드, 개별적으로 부여된 권한) — 레코드 유형 역할이에 더 이상 영향을 주지 않습니다.
상속이 비활성화된 경우 와일드카드는 &quot;초대된 사용자만 액세스할 수 있습니다&quot;이고 해당 사용자는 액세스 권한→ 받지 않고 개별적으로 추가되지 않습니다.

기타 권한 참고 사항

다른 사용자에게 개별적으로 액세스 권한을 부여하면 작업 영역/레코드 유형 액세스 권한이 부여되지 않습니다. 작업 영역에 별도로 추가될 때까지 비활성 상태(경고 아이콘 포함)로 표시됩니다.
글로벌 레코드 유형의 경우 필드 권한은 한 번 설정되고 모든 보조 작업 영역에 적용됩니다. 보조/팀 작업 영역 관리자는 이러한 권한을 로컬로 재정의할 수 없습니다.

## 필드 공유

