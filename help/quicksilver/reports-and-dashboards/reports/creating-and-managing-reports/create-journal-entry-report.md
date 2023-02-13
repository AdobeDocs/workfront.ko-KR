---
title: 업데이트 영역에 대한 보고서
description: 업데이트 영역에 대한 보고서
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: ecf947ce-54d8-4103-8903-f455b1d86c39
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2698'
ht-degree: 4%

---

# 업데이트 영역에 대한 보고서

분개 입력 보고서 서피스 시스템은 이전에 Adobe Workfront API를 통해서만 사용할 수 있었던 프로젝트, 작업, 문제 및 기타 객체의 갱신 영역에서 업데이트됩니다. 이 보고서는 특정 사용 사례를 위한 고급 보고서이지만 더 다이제블 형식을 사용하면 Workfront 내에서 프로젝트 활동 및 시스템 업데이트를 보다 쉽게 보고할 수 있습니다.

>[!TIP]
>
>분개 입력 보고서에는 객체의 갱신 영역의 시스템 갱신만 포함됩니다. 업데이트 영역에 남아 있는 주석을 보고하려면 노트 보고서를 사용해야 합니다.\
>참고 보고서에 대한 자세한 내용은 [참고 보고서에서 모든 업데이트 보기](../../../workfront-basics/updating-work-items-and-viewing-updates/view-all-updates-in-a-report.md)‍.

분개 입력 보고서에는 다음과 같은 내용이 표시됩니다.

* 발생한 상태 변경 수
* 작업 또는 문제가 삭제된 경우
* 프로젝트의 라이프 사이클에서 중요한 사용자 지정 필드의 값이 변경되는 방법
* 프로젝트 라이프 사이클에서 중요한 날짜가 변경된 날짜
* 프로젝트 소유자가 변경된 경우

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 표시하는 분개 항목이 포함된 객체에 대한 사용 권한 보기</p> <p>보고서를 만들면 보고서에 대한 관리 권한을 받게 됩니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

이 문서에 설명된 작업을 수행하려면 먼저 다음을 확인해야 합니다.

* 보고하려는 모든 필드는 Workfront에서 추적됩니다. 추적되는 업데이트 영역의 데이터만 보고할 수 있습니다.

   Workfront에서 추적할 필드를 추가하는 방법에 대해 알아보려면 [시스템 업데이트 구성](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

* 보고하려는 모든 사용자 지정 필드에 설정이 있습니다 **업데이트 피드에 필드 변경 사항 표시** 활성화되었습니다.

   사용자 지정 필드에 대해 이 설정을 활성화하는 방법을 알아보려면 섹션을 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 기사 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 분개 입력 보고서 개요

분개 입력 보고서는 시스템을 갱신하므로 상당한 수의 결과를 반환할 수 있습니다. 따라서 보고서를 만들 때 프로젝트, 프로그램, 포트폴리오, 그룹 등의 특정 개체(예: )로 필터링하는 것이 좋습니다.

Workfront의 다양한 개체 유형에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>분개 입력 보고서가 너무 많은 데이터를 반환하므로 보고서 전달 내보내기 및 예약된 배달은 지원되지 않습니다.

이 보고서의 기본 보기에는 다음 열이 포함되어 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>필드</th> 
   <th>설명</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>필드 이름</strong> </td> 
   <td> <p><span style="font-weight: normal;">영향을 받는 필드의 이름입니다. 보고서 설정 방법에 따라 이 열에는 상태, 소유자 ID, 작업 이름, 계획된 완료 날짜 또는 기타 필드가 포함될 수 있습니다.</span> </p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> 이 열에 표시되며, 이는 나열된 필드가 사용자 지정 필드임을 나타냅니다.</span></p> </td> 
  </tr> 
  <tr> 
   <td><strong>유형 변경</strong> </td> 
   <td> <p>영향을 받는 필드에 대한 변경 유형입니다. 설정한 필터 규칙과 사용자가 수행한 작업에 따라 이 필드에 다음 항목이 표시될 수 있습니다.</p> 
    <ul> 
     <li> <p>추가</p> </li> 
     <li> <p>감사</p> </li> 
     <li> <p>삭제</p> </li> 
     <li> <p>다이제스트</p> </li> 
     <li> <p>편집</p> </li> 
     <li> <p>복원</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>상위 ObjCode</strong> </td> 
   <td> <p>계층에서 가장 높은 상위 개체입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>범위</strong> </td> 
   <td> <p>변경된 객체 유형입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>시작 날짜</strong> </td> 
   <td> <p>필드가 변경된 날짜입니다.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>이름별로 편집됨</strong> </td> 
   <td> <p>필드를 변경한 사용자입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 보고서에서 정보를 구성하려면 기본 제공 그룹화 프로젝트를 사용할 수 있습니다. 프로젝트 그룹화는 프로젝트 이름의 1차 그룹화와 시작 날짜의 2차 그룹화를 제공합니다. 보고서를 만들 때 이 기존 그룹을 적용하거나 보고서를 볼 때 적용할 수 있습니다.

보고서에 사용할 보기, 필터 및 그룹화를 설정하는 방법을 알려면 관련 섹션을 참조하십시오.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: from&nbsp;Luke: Take this for what it's worth, but part of me wonders if all of these subsections should be separate articles.</p>
<p>The biggest reason for breaking these up would be searchability, in my mind. For example, as a user, I might want to know how to see if the owner of a project changed. If I search the help site for that, I would be a lot more likely to find a separate article called "See if the owner of a project changed" vs an article titled "Create a Journal Entry report" because "Journal Entry" might mean nothing to me.) </p>
</div>
-->

* [발생한 상태 변경 사항 확인](#see-what-status-changes-occurred)
* [작업 또는 문제가 삭제되는 시점을 확인합니다](#see-when-a-task-or-issue-was-deleted)
* [프로젝트 수명 주기 동안 사용자 정의 필드가 어떻게 변경되었는지 확인하십시오](#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle)
* [프로젝트 라이프 사이클에서 계획된 완료 일자가 어떻게 변경되었는지 확인합니다.](#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle)
* [프로젝트 소유자가 변경되었는지 확인합니다](#see-if-the-owner-of-a-project-changed)

## 발생한 상태 변경 사항 확인 {#see-what-status-changes-occurred}

분개 입력 보고서를 설정하여 다음을 표시할 수 있습니다.

* 프로젝트, 작업 또는 문제에 대한 상태 변경 횟수

* 이전 상태는 변경 전에 무엇이었습니까
* 상태를 변경한 사람
* 상태가 변경된 시기

프로젝트의 상태를 보려면 프로젝트를 사용하여 이와 동일한 정보를 표시하도록 보고서를 설정할 수도 있습니다 **조건** 필드.

이 정보는 감사 및 사용자와 조직이 얼마나 잘 계획 중인지 확인하는 데 도움이 될 수 있습니다.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;for tip below: When analytics adds the status option, update this note to say "these entries (status or condition changes)")</p>
-->

>[!TIP]
>
>조건 변경 사항 간의 일 차이를 비교하려면 Enhanced Analytics를 사용할 수 있습니다.\
>Enhanced Analytics에 대한 자세한 내용은 [향상된 분석 개요](../../../enhanced-analytics/enhanced-analytics-overview.md).

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 클릭 **새 보고서**&#x200B;를 선택하고 을 선택합니다. **분개 입력**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder가 로드됩니다.

1. 에서 **열(보기)** 탭에서 다음 열을 추가합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>열</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">필드 이름</p> </td> 
      <td> <p>영향을 받는 필드의 이름입니다. 이 경우 <strong>상태</strong> 이 열에 표시되어야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">유형 변경</p> </td> 
      <td> <p>영향을 받는 필드(예: )에 대한 변경 유형입니다 <strong>추가</strong>, <strong>삭제</strong>, 또는 <strong>편집</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이름별로 편집됨</p> </td> 
      <td> <p>상태를 업데이트한 사용자의 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">시작 날짜</p> </td> 
      <td> <p>상태가 변경된 날짜입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이전 텍스트 값</p> </td> 
      <td> <p>이전 상태에 대한 키입니다. 다음은 기본 프로젝트 상태에 대한 상태 키입니다.</p> 
       <ul> 
        <li> <p> <strong>CUR</strong>: 현재</p> </li> 
        <li> <p><strong>DE</strong>: 데드</p> </li> 
        <li> <p><strong>ONH</strong>: 보류 중</p> </li> 
        <li> <p><strong>PLN</strong>: 계획</p> </li> 
        <li> <p><strong>CPL</strong>: 완료</p> </li> 
        <li> <p><strong>REQ</strong>: 요청</p> </li> 
        <li> <p><strong>4월</strong>: 승인됨</p> </li> 
        <li> <p><strong>REJ</strong>: 거부됨</p> </li> 
        <li> <p><strong>IDA</strong>: 아이디어</p> </li> 
       </ul> <p>조직에서 사용자 지정 상태를 설정한 경우 다른 상태 키가 이 열에 표시될 수 있습니다. 상태 키와 관련된 사용자 지정 상태에 대해 알아보려면 Workfront 관리자 또는 그룹 관리자에게 문의하십시오.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">새 텍스트 값</p> </td> 
      <td> <p>업데이트된 상태에 대한 키입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">상위 ObjCode</p> </td> 
      <td> <p>상태가 변경된 필드의 가장 높은 상위 객체입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">범위</p> </td> 
      <td> <p>상태가 변경된 객체의 유형입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">문제 이름<br>(선택 사항)</p> </td> 
      <td> <p>상태가 변경된 문제의 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">작업 이름<br>(선택 사항)</p> </td> 
      <td> <p>상태가 변경된 작업의 이름입니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   열 추가에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 에서 **필터** 탭, **필터 규칙 추가**&#x200B;를 입력한 다음 필터 규칙 추가 **필드 이름** > **Equal** > **상태**.

   ![](assets/nwe-journal-entry-status-filter-rules-350x90.png)

   >[!TIP]
   >
   >조건 변경을 보고하려면 대신 필터 규칙을 추가할 수 있습니다 **필드 이름** > **Equal** > **조건**.

   필터 추가에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (선택 사항) 보고서의 초점을 줄이고 로드 시간을 줄이려면 메시지를 추가하십시오.

   또는

   특정 프로젝트, 작업 또는 문제를 포함할 추가 필터 규칙을 만듭니다.

   >[!IMPORTANT]
   >
   >수정자를 사용하는 필터 규칙 만들기 **다음 포함** 은 실제로 로드 시간을 늘릴 수 있습니다. 이러한 이유로 다음과 같은 다른 수정자를 사용하는 것이 좋습니다 **Equal** 특정 프로젝트 또는 상위 수준 개체 ID에 대해 필터링할 수 있는 경우.

   메시지를 추가하는 방법에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 에서 **그룹화** 탭, **기존 그룹 적용**&#x200B;를 선택하고 을 선택합니다. **프로젝트**.

   그룹화 추가에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 클릭 **저장 + 닫기**.

   새 보고서가 로드됩니다.

## 작업 또는 문제가 삭제되는 시점을 확인합니다 {#see-when-a-task-or-issue-was-deleted}

분개 입력 보고서를 설정하여 다음을 표시할 수 있습니다.

* 삭제된 작업 또는 문제
* 작업 또는 문제를 삭제한 사람

작업 또는 문제가 삭제되는 시기를 확인하려면:

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 클릭 **새 보고서**&#x200B;를 선택하고 을 선택합니다. **분개 입력**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder가 로드됩니다.

1. 에서 **열(보기)** 탭에서 다음 열을 추가합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>열</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">범위</p> </td> 
      <td> <p>삭제된 개체의 유형입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">유형 변경</p> </td> 
      <td> <p>발생한 변경 유형입니다. 다음 <strong>삭제</strong> 이 열에 변경 사항이 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">시작 날짜</p> </td> 
      <td> <p>작업 또는 문제가 삭제된 날짜입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이름별로 편집됨</p> </td> 
      <td> <p>작업 또는 문제를 삭제한 사용자의 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">프로젝트 이름</p> </td> 
      <td> <p>삭제된 작업 또는 문제가 있는 프로젝트의 이름입니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   열 추가에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 에서 **필터** 탭, **필터 규칙 추가**&#x200B;를 만든 다음 다음을 추가합니다.

   * **유형 변경** > **Equal** > **삭제**
   * **프로젝트 ID** > **Equal** > **`<project>`**

      <!--WRITER check link; this png file has spaces
     [![](assets/classic-task-or-issue-deleted-350x90.png)](../../../Resources/Images/Reports/Creating and Managing Reports/QS_Task or issue deleted.png)-->
   필터 추가에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (선택 사항) 보고서의 초점을 줄이고 로드 시간을 줄이려면 메시지를 추가하십시오.

   또는

   특정 프로젝트, 작업 또는 문제를 포함할 추가 필터 규칙을 만듭니다.

   >[!IMPORTANT]
   >
   >수정자를 사용하는 필터 규칙 만들기 **다음 포함** 은 실제로 로드 시간을 늘릴 수 있습니다. 이러한 이유로 다음과 같은 다른 수정자를 사용하는 것이 좋습니다 **Equal** 특정 프로젝트 또는 상위 수준 개체 ID에 대해 필터링할 수 있는 경우.

   메시지를 추가하는 방법에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (선택 사항)에서 **그룹화** 탭, **기존 그룹 적용**&#x200B;를 선택하고 을 선택합니다. **프로젝트**.

   그룹화 추가에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 클릭 **저장 + 닫기**.

   새 보고서가 로드됩니다.

## 프로젝트 수명 주기 동안 사용자 정의 필드가 어떻게 변경되었는지 확인하십시오 {#see-how-custom-fields-changed-over-the-course-of-a-project-s-life-cycle}

프로젝트 진행 과정에서 중요한 필드 변경 사항을 추적할 수 있습니다. 이렇게 하려면 분개 입력을 설정하여 다음을 추적할 수 있습니다.

* 특정 사용자 지정 필드가 추가, 업데이트 또는 편집된 경우
* 이러한 변경 사항이 발생한 경우
* 변경 작업을 수행한 사람

프로젝트 수명 주기 동안 사용자 정의 필드가 어떻게 변경되었는지 확인하려면:

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 클릭 **새 보고서**&#x200B;를 선택하고 을 선택합니다. **분개 입력**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder가 로드됩니다.

1. 에서 **열(보기)** 탭에서 다음 열을 추가합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>열</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">필드 이름</p> </td> 
      <td> <p>영향을 받는 사용자 지정 필드의 이름입니다.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> 이 열에 표시되며, 이는 나열된 필드가 사용자 지정 필드임을 나타냅니다.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">유형 변경</p> </td> 
      <td> <p>영향을 받는 필드(예: )에 대한 변경 유형입니다 <strong>추가</strong>, <strong>삭제</strong>, 또는 <strong>편집</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이름별로 편집됨</p> </td> 
      <td> <p>사용자 지정 필드를 업데이트한 사용자의 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">시작 날짜</p> </td> 
      <td> <p>사용자 지정 필드의 값이 변경된 날짜입니다.</p> <p>이 필드를 내림차순으로 정렬해야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이전 숫자 값</p> </td> 
      <td> <p>사용자 지정 필드의 이전 숫자 값입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">새 숫자 값</p> </td> 
      <td> <p>사용자 지정 필드의 현재 숫자 값입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이전 일자 값</p> </td> 
      <td> <p>사용자 지정 필드의 이전 날짜 값입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">새 일자 값</p> </td> 
      <td> <p>사용자 지정 필드의 현재 날짜 값입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이전 텍스트 값</p> </td> 
      <td> <p>사용자 지정 필드의 이전 텍스트 값입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">새 텍스트 값</p> </td> 
      <td> <p>사용자 지정 필드의 현재 텍스트 값입니다.</p> <p>사용자 지정 필드가 서체 필드인 경우 <strong>새 텍스트 값</strong> 열에는 객체 ID가 표시됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   열 추가에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 에서 **필터** 탭, **필터 규칙 추가**&#x200B;를 만든 다음 다음을 추가합니다.

   * **분개 입력 필드 이름** > **다음 포함** > **DE**

      >[!TIP]
      >
      >이 보고서를 특정 사용자 지정 필드로 제한하려면 필터 규칙을 추가하십시오 **분개 입력 필드 이름** > **Equal** > **`<custom field>`**.

   * **프로젝트 ID** > **Equal** > **`<project>`**

      ![](assets/qs-custom-form-changes-filter-350x92.png)
   필터 추가에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (선택 사항) 보고서의 초점을 줄이고 로드 시간을 줄이려면 메시지를 추가하십시오.

   또는

   특정 프로젝트, 작업 또는 문제를 포함할 추가 필터 규칙을 만듭니다.

   >[!IMPORTANT]
   >
   >수정자를 사용하는 필터 규칙 만들기 **다음 포함** 은 실제로 로드 시간을 늘릴 수 있습니다. 이러한 이유로 다음과 같은 다른 수정자를 사용하는 것이 좋습니다 **Equal** 특정 프로젝트 또는 상위 수준 개체 ID에 대해 필터링할 수 있는 경우.

   메시지를 추가하는 방법에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 에서 **그룹화** 탭, **기존 그룹 적용**&#x200B;를 선택하고 을 선택합니다. **프로젝트**.

   그룹화 추가에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 클릭 **저장 + 닫기**.

   새 보고서가 로드됩니다.

## 프로젝트 라이프 사이클에서 계획된 완료 일자가 어떻게 변경되었는지 확인합니다. {#see-how-the-planned-completion-date-changed-over-the-course-of-a-project-s-life-cycle}

분개 입력 보고서를 설정하여 프로젝트 수명 동안 계획된 완료 일자가 변경되는 빈도를 표시할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 클릭 **새 보고서**&#x200B;를 선택하고 을 선택합니다. **분개 입력**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder가 로드됩니다.

1. 에서 **열(보기)** 탭에서 다음 열을 추가합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>열</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">필드 이름</p> </td> 
      <td> <p>영향을 받는 필드의 이름입니다.</p> <p><span style="font-weight: normal;">When</span> <strong>DE</strong>:<span style="font-weight: normal;"> 이 열에 표시되며, 이는 나열된 필드가 사용자 지정 필드임을 나타냅니다.</span></p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">유형 변경</p> </td> 
      <td>발생한 변경 유형(예: ) <strong>추가</strong>, <strong>삭제</strong>, 또는 <strong>편집</strong>.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이름별로 편집됨</p> </td> 
      <td> <p>프로젝트의 계획 완료 일자를 갱신한 사용자의 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">시작 날짜</p> </td> 
      <td> <p>프로젝트의 계획 완료 일자가 변경된 일자.</p> <p>이 필드를 내림차순으로 정렬해야 합니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">상위 ObjCode</p> </td> 
      <td> <p>계획된 완료 일자가 변경된 필드의 가장 높은 상위 객체입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">범위</p> </td> 
      <td> <p>계획된 완료 일자가 변경된 객체입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이전 일자 값</p> </td> 
      <td> <p>계획 완료 일자에 대한 이전 값.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">새 일자 값</p> </td> 
      <td> <p>계획 완료 일자에 대한 현재 값.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">프로젝트 이름</p> <p>(선택 사항입니다)</p> </td> 
      <td> <p>계획 완료 일자가 변경된 프로젝트의 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">작업 이름</p> <p>(선택 사항입니다)</p> </td> 
      <td> <p>계획 완료 일자가 변경된 프로젝트의 태스크 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">문제 이름</p> <p>(선택 사항입니다)</p> </td> 
      <td>계획 완료 일자가 변경된 프로젝트의 문제점 이름</td> 
     </tr> 
    </tbody> 
   </table>

   열 추가에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 에서 **필터** 탭, **필터 규칙 추가**&#x200B;를 만든 다음 다음을 추가합니다.

   * **필드 이름** > **Equal** > **날짜**
   * **프로젝트 ID** > **Equal** > **`<project>`**

   ![](assets/qs-planned-completion-date-change-filter-350x91.png)

   필터 추가에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (선택 사항) 보고서의 초점을 줄이고 로드 시간을 줄이려면 메시지를 추가하십시오.

   또는

   특정 프로젝트, 작업 또는 문제를 포함할 추가 필터 규칙을 만듭니다.

   >[!IMPORTANT]
   >
   >수정자를 사용하는 필터 규칙 만들기 **다음 포함** 은 실제로 로드 시간을 늘릴 수 있습니다. 이러한 이유로 다음과 같은 다른 수정자를 사용하는 것이 좋습니다 **Equal** 특정 프로젝트 또는 상위 수준 개체 ID에 대해 필터링할 수 있는 경우.

   메시지를 추가하는 방법에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 에서 **그룹화** 탭, **기존 그룹 적용**&#x200B;를 선택하고 을 선택합니다. **프로젝트**.

   그룹화 추가에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 클릭 **저장 + 닫기**.

   새 보고서가 로드됩니다.

## 프로젝트 소유자가 변경되었는지 확인합니다 {#see-if-the-owner-of-a-project-changed}

분개 입력 보고서를 설정하여 프로젝트 수명 동안 프로젝트 소유자 또는 프로젝트 관리자가 몇 번 변경되었는지 표시할 수 있습니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **보고서**.
1. 클릭 **새 보고서**&#x200B;를 선택하고 을 선택합니다. **분개 입력**.

   ![](assets/nwe-select-journal-entry-350x273.png)

   Report Builder가 로드됩니다.

1. 에서 **열(보기)** 탭에서 다음 열을 추가합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>열</th> 
      <th>설명</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p style="font-weight: bold;">필드 이름</p> </td> 
      <td>영향을 받는 필드의 이름입니다. 다음 <strong>ownerID</strong> 이 열에 표시됩니다.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">유형 변경</p> </td> 
      <td> <p>발생한 변경 유형(예: ) <strong>추가</strong>, <strong>삭제</strong>, 또는 <strong>편집</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">상위 ObjCode</p> </td> 
      <td> <p>프로젝트 소유자가 업데이트된 프로젝트의 가장 높은 상위 개체입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">시작 날짜</p> </td> 
      <td>프로젝트 소유자가 변경된 날짜입니다.<br>이 필드를 내림차순으로 정렬해야 합니다.</td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">이름별로 편집됨</p> </td> 
      <td> <p>프로젝트 소유자를 업데이트한 사용자의 이름입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">추가 정보 1</p> </td> 
      <td> <p>프로젝트의 현재 프로젝트 소유자입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">추가 정보 2</p> </td> 
      <td> <p>프로젝트의 이전 프로젝트 소유자입니다.</p> </td> 
     </tr> 
     <tr> 
      <td> <p style="font-weight: bold;">프로젝트 이름</p> </td> 
      <td> <p>프로젝트 소유자 필드가 업데이트된 프로젝트입니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   열 추가에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 에서 **필터** 탭, **필터 규칙 추가**&#x200B;를 만든 다음 다음을 추가합니다.

   * **필드 이름** > **Equal** > **ownerID**
   * **프로젝트 ID** > **Equal** > **`<project name>`**

      ![](assets/qs-owner-changes-filter-350x94.png)
   필터 추가에 대한 자세한 내용은 [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (선택 사항) 보고서의 초점을 줄이고 로드 시간을 줄이려면 메시지를 추가하십시오.

   또는

   특정 프로젝트, 작업 또는 문제를 포함할 추가 필터 규칙을 만듭니다.

   >[!IMPORTANT]
   >
   >수정자를 사용하는 필터 규칙 만들기 **다음 포함** 은 실제로 로드 시간을 늘릴 수 있습니다. 이러한 이유로 다음과 같은 다른 수정자를 사용하는 것이 좋습니다 **Equal** 특정 프로젝트 또는 상위 수준 개체 ID에 대해 필터링할 수 있는 경우.

   메시지를 추가하는 방법에 대한 자세한 내용은 [보고서에 프롬프트 추가](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. (선택 사항)에서 **그룹화** 탭, **기존 그룹 적용**&#x200B;를 선택하고 을 선택합니다. **프로젝트**.

   그룹화 추가에 대한 자세한 내용은 다음을 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 클릭 **저장 + 닫기**.

   새 보고서가 로드됩니다.
