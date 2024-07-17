---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드에서 색상별로 스토리 분류
description: 스크럼 보드 스토리의 기본 색상 연관성은 스토리 보드가 반복에 위치하는지 프로젝트에 위치하는지에 따라 다릅니다.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# [!UICONTROL 스크럼] 보드에서 색상별로 스토리를 분류합니다.

## 스토리의 기본 색상 연결 변경

스토리 보드의 기본 색상 연관성은 스토리 보드가 반복에 있는지 아니면 프로젝트에 있는지에 따라 다릅니다.

* **[!UICONTROL 반복]**: 반복에서 스토리 보드 타일은 스토리와 연결된 프로젝트에 따라 색상으로 구분됩니다. (각 프로젝트에는 스토리 보드에 임의로 색상이 지정됩니다.) 각 애자일 팀에 대해 이 기본 동작을 변경할 수 있습니다. 반복에서 애자일 스토리의 색상은 프로젝트(기본값), 스토리 우선 순위, 소유자 또는 자유 형식에 연결할 수 있습니다. 자세한 내용은 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md) 문서에서 [애자일 스토리 보드에서 스토리에 색상 표시기가 사용되는 방법 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4)을 참조하십시오.

* **[!UICONTROL 프로젝트]**: 프로젝트에서 모든 하위 작업은 상위 작업의 색상과 일치하므로 주어진 스윔에 있는 모든 스토리의 색상은 동일합니다. 작업에 하위 작업이 없거나 상위 작업이 없는 경우 작업이 생성될 때 색상이 임의로 할당됩니다. 애자일 보기를 수정하여 이 기본 동작을 변경할 수 있습니다. 프로젝트에서 애자일 스토리의 색상은 상위 스토리(기본값), 스토리 우선 순위, 소유자 또는 자유 형식에 연결할 수 있습니다. 자세한 내용은 [다음에서 [애자일 [!UICONTROL 보기 만들기 또는 사용자 지정]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)을(를) 참조하십시오 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 자유 형식 사용 시 스토리 색상 변경

애자일 팀 설정이 구성되어 [!UICONTROL 카드 색상을 ]에 연결 옵션이 [!UICONTROL 자유 형식](으)로 설정된 경우 사용자가 개별 스토리 타일의 색상을 수동으로 변경할 수 있습니다. 이렇게 하면 팀이나 조직에 중요한 다른 유형의 정보를 전달하는 데 유용할 수 있습니다.

1. [!DNL Adobe] Workfront의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. 왼쪽 패널에서 **[!UICONTROL 반복]**&#x200B;을 선택하여 특정 반복을 선택하거나 **[!UICONTROL 현재 반복]**&#x200B;을 선택합니다.
1. 스토리 타일 상단의 컬러 배너 위로 마우스를 가져갑니다.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. **[!UICONTROL 색상 변경]**&#x200B;을 클릭한 다음 원하는 색상을 선택합니다.

   ![](assets/agile-story-color2-nwe-350x138.png)
