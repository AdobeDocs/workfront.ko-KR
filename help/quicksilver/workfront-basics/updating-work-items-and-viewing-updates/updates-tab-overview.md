---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 업데이트 섹션 개요
description: 업데이트 섹션에는 지난 90일 내에 수행된 최신 업데이트 중 최대 200개가 표시됩니다.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# 업데이트 섹션 개요

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

객체의 업데이트 섹션에는 객체의 변경 사항을 추적하는 객체 또는 시스템 업데이트 시 사용자가 수행하는 주석이 표시됩니다.

## 업데이트 섹션 개요

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

개체의 업데이트 섹션에는 지난 90일 내에 수행된 최신 업데이트 중 최대 200개가 표시됩니다.

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

업데이트 섹션에는 다음 정보가 표시됩니다.

* 사용자가 작성한 댓글과 해당 댓글에 대한 회신
* Workfront이 개체에 특정 이벤트를 기록하기 위해 만드는 정보 메시지인 시스템 업데이트. 예를 들어 시스템 업데이트를 통해 상태, 이름 또는 사용자 지정 필드의 변경 사항을 캡처할 수 있습니다. Workfront 또는 그룹 관리자가 객체에 대한 시스템 업데이트를 활성화할 수 있습니다. 자세한 내용은 [시스템 업데이트 구성](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

다음 객체에 대해 업데이트 섹션이 표시됩니다.

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
     <li>스토리</li> 
     <li>작업</li> 
     <li>템플릿</li> 
     <li>템플릿 작업</li> 
     <li>타임시트</li> 
     <li>사용자</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## 상위 등급 개체에도 표시되는 업데이트

다음 표에 표시된 대로 특정 개체의 업데이트에 대한 응답도 순위가 높은 개체의 업데이트 섹션에도 표시됩니다.

예를 들어, 작업에 업데이트를 추가하면 해당 업데이트가 작업의 업데이트 섹션과 작업이 포함된 프로젝트의 업데이트 섹션에 표시됩니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>원본 업데이트가 추가된 개체</strong> </th> 
   <th> <p><strong>원래 업데이트도 표시되는 등급이 높은 개체</strong> </p> </th> 
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
   <td>문서가 첨부된 객체, 프로젝트 </td> 
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
>시스템 업데이트에 추가된 응답이 상위 개체에 롤업되지 않습니다. 하위 개체에 대한 직접 답장과 기존 업데이트에 추가된 응답만 상위 개체에 롤업됩니다.
>
>Adobe Workfront의 개체 계층에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## 업데이트 섹션의 제한 사항

### 사용자 및 팀의 제한 사항

팀에서 업데이트할 수 없습니다. 팀의 업데이트 섹션은 다음 개체에 입력한 업데이트로 채워집니다.

* 사용자
* 타임시트
* 스토리
* 반복

사용자 및 팀의 업데이트 섹션에서 지난 90일 동안 입력한 업데이트를 볼 수 있습니다.

사용자 또는 팀이 90일 제한 이상의 업데이트를 모두 보려면 노트에 대한 보고서를 작성할 수 있습니다. 보고서에는 사용자 또는 팀에 대한 모든 업데이트를 표시하는 시간 필터가 있지 않아야 합니다. 자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 다른 사용자를 대신하여 주석을 입력할 때 제한 사항

Adobe Workfront 관리자 및 그룹 관리자는 다른 사용자로 로그인하여 Workfront에서 주석 입력과 같은 작업을 수행할 수 있습니다. (자세한 내용은 [다른 사용자로 로그인](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)) 다른 사용자를 대신하여 작성한 모든 주석은 주석에 표시됩니다.

그룹 관리자는 다른 사람을 대신하여 주석을 작성할 수 있지만 해당 설명을 삭제할 수는 없습니다. Adobe Workfront 관리자만 다른 사용자를 대신하여 작성한 주석을 삭제할 수 있습니다.

## 분개 입력 보고서를 사용하여 작업 항목에 대한 시스템 갱신 조회

분개 입력 보고서 시스템은 프로젝트, 작업 및 문제의 갱신 영역에서 갱신됩니다.

보고서를 통해 다음을 확인할 수 있습니다.

* 발생한 상태 변경 수
* 작업 또는 문제가 삭제된 경우
* 프로젝트 진행 중에 중요한 사용자 지정 필드의 값이 변경되는 방법
* 프로젝트 진행 중에 변경된 중요한 날짜
* 프로젝트 진행 과정에서 우선순위가 변경된 경우
* 프로젝트 소유자가 변경된 경우

자세한 내용은 [업데이트 영역에 대한 보고서](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
