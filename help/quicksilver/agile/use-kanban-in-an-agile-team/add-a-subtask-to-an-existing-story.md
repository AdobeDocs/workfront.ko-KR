---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 칸반 보드의 기존 스토리에 하위 작업 추가
description: 이 문서를 검토하여 Kanban 보드에서 기존 스토리에 대한 하위 작업을 만드는 방법을 알아보십시오.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Kanban 보드의 기존 스토리에 하위 작업 추가

기존 스토리에 대한 하위 작업을 만들 때는 다음 사항에 유의하십시오.

**프로젝트에 대한 [!UICONTROL 요약 완료 모드] 설정이 [!UICONTROL 수동]:**(으)로 설정된 경우

* 하위 작업이 있는 상위 스토리를 [!UICONTROL 완료]&#x200B;(으)로 이동하여 상위 스토리를 100%로 업데이트하고 [!UICONTROL 상태]을(를) [!UICONTROL 완료]&#x200B;(으)로 업데이트할 수 있습니다. 하위 작업은 업데이트되지 않습니다.
* 스토리에 대한 [!UICONTROL 완료율]을 업데이트하려면 개체의 [!UICONTROL 스토리] 탭 또는 [!UICONTROL 세부 정보] 페이지에서 업데이트해야 합니다.

**프로젝트에 대한 [!UICONTROL 요약 완료 모드] 설정이 [!UICONTROL 자동]:**(으)로 설정된 경우

* 게시판에서 상위 스토리를 이동할 수 없습니다. 스토리에 대한 [!UICONTROL 완료율]을 업데이트하려면 하위 작업에 대해 [!UICONTROL 완료율]을 업데이트해야 합니다. 스토리에 대한 [!UICONTROL 완료율]은(는) 모든 하위 작업의 [!UICONTROL 완료율]을(를) 기반으로 계산됩니다.
* 하위 작업이 있는 상위 스토리를 [!UICONTROL 완료]&#x200B;(으)로 이동하면 상위 스토리가 100%로 업데이트되고 [!UICONTROL 상태]이 [!UICONTROL 완료]&#x200B;(으)로 업데이트됩니다. 하위 작업도 100%로 업데이트되고 [!UICONTROL 상태]가 [!UICONTROL 완료]&#x200B;(으)로 업데이트됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p> 
   <p>작업 이상</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>하위 작업이 있는 작업에 대한 액세스 기여 또는 관리</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!UICONTROL Kanban] 보드의 기존 스토리에 하위 작업 추가

1. 하위 작업을 추가할 스토리가 포함된 [!UICONTROL Kanban] 보드로 이동합니다.
1. [!UICONTROL Kanban] 보드의 스토리 타일에서 작업 이름을 클릭합니다.
1. [!DNL Workfront]하위 작업 만들기[에 설명된 대로 ](../../manage-work/tasks/create-tasks/create-subtasks.md) 내의 다른 작업 목록에서처럼 작업에 하위 작업을 추가하십시오.
