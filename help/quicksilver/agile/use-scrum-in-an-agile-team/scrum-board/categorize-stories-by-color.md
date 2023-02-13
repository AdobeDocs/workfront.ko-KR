---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드의 색상별로 이야기를 분류합니다
description: Screm 보드 스토리의 기본 색상 연결은 스토리 보드가 반복 또는 프로젝트에 있는지 여부에 따라 다릅니다.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 이야기를 색상에 따라 분류합니다 [!UICONTROL 스크럼] 보드

## 스토리의 기본 색상 연결 변경

스토리의 기본 색상 연결은 스토리 보드가 반복 또는 프로젝트에 있는지 여부에 따라 다릅니다.

* **[!UICONTROL 반복]**: 반복 시 스토리 보드 타일은 스토리가 연결된 프로젝트에 따라 색상으로 구분됩니다. 각 프로젝트에는 스토리 보드에 색상이 임의로 할당됩니다. 각 애자일 팀에 대해 이 기본 동작을 변경할 수 있습니다. 반복 시 애자일 스토리의 색상은 프로젝트(기본값), 스토리 우선 순위, 소유자 또는 자유 양식에 연결할 수 있습니다. 자세한 내용은 [애자일 스토리 보드의 이야기에 색상 표시기가 사용되는 방식을 구성합니다](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) 기사 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL 프로젝트]**: 프로젝트에서, 모든 하위 작업은 상위 작업의 색상과 일치하므로 지정된 모든 수영장에 있는 모든 스토리의 색상이 동일합니다. 작업에 하위 작업이 없거나 상위 작업이 없는 경우 색상이 작업을 만들 때 작업에 임의로 할당됩니다. 애자일 보기를 수정하여 이 기본 동작을 변경할 수 있습니다. 프로젝트에 있는 애자일 스토리의 색상은 상위 스토리(기본값), 스토리 우선 순위, 소유자 또는 자유 양식에 연결할 수 있습니다. 자세한 내용은 [만들기 또는 사용자 지정 [!UICONTROL 애자일] 보기](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [의 보기 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 자유 양식을 사용할 때 스토리 색상 변경

애자일 팀 설정이 [!UICONTROL 카드 색상 연결] 옵션이 [!UICONTROL 자유 형식]에서는 개별 스토리 타일의 색상을 수동으로 변경할 수 있습니다. 이 기능은 팀이나 조직에 중요한 다른 유형의 정보를 전달하는 데 유용합니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]** 특정 이터레이션을 선택하려면 **[!UICONTROL 현재 반복]**.
1. 스토리 타일 위에 있는 컬러 배너를 마우스로 가리킵니다.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. 클릭 **[!UICONTROL 색상 변경]**&#x200B;을 선택한 다음 원하는 색상을 선택합니다.

   ![](assets/agile-story-color2-nwe-350x138.png)
