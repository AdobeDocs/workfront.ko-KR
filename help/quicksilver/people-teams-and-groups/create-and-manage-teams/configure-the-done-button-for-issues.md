---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 문제에 대한 완료 버튼 구성
description: 완료 버튼을 사용하면 작업 또는 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로 Adobe Workfront은 할당자가 작업 항목에서 완료 를 클릭하면 문제를 해결됨으로 표시합니다.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 3793f68faf2ec0a8050f8f0c6e06a32579b43879
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 1%

---

# 구성 [!UICONTROL 완료] 문제 버튼

다음 [!UICONTROL 완료] 버튼은 작업 또는 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로, [!DNL Adobe Workfront] 문제를 다음으로 표시 [!UICONTROL 해결됨] 피할당자가 클릭할 때 [!UICONTROL 완료] 작업 항목에서.

## 개요

특정 권한이 있는 사용자는 [!UICONTROL 완료] 시스템의 특정 상태를 반영하는 버튼. 다음과 같은 세 가지 방법이 있습니다. [!UICONTROL 완료] 버튼은 의 문제에 대해 작동합니다. [!DNL Workfront]:

* 사용자에게 할당된 이(가) 있는 경우 [!UICONTROL 홈 팀], a [!DNL Workfront] 관리자 또는 을 가진 사용자 [!UICONTROL 플랜] 라이선스에서 다음을 구성할 수 있습니다. [!UICONTROL 완료] 단추를 클릭하여 팀 구성원의 특정 상태를 반영합니다. 다음을 참조하십시오 [구성 [!UICONTROL 완료] 팀용 단추](#configure-the-uicontrol-done-button-for-a-team) 이 문서에서.
* 사용자에게 다음이 없는 경우 [!UICONTROL 홈 팀], 하지만[!UICONTROL 다른 팀] Workfront은 프로필에서 [!UICONTROL 완료] 사용자와 연결된 모든 팀의 단추입니다. 선택은 임의이며 팀과 연결된 상태가 문제에 사용됩니다.
* 사용자에게 다음이 없는 경우 [!UICONTROL 홈 팀] 할당됨, [!UICONTROL 완료] 문제 버튼은 시스템 생성 버튼과 연결되어 있습니다 [!UICONTROL 해결됨] 세 글자로 된 코드가 있는 상태 [!UICONTROL RLV]. 이 시나리오에는 사용 가능한 구성 옵션이 없습니다. 다음 [!UICONTROL 완료] 버튼의 기본값은 자동으로 이 상태로 설정됩니다.
* 다음과 같은 경우 [!UICONTROL 해결됨] ([!UICONTROL RLV]) 상태가 삭제되고 사용자가 문제를 다음으로 표시 [!UICONTROL 완료] 없음 [!UICONTROL 홈 팀], 기본 문제 상태는 기본값으로 설정된 모든 항목에 연결되어 있습니다. [!UICONTROL 종료됨] 이 문제가 속한 프로젝트에 할당된 그룹의 경우. Workfront 관리자는 그룹에 대한 시스템 전체 기본 설정을 구성할 수 있습니다. 다음을 참조하십시오 [구성 [!UICONTROL 완료] 단추를 클릭합니다. [!UICONTROL 해결됨] 상태가 삭제되었습니다.](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) 이 문서에서.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td>[!UICONTROL Resolved] 상태가 삭제될 때 [!UICONTROL Done] 단추를 구성하려면 시스템 관리자 액세스 권한이 필요합니다</td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

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
   >  예를 들어 [!UICONTROL 완료] [진행 중]이 있는 단추를 누르면 작업 항목이 다음으로 표시됩니다. [!UICONTROL 완료] (새로 만들기에서 진행 중으로 상태를 변경하는 사용자).
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
모든 팀 설정(예: 와 연관된 상태) [!UICONTROL 완료] 이제 이러한 사용자가 단추 를 볼 수 있습니다.

## 구성 [!UICONTROL 완료] 단추를 클릭합니다. [!UICONTROL 해결됨] 상태가 삭제되었습니다.

사용자에게 홈 팀이 없고 의 시스템 전체 기본값이 [!UICONTROL 해결됨] ([!UICONTROL RLV])이(가) 삭제되었습니다. [!DNL Workfront] 관리자가 다음을 구성할 수 있습니다. [!UICONTROL 종료됨] 프로젝트에 대한 그룹의 상태입니다. [!DNL Workfront] 사용자가 을(를) 클릭할 때 종료된 문제에 대해 이 상태를 선택합니다. [!DNL Done] 단추를 클릭합니다.

### 프로젝트와 연계된 그룹 찾기

사용자가 프로젝트를 만들 때 홈 그룹이 프로젝트에 자동으로 할당됩니다. 을 사용하는 사용자 [!UICONTROL 관리] 프로젝트에 대한 액세스 권한으로 [!UICONTROL 프로젝트 세부 정보] 언제든지 섹션을 볼 수 있습니다. 상태를 이해하려면 [!DNL Workfront] 이 경우 완료된 문제에 를 사용합니다. 문제가 있는 프로젝트와 연결된 그룹과 기본 상태를 이해해야 합니다. [!UICONTROL 종료됨] 이 그룹에는 문제가 있습니다.

프로젝트와 연계된 그룹을 찾으려면 다음을 수행합니다.

1. 프로젝트로 이동합니다.
1. 페이지 왼쪽에서 **[!UICONTROL 프로젝트 세부 정보]**.
1. 를 찾습니다. **[!UICONTROL 프로젝트 연결]** 섹션, 찾기 **[!UICONTROL 그룹]**.\
   설정 영역에서 상태를 확인하는 데 사용해야 하는 그룹 이름입니다. 특정 그룹의 기본 상태를 업데이트하는 방법에 대한 지침은 다음 섹션을 참조하십시오.

### 특정 그룹에 대한 기본 상태 업데이트

로서의 [!UICONTROL Workfront] 관리자는 특정 그룹의 상태를 업데이트할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 패널에서 **[!UICONTROL 프로젝트 환경 설정]**, 그런 다음 **[!UICONTROL 상태]**.

1. 클릭 **[!UICONTROL 문제]**&#x200B;을(를) 클릭한 다음, **[!UICONTROL 시스템 상태]** 오른쪽에 있는 검색 상자.

1. 그룹을 선택합니다.
1. 다음을 클릭합니다. **[!UICONTROL 기본 상태 설정]** 드롭다운 메뉴를 선택한 다음 의 기본 상태를 선택합니다. [!UICONTROL 종료됨]. [!DNL Workfront] 사용자가 을(를) 클릭할 때 닫힌 문제에 대해 이 상태를 사용합니다. [!UICONTROL 완료] 단추를 클릭합니다.

   >[!IMPORTANT]
   >
   >이 상태는 사용자에게 할당된 홈 팀과 [!UICONTROL RLV] 상태가 삭제되었습니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
