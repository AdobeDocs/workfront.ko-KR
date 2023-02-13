---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: 문제에 대한 완료 단추 구성
description: 완료 단추는 작업이나 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로 Adobe Workfront은 할당자가 작업 항목에서 완료 를 클릭하면 문제를 해결됨으로 표시합니다.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 1%

---

# 구성 [!UICONTROL 완료] 문제에 대한 단추

다음 [!UICONTROL 완료] 버튼은 작업 또는 문제의 상태를 자동으로 설정할 수 있습니다. 기본적으로 [!DNL Adobe Workfront] 은 문제를 [!UICONTROL 해결됨] 할당자가 클릭하는 경우 [!UICONTROL 완료] 작업 항목에 대한 정보를 제공합니다.

## 개요

특정 권한이 있는 사용자는 [!UICONTROL 완료] 시스템에 있는 특정 상태를 반영하도록 하는 단추입니다. 다음과 같은 세 가지 방법이 있습니다 [!UICONTROL 완료] 버튼이 의 문제에 대해 작동합니다. [!DNL Workfront]:

* 사용자에게 할당된 경우 [!UICONTROL 홈 팀], [!DNL Workfront] 관리자 또는 [!UICONTROL 계획] 라이센스는 [!UICONTROL 완료] 팀 구성원의 특정 상태를 반영하기 위한 단추입니다. 자세한 내용은 [구성 [!UICONTROL 완료] 팀 단추](#configure-the-uicontrol-done-button-for-a-team) 참조하십시오.
* 사용자에게 [!UICONTROL 홈 팀] 지정됨, [!UICONTROL 완료] 문제가 발생하면 시스템이 생성한 버튼에 연결됩니다 [!UICONTROL 해결됨] 세 문자 코드가 있는 상태 [!UICONTROL RLV]. 이 시나리오에는 사용 가능한 구성 옵션이 없습니다. 다음 [!UICONTROL 완료] 버튼은 자동으로 이 상태로 설정됩니다.
* 만약 [!UICONTROL 해결됨] ([!UICONTROL RLV]) 상태가 삭제되고 사용자가 문제를 로 표시합니다 [!UICONTROL 완료] 아니요 [!UICONTROL 홈 팀]로 설정되어 있는 경우, 기본 문제 상태는 가 기본값으로 설정된 항목에 연결되어 있습니다. [!UICONTROL 닫힘] 문제가 속한 프로젝트에 지정된 그룹에 대해, Workfront 관리자는 그룹에 대한 시스템 차원의 기본 설정을 구성할 수 있습니다. 자세한 내용은 [구성 [!UICONTROL 완료] 단추 사용 시 [!UICONTROL 해결됨] 상태가 삭제됨](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) 참조하십시오.

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
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td>[!UICONTROL Resolved] 상태가 삭제될 때 [!UICONTROL Done] 단추를 구성하려면 시스템 관리자 액세스 권한이 필요합니다</td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

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
   >  예를 들어 [!UICONTROL 완료] 진행 중인 단추가 있으면 작업 항목이 [!UICONTROL 완료] 상태를 새로 작성에서 진행 중으로 변경하는 사용자용.
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
연결된 상태를 포함한 모든 팀 설정 [!UICONTROL 완료] 이제 이러한 사용자가 버튼을 사용할 수 있습니다.

## 구성 [!UICONTROL 완료] 단추 사용 시 [!UICONTROL 해결됨] 상태가 삭제됨

사용자에게 홈 팀 및 [!UICONTROL 해결됨] ([!UICONTROL RLV])이 삭제되고 [!DNL Workfront] 관리자는 [!UICONTROL 닫힘] 프로젝트에 대한 그룹의 상태입니다. [!DNL Workfront] 사용자가 [!DNL Done] 버튼을 클릭합니다.

### 프로젝트와 연결된 그룹 찾기

사용자가 프로젝트를 만들면 홈 그룹이 프로젝트에 자동으로 할당됩니다. 사용 중인 사용자 [!UICONTROL 관리] 프로젝트에 대한 액세스는 [!UICONTROL 프로젝트 세부 사항] 언제든지 섹션을 참조하십시오. 어떤 상태를 이해하려면 [!DNL Workfront] 이 경우 완료된 문제에 대해 을 사용하는 경우, 문제가 있는 프로젝트와 연관된 그룹 및 [!UICONTROL 닫힘] 이 그룹에 문제가 있습니다.

프로젝트와 연관된 그룹을 찾으려면

1. 프로젝트로 이동합니다.
1. 페이지 왼쪽에서 **[!UICONTROL 프로젝트 세부 사항]**.
1. 을(를) 찾습니다 **[!UICONTROL 프로젝트 연결]** 섹션을 찾은 다음 **[!UICONTROL 그룹]**.\
   설정 영역에서 상태를 확인하는 데 사용해야 하는 그룹 이름입니다. 특정 그룹의 기본 상태를 업데이트하는 방법에 대한 지침은 다음 섹션을 참조하십시오.

### 특정 그룹의 기본 상태 업데이트

로서의 [!UICONTROL Workfront] 관리자는 특정 그룹의 상태를 업데이트할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 왼쪽 패널에서 **[!UICONTROL 프로젝트 환경 설정]**, 그런 다음 **[!UICONTROL 상태]**.

1. 클릭 **[!UICONTROL 문제]**&#x200B;를 입력한 다음 **[!UICONTROL 시스템 상태]** 오른쪽에 있는 검색 상자.

1. 그룹을 선택합니다.
1. 을(를) 클릭합니다. **[!UICONTROL 기본 상태 설정]** 드롭다운 메뉴에서 [!UICONTROL 닫힘]. [!DNL Workfront] 사용자가 [!UICONTROL 완료] 버튼을 클릭합니다.

   >[!IMPORTANT]
   >
   >이 상태는 사용자에게 홈 팀 및 [!UICONTROL RLV] 상태가 삭제되었습니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
