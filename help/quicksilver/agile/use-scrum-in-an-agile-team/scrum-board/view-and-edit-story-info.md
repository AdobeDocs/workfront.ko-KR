---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드에서 스토리 정보 보기 및 편집
description: Kanban 보드에서 스토리 타일을 볼 때 특정 정보는 스토리 타일에서 직접 인라인으로 편집할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# [!UICONTROL 스크럼] 게시판에서 스토리 정보를 보고 편집합니다.

## 보고 편집할 수 있는 정보 이해

스토리 보드에서 스토리 타일을 볼 때 다음 표의 정보를 사용할 수 있습니다. 대부분의 정보를 스토리 타일에서 직접 인라인으로 편집할 수 있습니다.

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
   <td>✓ 덧신</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트에 직접 연결되는 링크가 있는 프로젝트 이름<br>이 링크는 반복에서 애자일 보기를 사용할 때는 스토리(하위 작업이 아닌 상위 작업)에만 표시되고 프로젝트에서 애자일 보기를 사용할 때는 표시되지 않습니다.</p> </td> 
   <td>✓ 덧신 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>스토리의 완료 지점 또는 시간 수와 스토리에 할당된 지점 또는 시간 수<br>이 수치는 각 스토리에 대한 [!UICONTROL 완료율]을 계산하고 표시하는 데 사용됩니다.</p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td> <p>각 스토리 및 문제에 대한 [!UICONTROL 완료율].<br>반복에 대한 [!UICONTROL 완료율]은 각 스토리의 [!UICONTROL 완료율]을 기반으로 계산됩니다.</p> <p>스토리 또는 문제에 대해 [!UICONTROL 완료율]을 업데이트할 때 0에서 100 사이의 숫자를 선택할 수 있습니다.</p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td> <p>스토리가 할당된 사람</p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td> <p>타일의 색상 또는 범주</p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">[!UICONTROL Adobe Workfront]의 보기 개요</a>에서 "[!UICONTROL 애자일] 보기 만들기 및 사용자 지정"에 설명된 대로 애자일 보기를 수정하여 애자일 보기에 추가되었을 수 있는 추가 필드(사용자 지정 필드 포함)입니다.</p> </td> 
   <td>✓ 덧신</td> 
   <td>✓ 덧신</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업 또는 문제에 대한 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 [!DNL Workfront] 관리자에게 문의하세요.

## 스토리 타일에 대한 정보 보기 및 편집

1. [!DNL Adobe Workfront]의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 팀]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)을 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 창에서 팀을 검색합니다.

1. 왼쪽 패널에서 **[!UICONTROL 반복]**&#x200B;을 선택하여 특정 반복을 선택하거나 **[!UICONTROL 현재 반복]**&#x200B;을 선택합니다.

1. [!UICONTROL 스크럼] 애자일 스토리 보드로 이동합니다.
1. [!UICONTROL 스토리] 타일을 확장하여 스토리와 연결된 모든 필드를 봅니다.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (선택 사항) 필드를 편집하려면 필드를 클릭한 후 변경합니다.

   스토리 타일을 편집하려면 작업 또는 문제에 대한 [!UICONTROL 편집] 권한이 있어야 합니다.

>[!NOTE]
>
>[!UICONTROL 완료율]을 변경하려면 0에서 100 사이의 숫자를 입력해야 합니다. 필드가 이동할 수 있는 슬라이더가 아닙니다.
