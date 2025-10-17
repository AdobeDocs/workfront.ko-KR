---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 카드 목록 사용
description: 작업 스트림에 카드 목록을 만들고 카드를 반복에 추가할 수 있습니다.
author: Jenny
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# 카드 목록 사용

>[!IMPORTANT]
>
>일부 고객은 워크스트림을 사용할 수 없습니다.

작업 스트림에 카드 목록을 만들고 카드를 반복에 추가할 수 있습니다.

카드 목록은 워크스트림에 대한 작업 백로그로 작동할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>기여자 이상</p> 
   <p>요청 이상</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 카드 목록에 카드 추가

{{step1-to-boards}}

1. 작업 스트림을 열려면 [!UICONTROL **작업 스트림 보기**]&#x200B;를 클릭합니다.
1. [!UICONTROL **카드 목록**] 탭을 클릭합니다.
1. [!UICONTROL **카드 추가**]&#x200B;를 클릭합니다.
1. [!UICONTROL **카드 만들기/편집**] 대화 상자에서 다음 정보를 추가합니다.

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL 이름]</strong></td> 
      <td>카드의 이름입니다.</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL 설명]</strong></td> 
      <td>카드에 대한 설명.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>카드를 완료할 예상 시간입니다. 수동 입력만 가능합니다.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 상태]</strong></td> 
      <td>카드 상태를 선택합니다.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 반복]</strong></td> 
      <td>카드를 할당할 반복을 선택하십시오.</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 담당자]</strong></td> 
      <td><p>카드를 할당하려면 검색 필드에 이름을 입력한 다음 목록에 표시될 때 선택합니다. 개인 및 팀을 모두 추가할 수 있으며 한 카드에 둘 이상의 개인 또는 팀을 할당할 수 있습니다.</p><p>할당자는 작업 스트림의 구성원이어야 합니다. 그렇지 않으면 선택 목록에 표시되지 않습니다.</p></td> 
     </tr>
    </tbody> 
   </table>

1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.
1. 카드 목록을 빌드할 때까지 카드를 계속 추가합니다.

## 카드 보기

작업 스트림의 모든 카드를 단일 목록으로 보려면 [카드 목록] 탭에서 [!UICONTROL **목록 보기**]&#x200B;를 클릭하십시오.

반복별로 그룹화된 작업 스트림의 모든 카드를 보려면 [!UICONTROL **반복 보기**]&#x200B;를 클릭하십시오. 계획되지 않은 카드가 자체 그룹에 표시됩니다.

기존 카드를 편집하려면 목록에서 해당 카드를 선택한 다음 [!UICONTROL **편집**]&#x200B;을 클릭하세요.

카드를 삭제하려면 목록에서 카드를 선택한 다음 [!UICONTROL **삭제**]&#x200B;를 클릭합니다.

### 카드 필터링

카드는 반복 보드에서만 보관할 수 있습니다. 카드가 보관된 경우 보관된 카드를 표시하도록 필터링하지 않으면 카드 목록에 표시되지 않습니다. 카드 보관에 대한 자세한 내용은 [보드에서 카드 삭제 또는 보관](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md)을 참조하십시오.

1. 워크스트림에 대한 카드 목록에 액세스합니다.
1. [!UICONTROL **필터**]&#x200B;를 클릭하고 [!UICONTROL **모두**], [!UICONTROL **활성 카드**] 또는 [!UICONTROL **보관된 카드**]&#x200B;를 선택합니다.

   카드 목록에 기본값이 아닌 필터가 적용되면 필터 아이콘 ![필터 적용됨](assets/boards-filterapplied-30x30.png)에 표시기가 표시됩니다.

### 카드 목록에서 검색

1. 워크스트림에 대한 카드 목록에 액세스합니다.
1. [!UICONTROL **검색**]&#x200B;을 클릭하고 검색어를 입력하세요. 그런 다음 Enter 키를 누릅니다.

   검색어가 포함된 모든 카드가 표시됩니다.
X를 클릭하여 검색을 지웁니다.

   ![보드에서 카드 검색](assets/boards-searchbox.png)

## 반복에 카드 추가

>[!NOTE]
>
>카드를 추가하려면 먼저 반복을 만들어야 합니다. 자세한 내용은 [워크플로에서 반복 만들기](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)를 참조하십시오.

1. 워크스트림에 대한 카드 목록에 액세스합니다.
1. [!UICONTROL **반복 보기**]&#x200B;를 선택하여 어떤 카드가 반복에 할당되고 어떤 카드가 계획되지 않았는지 확인하십시오.
1. 목록에서 계획되지 않은 카드를 선택하고 [!UICONTROL **편집**]&#x200B;을 클릭합니다.
1. [!UICONTROL **반복**] 필드에서 반복을 선택합니다.
1. 스토리 포인트를 사용하는 경우 [!UICONTROL **예상**] 필드에 값을 입력하십시오.
1. [!UICONTROL **저장**]&#x200B;을 클릭합니다.

   카드가 반복으로 이동되고 반복 지표가 카드 및 포인트 수를 반영합니다.

   계획되지 않은 카드 그룹에서 카드를 반복으로 끌어다 놓거나 [!UICONTROL **카드 추가**]&#x200B;를 클릭하여 새 카드를 반복에 추가할 수도 있습니다.

>[!TIP]
>
>반복 프로세스 보드를 만든 경우 카드 목록에 있는 계획되지 않은 모든 카드가 [!UICONTROL 백로그] 열에 나타납니다. 카드가 다른 열로 이동되면 활성 반복의 일부가 됩니다. 카드 목록의 반복에 추가하는 카드는 해당 상태에 따라 열에 추가됩니다.
