---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 작업에 대한 완료 단추 구성
description: 완료 단추는 작업이나 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로 Adobe Workfront은 할당자가 작업 항목에서 완료 를 클릭하면 작업을 완료됨으로 표시합니다.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# 구성 [!UICONTROL 완료] 작업의 단추

다음 [!UICONTROL 완료] 버튼은 작업 또는 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로 [!UICONTROL Adobe Workfront] 작업을 로 표시 [!UICONTROL 완료됨] 할당자가 작업 항목에 대해 완료 를 클릭하는 경우.

## 개요

특정 권한이 있는 사용자는 [!UICONTROL 완료] 시스템에 있는 특정 상태를 반영하도록 하는 단추입니다. 두 가지 방법으로 [!UICONTROL 완료] 버튼은 의 작업에 작동합니다. [!UICONTROL Workfront]:

* 사용자에게 홈 팀이 할당된 경우 [!DNL Workfront] 관리자 또는 [!UICONTROL 계획] 라이센스는 [!UICONTROL 완료] 팀 구성원의 특정 상태를 반영하기 위한 단추입니다. 자세한 내용은 [구성 [!UICONTROL 완료] 팀 단추](#configure-the-uicontrol-done-button-for-a-team) 참조하십시오.
* 사용자에게 홈 팀이 할당되지 않은 경우 [!UICONTROL 완료] 작업에 대한 단추가 완료 상태에 연결되어 있습니다. 이 시나리오에는 사용 가능한 구성 옵션이 없습니다. 다음 [!UICONTROL 완료] 버튼은 자동으로 이 상태로 설정됩니다.

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
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜 또는 라이선스 유형을 확인하려면 [!DNL Workfront] 관리자

## 구성 [!UICONTROL 완료] 팀 단추

작업 항목에 적용되는 상태를 [!UICONTROL 완료] 버튼을 클릭합니다. 여러 상태를 설정하고 사용자가 적절한 상태를 선택할 수도 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 팀]**.

1. 을(를) 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 클릭한 다음 **[!UICONTROL 편집]**.
1. 를 찾습니다. **[!UICONTROL 완료 단추]** 섹션 아래쪽에서 **[!UICONTROL 팀 설정]** 페이지.

1. 각 작업 항목 유형에 대해 상태를 하나 이상 선택합니다.

   >[!NOTE]
   >
   >작업 또는 문제에 대한 상태를 선택할 때는 다음 사항을 고려하십시오.
   >
   >* 각 작업 항목 유형에 대해 하나의 상태를 선택하면, 사용자가 클릭하면 작업이나 문제 상태가 해당 상태로 설정됩니다 [!UICONTROL 완료] 해당 항목이 없습니다. 각 작업 항목 유형에 대해 여러 상태를 설정하면 드롭다운 메뉴가 [!UICONTROL 완료] 버튼을 누르면 사용자가 상태를 선택하여 작업 항목의 상태를 변경해야 합니다.
   >* 시스템 수준 상태만 [!UICONTROL 완료] 버튼을 클릭합니다. 그룹별 상태를 작업 항목 상태와 연결할 수 없습니다.
   >* 항목에 지정된 사용자가 해당 항목과 연관된 상태에 항목을 놓으면 [!UICONTROL 완료] 버튼, 항목이 [!UICONTROL 완료] 선택한 상태가 [!UICONTROL 완료됨] 또는 [!UICONTROL 닫힘] 상태 또는 작업 상태입니다.

   >   
   >   
   >  예를 들어 [!UICONTROL 완료] 버튼 [!UICONTROL 진행 중] 작업 항목이 [!UICONTROL 완료] 상태를 변경한 사용자의 경우 [!UICONTROL 새로 만들기] to [!UICONTROL 진행 중].
   >   
   >* 문제 유형은 사용자 지정할 수 있으며 환경에 아래 나열된 이름과 다른 이름을 가질 수 있습니다.\
      >  다음은 기본 작업 및 문제 유형입니다.
      >     
      >   * [!UICONTROL 작업]
      >   * [!UICONTROL 문제]
      >   * [!UICONTROL 요청]
      >   * [!UICONTROL 순서 변경]
      >   * [!UICONTROL 버그 신고]


   작업 또는 문제가 여러 사용자에게 할당된 경우 &quot;[!UICONTROL 내 몫으로 끝남]팀에 대해 선택한 여러 상태 외에 드롭다운 메뉴의 &quot;옵션&quot;을 사용하십시오.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 홈 팀과 사용자 연결

을 변경하려면 [!UICONTROL 완료] 사용자가 단추 기능을 볼 수 있도록 설정하면 사용자의 홈 팀을 변경한 팀을 만들 수 있습니다.

사용자를 홈 팀과 연결하려면

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront].

1. 클릭 **[!UICONTROL 사용자]**&#x200B;를 선택한 다음 홈 팀과 연결할 사용자 또는 사용자를 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 에서 **[!UICONTROL 조직]** 섹션에서 **[!UICONTROL 홈 팀]** 필드. 사용자와 연결할 설정의 팀 이름을 입력하기 시작합니다. 목록에 팀 이름이 표시되면 이름을 클릭합니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.\
   선택한 사용자가 이제 홈 팀과 연결됩니다.
연결된 상태를 포함한 모든 팀 설정 [!UICONTROL 완료] 이제 이러한 사용자가 버튼을 볼 수 있습니다.
