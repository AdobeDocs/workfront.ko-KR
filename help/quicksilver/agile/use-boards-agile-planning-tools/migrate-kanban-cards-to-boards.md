---
content-type: reference
navigation-topic: boards
title: 애자일 팀 간판 카드를 Workfront 보드로 마이그레이션
description: 작업 항목을 애자일 팀 간판 보드에서 신규 또는 기존 Workfront 보드로 마이그레이션할 수 있습니다.
author: Lisa
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: f6bee61bbfbac98595d737fa002bbe01c0c573dc
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# 애자일 팀 간판 카드를 Workfront 보드로 마이그레이션

작업 항목을 애자일 팀 간판 보드에서 신규 또는 기존 Workfront 보드로 마이그레이션할 수 있습니다. 마이그레이션을 실행하면 간판 보드의 모든 카드가 Workfront 보드에 복사됩니다. 특정 카드를 선택할 수 없습니다.

Workfront 보드에 카드 배치는 열 정책을 기반으로 합니다. (예를 들어 정책이 &quot;진행 중&quot; 상태인 모든 카드를 특정 열로 이동할 수 있습니다. 열 정책에 대한 자세한 내용은 [보드 열 관리](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)) 정책이 없거나 카드가 정책과 일치하지 않으면 카드가 보드의 맨 왼쪽 열에 배치됩니다. 현재 레거시 보드의 백로그 열에 있는 카드는 Workfront 보드에 추가되지 않습니다.

카드가 애자일 팀 간판 보드에서 제거되지 않으며 카드 상태 변경 사항이 두 보드와 동기화됩니다. Workfront 보드로 전환할 준비가 될 때까지 두 보드를 모두 활성 상태로 유지할 수 있습니다.

>[!NOTE]
>
>이 기능은 Workfront 보드의 초기 기능 옵트인을 통해서만 사용할 수 있습니다.

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
   <td> <p>[!UICONTROL Request] 이상</p> </td>
  </tr>
 </tbody>
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 간판 카드를 새 보드로 마이그레이션

{{step1-to-team}}

1. 간판 보드에 액세스합니다.
1. 클릭 [!UICONTROL **보드에 추가**] 을(를) 선택합니다. [!UICONTROL **새 보드**].
1. 설정 [!UICONTROL 새 보드에 추가] 대화 상자에서 새 보드의 이름(현재 보드의 이름)을 입력합니다 [!UICONTROL 간판] 보드가 자동으로 표시됨)을 클릭하고 [!UICONTROL **추가**].

   ![새 보드에 간판 카드 추가](assets/add-kanban-cards-to-new-board-dialog.png)

1. (선택 사항) 나타나는 성공 메시지에서 링크를 클릭하여 새 보드를 엽니다.

## 기존 보드로 간판 카드 마이그레이션

{{step1-to-team}}

1. 간판 보드에 액세스합니다.
1. 클릭 [!UICONTROL **보드에 추가**] 을(를) 선택합니다. [!UICONTROL **기존 보드**].
1. 설정 [!UICONTROL 기존 보드에 추가] 카드를 마이그레이션할 보드를 검색하여 선택합니다. 그런 다음 [!UICONTROL **추가**].

   ![기존 보드에 간판 카드 추가](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (선택 사항) 나타나는 성공 메시지에서 링크를 클릭하여 보드를 엽니다.
