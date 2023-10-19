---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 업데이트 섹션 개요
description: 객체의 업데이트 섹션에는 사용자가 객체에 대해 수행하는 설명이나 객체에 대한 변경 사항을 추적하는 시스템 업데이트가 표시됩니다.
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: bc7039bc4b8b257fc55e71e73f72327fdb417837
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 5%

---

# 업데이트 섹션 개요

<!--take "Beta" references out when we remove the beta-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>\
<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 활성화 또는 비활성화](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<span class="preview">현재 릴리스 일정에 대한 자세한 내용은 [2023년 4분기 릴리스 개요](../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span>

>[!IMPORTANT]
>
>현재 Adobe Workfront의 댓글 달기 환경을 다시 디자인하고 있습니다.
>
>댓글 달기 경험에 액세스하는 환경과 개체에 따라 업데이트 섹션에 다른 기능이 표시될 수 있습니다.
>
>새 댓글 달기 경험과 사용 가능 여부에 대한 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>새 주석 달기 경험은 업데이트 섹션에만 사용할 수 있고 다음 영역에는 사용할 수 없습니다.
>
> * 홈
> * 목록의 요약 패널
> * 타임시트의 요약 패널

<!-- with October 26 release: add somewhere this:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old note, removed with August 2023: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the new commenting experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).

The Updates section of an object displays comments that users make on the object or system updates that track changes to the object.

-->

## 업데이트 섹션 개요

* 오브젝트의 업데이트 섹션에는 지난 90일 이내에 이루어진 가장 최근 업데이트 중 최대 200개가 표시됩니다.

  ![](assets/updates-tab-before-unified-experience-for-issues.png)

* 다음 객체에 대해 업데이트 섹션이 표시됩니다.

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td> 
      <ul> 
      <li>문서</li> 
      <li>목표</li> 
      <li>문제</li> 
      <li>반복</li> 
      <li>프로젝트</li> 
      <li>프로그램</li> 
      <li>포트폴리오</li> 
      </ul> </td> 
    <td> 
      <ul> 
      <li>스토리*</li> 
      <li>작업</li> 
      <li>템플릿</li> 
      <li>템플릿 작업</li> 
      <li>타임시트</li> 
      <li>사용자</li>
      <li>보드에 있는 카드</li>
      </ul> </td> 
    </tr> 
  </tbody> 
  </table>

  *스토리는 작업입니다. 작업과 관련된 모든 정보를 스토리에 사용할 수도 있습니다.

업데이트 섹션의 정보는 액세스하는 환경에 따라 다르게 구성됩니다.


### 현재 업데이트 섹션의 개요

<!--October 26 - replace current with legacy-->

* 현재 업데이트 섹션에는 다음 정보가 표시됩니다.

   * **사용자 업데이트**: 사용자가 작성한 댓글과 해당 댓글에 대한 답글.
   * **시스템 업데이트**: Workfront이 개체에 특정 이벤트를 기록하기 위해 만드는 정보 메시지입니다. 예를 들어 시스템 업데이트를 통해 상태, 이름 또는 사용자 정의 필드의 변경 사항을 캡처할 수 있습니다. Workfront 또는 그룹 관리자가 개체에 대한 시스템 업데이트를 활성화할 수 있습니다. 자세한 내용은 [시스템 업데이트 구성](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 다음 개체는 시스템 업데이트를 기록하지 않습니다.

   * 팀
   * 템플릿
   * 템플릿 작업

### 새 댓글 달기 환경의 업데이트 섹션 개요

새 댓글 달기 환경에 사용할 수 있는 기능과 개체에 대한 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

<span class="preview">![](assets/updates-tab-after-unified-experience-for-tasks.png)</span>

* 업데이트 섹션에는 새 댓글 달기 환경의 다음 탭에 정보가 표시됩니다.

   * **댓글**: 사용자가 작성한 댓글과 해당 댓글에 대한 답글을 표시합니다. 새 댓글 달기 환경에서 오브젝트를 업데이트하는 방법에 대한 자세한 내용은 [작업 업데이트](../updating-work-items-and-viewing-updates/update-work.md).
   * **시스템 활동**: Workfront이 개체에 특정 이벤트를 기록하기 위해 만드는 정보 메시지인 시스템 업데이트를 표시합니다. 예를 들어 시스템 업데이트를 통해 상태, 이름 또는 사용자 정의 필드의 변경 사항을 캡처할 수 있습니다. Workfront 또는 그룹 관리자가 개체에 대한 시스템 업데이트를 활성화할 수 있습니다. 자세한 내용은 [시스템 업데이트 구성](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

      * 다음 개체에는 시스템 활동 탭이 없습니다.

         * 팀
         * 템플릿
         * 템플릿 작업
         * 임시 카드

* 현재 다음 개체에 대한 새 댓글 달기 환경을 사용하여 댓글을 추가하고 업데이트에 답글을 달 수 있습니다.


   * 프로젝트
   * 작업(및 스토리)
   * 문제
   * 문서
   * 목표

  >[!NOTE]
  >
  >Workfront 목표에 액세스하려면 추가 라이선스가 있어야 합니다. 자세한 내용은 [Workfront 목표 사용 요구 사항](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   * 보드에 있는 카드

  >[!NOTE]
  >
  > 카드에서 주석 및 시스템 활동 섹션을 활성화하면 보드 영역에서 카드에 대한 업데이트를 추가하고 볼 수 있습니다. 자세한 내용은 [보드에 애드혹 카드 추가](../../agile/get-started-with-boards/add-card-to-board.md).


  <span class="preview">

   * 템플릿
   * 템플릿 작업
   * 타임시트
   * 사용자
   * 포트폴리오
   * 프로그램

  >[!NOTE]
  >
  >    반복에 대한 새 주석 달기 경험을 표시할 수 없습니다.

  </span>

<!--hidden in August 2023 and replaced by the list above: 

  <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
      <tr> 
      <td> 
        <ul> 
        <li><p>Goals</p>
        <li>Cards in the Boards area*</li>
          This is the only experience for goals and cards.
        </li> 
        <li>Projects</li>
        </ul> </td> 
      <td> 
        <ul> 
        <li>Issues</li> 
        <li>Tasks</li>
        <li>Documents</li>
        </ul> </td> 
      </tr> 
    </tbody> 
    </table>

  *You can add and view updates to cards in the Board areas when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md). 
  -->

## 상위 등급 개체에도 표시되는 업데이트

특정 개체의 업데이트에 대한 댓글이나 답글은 상위 개체의 업데이트 섹션에도 표시됩니다.

예를 들어 작업에 업데이트를 추가하면 해당 작업의 업데이트 섹션과 해당 작업이 포함된 프로젝트의 업데이트 섹션에 업데이트가 나타납니다.

>[!NOTE]
>
>새 댓글 달기 경험을 활성화하면 다음과 같은 상위 오브젝트에 댓글이 표시됩니다.
>
>* 문제
>* 프로젝트
>* 작업
>
>자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

다음 표는 주석이 상위 객체에 표시되는 객체를 보여 줍니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>원래 업데이트가 추가된 개체</strong> </th> 
   <th> <p><strong>원래 업데이트가 표시되는 상위 오브젝트</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>문제</td> 
   <td>프로젝트</td> 
  </tr> 
  <tr> 
   <td>작업</td> 
   <td>프로젝트</td> 
  </tr> 
  <tr> 
   <td>프로젝트</td> 
   <td>프로그램, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>문서 </td> 
   <td>문서가 첨부된 오브젝트, 프로젝트 </td> 
  </tr> 
  <tr> 
   <td>프로그램</td> 
   <td>포트폴리오</td> 
  </tr> 
  <tr> 
   <td>사용자</td> 
   <td>팀</td> 
  </tr> 
  <tr> 
   <td>타임시트</td> 
   <td>사용자, 팀</td> 
  </tr> 
  <tr> 
   <td>템플릿 작업</td> 
   <td>템플릿</td> 
  </tr> 
  <tr> 
   <td>스토리</td> 
   <td>반복, 팀</td> 
  </tr> 
  <tr> 
   <td>반복</td> 
   <td>팀</td> 
  </tr>

<tr> 
   <td>목표</td> 
   <td>결과, 활동</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>시스템 업데이트에 추가된 답글은 상위 개체로 롤업되지 않습니다. 하위 개체에 직접 회신과 기존 업데이트에 추가된 회신만 상위 개체에 롤업됩니다.
>
>Adobe Workfront의 개체 계층에 대한 자세한 내용은 [Adobe Workfront의 오브젝트 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> 새 댓글 달기 환경에서 시스템 업데이트에 회신할 수 없습니다. 자세한 내용은 [새 댓글 달기 환경](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

## 업데이트 섹션의 제한 사항

팀의 업데이트 섹션과 다른 사용자 대신 업데이트를 입력할 때 몇 가지 제한 사항이 있습니다.

### 사용자 및 팀에 대한 제한 사항

팀의 업데이트 섹션에서 새 주석을 추가할 수 없습니다.

<span class="preview">팀에서 보는 업데이트에 회신을 추가할 수 있습니다. 응답이 속한 객체의 업데이트 섹션뿐만 아니라 팀의 업데이트 섹션에도 표시됩니다. </span>

팀의 업데이트 섹션은 다음 개체에 입력한 업데이트로 채워집니다.

* 사용자
* 타임시트
* 스토리
* 반복

사용자 및 팀을 위한 업데이트 섹션에서 지난 90일 동안 입력한 업데이트를 볼 수 있습니다.

90일 제한을 초과하여 사용자 또는 팀에 대한 모든 업데이트를 보려면 메모에 대한 보고서를 작성할 수 있습니다. 보고서에는 사용자 또는 팀에 대한 모든 업데이트를 표시하는 시간 필터가 없어야 합니다. 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 다른 사용자를 대신하여 주석을 입력할 때의 제한 사항

Adobe Workfront 관리자 및 그룹 관리자는 다른 사용자로 로그인하고 주석 입력과 같은 작업을 Workfront에서 수행할 수 있습니다.

자세한 내용은 [다른 사용자로 로그인](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

다른 사용자로 로그인하고 주석을 추가할 때 다음 사항을 고려하십시오.

* 다른 사용자를 대신하여 작성한 모든 주석은 주석에 표시됩니다.

* 그룹 관리자는 다른 사용자를 대신하여 댓글을 달 수 있지만 해당 댓글을 삭제할 수는 없습니다. Adobe Workfront 관리자만 다른 사용자를 대신하여 작성한 댓글을 삭제할 수 있습니다.

* Workfront 또는 그룹 관리자는 사용자로 로그아웃하고 자신으로 다시 로그인하는 경우에만 다른 사용자를 대신하여 추가한 주석을 편집할 수 있습니다.

## 분개 입력 보고서를 사용하여 작업 항목에 대한 시스템 갱신 조회

분개 기입 보고서는 프로젝트, 작업 및 문제의 업데이트 영역에서 시스템 업데이트를 표시합니다.

이 보고서를 통해 다음을 볼 수 있습니다.

* 얼마나 많은 상태 변경 발생
* 작업 또는 문제가 삭제된 경우
* 프로젝트 진행 중 중요한 사용자 정의 필드의 값이 변경되는 방법
* 프로젝트 진행 중 변경된 중요한 일자
* 프로젝트 진행 중 우선순위가 변경된 경우
* 프로젝트 소유자가 변경된 경우

자세한 내용은 [업데이트 영역에 대한 보고서](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
