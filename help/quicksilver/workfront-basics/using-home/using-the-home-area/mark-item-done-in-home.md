---
product-area: projects
navigation-topic: use-the-home-area
title: 홈 영역에서 항목을 완료로 표시
description: 작업 또는 문제 피할당자인 경우 작업 또는 문제를 완료로 표시할 수 있습니다. 작업 또는 문제를 완료로 표시하면 작업 또는 문제의 상태가 완료로 변경됩니다.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 항목을 다음으로 표시 [!UICONTROL 완료] 다음에서 [!UICONTROL 홈] 영역

작업 또는 문제 피할당자인 경우 작업 또는 문제를 완료로 표시할 수 있습니다. 작업 또는 문제를 (으)로 표시할 경우 [!UICONTROL 완료], 작업 또는 문제의 상태가 (으)로 변경됨 [!UICONTROL 완료].

>[!NOTE]
>
>이 표시되지 않습니다. [!UICONTROL 완료] 작업 또는 문제에 할당된 리소스 중 하나가 아닌 경우 버튼을 누릅니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td> <p>작업 및 문제에 대한 [!UICONTROL 편집] 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 권한 이상 부여</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 작업 또는 문제를 다음으로 표시 [!UICONTROL 완료]

작업 또는 문제에 할당된 사용자만 다음으로 표시할 수 있습니다. [!UICONTROL 완료].

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** ![](assets/main-menu-icon.png) 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 홈]**.
1. 다음에서 **[!UICONTROL 작업 목록]**&#x200B;을(를) 클릭하여 작업을 기다리고 있는 항목을 찾습니다.
1. 다음 중 하나를 수행합니다.

* 클릭 **[!UICONTROL 완료]** 작업 항목.\
   다음을 참조하십시오 [의 옵션 이해 [!UICONTROL 완료] 단추](#understand-the-options-of-the-done-button) 이 단추가 표시되는 방법에 대한 자세한 내용은 을 참조하십시오.

* 완료로 표시할 항목을 선택하고 오른쪽 패널에서 을 클릭합니다. **[!UICONTROL 업데이트 상태]**&#x200B;를 클릭한 다음 항목의 상태를 다음과 같은 상태로 변경합니다. [!UICONTROL 완료] 또는 [!UICONTROL 종료됨].

## 의 옵션 이해 [!UICONTROL 완료] 단추

기본적으로 [!UICONTROL 완료] 작업 항목에 대한 버튼을 클릭하면 해당 항목의 상태가 다음으로 변경됩니다. [!UICONTROL 완료] (작업용) 또는 [!UICONTROL 해결됨] (문제의 경우).

사용자 [!DNL Adobe Workfront] 관리자는 와(과) 연관된 상태를 사용자 정의할 수 있습니다. [!UICONTROL 완료] 을 누르고 홈 팀에 이러한 사용자 지정을 적용합니다.

와 연결된 상태의 수에 따라 [!UICONTROL 완료] 버튼 또는 작업 또는 문제에 할당된 리소스 수, 모양 [!UICONTROL 완료] 버튼은 변경될 수 있습니다.

* [[!UICONTROL 완료] 하나의 상태와 연결된 단추](#done-button-associated-with-one-status)
* [[!UICONTROL 완료] 여러 상태와 연결된 단추](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL 완료] 여러 리소스에 할당된 항목에 대한 단추](#done-button-for-items-assigned-to-multiple-resources)

### [!UICONTROL 완료] 하나의 상태와 연결된 단추

다음의 경우 [!UICONTROL 완료] 버튼은 하나의 상태와 연결되어 있고 작업 항목이 사용자에게만 할당되어 있습니다. 버튼은 다음과 같이 표시됩니다. **[!UICONTROL 완료]**. 클릭하면 작업 또는 문제의 상태가 와 연결된 상태로 변경됩니다. [!UICONTROL 완료] 단추를 클릭합니다.

![완료 버튼](assets/Done.png)

연결된 상태를 이해하려면 [!UICONTROL 완료] 단추, 확인 [!UICONTROL 팀 설정] 홈 팀 의 [!UICONTROL 완료 단추] 섹션에 설명된 대로 섹션 [팀 설정 편집](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

홈 팀에 할당되지 않은 경우 을 클릭하면 기본 상태가 선택됩니다. [!UICONTROL 완료]에서 위에 설명된 대로 [의 옵션 이해 [!UICONTROL 완료] 단추](#understand-the-options-of-the-done-button).

### [!UICONTROL 완료] 여러 상태와 연결된 단추

다음의 경우 [!UICONTROL 완료] 단추는 둘 이상의 상태와 연결되어 있으며 단추에 단어가 표시됩니다. **[!UICONTROL 완료]** 드롭다운 메뉴 뒤에 표시됩니다. 이 시나리오에서는 [!UICONTROL 완료]. 드롭다운 메뉴에서 상태를 선택해야 합니다. 작업 항목 완료에 가장 적합한 상태를 선택합니다. 이렇게 하면 작업 항목의 상태가 변경됩니다.

여러 상태를 와 연결하는 방법을 이해하려면 [!UICONTROL 완료] 단추, 참조 [구성 [!UICONTROL 완료] 작업 단추](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) 및 [구성 [!UICONTROL 완료] 문제 버튼](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL 완료] 여러 리소스에 할당된 항목에 대한 단추

작업 또는 문제가 둘 이상의 리소스에 할당되면 버튼에 단어가 표시됩니다 **[!UICONTROL 완료]** 드롭다운 메뉴 뒤에 표시됩니다. 드롭다운 메뉴에서 다음 중 하나를 선택할 수 있습니다 **[!UICONTROL 내 부분 완료]** (팀 멤버에게 사용자가 작업 부분을 완료했다는 것을 알려줌) 또는 과 연관된 상태 [!UICONTROL 완료] 단추(항목이 완료됨) 다음을 선택한 후 **[!UICONTROL 내 부분 완료]**, 작업 항목이 작업 목록에서 제거되지만 여전히 작업 항목에 할당된 사용자의 작업 목록에 남아 있습니다.\
완료 버튼이 여러 상태와 연관되어 있으면 아래에 나열됩니다. **내 부분 완료**.

>[!NOTE]
>
>여러 명의 할당자가 있는 작업 또는 문제에서 각 사용자는 작업 또는 문제에 대한 자신의 할당이 실제로 완료되었음을 표시할 책임이 있습니다. 따라서 각 할당자는 [!UICONTROL 완료] 항목에 할당된 작업이 완료되었음을 보여 줍니다.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
