---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 요청 유형 구성
description: 프로젝트에서 작업하는 동안 예기치 않은 이벤트가 발생할 수 있습니다. 이러한 예기치 않은 이벤트를 특정 프로젝트 또는 작업의 문제로 기록할 수 있습니다. 요청 큐로 지정된 프로젝트의 문제로 기록된 요청을 제출할 수도 있습니다. 문제 및 요청은 Adobe Workfront에서 서로 다른 것으로 간주됩니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 요청 유형 구성

프로젝트에서 작업하는 동안 예기치 않은 이벤트가 발생할 수 있습니다. 이러한 예기치 않은 이벤트를 특정 프로젝트 또는 작업의 문제로 기록할 수 있습니다. 요청 큐로 지정된 프로젝트의 문제로 기록된 요청을 제출할 수도 있습니다. 문제 및 요청은 Adobe Workfront에서 서로 다른 것으로 간주됩니다.

의 문제 만들기에 대한 정보 [!DNL Workfront]를 참조하십시오. [문제 만들기](../../../manage-work/issues/manage-issues/create-issues.md). 에서 요청 만들기에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오. [만들기 및 제출 [!DNL Adobe Workfront] 요청](../../../manage-work/requests/create-requests/create-submit-requests.md). 요청 유형을 프로젝트와 연결하는 방법에 대한 자세한 내용은 [프로젝트에 대한 요청 유형 정의](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## 요청 유형의 이름 사용자 지정

로서의 [!DNL Workfront] 관리자는 시스템에서 요청 유형의 이름을 구성할 수 있습니다. 새 이름은 [!DNL Workfront] 여기서 **[!UICONTROL 문제 유형]** 또는 **[!UICONTROL 요청 유형]** 필드 표시:

* 에서 **[!UICONTROL 큐 세부 정보]** 문제 또는 요청을 받을 프로젝트의 영역입니다.
* 요청 큐에 대해 두 개 이상의 요청 유형을 선택한 경우, **[!UICONTROL 새 문제] 양식** 에서 **[!UICONTROL 문제 유형]** 필드를 사용하여 새 문제를 만들거나 새 요청을 제출할 수 있습니다.

   에서 문제를 만드는 방법에 대한 자세한 정보 [!DNL Workfront]를 참조하십시오.  [문제 만들기](../../../manage-work/issues/manage-issues/create-issues.md)

   에서 요청 만들기에 대한 자세한 내용은 [!DNL Workfront]를 참조하십시오.  [만들기 및 제출 [!DNL Adobe Workfront] 요청](../../../manage-work/requests/create-requests/create-submit-requests.md).

* 설정 **[!UICONTROL 큐 항목 세부 정보]** 폼, 대기열 항목을 구성할 때\
   큐 항목 만들기에 대한 자세한 내용은 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

요청 유형의 이름을 사용자 지정하는 방법은 다음과 같습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 프로젝트 환경 설정]** > **[!UICONTROL 상태]**.

1. 을(를) 클릭합니다. **[!UICONTROL 문제]** 탭.
1. 맨 위에 **[!UICONTROL 문제]** 탭에서 요청 유형의 이름을 마우스로 가리킨 다음 **[!UICONTROL 편집]** 아이콘이 표시됩니다.

   ![](assets/edit-request-type-name-nwe.png)

1. 표시되는 상자에 새 이름을 입력한 다음 키를 누릅니다 **[!UICONTROL Enter 키]**.

## 다양한 요청 유형 내에서 문제 상태 구성

각 요청 유형을 다른 문제 상태와 연결할 수 있습니다. 문제의 종류에 따라 문제에 상태가 표시되는 순서를 변경할 수도 있습니다.

문제 상태의 기본 순서 변경 및 문제 상태 구성에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) 섹션 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
