---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 처리 중 단추를 시작 단추로 바꾸기
description: Adobe Workfront의 기본 구성에는 할당된 항목에 대해 표시되는 작업 및 문제에 대한 처리 중 버튼이 포함되어 있습니다.
author: Jenny
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# [!UICONTROL 처리 중] 단추를 [!UICONTROL 시작] 단추로 바꾸기

[!DNL Adobe Workfront]의 기본 구성에는 할당된 항목에 대해 표시되는 작업 및 문제에 대한 [!UICONTROL 처리 중] 단추가 포함되어 있습니다. 할당된 항목에서 [!UICONTROL 작업]을 클릭하면 작업을 받았음을 다른 사용자에게 알리고 작업을 수행할 것임을 확인합니다. 그러나 [!DNL Work On It] 단추는 작업이 실제로 시작되었음을 알리는 작업 또는 문제 상태를 업데이트하지 않습니다.

[!DNL Work On It] 단추를 소속 팀의 [!UICONTROL 시작] 단추로 바꿀 수 있습니다. 이 경우 [!UICONTROL 처리 중] 대신 [!UICONTROL 시작] 단추를 클릭하면 상태 및 작업 항목의 [!UICONTROL 실제 시작 날짜]가 자동으로 업데이트되어 작업을 시작했음을 나타냅니다. [!UICONTROL 처리 중] 단추의 변경 내용에 영향을 줄 수 있는 팀의 설정에 대한 자세한 내용은 이 문서의 [[!UICONTROL 시작] 단추 구성](#configure-the-uicontrol-start-button) 섹션을 참조하십시오.

>[!IMPORTANT]
>
>[!UICONTROL 시작] 단추를 클릭하면 항목의 상태와 [!UICONTROL 실제 시작 날짜]가 변경됩니다. 다른 사용자가 작업 또는 문제에 대한 작업을 시작한 경우(상태를 [!UICONTROL 진행 중]&#x200B;(으)로 변경하고 [!UICONTROL 실제 시작 일자]를 채운 경우), 사용자가 속한 팀이 [!UICONTROL 시작] 단추로 단추를 교체한 경우에도 항목의 단추가 [!UICONTROL 처리 중]으로 표시됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 패키지</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!UICONTROL 시작] 단추 구성

[!UICONTROL 플랜] 라이선스가 있는 경우 [!UICONTROL 편집] 팀 창에서 팀에 대한 [!UICONTROL 시작] 단추를 구성할 수 있습니다. 다음은 팀에 대해 버튼이 활성화된 후 작동하는 방식입니다.

* **팀이 작업 항목에 할당되었습니다**: 팀이 작업 항목에 할당되면 해당 팀의 구성원은 [!UICONTROL 시작] 단추와 해당 팀에 대해 구성된 상태를 볼 수 있습니다.
* **사용자가 홈 팀에 속함**: 작업 항목에 할당된 팀이 없지만 사용자의 프로필에서 홈 팀에 할당된 경우 [!UICONTROL 시작] 단추와 해당 팀에 대해 구성된 상태가 표시됩니다. 사용자가 [!UICONTROL 시작] 단추를 자주 사용하려는 경우 권장되는 시나리오입니다.
* **사용자가 작업 항목에 할당됨**: 작업 항목에 할당된 팀이 없고 홈 팀이 없지만 사용자가 작업 항목에 할당되면 [!UICONTROL 시작] 단추와 할당된 모든 팀에 대해 구성된 결합된 상태가 표시됩니다.
* **사용자가 팀에 할당되지 않았습니다.** 작업 항목에 할당된 팀이 없고 홈 팀을 포함하여 사용자에 대한 팀이 없는 경우 항목이 사용자에게 할당되면 사용자는 [!UICONTROL 작업 중] 단추로 보입니다.

>[!NOTE]
>
>이 기능은에서 현재 사용할 수 없습니다.
>
>* [!DNL Workfront] 모바일 앱
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront]개의 전자 메일 알림
>

시작 단추를 구성하려면 다음 작업을 수행하십시오.

{{step1-to-team}}

1. **[!UICONTROL 팀]** 드롭다운 메뉴에서 팀을 선택합니다.\
   또는\
   **[!UICONTROL 새 팀 만들기]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 자세히]** 아이콘 ![](assets/more-icon.png)을 클릭한 다음 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 팀 편집]** 페이지 아래쪽에서 [!UICONTROL 작업] 단추 섹션을 찾습니다.
1. **[!UICONTROL 처리 중 단추를 시작 단추로 변경하여 항목의 상태를 자동으로 업데이트]** 확인란을 선택하십시오.
1. 각 작업 항목 유형에 대해 하나 이상의 상태를 선택합니다. 두 개 이상의 상태를 선택하면 [!UICONTROL 시작]을 클릭하면 원하는 상태를 선택할 수 있는 드롭다운 메뉴가 나타납니다.
1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다. 이제 사용자에게 작업 항목이 할당되면 [!UICONTROL 작업 시작] 또는 [!UICONTROL 처리 중] 단추 대신 [!UICONTROL 문제 시작] 단추가 표시됩니다.

   >[!NOTE]
   >
   >할당된 모든 작업 항목에 시작 단추가 표시되도록 팀을 사용자의 홈 팀으로 설정하는 것이 좋습니다. 아래의 [사용자를 홈 팀과 연결](#associate-users-with-a-home-team)을 참조하세요.

## 홈 팀과 사용자 연결

사용자를 홈 팀과 연결하려면 다음 작업을 수행하십시오.

{{step-1-to-users}}

1. 홈 팀과 연결할 사용자를 선택합니다.
1. **[!UICONTROL 자세히]** 메뉴를 클릭한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.\
   ![](assets/user-settings-nwe-350x291.png)

1. **[!UICONTROL 조직]** 섹션에서 **[!UICONTROL 홈 팀]** 필드를 선택합니다. 설정을 사용자와 연결할 팀의 이름을 입력하십시오. 목록에 팀의 이름이 표시되면 클릭합니다.

1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.\
   선택한 사용자가 이제 홈 팀과 연결되었습니다.

   이제 [!UICONTROL 완료] 단추와 연결된 상태를 포함한 모든 팀 설정이 이 사용자에게 표시됩니다.

