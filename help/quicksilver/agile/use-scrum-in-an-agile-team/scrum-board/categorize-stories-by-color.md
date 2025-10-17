---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드에서 색상별로 스토리 분류
description: 스크럼 보드 스토리의 기본 색상 연관성은 스토리 보드가 반복에 위치하는지 프로젝트에 위치하는지에 따라 다릅니다.
author: Jenny
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# [!UICONTROL 스크럼] 보드에서 색상별로 스토리를 분류합니다.

## 스토리의 기본 색상 연결 변경

스토리 보드의 기본 색상 연관성은 스토리 보드가 반복에 있는지 아니면 프로젝트에 있는지에 따라 다릅니다.

* **[!UICONTROL 반복]**: 반복에서 스토리 보드 타일은 스토리와 연결된 프로젝트에 따라 색상으로 구분됩니다. (각 프로젝트에는 스토리 보드에 임의로 색상이 지정됩니다.) 각 애자일 팀에 대해 이 기본 동작을 변경할 수 있습니다. 반복에서 애자일 스토리의 색상은 프로젝트(기본값), 스토리 우선 순위, 소유자 또는 자유 형식에 연결할 수 있습니다. 자세한 내용은 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) 문서에서 [애자일 스토리 보드에서 스토리에 색상 표시기가 사용되는 방법 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)을 참조하십시오.

* **[!UICONTROL 프로젝트]**: 프로젝트에서 모든 하위 작업은 상위 작업의 색상과 일치하므로 주어진 스윔에 있는 모든 스토리의 색상은 동일합니다. 작업에 하위 작업이 없거나 상위 작업이 없는 경우 작업이 생성될 때 색상이 임의로 할당됩니다. 애자일 보기를 수정하여 이 기본 동작을 변경할 수 있습니다. 프로젝트에서 애자일 스토리의 색상은 상위 스토리(기본값), 스토리 우선 순위, 소유자 또는 자유 형식에 연결할 수 있습니다. 자세한 내용은 [다음에서 [!UICONTROL 애자일 ]보기 만들기 또는 사용자 지정](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)[을(를) 참조하십시오 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p> 
   또는
   <p>현재: [!UICONTROL Work] 이상</p> </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 자유 형식 사용 시 스토리 색상 변경

애자일 팀 설정이 구성되어 [!UICONTROL 카드 색상을 ]에 연결 옵션이 [!UICONTROL 자유 형식]&#x200B;(으)로 설정된 경우 사용자가 개별 스토리 타일의 색상을 수동으로 변경할 수 있습니다. 이렇게 하면 팀이나 조직에 중요한 다른 유형의 정보를 전달하는 데 유용할 수 있습니다.

{{step1-to-team}}

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. 왼쪽 패널에서 **[!UICONTROL 반복]**&#x200B;을 선택하여 특정 반복을 선택하거나 **[!UICONTROL 현재 반복]**&#x200B;을 선택합니다.
1. 스토리 타일 상단의 컬러 배너 위로 마우스를 가져갑니다.

   ![스토리 카드](assets/agile-story-color1-nwe-350x140.png)

1. **[!UICONTROL 색상 변경]**&#x200B;을 클릭한 다음 원하는 색상을 선택합니다.

   ![색상 선택](assets/agile-story-color2-nwe-350x138.png)
