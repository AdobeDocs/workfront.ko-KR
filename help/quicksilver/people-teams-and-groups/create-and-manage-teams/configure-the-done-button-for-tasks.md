---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 작업에 대한 완료 버튼 구성
description: 완료 버튼을 사용하면 작업 또는 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로 Adobe Workfront은 할당자가 작업 항목에서 완료 를 클릭하면 작업을 완료됨으로 표시합니다.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# 구성 [!UICONTROL 완료] 작업 단추

다음 [!UICONTROL 완료] 버튼은 작업 또는 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로, [!UICONTROL Adobe Workfront] 작업을 다음으로 표시 [!UICONTROL 완료됨] 피할당자가 작업 항목에서 완료 를 클릭할 때.

## 개요

특정 권한이 있는 사용자는 [!UICONTROL 완료] 시스템의 특정 상태를 반영하는 버튼. 다음 두 가지 방법으로 [!UICONTROL 완료] 버튼은 의 작업에 대해 작동합니다. [!UICONTROL Workfront]:

* 사용자에게 할당된 홈 팀이 있는 경우 [!DNL Workfront] 관리자 또는 을 가진 사용자 [!UICONTROL 플랜] 라이선스에서 다음을 구성할 수 있습니다. [!UICONTROL 완료] 단추를 클릭하여 팀 구성원의 특정 상태를 반영합니다. 다음을 참조하십시오 [구성 [!UICONTROL 완료] 팀용 단추](#configure-the-uicontrol-done-button-for-a-team) 이 문서에서.
* 사용자에게 다음이 없는 경우 [!UICONTROL 홈 팀], 하지만 [!UICONTROL 다른 팀] Workfront은 프로필에서 [!UICONTROL 완료] 사용자와 연결된 모든 팀의 단추입니다. 선택은 임의이며 팀과 연관된 상태가 작업에 사용됩니다.
* 사용자에게 할당된 홈 팀이 없는 경우 [!UICONTROL 완료] 작업 버튼은 완료 상태에 연결되어 있습니다. 이 시나리오에는 사용 가능한 구성 옵션이 없습니다. 다음 [!UICONTROL 완료] 버튼의 기본값은 자동으로 이 상태로 설정됩니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] 플랜*</strong></p></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] 라이센스*</strong></p></td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜 또는 라이선스 유형을 확인하려면 다음으로 문의하십시오. [!DNL Workfront] 관리자.

## 구성 [!UICONTROL 완료] 팀용 단추

을 사용하여 작업 항목에 적용되는 상태를 변경할 수 있습니다. [!UICONTROL 완료] 단추를 클릭합니다. 여러 상태를 설정하고 사용자가 적절한 상태를 선택할 수도 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 팀]**.

1. 다음을 클릭합니다. **[!UICONTROL 팀 전환]** 아이콘을 클릭한 다음 드롭다운 메뉴에서 새 팀을 선택하거나 검색 막대에서 팀을 검색합니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴를 선택한 다음 **[!UICONTROL 편집]**.
1. 다음 찾기 **[!UICONTROL 완료 단추]** 의 맨 아래에 있는 섹션 **[!UICONTROL 팀 설정]** 페이지를 가리키도록 업데이트하는 중입니다.

1. 각 작업 항목 유형에 대해 하나 이상의 상태를 선택하거나 상태를 선택합니다.

   >[!NOTE]
   >
   >작업 또는 문제의 상태를 선택할 때는 다음 사항을 고려하십시오.
   >
   >* 각 작업 항목 유형에 대해 하나의 상태를 선택하면 사용자가 클릭하면 작업 또는 문제 상태가 해당 상태로 설정됩니다 [!UICONTROL 완료] 항목에서 참조할 수 있습니다. 각 작업 항목 유형에 대해 여러 상태를 설정하면 드롭다운 메뉴가 [!UICONTROL 완료] 버튼을 클릭하고 작업 항목의 상태를 변경하려면 상태를 선택해야 합니다.
   >* 시스템 레벨 상태만 과 연결할 수 있습니다. [!UICONTROL 완료] 단추를 클릭합니다. 그룹별 상태를 작업 항목 상태와 연결할 수 없습니다.
   >* 항목에 할당된 사용자가 항목을 와(과) 연결된 상태에 배치할 때 [!UICONTROL 완료] 버튼, 항목이 로 표시됩니다. [!UICONTROL 완료] 선택한 상태가 [!UICONTROL 완료됨] 또는 [!UICONTROL 종료됨] 상태 또는 작업 상태입니다.
   >   
   >   
   >  예를 들어 [!UICONTROL 완료] 단추 포함 [!UICONTROL 진행 중] 작업 항목을 다음으로 표시 [!UICONTROL 완료] 에서 상태를 변경하는 사용자용 [!UICONTROL 신규] 끝 [!UICONTROL 진행 중].
   >   
   >* 문제 유형은 사용자 정의할 수 있으며 사용자 환경에 아래에 나열된 것과 다른 이름을 가질 수 있습니다.\
   >  다음은 기본 작업 및 문제 유형입니다.
   >     
   >   * [!UICONTROL 작업]
   >   * [!UICONTROL 문제]
   >   * [!UICONTROL 요청]
   >   * [!UICONTROL 순서 변경]
   >   * [!UICONTROL 버그 신고]

   작업 또는 문제가 여러 사용자에게 할당되면 &quot;[!UICONTROL 내 부분 완료]팀에 대해 선택된 여러 상태 외에 드롭다운 메뉴의 &quot;옵션.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.

## 홈 팀과 사용자 연결

을 변경하려면 [!UICONTROL 완료] 버튼 기능을 사용자에게 표시하면 설정을 변경한 팀을 사용자의 홈 팀으로 만들 수 있습니다.

사용자를 홈 팀과 연결하려면 다음 작업을 수행하십시오.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront].

1. 클릭 **[!UICONTROL 사용자]**&#x200B;을 선택한 다음 홈 팀과 연결할 사용자를 선택합니다.
1. 다음을 클릭합니다. **[!UICONTROL 자세히]** 메뉴, 선택 **[!UICONTROL 편집]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. 다음에서 **[!UICONTROL 조직]** 섹션에서 **[!UICONTROL 홈 팀]** 필드. 설정을 사용자와 연결할 팀의 이름을 입력하십시오. 목록에 팀의 이름이 표시되면 클릭합니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.\
   선택한 사용자가 이제 홈 팀과 연결되었습니다.
모든 팀 설정(예: 와 연관된 상태) [!UICONTROL 완료] 이제 이러한 사용자가 단추를 볼 수 있습니다.
