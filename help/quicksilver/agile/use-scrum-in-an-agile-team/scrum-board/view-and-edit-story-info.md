---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 스크럼 보드에서 스토리 정보 보기 및 편집
description: 간판 보드에서 스토리 타일을 볼 때 특정 정보를 스토리 타일에서 직접 인라인으로 편집할 수 있습니다.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# 에서 스토리 정보 보기 및 편집 [!UICONTROL 스크럼] 보드

## 보고 편집할 수 있는 정보를 이해합니다

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
   <td>작업 또는 문제에 직접 연결되는 링크가 있는 스토리 이름입니다</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>프로젝트에 직접 연결되는 링크가 있는 프로젝트 이름<br>이 링크는 반복에서 애자일 보기를 사용할 때 스토리(하위 작업이 아닌 상위 작업)에만 표시됩니다. 프로젝트에서 애자일 보기를 사용할 때에는 표시되지 않습니다.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>스토리에 대한 완료 지점 또는 시간 수와 스토리에 할당된 포인트 또는 시간 수<br>이 숫자는 각 스토리에 대한 [!UICONTROL Percent Complete]를 계산하고 표시하는 데 사용됩니다.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>각 스토리 및 문제에 대한 [!UICONTROL Percent Complete].<br>반복에 대한 [!UICONTROL Percent Complete]는 각 스토리에 대한 [!UICONTROL Percent Complete]를 기반으로 계산됩니다.</p> <p>스토리나 문제에 대해 [!UICONTROL 완료율]을 업데이트할 때 0에서 100 사이의 숫자를 선택할 수 있습니다.</p> </td> 
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
   <td> <p>의 "[!UICONTROL Agile] 보기 만들기 및 사용자 지정에 설명된 대로 애자일 보기를 수정하여 애자일 보기에 추가할 수 있는 모든 추가 필드(사용자 지정 필드 포함)가 있습니다 <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">[!UICONTROL Adobe Workfront]의 보기 개요</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>[!UICONTROL Work] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>작업 또는 문제에 대한 액세스 편집</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 스토리 타일에 대한 정보 보기 및 편집

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 팀]**.

1. (선택 사항) **[!UICONTROL 팀 전환]** 아이콘 ![팀 전환 아이콘](assets/switch-team-icon.png)를 클릭한 다음 드롭다운 메뉴에서 새 스크럼 팀을 선택하거나 검색 막대에서 팀을 검색합니다.

1. 왼쪽 패널에서 을 선택합니다 **[!UICONTROL 반복]** 특정 이터레이션을 선택하려면 **[!UICONTROL 현재 반복]**.

1. 로 이동합니다. [!UICONTROL 스크럼] 애자일 스토리보드
1. 를 확장합니다. [!UICONTROL 스토리] 타일을 사용하여 스토리와 연결된 모든 필드를 볼 수 있습니다.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (선택 사항) 필드를 편집하려면 필드를 클릭한 다음 모든 사항을 변경합니다.

   다음을 수행해야 합니다. [!UICONTROL 편집] 작업 또는 문제에 대한 작업 타일 편집 권한

>[!NOTE]
>
>를 변경하려면 [!UICONTROL 완료율]를 지정하는 경우 0에서 100 사이의 숫자를 입력해야 합니다. 필드가 이동할 수 있는 슬라이더가 아닙니다.
