---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 카드 목록 사용
description: 작업 스트림에 카드 목록을 만들고 이 카드를 이터레이션에 추가할 수 있습니다.
author: Lisa
feature: Agile
source-git-commit: 8c02f5364154bdc343512416d0c7e38ef563a170
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# 카드 목록 사용

작업 스트림에 카드 목록을 만들고 이 카드를 이터레이션에 추가할 수 있습니다.

카드 목록은 작업 스트림에 대한 작업 백로그로 작동할 수 있습니다.

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

## 카드 목록에 카드 추가

{{step1-to-boards}}

1. 작업 스트림을 열려면 [!UICONTROL **작업 스트림 보기**].
1. 을(를) 클릭합니다. [!UICONTROL **카드 목록**] 탭.
1. 클릭 [!UICONTROL **카드 추가**].
1. 에서 [!UICONTROL **카드 만들기/편집**] 대화 상자에서 다음 정보를 추가합니다.

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>카드의 이름입니다.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>카드에 대한 설명입니다.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>카드를 완료하는 데 필요한 예상 시간 수입니다. 수동 입력만 가능합니다.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 상태]</strong></td> 
      <td>카드의 상태를 선택합니다.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 반복]</strong></td> 
      <td>카드를 할당할 이터레이션을 선택합니다.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>카드를 할당하려면 검색 필드에 이름을 입력한 다음 목록에 표시될 때 선택합니다. 개인 사용자와 팀을 모두 추가할 수 있으며, 두 명 이상의 개인 또는 팀을 카드에 할당할 수 있습니다.</p><p>할당자는 작업 스트림의 구성원이어야 합니다. 그렇지 않으면 선택 목록에 표시되지 않습니다.</p></td> 
     </tr>
    </tbody> 
   </table>

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.
1. 카드 목록을 작성할 때까지 카드를 계속 추가합니다.

## 카드 보기

단일 목록에서 작업 스트림에 대한 모든 카드를 보려면 [!UICONTROL **목록 보기**] 카드 목록 탭에서 다음을 수행합니다.

반복별로 그룹화된 작업 스트림의 모든 카드를 보려면 [!UICONTROL **반복 보기**]. 계획되지 않은 카드는 해당 그룹에 표시됩니다.

기존 카드를 편집하려면 목록에서 카드를 선택하고 [!UICONTROL **편집**].

카드를 삭제하려면 목록에서 카드를 선택하고 [!UICONTROL **삭제**].

### 카드 필터링

카드는 이터레이션 보드에서만 보관할 수 있습니다. 카드가 보관되면 보관된 카드를 표시하도록 필터링하지 않으면 카드 목록에 표시되지 않습니다. 카드 보관에 대한 자세한 내용은 [보드에서 카드 삭제 또는 보관](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. 워크플로우에 대한 카드 목록에 액세스합니다.
1. 클릭 [!UICONTROL **필터**] 을(를) 선택합니다. [!UICONTROL **모두**], [!UICONTROL **활성 카드**], 또는 [!UICONTROL **보관된 카드**].

   카드 목록에 기본 이외의 필터가 적용되면 필터 아이콘에 표시기가 표시됩니다 ![적용된 필터](assets/boards-filterapplied-30x30.png).

### 카드 목록에서 검색

1. 워크플로우에 대한 카드 목록에 액세스합니다.
1. 클릭 [!UICONTROL **검색**] 검색어를 입력합니다. 그런 다음 Enter 키를 누릅니다.

   검색어가 포함된 모든 카드가 표시됩니다.
X를 클릭하여 검색을 지웁니다.

   ![보드에서 카드 검색](assets/boards-searchbox.png)

## 반복에 카드 추가

>[!NOTE]
>
>카드를 추가하려면 먼저 반복을 만들어야 합니다. 자세한 내용은 [워크플로우에서 반복 만들기](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. 워크플로우에 대한 카드 목록에 액세스합니다.
1. 을(를) 선택합니다 [!UICONTROL **반복 보기**] 이터레이션에 지정된 카드와 계획되지 않은 카드를 확인합니다.
1. 목록에서 계획되지 않은 카드를 선택하고 [!UICONTROL **편집**].
1. 에서 이터레이션을 선택합니다 [!UICONTROL **반복**] 필드.
1. 스토리 포인트를 사용하는 경우 [!UICONTROL **예측**] 필드.
1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   카드가 이터레이션으로 이동되고 이터레이션 지표는 카드 및 점 수를 반영합니다.

   또한 계획되지 않은 카드 그룹의 카드를 이터레이션으로 끌어다 놓거나 [!UICONTROL **카드 추가**] 새 카드를 이터레이션에 추가하려면

>[!TIP]
>
>반복 프로세스 보드를 생성한 경우 카드 목록의 모든 계획되지 않은 카드가 [!UICONTROL 백로그] 열. 카드를 다른 열로 이동하면 활성 이터레이션의 일부가 됩니다. 카드 목록에서 이터레이션에 추가하는 카드는 해당 상태에 따라 열에 추가됩니다.

