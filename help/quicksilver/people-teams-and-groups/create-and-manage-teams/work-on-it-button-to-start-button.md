---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Work On It 단추를 시작 단추로 바꿉니다.
description: Adobe Workfront의 기본 구성에는 할당된 항목에 대해 표시되는 작업 및 문제에 대한 IT 작업 단추가 포함되어 있습니다.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 바꾸기 [!UICONTROL 작업] 버튼 [!UICONTROL 시작] 버튼

[!DNL Adobe Workfront]의 기본 구성에는 다음이 포함됩니다 [!UICONTROL 작업] 지정된 항목에 대해 표시되는 작업 및 문제에 대한 단추입니다. 를 클릭하면 [!UICONTROL 작업] 자신에게 할당된 항목에서는 작업을 받은 다른 사용자에게 신호를 보내고 해당 작업을 수행할 것임을 확인합니다. 하지만, [!DNL Work On It] 버튼은 작업이 실제로 시작되었음을 알리는 작업 또는 문제 상태를 업데이트하지 않습니다.

을 대체할 수 있습니다 [!DNL Work On It] 버튼 [!UICONTROL 시작] 사용자가 속한 팀의 단추입니다. 이 경우 [!UICONTROL 시작] 버튼 대신 [!UICONTROL 작업]를 업데이트하면 상태와 [!UICONTROL 실제 시작 날짜] 작업을 시작했음을 나타내는 작업 항목 의 변경 사항에 영향을 줄 수 있는 팀의 설정에 대한 자세한 내용은 [!UICONTROL 작업] 버튼을 클릭하고 섹션을 참조하십시오 [구성 [!UICONTROL 시작] 버튼](#configure-the-uicontrol-start-button) 참조하십시오.

>[!IMPORTANT]
>
>클릭 [!UICONTROL 시작] 버튼은 항목의 상태를 변경하고 [!UICONTROL 실제 시작 날짜]. 다른 사람이 작업이나 문제 작업을 시작한 경우(작업 상태가 [!UICONTROL 진행 중] 그리고 [!UICONTROL 실제 시작 날짜]), 항목의 버튼이 로 표시됩니다. [!UICONTROL 작업] 사용자가 속한 팀이 단추를 [!UICONTROL 시작] 버튼을 클릭합니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>플랜</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 구성 [!UICONTROL 시작] 버튼

만약 [!UICONTROL 계획] 라이센스, 구성 [!UICONTROL 시작] 의 팀 버튼 [!UICONTROL 편집] 팀 창 다음은 팀에 대해 활성화된 버튼이 작동하는 방식입니다.

* **팀이 작업 항목에 할당되었습니다**: 팀이 작업 항목에 지정되면 해당 팀의 구성원이 [!UICONTROL 시작] 버튼과 해당 팀에 대해 구성된 상태
* **사용자가 홈 팀에 속합니다.**: 작업 항목에 지정된 팀이 없지만 사용자가 프로필에서 홈 팀에 할당되면 사용자는 [!UICONTROL 시작] 버튼과 해당 팀에 대해 구성된 상태 사용자가 다음을 사용하도록 하려는 경우 권장되는 시나리오입니다 [!UICONTROL 시작] 자주 사용합니다.
* **사용자가 작업 항목에 할당됨**: 작업 항목에 지정된 팀이 없고 사용자에게 할당된 홈 팀이 없지만 사용자가 작업 항목에 지정되면 사용자는 [!UICONTROL 시작] 버튼과 해당 팀이 지정된 모든 팀에 대해 구성된 결합 상태.
* **사용자가 팀에 할당되지 않았습니다.** 작업 항목에 지정된 팀이 없고 홈 팀을 포함하여 사용자의 팀이 없는 경우 해당 항목이 사용자에게 할당되면 사용자는 [!UICONTROL 작업] 버튼을 클릭합니다.

>[!NOTE]
>
>이 기능은 현재
>
>* 다음 [!DNL Workfront] 모바일 앱
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] 이메일 알림
>


시작 단추를 구성하려면:

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 팀]**.

1. 에서 **[!UICONTROL 팀]** 드롭다운 메뉴에서 팀을 선택합니다.\
   또는\
   클릭 **[!UICONTROL 팀 만들기]**.

1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 아이콘 ![](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL 편집]**.

1. 를 찾습니다. **[!UICONTROL 작업]** 단추 섹션 [!UICONTROL 팀 편집] 페이지.
1. 을(를) 선택합니다 **[!UICONTROL 항목의 상태를 자동으로 갱신하려면 Work On It 버튼을 시작 단추로 변경합니다]** 확인란을 선택합니다.
1. 각 작업 항목 유형에 대해 하나 이상의 상태를 선택합니다. 두 개 이상의 상태를 선택하면 [!UICONTROL 시작] 여기서 원하는 상태를 선택할 수 있습니다.
1. 클릭 **[!UICONTROL 변경 내용 저장]**. 이제 사용자에게 [!UICONTROL 작업 시작] 또는 [!UICONTROL 시작 문제] 버튼 대신 [!UICONTROL 작업] 작업 항목이 지정되면 버튼을 클릭합니다.

   >[!NOTE]
   >
   >지정된 모든 작업 항목에 시작 단추가 표시되도록 팀을 사용자의 홈 팀으로 설정하는 것이 좋습니다. 자세한 내용은 [홈 팀과 사용자 연결](#associate-users-with-a-home-team) 아래의 제품에서 사용할 수 있습니다.

## 홈 팀과 사용자 연결

사용자를 홈 팀과 연결하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront].

1. 클릭 **[!UICONTROL 사용자]**&#x200B;를 선택한 다음 홈 팀과 연결할 사용자 또는 사용자를 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 에서 **[!UICONTROL 조직]** 섹션에서 **[!UICONTROL 홈 팀]** 필드. 사용자와 연결할 설정의 팀 이름을 입력하기 시작합니다. 목록에 팀 이름이 표시되면 이름을 클릭합니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.\
   선택한 사용자가 이제 홈 팀과 연결됩니다.

   연결된 상태를 포함한 모든 팀 설정 [!UICONTROL 완료] 이제 이러한 사용자가 버튼을 볼 수 있습니다.

