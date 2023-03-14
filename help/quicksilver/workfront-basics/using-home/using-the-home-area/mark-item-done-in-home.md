---
product-area: projects
navigation-topic: use-the-home-area
title: 홈 영역에서 완료 로 항목 표시
description: 작업 또는 문제 담당자인 경우 작업이나 문제를 완료 로 표시할 수 있습니다. 작업이나 문제를 완료 로 표시하면 작업이나 문제의 상태가 완료 로 변경됩니다.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 항목을 다음으로 표시 [!UICONTROL 완료] 에서 [!UICONTROL 홈] 영역

작업 또는 문제 담당자인 경우 작업이나 문제를 완료 로 표시할 수 있습니다. 작업 또는 문제를 [!UICONTROL 완료]로 설정하면 작업이나 문제의 상태가 [!UICONTROL 완료].

>[!NOTE]
>
>이 표시되지 않습니다 [!UICONTROL 완료] 작업 또는 문제에 할당된 리소스 중 하나가 아니면 버튼을 클릭합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>작업 및 문제에 대한 [!UICONTROL 편집] 액세스</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 대한 사용 권한 이상을 제공합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 작업 또는 문제를 다음으로 표시 [!UICONTROL 완료]

작업이나 문제에 지정된 사용자만 해당 작업을 [!UICONTROL 완료].

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** ![](assets/main-menu-icon.png) 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 홈]**.
1. 에서 **[!UICONTROL 작업 목록]**&#x200B;에서 작업 대기 중인 항목을 찾습니다.
1. 다음 중 하나를 수행합니다.

* 클릭 **[!UICONTROL 완료]** 작업 항목에 있는 경우\
   자세한 내용은 [다음 옵션 이해 [!UICONTROL 완료] 버튼](#understand-the-options-of-the-done-button) 을 참조하십시오.

* 표시하려는 항목을 선택하고 오른쪽 패널에서 **[!UICONTROL 업데이트 상태]**&#x200B;를 입력한 다음 항목의 상태를 와 같은 상태로 변경합니다. [!UICONTROL 완료] 또는 [!UICONTROL 닫힘].

## 다음 옵션 이해 [!UICONTROL 완료] 버튼

기본적으로 [!UICONTROL 완료] 작업 항목의 버튼은 해당 항목의 상태를 [!UICONTROL 완료] (작업의 경우) 또는 [!UICONTROL 해결됨] (문제)

사용자 [!DNL Adobe Workfront] 관리자는 어떤 상태와 연결되어 있는지 사용자 정의할 수 있습니다 [!UICONTROL 완료] 를 클릭하고 이러한 사용자 지정 사항을 홈 팀에 적용합니다.

연관된 상태 수에 따라 [!UICONTROL 완료] 단추나 작업 또는 문제에 할당되는 리소스, [!UICONTROL 완료] 버튼을 변경할 수 있습니다.

* [[!UICONTROL 완료] 하나의 상태에 연결된 단추](#done-button-associated-with-one-status)
* [[!UICONTROL 완료] 여러 상태에 연결된 단추](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL 완료] 여러 리소스에 할당된 항목의 단추](#done-button-for-items-assigned-to-multiple-resources)

### [!UICONTROL 완료] 하나의 상태에 연결된 단추

이 [!UICONTROL 완료] 버튼은 하나의 상태와 연결되며 작업 항목은 사용자에게 할당되며 버튼 읽기는 사용자에게 할당됩니다 **[!UICONTROL 완료]**. 이 옵션을 클릭하면 작업 또는 문제의 상태가 [!UICONTROL 완료] 버튼을 클릭합니다.

![완료 단추](assets/Done.png)

어떤 상태와 연관되는지를 이해하기 위해 [!UICONTROL 완료] 버튼을 클릭하고 [!UICONTROL 팀 설정] 귀하 홈팀 [!UICONTROL 완료 단추] 섹션에 설명된 대로 [팀 설정 편집](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

홈 팀에 할당되지 않은 경우 [!UICONTROL 완료]에 설명된 대로, [다음 옵션 이해 [!UICONTROL 완료] 버튼](#understand-the-options-of-the-done-button).

### [!UICONTROL 완료] 여러 상태에 연결된 단추

이 [!UICONTROL 완료] 버튼은 두 개 이상의 상태와 연결되며 버튼은 단어를 표시합니다 **[!UICONTROL 완료]** 그 뒤에는 드롭다운 메뉴가 옵니다. 이 시나리오에서는 [!UICONTROL 완료]. 드롭다운 메뉴에서 상태를 선택해야 합니다. 작업 항목의 완료에 가장 적합한 상태를 선택합니다. 이렇게 하면 작업 항목의 상태가 변경됩니다.

여러 상태를 [!UICONTROL 완료] 버튼 [구성 [!UICONTROL 완료] 작업의 단추](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) 및 [구성 [!UICONTROL 완료] 문제에 대한 단추](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL 완료] 여러 리소스에 할당된 항목의 단추

작업 또는 문제가 둘 이상의 리소스에 할당되면 단추에 라는 단어가 표시됩니다 **[!UICONTROL 완료]** 그 뒤에는 드롭다운 메뉴가 옵니다. 드롭다운 메뉴에서 다음 중 선택할 수 있습니다 **[!UICONTROL 내 몫으로 끝남]** (이 기능을 통해 팀 구성원에게 사용자가 작업 일부를 완료했음을 알 수 있음) 또는 [!UICONTROL 완료] 단추(항목을 완료하는). 선택한 후 **[!UICONTROL 내 몫으로 끝남]**&#x200B;작업 항목은 작업 목록에서 제거되지만 작업 항목에 지정된 작업 목록에 남아 있습니다.\
완료 단추가 여러 상태와 연결된 경우 아래에 나열됩니다 **내 몫으로 끝남**.

>[!NOTE]
>
>여러 직원이 있는 작업이나 문제에 대해, 각 사용자는 작업이나 문제에 대한 자신의 할당이 실제로 완료되었음을 나타냅니다. 이러한 이유로 각 할당자는 [!UICONTROL 완료] 항목에 지정된 작업을 완료했음을 보여 줍니다.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
