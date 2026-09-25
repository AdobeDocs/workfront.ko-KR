---
title: Planning 요청 공유
description: Workfront Planning 요청이 제출된 후 다른 사용자와 공유할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3934b1b333f86c8c700617871bfaac23d2b19213
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%
---
# Planning 요청 공유

<!--add to TOC, and miniTOC-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기에 릴리스된 후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 매월 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


{{planning-important-intro}}

Planning 요청이 제출된 후 이를 보는 사람, 해당 요청을 처리할 수 있는 사람, 각 개인 또는 팀이 취할 수 있는 조치를 제어할 수 있습니다. 이렇게 하면 적합한 사람들이 적합한 요청에 집중할 수 있으며 자신의 역할에 적합한 작업만 수행할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p> 
또는
<p>독립 실행형 제품으로 구입할 경우 모든 Workfront Planning</p> 
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
   <td>   <p>Workfront 사용자인 경우 작업 공간 및 레코드 유형에 대한 이상의 권한을 봅니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 공유 시 고려 사항

* 요청에 대해 사용자에게 다음 권한을 부여할 수 있습니다.

  * 보기: 사용자는 요청만 볼 수 있습니다.
  * Contribute: 사용자는 요청을 보고, 편집하고, 댓글을 달 수 있습니다.
  * 관리: 사용자는 요청을 보고, 편집하고, 댓글을 달고, 삭제할 수 있습니다.

* 관리자가 다른 기본값을 구성하지 않은 경우 요청자에게 제출하는 요청에 대한 관리 액세스 권한이 자동으로 부여됩니다.

  자세한 내용은 [요청 양식 만들기](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.

* Workfront 관리자는 모든 요청에 액세스하고 관리할 수 있습니다.
* 레코드 유형에 대한 관리 액세스 권한이 있는 사용자는 해당 레코드 유형의 접수 양식과 이를 통해 제출된 모든 요청에 대한 관리 액세스 권한을 상속합니다.
* 요청에 대한 권한이 있는 모든 사용자는 동일한 권한 수준으로 요청을 공유하거나 자신의 권한 수준보다 낮은 수준으로 요청을 공유할 수 있습니다.

  기여 권한이 있는 사용자는 다른 사용자에게 요청에 대한 관리 권한을 부여할 수 없습니다.

* 서로 다른 사용자와 팀이 동일한 요청에 대해 서로 다른 액세스 수준을 보유할 수 있습니다.
* 여러 엔티티를 통해 권한을 할당할 수 있습니다. 사용자에게 요청에 대한 기여 권한이 있지만 그룹 또는 작업 역할에 보기 권한이 있는 경우 기여 권한에 대해 가장 높은 수준을 유지합니다.
* 요청은 작업 공간 및 레코드 유형에서 권한을 상속합니다. Planning 요청에 대해 상속된 권한은 제거하거나 편집할 수 없습니다.

## 요청 공유

새 요청 경험을 사용하고 있는지 확인합니다.

1. {{step1-to-requests}}
1. Planning 요청을 찾아 클릭하여 엽니다.
1. **공유**&#x200B;를 클릭합니다.

   선택한 요청에 대해 **공유** 상자가 열립니다.

   ![공유 상자 요청](assets/requests-sharing-box.png)

1. **이 요청 필드에 대한 액세스 권한 부여**&#x200B;에서 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력하고 목록에 표시될 때 클릭합니다.

   활성 엔티티만 목록에 표시됩니다.
1. 드롭다운 메뉴에서 각 엔티티 이름의 오른쪽에 있는 다음 권한 수준 중 하나를 선택합니다.

   * 관리
   * 참여
   * 보기
1. (선택 사항) 각 권한 수준에 대해 세분화된 권한 아이콘을 클릭하고 **편집**, **댓글**, **공유** 또는 **삭제**&#x200B;와 같은 세분화된 권한을 선택하거나 선택 취소합니다.

   ![요청에 대한 세분화된 권한](assets/granular-permissions-on-requests.png)
1. (선택 사항) 상속된 권한 라인을 확장하여 작업 공간 및 레코드 유형에서 권한을 부여받은 사용자를 확인합니다.

   >[!TIP]
   >
   >Planning 요청에 대해 상속된 권한은 제거하거나 편집할 수 없습니다.

1. **저장**&#x200B;을 클릭합니다.


   이 요청은 선택한 엔티티와 공유됩니다.


