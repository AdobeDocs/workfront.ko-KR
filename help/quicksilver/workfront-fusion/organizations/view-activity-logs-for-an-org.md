---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion에서 조직에 대한 활동 로그 보기
description: 조직의 시나리오 생성 또는 활성화와 같은 활동 로그를 볼 수 있습니다.
author: Becky
feature: Workfront Fusion
exl-id: d60dc97d-2da6-44f4-a2ee-bb5e56317695
source-git-commit: 1694d54c8b2d6ee3707e8e8bcb3b394c1dfa7a48
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 1%

---

# Adobe Workfront Fusion에서 조직에 대한 활동 로그 보기

<!--Move to new repo-->

시나리오를 만들거나 사용자를 조직에 초대하는 것과 같은 활동 로그를 볼 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 기능을 사용하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td>
   <td> <p>새로운 기능: Ultimate</p> <p>또는</p> <p>현재: 사용할 수 없음</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: [!UICONTROL Standard]</p><p>또는</p><p>현재: 사용할 수 없음</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 라이센스**</td> 
   <td>
   <p>현재: [!DNL Workfront Fusion] 라이선스 요구 사항이 없습니다.</p>
   <p>또는</p>
   <p>레거시: 모두 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">제품</td> 
   <td>
   <p>새 항목: [!DNL Workfront Fusion]이(가) Ultimate Workfront 플랜에 포함되어 있습니다.</p> <p>또는</p>
   <p>현재: 사용할 수 없음</p>
   </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

[!DNL Adobe Workfront Fusion] 라이선스에 대한 자세한 내용은 [[!DNL Adobe Workfront Fusion] 라이선스](../../workfront-fusion/get-started/license-automation-vs-integration.md)를 참조하세요.

+++



## 활동 로그 보기

1. 왼쪽 탐색 패널에서 **조직 개요** ![조직 개요 아이콘](assets/org-overview-icon.png)을 클릭합니다.
1. 현재 활동 로그를 보려는 조직에 있지 않은 경우 화면 오른쪽 상단에 있는 조직 이름을 클릭하고 드롭다운에서 조직을 선택합니다.
1. 화면 상단 근처에 있는 **[!UICONTROL 활동 로그]** 탭을 클릭합니다.

   활동 로그 페이지가 열립니다.
1. (선택 사항) 활동 로그를 필터링하여 지정한 기준별로 결과를 제한합니다.

   자세한 지침은 이 문서에서 [활동 로그 필터링](#filter-the-activity-logs)을 참조하십시오.
1. (선택 사항) 적용된 필터를 지우려면 화면 오른쪽 상단 근처에 있는 필터를 찾은 다음 필터 상자에서 **X**&#x200B;을 클릭합니다.
1. (선택 사항) 로그를 내보냅니다.

   지침은 이 문서에서 [활동 로그 내보내기](#export-the-activity-logs)를 참조하십시오.


## 활동 로그 필터링

1. 왼쪽 탐색 패널에서 **조직 개요** ![조직 개요 아이콘](assets/org-overview-icon.png)을 클릭합니다.
1. 현재 활동 로그를 보려는 조직에 있지 않은 경우 화면 오른쪽 상단에 있는 조직 이름을 클릭하고 드롭다운에서 조직을 선택합니다.
1. 화면 상단 근처에 있는 **[!UICONTROL 활동 로그]** 탭을 클릭합니다.

   활동 로그 페이지가 열립니다.
1. **필터** ![필터 아이콘](assets/filter-activity-log.png)을 클릭합니다.
1. 필드를 클릭하여 다음 필터 중 하나 이상을 구성합니다.

   * **시작 날짜 및 종료 날짜**: 달력에서 날짜를 선택하고(선택 사항) 시간을 입력합니다.
   * **사용자**: 드롭다운에서 사용자를 선택합니다.
   * **팀**: 드롭다운에서 팀을 선택합니다. 회원인 팀만 드롭다운에 표시됩니다.
   * **엔터티**: 작업 로그를 보려는 Fusion 개체의 형식을 선택하십시오.
   * **작업**: 작업 로그를 볼 작업을 선택하십시오.

1. **적용** 클릭

## 활동 로그 내보내기

1. 왼쪽 탐색 패널에서 **조직 개요** ![조직 개요 아이콘](assets/org-overview-icon.png)을 클릭합니다.
1. 현재 활동 로그를 보려는 조직에 있지 않은 경우 화면 오른쪽 상단에 있는 조직 이름을 클릭하고 드롭다운에서 조직을 선택합니다.
1. 화면 상단 근처에 있는 **[!UICONTROL 활동 로그]** 탭을 클릭합니다.

   활동 로그 페이지가 열립니다.
1. 달력에서 날짜 범위를 선택하고 (선택 사항) 시간을 입력합니다.
1. Excel 파일을 내보낼 것인지 CSV 파일을 내보낼 것인지 선택합니다.
1. **적용**&#x200B;을 클릭합니다.

