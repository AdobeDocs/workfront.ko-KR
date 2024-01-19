---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: 에서 리소스 레벨링  [!UICONTROL 간트 차트]
description: 간트 차트에서 리소스를 레벨링하는 방법에 대한 정보입니다.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# 에서 리소스 레벨링 [!UICONTROL 간트 차트]

프로젝트에 대한 리소스 레벨링은 두 가지 목적이 있습니다.

* 할당자에 대한 시간 초과 할당을 자동으로 조정하려면 다음을 수행하십시오.
* 프로젝트에 대한 현실적인 작업 일정을 자동으로 만듭니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 편집] 액세스 권한</p> <p><b>메모</b>

아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 관리] 액세스 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 리소스 레벨링 개요

동일한 자원이 두 개의 서로 다른 작업에 할당된 경우 리소스 레벨링을 사용하여 작업의 타임라인을 조정하면 동시에 작업이 발생하지 않습니다.

프로젝트에서 리소스를 레벨링할 때는 다음 사항을 고려하십시오.

* 리소스 레벨링은 하나의 프로젝트에만 적용되므로 [!DNL Adobe Workfront] 은 한 번에 두 개 이상의 프로젝트에서 리소스를 레벨링하지 않습니다.
* If **[!UICONTROL 작업량 고정]** 이(가) (으)로 선택됨 **[!UICONTROL 기간 유형]**, [!DNL Workfront] 리소스를 레벨링하지 않습니다.
* 동일한 작업에 여러 사용자가 할당되면 레벨링이 취소됩니다.
* 유형 조건 **[!UICONTROL 작업 제한]** 은(는) 리소스 레벨링보다 우선합니다. 예를 들어 다음과 같습니다. **[!UICONTROL 고정 날짜]** 이(가) (으)로 선택됨 [!UICONTROL 작업 제한], 리소스 레벨링은 작업 날짜를 변경하지 않습니다.
* 전임 작업 관계는 리소스 배정 평준화보다 우선합니다.
* **[!UICONTROL 리소스 레벨링]** 을(를) (으)로 설정해야 함 **[!UICONTROL 수동]** 의 레벨링을 조정하기 위한 프로젝트용 [!UICONTROL 간트 차트]. 프로젝트에 대한 관리 권한이 있는 경우 프로젝트에서 이 설정을 조정하고 을 선택하면 시스템에서 자동으로 리소스 수준을 조정할 수 있습니다. **[!UICONTROL 자동]** 대신 **[!UICONTROL 수동]** 다음에서 **[!UICONTROL 프로젝트 편집]** 상자.

  ![](assets/resource-leveling-mode-350x177.png)

* 프로젝트 소유자 또는 작업 할당자는 작업에 레벨링 지연을 도입하여 작업에 추가 시간이 필요할 수 있음을 나타낼 수 있습니다. 작업에 레벨링 지연 추가에 대한 자세한 내용은 [작업 레벨링 지연 업데이트](../../../manage-work/tasks/task-information/task-leveling-delay.md).

## 에서 리소스 레벨링 적용 [!UICONTROL 간트 차트]

작업 목록을 사용할 수 있습니다. [!UICONTROL 간트 차트] 리소스를 레벨링합니다.

1. 레벨링할 프로젝트로 이동합니다.
1. 다음에서 **[!UICONTROL 작업]** 영역을 클릭하고 **[!UICONTROL 간트 차트]** 아이콘.

   다음 경우에 모든 변경 사항이 자동으로 저장됩니다. **[!UICONTROL 자동 저장]** 옵션이 활성화되어 있습니다. 기본적으로 활성화되어 있습니다.

1. (선택 사항) **[!UICONTROL 플랜] 모드** 아이콘 및 선택 **[!UICONTROL 수동 저장 Standard]** 또는 **[!UICONTROL 타임라인 계획 수립]** 변경 사항을 수동으로 저장합니다.

   >[!TIP]
   >
   >에서 리소스를 레벨링할 수 없습니다.  [!UICONTROL 간트 차트] 다음과 같은 경우 [!UICONTROL 자동 저장] 옵션이 활성화되어 있습니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 다음을 클릭합니다. **[!UICONTROL 리소스 레벨링]** 드롭다운 메뉴.

   ![Level_resources.png](assets/level-resouces.png)

1. 다음 옵션 중 하나를 선택합니다.

   * **[!UICONTROL 지금 레벨링]**: 선택한 작업에 리소스 레벨링을 적용합니다.
   * **[!UICONTROL 레벨링 지우기]**: 선택한 작업에서 모든 리소스 레벨링을 제거합니다.

   >[!NOTE]
   >
   >동일한 시간대 동안 발생하는 여러 작업에 자원이 할당되면 자원이 초과 할당될 수 있습니다.

1. (선택 사항 및 조건부) 자동 저장 옵션을 비활성화한 경우 **[!UICONTROL 실행 취소]** 또는&#x200B;**[!UICONTROL 다시 실행]** 아이콘을 클릭하여 변경 내용을 취소하거나 복제합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 의 변경 내용을 실행 취소하거나 재실행할 수 있습니다. [!UICONTROL 간트 차트]:
   >
   >* [!DNL Mac]: 사용 [!UICONTROL Command + Z] 실행 취소 및 [!UICONTROL Command + Shift + Z] 다시 실행합니다.
   >* Windows: [!UICONTROL Ctrl + Z] 실행 취소 및 [!UICONTROL Ctrl + Y] 다시 실행합니다.


1. 클릭 **[!UICONTROL 저장]** 의 오른쪽 위 모서리 [!UICONTROL 간트 차트].

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Overview of Leveling Delay</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article: /Content/Manage work/Tasks/Task information/task-leveling-delay.htm) </p>
<p>At times, there might be conflicts between task schedules on a project. You can level resources or address resource conflicts by rescheduling resources and tasks so that all tasks can be completed within a realistic schedule. </p>
<p>As the project manager, or the task assignee, you can also add a Leveling Delay on individual tasks to account for any resource or scheduling conflicts. In other words, a task might be scheduled with a delay to ensure that when Adobe Workfront levels the tasks a more realistic schedule overcomes resource conflicts.</p>
<p>To manually add a Leveling Delay to a task:</p>
<ol>
<li value="1">Navigate to a task for which you want to add a Leveling Delay.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the <strong>More icon</strong> to the right of the task name, then click <strong>Edit</strong>. </p>  </li>
<li value="3">Click <strong>Settings</strong>.<br></li>
<li value="4">Specify the <strong>Leveling Delay</strong>, in hours.<br>This is the time that the resource will be delayed starting the task due to resource conflicts.</li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
