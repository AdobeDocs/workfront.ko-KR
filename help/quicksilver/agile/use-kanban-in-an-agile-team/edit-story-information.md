---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 스토리 정보 편집
description: Kanban 보드에서 스토리 타일을 볼 때 특정 정보는 스토리 타일에서 직접 인라인으로 편집할 수 있습니다.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 91dc9946566e15bf32d0d89975e3e6b66b39e873
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 스토리 정보 편집

## 보고 편집할 수 있는 정보 이해 {#understand-what-information-can-be-viewed-and-edited}

[!UICONTROL Kanban] 보드에서 스토리 타일을 볼 때 다음 표의 정보를 사용할 수 있습니다. 대부분의 정보를 스토리 타일에서 직접 인라인으로 편집할 수 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>정보</strong> </th> 
   <th><strong>표시</strong> </th> 
   <th><strong>편집 가능한 인라인</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>작업 또는 문제에 직접 연결된 링크가 있는 스토리 이름</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트에 직접 연결되는 링크가 있는 프로젝트 이름</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>스토리의 완료점 또는 완료 시간 및 스토리에 할당된 완료점 또는 완료 시간<br>이 수치는 각 스토리의 완료율을 계산하고 표시하는 데 사용됩니다.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>각 스토리 및 문제에 대한 [!UICONTROL 완료율].반복에 대한 <br>[!UICONTROL 완료율]은 각 스토리에 대한 [!UICONTROL 완료율]을 기반으로 계산됩니다.<br></p> <p>스토리 또는 문제에 대해 [!UICONTROL 완료율]을 업데이트할 때 0에서 100 사이의 숫자를 선택할 수 있습니다.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>스토리가 할당된 사람</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>타일의 색상 또는 범주</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]</a>의 <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">보기 개요에서 "애자일 보기 만들기 및 사용자 지정"에 설명된 대로 애자일 보기를 수정하여 애자일 보기에 추가되었을 수 있는 추가 필드(사용자 지정 필드 포함)</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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

## 스토리 타일에 대한 정보 보기 및 편집

{{step1-to-team}}

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 Kanban 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. [!UICONTROL Kanban] 보드로 이동합니다.
1. 스토리 타일을 확장하여 스토리와 연결된 모든 필드를 표시합니다.

   ![스토리 카드](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (선택 사항) 필드를 편집하려면 필드를 클릭한 후 변경합니다.
스토리 타일을 편집하려면 작업 또는 문제에 대한 [!UICONTROL 편집] 권한이 있어야 합니다.
각 필드 및 편집 가능 여부에 대한 자세한 내용은 [보고 편집할 수 있는 정보 이해](#understand-what-information-can-be-viewed-and-edited)를 참조하십시오.

>[!NOTE]
>
>[!UICONTROL 완료율]을 변경하려면 0에서 100 사이의 숫자를 입력해야 합니다. 필드가 이동할 수 있는 슬라이더가 아닙니다.
