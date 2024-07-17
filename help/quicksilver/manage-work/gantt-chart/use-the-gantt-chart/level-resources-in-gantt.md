---
product-area: resource-management
navigation-topic: use-the-gantt-chart
title: '[!UICONTROL 간트 차트]에서 리소스 레벨링'
description: 간트 차트에서 리소스를 레벨링하는 방법에 대한 정보입니다.
author: Alina
feature: Work Management
exl-id: ba96c01d-03b8-4728-b5e3-b10d227f51b0
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# [!UICONTROL 간트 차트]에서 리소스 레벨링

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

아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 [!UICONTROL 관리] 액세스 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 리소스 레벨링 개요

동일한 자원이 두 개의 서로 다른 작업에 할당된 경우 리소스 레벨링을 사용하여 작업의 타임라인을 조정하면 동시에 작업이 발생하지 않습니다.

프로젝트에서 리소스를 레벨링할 때는 다음 사항을 고려하십시오.

* 리소스 레벨링은 한 프로젝트에만 적용되므로 [!DNL Adobe Workfront]에서는 한 번에 두 개 이상의 프로젝트에서 리소스를 레벨링하지 않습니다.
* **[!UICONTROL 작업량 고정]**&#x200B;을(를) **[!UICONTROL 기간 형식]**(으)로 선택하면 [!DNL Workfront]에서 리소스를 레벨링하지 않습니다.
* 동일한 작업에 여러 사용자가 할당되면 레벨링이 취소됩니다.
* **[!UICONTROL 작업 제한]** 유형에 대한 조건이 리소스 레벨링보다 우선합니다. 예를 들어 **[!UICONTROL 고정 날짜]**&#x200B;을(를) [!UICONTROL 작업 제한](으)로 선택하면 리소스 레벨링이 작업 날짜를 변경하지 않습니다.
* 전임 작업 관계는 리소스 배정 평준화보다 우선합니다.
* [!UICONTROL 간트 차트]에서 수준을 조정하려면 프로젝트에 대해 **[!UICONTROL 리소스 수준 조정]**&#x200B;을 **[!UICONTROL 수동]**(으)로 설정해야 합니다. 프로젝트에 대한 관리 권한이 있는 경우 프로젝트에서 이 설정을 조정하고 **[!UICONTROL 프로젝트 편집]** 상자에서 **[!UICONTROL 수동]** 대신 **[!UICONTROL 자동]**&#x200B;을 선택하여 시스템에서 자동으로 리소스 수준을 조정할 수 있습니다.

  ![](assets/resource-leveling-mode-350x177.png)

* 프로젝트 소유자 또는 작업 할당자는 작업에 레벨링 지연을 도입하여 작업에 추가 시간이 필요할 수 있음을 나타낼 수 있습니다. 작업에 레벨링 지연을 추가하는 방법에 대한 자세한 내용은 [작업 레벨링 지연 업데이트](../../../manage-work/tasks/task-information/task-leveling-delay.md)를 참조하십시오.

## [!UICONTROL 간트 차트]에서 리소스 레벨링 적용

작업 목록 [!UICONTROL 간트 차트]를 사용하여 리소스를 레벨링할 수 있습니다.

1. 레벨링할 프로젝트로 이동합니다.
1. **[!UICONTROL 작업]** 영역에서 **[!UICONTROL 간트 차트]** 아이콘을 클릭합니다.

   **[!UICONTROL 자동 저장]** 옵션을 사용하면 모든 변경 내용이 자동으로 저장됩니다. 기본적으로 활성화되어 있습니다.

1. (선택 사항) **[!UICONTROL 계획] 모드** 아이콘을 클릭하고 **[!UICONTROL 표준 수동 저장]** 또는 **[!UICONTROL 타임라인 계획 수립]**&#x200B;을 선택하여 변경 사항을 수동으로 저장합니다.

   >[!TIP]
   >
   >[!UICONTROL 자동 저장] 옵션이 활성화된 경우 [!UICONTROL 간트 차트]에서 리소스의 수준을 조정할 수 없습니다.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. **[!UICONTROL 리소스 수준]** 드롭다운 메뉴를 클릭합니다.

   ![Level_resources.png](assets/level-resouces.png)

1. 다음 옵션 중 하나를 선택합니다.

   * **[!UICONTROL 지금 레벨링]**: 선택한 작업에 리소스 레벨링을 적용합니다.
   * **[!UICONTROL 레벨링 지우기]**: 선택한 작업에서 모든 리소스 레벨링을 제거합니다.

   >[!NOTE]
   >
   >동일한 시간대 동안 발생하는 여러 작업에 자원이 할당되면 자원이 초과 할당될 수 있습니다.

1. (선택 사항 및 조건부) 자동 저장 옵션을 비활성화한 경우 변경 내용을 취소하거나 복제하려면 **[!UICONTROL 실행 취소]** 또는 &#x200B;**[!UICONTROL 다시 실행]** 아이콘을 클릭합니다.

   >[!TIP]
   >
   >다음 키보드 단축키를 사용하여 [!UICONTROL 간트 차트]의 변경 내용을 실행 취소하거나 다시 실행할 수 있습니다.
   >
   >* [!DNL Mac]: [!UICONTROL Command + Z]를 사용하여 실행을 취소하고 [!UICONTROL Command + Shift + Z]를 사용하여 실행을 취소합니다.
   >* Windows: 실행을 취소하려면 [!UICONTROL Ctrl + Z]를 사용하고 실행을 취소하려면 [!UICONTROL Ctrl + Y]를 사용하십시오.


1. [!UICONTROL 간트 차트]의 오른쪽 상단 모서리에서 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

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
