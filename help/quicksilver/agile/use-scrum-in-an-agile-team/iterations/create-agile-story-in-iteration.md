---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 반복에서 민첩한 스토리 만들기
description: 이 문서에서는 이미 이터레이션에 있는 경우 새 Agile 스토리를 만드는 방법에 대해 설명합니다.
author: Courtney
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 4%

---

# 반복에서 민첩한 스토리 만들기

이 문서에서는 이미 이터레이션에 있는 경우 새 Agile 스토리를 만드는 방법에 대해 설명합니다. [!DNL Adobe Workfront]의 작업, 문제 또는 기타 영역에서 Agile 스토리를 만드는 방법에 대한 자세한 내용은 [기존 반복에 스토리 추가](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스</td> 
   <td> <p>표준</p> 
   <p>작업 이상</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>스토리가 있는 프로젝트에 대한 액세스 권한 관리 </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 반복에서 민첩한 스토리 만들기

1. 스토리를 만들려는 애자일 반복으로 이동합니다.

   {{step1-to-team}}

   1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

   1. 왼쪽 패널에서 **[!UICONTROL 반복]**&#x200B;을 선택합니다.
   1. 스토리를 작성할 특정 이터레이션의 이름을 클릭합니다.
   1. 왼쪽 패널에서 **[!UICONTROL 스토리]**&#x200B;를 선택합니다.

1.  **[!UICONTROL 새 스토리]**&#x200B;를 클릭합니다.
1. 다음 정보를 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>스토리 이름을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 설명]</strong></td>
      <td>스토리에 대한 설명을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 준비]</strong></td>
      <td>스토리를 이터레이션에 추가할 준비가 된 경우 이 옵션을 선택합니다. 이 옵션을 선택하면 백로그의 스토리를 이터레이션에 추가할 준비가 된 스토리가 사용자에게 표시됩니다.<br>스토리가 <strong>[!UICONTROL Ready](으)로 표시되어 있는지 여부에 관계 없이 반복에 스토리를 추가할 수 있습니다.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 예상](포인트)</strong></td>
      <td>스토리에 대한 견적을 지정합니다. 민첩한 팀이 스토리를 포인트로 추정하도록 구성된 경우 기본적으로 1포인트는 8시간과 같습니다. 예측은 스토리에 [!UICONTROL 계획 시간]으로 추가됩니다.<br>예를 들어 스토리를 3점으로 예상하는 경우 기본 동작은 스토리에 24시간의 예정 시간을 추가하는 것입니다.<br>스토리에 하위 작업이 포함되어 있는 경우 모든 하위 작업에 대한 전체 추정치가 상위 스토리의 예측을 결정한다는 것을 기억하십시오. 자세한 내용은 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">[!UICONTROL Scrum] 보드의 기존 스토리에 하위 작업 추가</a>를 참조하세요.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 부모 프로젝트]</strong></td>
      <td>이 스토리가 연결될 프로젝트의 이름을 입력하세요.<br>기본적으로 스토리 색상은 이 프로젝트의 다른 스토리와 같은 색상으로 표시됩니다.<br>프로젝트 상태는 [!UICONTROL Current]로 설정해야 합니다. 프로젝트 상태가 [!UICONTROL Current]가 아닌 경우에는 드롭다운 메뉴에 표시되지 않습니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 상위 작업]</strong></td>
      <td>상위 프로젝트를 선택한 후 상위 작업을 선택할 수 있습니다. 상위 작업을 선택하면 스토리가 선택한 프로젝트에 상위 작업의 하위 작업으로 만들어집니다.<br>스토리의 상위 작업 이름을 입력하고 드롭다운 목록에 나타나면 클릭합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 사용자 지정 Forms]</strong></td>
      <td>스토리에 추가할 사용자 지정 양식을 선택합니다.</td>
     </tr>
    </tbody>
   </table>

1. **[!UICONTROL 스토리 저장]**&#x200B;을 클릭합니다.
