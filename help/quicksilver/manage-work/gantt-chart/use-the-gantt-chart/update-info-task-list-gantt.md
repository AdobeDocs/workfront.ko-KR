---
product-area: projects
navigation-topic: use-the-gantt-chart
title: 작업 목록 간트 차트에서 정보 업데이트
description: 작업 목록 간트 차트는 프로젝트 또는 템플릿에 있는 작업에 대한 세부 정보를 보여 줍니다.
author: Alina
feature: Work Management
exl-id: 0a8e6fd5-985c-49e5-842d-67ade29ee1c9
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 1%

---

# 작업 목록에서 정보 업데이트 [!UICONTROL 간트 차트]

작업 목록 [!UICONTROL 간트 차트] 프로젝트 또는 템플릿에 있는 작업에 대한 세부 정보를 표시합니다.

템플릿의 작업 목록 [!UICONTROL 간트 차트] 은 작업 수준에서 템플릿의 작업 목록에 수행된 업데이트를 반영합니다. 다음을 편집할 수 없습니다. [!UICONTROL 간트 차트] 템플릿에 연결됩니다.

프로젝트에서 작업 목록에서 직접 작업 정보를 업데이트할 수 있습니다 [!UICONTROL 간트 차트].

이 문서에서는 작업 목록에서 직접 수행할 수 있는 다음 작업에 대해 설명합니다 [!UICONTROL 간트 차트]:

* 작업 기간 수정
* 전임 작업 관계 만들기 또는 제거
* 작업 시작 및 종료 날짜 변경
* 완료율 업데이트
* 프로젝트 리소스 레벨링

## 액세스 요구 사항

이 문서의 단계를 따르려면 다음 사항이 있어야 합니다.

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
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL 편집] 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 작업에 대한 [!UICONTROL 관리] 액세스 권한 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 작업 기간 수정

1. 수정할 프로젝트로 이동합니다.
1. 클릭 **[!UICONTROL 작업]** 왼쪽 패널에서

   ![](assets/qs-tasks-area-highlighted-in-the-secondary-nav-350x206.png)

1. 다음을 클릭합니다. **[!UICONTROL 간트 차트]** 아이콘.

   ![간트 차트 아이콘 클릭](assets/click-gantt-chart-icon.png)

   다음 경우에 모든 변경 사항이 자동으로 저장됩니다. **[!UICONTROL 자동 저장]** 옵션이 활성화되어 있습니다. 기본적으로 활성화되어 있습니다.

1. (선택 사항) **[!UICONTROL 플랜 모드]** 아이콘 및 선택 **[!UICONTROL 수동 저장 Standard]** 또는 **[!UICONTROL 타임라인 계획 수립]** 변경 사항을 수동으로 저장합니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 작업의 타임라인을 마우스로 가리킨 다음 타임라인 표시기를 다른 날짜로 끕니다.
1. 작업의 올바른 새 완료 날짜에 도달하면 표시기를 놓습니다.
1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는&#x200B;**[!UICONTROL 다시 실행]** 아이콘을 클릭하여 변경 내용을 취소하거나 복제합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 간트 차트에서 변경 사항을 실행 취소하거나 재실행할 수 있습니다.
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행합니다.
   >   * [!DNL Windows]: 사용 [!UICONTROL Ctrl + Z] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행합니다.
   >   
   >

1. 클릭 **[!UICONTROL 저장]** 의 오른쪽 위 모서리 [!UICONTROL 간트 차트].

## 전임 작업 관계 만들기 또는 제거

1. 수정할 프로젝트로 이동합니다.
1. 다음에서 **[!UICONTROL 작업]** 영역을 클릭하고 **[!UICONTROL 간트 차트]** 아이콘.

   다음 **[!UICONTROL 자동 저장]** 기본적으로 옵션이 선택되어 있으며, 이 경우 모든 변경 사항이 자동으로 저장됩니다.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (선택 사항) **[!UICONTROL 플랜 모드]** 아이콘 및 선택 **[!UICONTROL 수동 저장 Standard]** 또는 **[!UICONTROL 타임라인 계획 수립]** 변경 사항을 수동으로 저장합니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 전임 작업 관계를 만들려면 작업의 시작점을 클릭하고 작업의 끝점으로 끕니다.
1. 전임 작업 관계를 삭제하려면 두 작업을 연결하는 전임 작업 줄을 클릭하여 선택한 다음 키를 누릅니다 **[!UICONTROL 삭제]** 키보드에서.\
   ![Delete_predecesser.png](assets/delete-predecessor-350x152.png)

1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는&#x200B;**[!UICONTROL 다시 실행]** 아이콘을 클릭하여 변경 내용을 취소하거나 복제합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 간트 차트에서 변경 사항을 실행 취소하거나 재실행할 수 있습니다.
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행합니다.
   >   * [!DNL Windows]: [!UICONTROL Ctrl + Z 사용] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행합니다.
   >   
   >

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다 .

## 작업 시작 및 종료 날짜 변경

1. 수정할 프로젝트로 이동합니다.
1. 다음에서 **[!UICONTROL 작업]** 영역을 클릭하고 **[!UICONTROL 간트 차트]** 아이콘.

   다음 경우에 모든 변경 사항이 자동으로 저장됩니다. **[!UICONTROL 자동 저장]** 옵션이 활성화되어 있습니다. 기본적으로 활성화되어 있습니다.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

1. (선택 사항) **[!UICONTROL 플랜 모드]** 아이콘 및 선택 **[!UICONTROL 수동 저장 Standard]** 또는 **[!UICONTROL 타임라인 계획 수립]** 변경 사항을 수동으로 저장합니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 작업의 가운데로 마우스를 가져간 후 여러 방향 화살표를 찾습니다.
1. 을(를) 클릭하고 작업을 원하는 날짜로 드래그합니다.

   ![Change_start_end_date.png](assets/change-start-end-date.png)

1. 작업 제한 사항에 영향을 주는 방식으로 작업 날짜를 변경하는 경우 **[!UICONTROL Accept]** 작업 제한 사항 변경을 확인합니다.

   >[!NOTE]
   >
   >작업에 다음 제한 사항 중 하나가 있으면 시스템이 [!UICONTROL 작업 제한] 끝 [!UICONTROL 더 이상 시작하지 않음] 프로젝트가 다음에서 예약되는 경우: [!UICONTROL 시작일] 또는 [!UICONTROL 다음 이후에 완료:] 프로젝트가 다음 위치에서 예약되는 경우 [!UICONTROL 완료 일자]:
   >
   >   
   >   
   >   * [!UICONTROL 빠른 시일 내에]
   >   * [!UICONTROL 가능한 한 늦게]
   >   * [!UICONTROL 가장 빠른 가용 시간]
   >   * [!UICONTROL 최근 사용 가능한 시간]
   >   
   >   
   >경우에 따라 전임 작업 관계로 인해 작업이 더 일찍 시작되지 않을 수 있으며 작업 이동이 허용되지 않습니다.

1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는&#x200B;**[!UICONTROL 다시 실행]** 아이콘을 클릭하여 변경 내용을 취소하거나 복제합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 의 변경 내용을 실행 취소하거나 재실행할 수 있습니다. [!UICONTROL 간트 차트]:
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행합니다.
   >   * [!DNL Windows]: 사용 [!UICONTROL Ctrl + Z] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행합니다.
   >   
   >

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 완료율 업데이트

1. 수정할 프로젝트로 이동합니다.
1. 다음에서 **[!UICONTROL 작업]** 영역을 클릭하고 **[!UICONTROL 간트 차트]** 아이콘.

   ![](assets/qs-gantt-icon-on-task-list-highlighted-350x199.png)

   다음 경우에 모든 변경 사항이 자동으로 저장됩니다. **[!UICONTROL 자동 저장]** 옵션이 활성화되어 있습니다. 기본적으로 활성화되어 있습니다.

1. (선택 사항) **[!UICONTROL 플랜 모드]** 아이콘 및 선택 **[!UICONTROL 수동 저장 Standard]** 또는 **[!UICONTROL 타임라인 계획 수립]** 변경 사항을 수동으로 저장합니다.
1. 작업 내의 백분율 숫자를 두 번 클릭하고 숫자를 입력합니다.

   >[!IMPORTANT]
   >
   >다음을 수행해야 합니다. [!UICONTROL % 완료] 다음에서 선택됨: [!UICONTROL 옵션] 완료율을 업데이트하는 대화 상자. 이렇게 하려면 **[!UICONTROL 옵션]** 아이콘 및 선택 **[!UICONTROL % 완료]**.
   >
   >
   >![update_percent_complete.png](assets/update-percent-complete-350x175.png)   >
   >

1. (선택 사항 및 조건부) 변경 사항을 수동으로 저장하도록 선택한 경우 **[!UICONTROL 실행 취소]** 또는&#x200B;**[!UICONTROL 다시 실행]** 아이콘을 클릭하여 변경 내용을 취소하거나 복제합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 의 변경 내용을 실행 취소하거나 재실행할 수 있습니다. [!UICONTROL 간트 차트]:
   >
   >   
   >   
   >   * [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행합니다.
   >   * [!DNL Windows]: 사용 [!UICONTROL Ctrl + Z] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행합니다.
   >   
   >

1. 클릭 **[!UICONTROL 저장]** 의 오른쪽 위 모서리 [!UICONTROL 간트 차트].

## 프로젝트 리소스 레벨링

작업 목록을 사용할 수 있습니다. [!UICONTROL 간트 차트] 리소스를 레벨링합니다.

의 리소스 레벨링에 대한 자세한 내용 [!UICONTROL 간트 차트], 참조 [에서 리소스 레벨링 [!UICONTROL 간트 차트]](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

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
