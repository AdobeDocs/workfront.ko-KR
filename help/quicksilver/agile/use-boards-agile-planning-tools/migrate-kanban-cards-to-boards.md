---
content-type: reference
navigation-topic: boards
title: 애자일 팀 간판 카드를 Workfront 보드로 마이그레이션
description: 애자일 팀 Kanban 보드에서 신규 또는 기존 Workfront 보드로 작업 항목을 마이그레이션할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# 애자일 팀 Kanban 카드를 Workfront 보드로 마이그레이션

애자일 팀 Kanban 보드에서 신규 또는 기존 Workfront 보드로 작업 항목을 마이그레이션할 수 있습니다. 마이그레이션을 실행하면 Kanban 보드의 모든 카드가 Workfront 보드에 복사됩니다. 특정 카드를 선택할 수 없습니다.

Workfront 보드의 카드 배치는 열 정책을 기반으로 합니다. (예를 들어, 정책이 &quot;진행 중&quot; 상태의 모든 카드를 특정 열로 이동할 수 있습니다. 열 정책에 대한 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)를 참조하십시오. 정책이 없거나 카드가 정책과 일치하지 않으면 카드는 보드의 맨 왼쪽 열에 배치됩니다. 현재 레거시 보드의 백로그 열에 있는 카드는 Workfront 보드에 추가되지 않습니다.

카드는 애자일 팀 Kanban 보드에서 제거되지 않으며 카드 상태 변경 사항은 두 보드에 모두 동기화됩니다. Workfront 보드로 전환할 준비가 될 때까지 두 보드를 모두 활성 상태로 유지할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> 
   <p>새로운 기능: [!UICONTROL Contributor] 이상</p> 
   <p>또는</p>
   <p>현재: [!UICONTROL Request] 이상</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 칸반 카드를 새 보드로 마이그레이션

{{step1-to-team}}

1. 칸반 보드에 액세스합니다.
1. [!UICONTROL **보드에 추가**]&#x200B;를 클릭하고 [!UICONTROL **새 보드**]&#x200B;를 선택합니다.
1. [!UICONTROL 새 보드에 추가] 대화 상자에서 새 보드의 이름(현재 [!UICONTROL Kanban] 보드의 이름이 자동으로 표시됨)을 입력하고 [!UICONTROL **추가**]&#x200B;를 클릭합니다.

   ![새 보드에 칸반 카드 추가](assets/add-kanban-cards-to-new-board-dialog.png)

1. (선택 사항) 표시되는 성공 메시지에서 링크를 클릭하여 새 보드를 엽니다.

## Kanban 카드를 기존 보드로 마이그레이션

{{step1-to-team}}

1. 칸반 보드에 액세스합니다.
1. [!UICONTROL **보드에 추가**]&#x200B;를 클릭하고 [!UICONTROL **기존 보드**]&#x200B;를 선택합니다.
1. [!UICONTROL 기존 보드에 추가] 대화 상자에서 카드를 마이그레이션할 보드를 검색하여 선택하십시오. [!UICONTROL **추가**]&#x200B;를 클릭합니다.

   ![기존 보드에 칸반 카드 추가](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (선택 사항) 표시되는 성공 메시지에서 링크를 클릭하여 보드를 엽니다.
