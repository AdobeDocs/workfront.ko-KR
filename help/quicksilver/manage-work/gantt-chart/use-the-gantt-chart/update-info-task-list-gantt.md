---
product-area: projects
navigation-topic: use-the-gantt-chart
title: 작업 목록 Gantt 차트의 정보 업데이트
description: 작업 목록 Gantt 차트에는 프로젝트 또는 템플릿에 있는 작업에 대한 세부 정보가 표시됩니다.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 1%

---

# 작업 목록에서 정보 업데이트 [!UICONTROL 간트 차트]

작업 목록 [!UICONTROL 간트 차트] 프로젝트나 템플릿에 있는 작업에 대한 세부 정보를 표시합니다.

템플릿에서 작업 목록 [!UICONTROL 간트 차트] 은 작업 수준의 템플릿의 작업 목록에서 수행한 업데이트를 반영합니다. 는 편집할 수 없습니다 [!UICONTROL 간트 차트] 관련 항목이 없습니다.

프로젝트에서 작업 목록에서 직접 작업 정보를 업데이트할 수 있습니다 [!UICONTROL 간트 차트].

이 문서에서는 작업 목록에서 직접 수행할 수 있는 다음 작업에 대해 설명합니다 [!UICONTROL 간트 차트]:

* 작업 기간 수정
* 이전 관계 만들기 또는 제거
* 작업 시작 및 종료 날짜 변경
* 업데이트 완료율
* 수준 프로젝트 리소스

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL 편집] 액세스</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL Manage] 액세스 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 작업 기간 수정

1. 수정할 프로젝트로 이동합니다.
1. 클릭 **[!UICONTROL 작업]** 왼쪽 패널에 표시됩니다.

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. 을(를) 클릭합니다. **[!UICONTROL 간트 차트]** 아이콘.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   모든 변경 사항은 **[!UICONTROL 자동 저장]** 옵션이 활성화되어 있습니다. 기본적으로 활성화되어 있습니다.

1. (선택 사항) **[!UICONTROL 계획 모드]** 아이콘을 클릭하고 **[!UICONTROL 수동 Save Standard]** 또는 **[!UICONTROL 타임라인 계획]** 변경 사항을 수동으로 저장하려면 을 클릭합니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 작업의 타임라인 위로 마우스를 가져간 후 시간 선 표시기를 다른 날짜로 드래그합니다.
1. 작업에 대한 올바른 새 완료 날짜에 도달하면 표시기를 삭제합니다.
1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는 &#x200B;**[!UICONTROL 다시 실행]** 변경 사항을 취소하거나 복제하려면 아이콘을 사용합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 Gantt 차트에서 변경 사항을 실행 취소하거나 재실행할 수 있습니다.
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행하려면
   >   * [!DNL Windows]: 사용 [!UICONTROL Ctrl + Z] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행하려면


1. 클릭 **[!UICONTROL 저장]** 오른쪽 위 모서리에서 [!UICONTROL 간트 차트].

## 이전 관계 만들기 또는 제거

1. 수정할 프로젝트로 이동합니다.
1. 에서 **[!UICONTROL 작업]** 영역에서 **[!UICONTROL 간트 차트]** 아이콘.

   다음 **[!UICONTROL 자동 저장]** 옵션이 기본적으로 선택됩니다. 이 경우 모든 변경 사항이 자동으로 저장됩니다.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (선택 사항) **[!UICONTROL 계획 모드]** 아이콘을 클릭하고 **[!UICONTROL 수동 Save Standard]** 또는 **[!UICONTROL 타임라인 계획]** 변경 사항을 수동으로 저장하려면 을 클릭합니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 선행 관계를 만들려면 작업의 시작점을 클릭하고 작업 끝점으로 드래그합니다.
1. 선행 관계를 삭제하려면 두 작업을 연결하는 선행 선을 클릭하여 선택한 다음 키를 누릅니다 **[!UICONTROL 삭제]** 클릭합니다.\
   ![Delete_premander.png](assets/delete-predecessor-350x152.png)

1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는 &#x200B;**[!UICONTROL 다시 실행]** 변경 사항을 취소하거나 복제하려면 아이콘을 사용합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 Gantt 차트에서 변경 사항을 실행 취소하거나 재실행할 수 있습니다.
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행하려면
   >   * [!DNL Windows]: [!UICONTROL Ctrl + Z 사용] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행하려면


1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다 .

## 작업 시작 및 종료 날짜 변경

1. 수정할 프로젝트로 이동합니다.
1. 에서 **[!UICONTROL 작업]** 영역에서 **[!UICONTROL 간트 차트]** 아이콘.

   모든 변경 사항은 **[!UICONTROL 자동 저장]** 옵션이 활성화되어 있습니다. 기본적으로 활성화되어 있습니다.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (선택 사항) **[!UICONTROL 계획 모드]** 아이콘을 클릭하고 **[!UICONTROL 수동 Save Standard]** 또는 **[!UICONTROL 타임라인 계획]** 변경 사항을 수동으로 저장하려면 을 클릭합니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 작업 중심을 마우스로 가리킨 다음 다방향 화살표를 찾습니다.
1. 을(를) 클릭하고 작업을 원하는 날짜로 드래그합니다.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. 작업 제약 조건에 영향을 주는 방식으로 작업 날짜를 변경하는 경우 **[!UICONTROL 수락]** 작업 제한 변경을 승인하려면

   >[!NOTE]
   >
   >작업에 다음 제약 조건 중 하나가 있으면 시스템이 [!UICONTROL 작업 제한] to [!UICONTROL 일찍 시작 아니요] 프로젝트를 [!UICONTROL 시작 날짜] 또는 [!UICONTROL 늦어도 다음 날짜 전까지 완료] 프로젝트를 [!UICONTROL 완료 날짜]:
   >
   >   
   >   
   >   * [!UICONTROL 빠른 시일 내에]
   >   * [!UICONTROL 가능한 한 늦게]
   >   * [!UICONTROL 가장 빠른 가용 시간]
   >   * [!UICONTROL 최근 사용 가능한 시간]

   >   
   >   
   >일부 경우에는 이전 관계가 작업을 일찍 시작하지 못하도록 하고 작업 이동을 허용하지 않는 경우도 있습니다.

1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는 &#x200B;**[!UICONTROL 다시 실행]** 변경 사항을 취소하거나 복제하려면 아이콘을 사용합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 변경 사항을 실행 취소하거나 재실행할 수 있습니다 [!UICONTROL 간트 차트]:
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행하려면
   >   * [!DNL Windows]: 사용 [!UICONTROL Ctrl + Z] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행하려면


1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 업데이트 완료율

1. 수정할 프로젝트로 이동합니다.
1. 에서 **[!UICONTROL 작업]** 영역에서 **[!UICONTROL 간트 차트]** 아이콘.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   모든 변경 사항은 **[!UICONTROL 자동 저장]** 옵션이 활성화되어 있습니다. 기본적으로 활성화되어 있습니다.

1. (선택 사항) **[!UICONTROL 계획 모드]** 아이콘을 클릭하고 **[!UICONTROL 수동 Save Standard]** 또는 **[!UICONTROL 타임라인 계획]** 변경 사항을 수동으로 저장하려면 을 클릭합니다.
1. 작업 내의 퍼센트 번호를 두 번 클릭하고 번호를 입력합니다.

   >[!IMPORTANT]
   >
   >다음을 수행해야 합니다. [!UICONTROL 완료율] 에서 선택됨 [!UICONTROL 옵션] 완료율을 업데이트하는 대화 상자 이렇게 하려면 **[!UICONTROL 옵션]** 아이콘을 클릭하고 **[!UICONTROL 완료율]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >

1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는 &#x200B;**[!UICONTROL 다시 실행]** 변경 사항을 취소하거나 복제하려면 아이콘을 사용합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 변경 사항을 실행 취소하거나 재실행할 수 있습니다 [!UICONTROL 간트 차트]:
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행하려면
   >   * [!DNL Windows]: 사용 [!UICONTROL Ctrl + Z] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행하려면


1. 클릭 **[!UICONTROL 저장]** 오른쪽 위 모서리에서 [!UICONTROL 간트 차트].

## 프로젝트 리소스 수준

작업 목록을 사용할 수 있습니다 [!UICONTROL 간트 차트] 리소스 수준을 높입니다.

의 자원 평준화에 대한 자세한 내용은 [!UICONTROL 간트 차트]를 참조하십시오. [의 수준 리소스 [!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;this is drafted because I moved the whole content to the article linked above)</p>
<ol>
<li value="1">Go to the project you want to level.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> In the <strong>Tasks</strong> area, click the <strong>Gantt chart</strong> icon.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">All changes are saved automatically when the <strong>Autosave</strong> option is enabled. It is enabled by default. </p> </li>
<li value="3">
<div>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) Click the <strong>Plan mode</strong> icon and select <strong>Manual save Standard</strong> or <strong>Timeline Planning</strong> to save your changes manually.</p> <note type="tip">
You cannot level resources in the Gantt chart when the Autosave option is enabled.
</note>
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png" style="width: 350;height: 493;"> </p>
</div> </li>
<li value="4"> <p>Click the <strong>Level Resources</strong> drop-down menu.</p> <p> <img src="assets/level-resouces.png" alt="Level_resouces.png"> </p> </li>
<li value="5">Select one of following options:
<ul>
<li><strong>Level Now</strong>: Applies resource leveling to the selected task.</li>
<li><p><strong>Clear Leveling</strong>: Removes all resource leveling from the selected task.</p></li>
</ul><note type="note">
Your resources might be overallocated if they are assigned to multiple tasks which occur during the same time frame.
</note></li>
<li value="6"> <p>(Optional and conditional) If you have disabled the Autosave option, click the <strong>Undo</strong> or<strong>Redo</strong> icons if you want to cancel or duplicate any of the changes. </p> <note type="tip">
<p>You can use the following keyboard shortcuts to undo or redo changes on the Gantt chart:</p>
<ul>
<li>Mac: Use Command + Z to undo and Command + Shift + Z to redo.</li>
<li>Windows: Use Ctrl + Z to undo and Ctrl + Y to redo.</li>
</ul>
</note> </li>
<li value="7">Click <strong>Save</strong> in the upper-right corner of the Gantt chart.</li>
</ol>
</div>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"> </h2>
-->
