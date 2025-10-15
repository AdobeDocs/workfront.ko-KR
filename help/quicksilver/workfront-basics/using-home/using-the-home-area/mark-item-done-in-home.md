---
product-area: projects
navigation-topic: use-the-home-area
title: 홈 영역에서 항목을 완료로 표시
description: 작업 또는 문제 피할당자인 경우 작업 또는 문제를 완료로 표시할 수 있습니다. 작업 또는 문제를 완료로 표시하면 작업 또는 문제의 상태가 완료로 변경됩니다.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 41f58261d4f2e6075187886b371a23eb5e97d823
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# [!UICONTROL Home] 영역에서 항목을 [!UICONTROL Done]&#x200B;(으)로 표시

작업 또는 문제 피할당자인 경우 작업 또는 문제를 완료로 표시할 수 있습니다. 작업 또는 문제를 [!UICONTROL 완료]&#x200B;(으)로 표시하면 작업 또는 문제의 상태가 [!UICONTROL 완료]&#x200B;(으)로 변경됩니다.

>[!NOTE]
>
>작업 또는 문제에 할당된 리소스 중 하나가 아니면 [!UICONTROL 완료] 단추가 표시되지 않습니다.

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td> 
   <p>표준</p>
   <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>작업 및 문제에 대한 [!UICONTROL 편집] 액세스</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업해야 하는 작업 및 문제에 권한 이상 부여</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 내 작업 위젯에서 작업 항목을 완료로 표시

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 작업** 위젯을 추가합니다.
1. 작업 항목을 찾은 다음 작업 항목에서 **[!UICONTROL 완료로 표시]**를 클릭합니다.
이 단추가 표시되는 방법에 대한 자세한 내용은 [[!UICONTROL 완료] 단추의 옵션 이해](#understand-the-options-of-the-done-button)를 참조하십시오.
   ![내 작업 표시 완료](assets/my-work-done.png)


## 요약 패널에서 작업 항목을 완료됨으로 표시

요약 패널을 사용하여 내 작업 및 내 문제 위젯에서 작업 항목을 완료 로 표시할 수 있습니다.

1. 오른쪽 상단의 **[!UICONTROL 주 메뉴]** ![주 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 홈]**&#x200B;을 클릭합니다.
1. (조건부) **사용자 지정**&#x200B;을 클릭하여 **내 작업** 또는 **내 문제** 위젯을 추가합니다.
1. 작업 항목을 마우스로 가리킨 다음 **요약** 아이콘을 클릭합니다.
   ![요약 열기](assets/open-summary-new-home.png)
1. 요약 패널 상단의 **완료 표시**&#x200B;를 클릭합니다.


## [!UICONTROL 완료] 단추의 옵션 이해

기본적으로 작업 항목에서 [!UICONTROL 완료] 단추를 클릭하면 해당 항목의 상태가 [!UICONTROL 완료]&#x200B;(작업의 경우) 또는 [!UICONTROL 해결됨]&#x200B;(문제의 경우)으로 변경됩니다.

[!DNL Adobe Workfront] 관리자는 [!UICONTROL 완료] 단추와 연결된 상태를 사용자 지정하고 이러한 사용자 지정을 홈 팀에 적용할 수 있습니다.

[!UICONTROL 완료] 단추와 연결된 상태 수 또는 작업 또는 문제에 할당된 리소스 수에 따라 [!UICONTROL 완료] 단추의 모양이 변경될 수 있습니다.

* [하나의 상태와 연결된 [!UICONTROL 완료] 단추](#done-button-associated-with-one-status)
* [여러 상태와 연결된 [!UICONTROL 완료] 단추](#done-button-associated-with-multiple-statuses)
* [여러 리소스에 할당된 항목에 대한 [!UICONTROL 완료] 단추](#done-button-for-items-assigned-to-multiple-resources)

### 하나의 상태와 연결된 [!UICONTROL 완료] 단추

[!UICONTROL 완료] 단추가 하나의 상태와 연결되어 있고 작업 항목만 사용자에게 할당되어 있으면 단추는 **[!UICONTROL 완료]**&#x200B;입니다. 클릭하면 작업 또는 문제의 상태가 [!UICONTROL 완료] 단추와 연결된 상태로 변경됩니다.

![완료 단추](assets/done-button-status.png)

[!UICONTROL 완료] 단추와 관련된 상태를 이해하려면 [!UICONTROL 팀 설정 편집]에 설명된 대로 홈 팀의 [!UICONTROL 팀 설정]에서 [완료 단추](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md) 섹션을 확인하십시오.

홈 팀에 할당되지 않은 경우 [!UICONTROL 완료] 단추의 옵션 이해[에서 설명한 대로 [!UICONTROL 완료]를 클릭하면 기본 상태가 선택됩니다.](#understand-the-options-of-the-done-button)

### 여러 상태와 연결된 [!UICONTROL 완료] 단추

[!UICONTROL 완료] 단추가 둘 이상의 상태와 연결되어 있으면 단추에 **[!UICONTROL 완료]**&#x200B;라는 단어가 표시되고 그 뒤에 드롭다운 메뉴가 나타납니다. 이 시나리오에서는 [!UICONTROL 완료]를 클릭할 수 없습니다. 드롭다운 메뉴에서 상태를 선택해야 합니다. 작업 항목 완료에 가장 적합한 상태를 선택합니다. 이렇게 하면 작업 항목의 상태가 변경됩니다.

여러 상태를 [!UICONTROL 완료] 단추와 연결하는 방법은 [작업에 대한 [!UICONTROL 완료] 단추 구성](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) 및 [문제에 대한 [!UICONTROL 완료] 단추 구성](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)을 참조하세요.

### 여러 리소스에 할당된 항목에 대한 [!UICONTROL 완료] 단추

작업 또는 문제가 둘 이상의 리소스에 할당되면 버튼에 **[!UICONTROL 완료]**&#x200B;라는 단어가 표시되며 그 뒤에는 드롭다운 메뉴가 표시됩니다. 드롭다운 메뉴에서 **[!UICONTROL 내 파트 완료]**(작업의 일부 완료됨) 또는 [!UICONTROL 완료] 버튼(항목 완료)과 관련된 상태 중 하나를 선택할 수 있습니다. **[!UICONTROL 내 파트로 완료]**&#x200B;를 선택하면 작업 항목이 작업 목록에서 제거되지만 작업 항목에 할당된 작업 목록에는 남아 있습니다.\
완료 단추가 여러 상태와 연결되어 있으면 **내 부분으로 완료** 아래에 나열됩니다.

>[!NOTE]
>
>여러 명의 할당자가 있는 작업 또는 문제에서 각 사용자는 작업 또는 문제에 대한 자신의 할당이 실제로 완료되었음을 표시할 책임이 있습니다. 따라서 각 할당자는 [!UICONTROL 완료]를 클릭하여 항목에서 할당된 작업을 완료했음을 표시해야 합니다.

![내 파트 완료](assets/done-with-my-part.png)

