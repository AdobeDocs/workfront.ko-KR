---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 스토리 정보 편집
description: 간판 보드에서 스토리 타일을 볼 때 특정 정보를 스토리 타일에서 직접 인라인으로 편집할 수 있습니다.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 스토리 정보 편집

## 보고 편집할 수 있는 정보를 이해합니다 {#understand-what-information-can-be-viewed-and-edited}

에서 스토리 타일을 볼 때 [!UICONTROL 간판] 보드에서는 다음 표의 정보를 사용할 수 있습니다. 대부분의 정보를 스토리 타일에서 직접 인라인으로 편집할 수 있습니다.

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
   <td>작업 또는 문제에 직접 연결되는 링크가 있는 스토리 이름입니다</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트에 직접 연결되는 링크가 있는 프로젝트 이름</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>스토리에 대한 완료 지점 또는 시간 수와 스토리에 할당된 포인트 또는 시간 수<br>이 숫자들은 각 스토리에 대한 완료율을 계산하고 표시하는 데 사용됩니다.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>각 스토리 및 문제에 대한 [!UICONTROL Percent Complete].<br>반복에 대한 [!UICONTROL Percent Complete]는 각 스토리에 대한 [!UICONTROL Percent Complete]를 기반으로 계산됩니다.<br></p> <p>스토리나 문제에 대해 [!UICONTROL 완료율]을 업데이트할 때 0에서 100 사이의 숫자를 선택할 수 있습니다.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>그 이야기는 누가 담당합니까</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>타일의 색상 또는 카테고리입니다</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>의 "애자일 보기 만들기 및 사용자 지정"에 설명된 대로, 애자일 보기를 수정하여 애자일 보기에 추가되었을 수 있는 모든 추가 필드(사용자 지정 필드 포함)입니다 <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">의 보기 개요 [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 스토리 타일에 대한 정보 보기 및 편집

1. 을(를) 클릭합니다. *[!UICONTROL *주 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 선택한 다음 드롭다운 메뉴에서 새 간판 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 로 이동합니다. [!UICONTROL 간판] 보드.
1. 스토리 타일을 확장하여 스토리와 연결된 모든 필드를 봅니다.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (선택 사항) 필드를 편집하려면 필드를 클릭한 다음 모든 사항을 변경합니다.\
   다음을 수행해야 합니다. [!UICONTROL 편집] 작업 또는 문제에 대한 권한 을 사용하여 작업 타일을 편집할 수 있습니다.\
   각 필드 및 편집 가능 여부에 대한 자세한 내용은 [보고 편집할 수 있는 정보를 이해합니다](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>를 변경하려면 [!UICONTROL 완료율]를 지정하는 경우 0에서 100 사이의 숫자를 입력해야 합니다. 필드가 이동할 수 있는 슬라이더가 아닙니다.
