---
title: 내역 섹션 개요
description: Adobe Workfront Planning에서 레코드의 오른쪽 패널에서 레코드와 시스템에 의해 기록되는 변경 사항을 검토할 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 3%

---

# 내역 섹션 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

레코드의 오른쪽 패널에 댓글 또는 답글을 추가하여 Adobe Workfront Planning 레코드에 대한 공동 작업을 수행할 수 있습니다. 이 영역에서 레코드에 대해 수행된 다른 변경 사항 및 시스템에서 기록한 변경 사항을 볼 수도 있습니다.

레코드의 오른쪽 패널에는 다음 섹션이 표시됩니다.

* **댓글**: 사용자가 레코드에 추가하는 댓글과 답글을 표시합니다. Workfront Planning 레코드의 댓글 관리에 대한 자세한 내용은 [레코드 댓글 관리](/help/quicksilver/planning/records/manage-record-comments.md)를 참조하십시오.
* **기록**: 사용자가 레코드 필드에 적용한 시스템 기록 변경 내용을 표시합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Workfront 및 모든 Planning 패키지</p> <p>모든 워크플로우 및 모든 Planning 패키지</p>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>기여자 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간 및 레코드 유형에 대한 이상의 권한 보기</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p> </td> 
  </tr> 
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

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Contributor or higher license</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>
</tbody> 
</table> -->

## 레코드의 내역 섹션 찾기

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 기록 유형이 카드에 표시됩니다.

1. 레코드 유형 카드를 클릭합니다.
레코드 유형 페이지가 열리고 해당 유형의 모든 레코드가 표시됩니다.

1. 보기에서 레코드 이름을 클릭합니다.

   레코드 페이지가 열립니다. 주석(Comments) 영역은 기본적으로 오른쪽 패널에 열립니다.
1. **내역 표시** 아이콘 ![내역 표시 아이콘](assets/show-history-icon.png)을 클릭합니다. 레코드의 필드에 대한 모든 변경 사항은 가장 최근 것부터 시작하여 오른쪽 패널에 표시됩니다.
1. (선택 사항) **내역 숨기기** 아이콘 ![내역 숨기기 아이콘](assets/hide-history-icon.png)을 클릭하여 오른쪽 패널을 닫습니다.

## 작업 내역 섹션에 대한 고려 사항

레코드 페이지의 오른쪽 패널에 있는 기록 섹션에서 레코드 필드에 대한 변경 사항을 검토할 수 있습니다.

![댓글의 기록 영역](assets/history-area-in-comments.png)

* Workfront Planning은 내역 섹션에 다음 정보를 기록합니다.

   * 모든 필드 변경 사항

   * 값이 변경될 때 필드의 이전 값과 새 값. 이전 값은 취소선 형식으로 표시됩니다.

   * 변경한 사용자의 전체 이름

   * 변경이 발생한 날짜 및 시간 기록.

* 다음 유형의 필드에는 항상 이전 값(취소선 형식)과 새 값이 표시됩니다.

   * 텍스트
   * 단락
   * 통화
   * Date
   * 숫자
   * 백분율
   * 단일 선택

* 다음 유형의 필드에는 여러 값 중 하나 이상이 제거된 경우에만 이전 값이 취소선 형식으로 표시됩니다.

   * 다중 선택
   * 연결된 레코드 필드
   * 사람

  변경 사항이 필드에 값을 추가하기만 하면 이전 값은 표시되지 않고 새 필드 값만 표시됩니다.

* 확인란 유형 필드에는 이전 값이 취소선 형식으로 표시되지 않습니다. 필드를 편집하면 변경한 시점의 현재 상태만 표시됩니다.

  Workfront Planning 필드에 대한 자세한 내용은 [필드 만들기](/help/quicksilver/planning/fields/create-fields.md)를 참조하십시오.

* 다음 유형의 필드에 대한 변경 사항은 기록 섹션에 표시되지 않습니다.

   * 연결된(조회) 필드
   * 공식
   * 제작자
   * 만든 날짜
   * 마지막 수정자
   * 마지막 수정일

* 시스템에서 필드를 제거하면 해당 필드에 대한 업데이트가 기록 섹션에 남아 있습니다. 레코드의 내역 섹션에 필드가 제거되었다는 표시가 없습니다.
