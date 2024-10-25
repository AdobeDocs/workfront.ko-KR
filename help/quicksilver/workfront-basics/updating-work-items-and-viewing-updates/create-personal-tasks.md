---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 개인 작업 만들기
description: 개인 작업은 사용자에게 보내는 임시 작업 요청이나 홈 영역에서 직접 생성하는 할 일 항목입니다. Workfront은 임시 작업 요청을 저장하고 항목을 개인 작업으로 수행합니다.
author: Lisa
feature: Get Started with Workfront
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---


# 개인 작업 만들기

<!--Audited: 10/2024-->

개인 작업은 사용자에게 보내는 임시 작업 요청이나 홈 영역에서 직접 생성하는 할 일 항목입니다.

Workfront은 임시 작업 요청을 저장하고 항목을 개인 작업으로 수행합니다.

기본적으로 Workfront의 모든 사용자에게는 &quot;&lt; 전체 이름 > 의 작업&quot;이라는 프로젝트가 있습니다. 예를 들어 &quot;Rick Kuvec의 작업&quot;입니다.

이 프로젝트는 검색에 표시되지 않으며 숨겨집니다. 모든 개인 작업은 이 프로젝트에 저장됩니다.

필요한 경우 개인 작업을 프로젝트로 이동할 수 있습니다.

다음과 같은 방법으로 개인 태스크를 생성할 수 있습니다.

* 홈 영역에 할 일 항목 만들기

  자세한 내용은 [홈 영역에서 작업 항목 및 프로젝트 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)를 참조하십시오.

* 다른 사용자에게 개인 작업 요청 만들기
* 사용자에 대한 개인 작업 요청 만들기

이 문서에서는 사용자에 대한 개인 작업 요청을 만드는 방법에 대해 설명합니다.

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
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> 
   <p>현재: 다른 사용자에게 요청을 보낼 계획입니다. 모든 사용자는 자신을 위해 작업 요청을 만들 수 있습니다.</p>
   <p>새로운 기능: 다른 사용자에게 요청을 보내는 표준. 모든 사용자는 자신을 위해 작업 요청을 만들 수 있습니다.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>사용자에 대한 액세스 권한을 편집하여 해당 사용자에 대한 작업 요청을 만듭니다. 액세스 권한을 보고 개인 작업 요청을 직접 만듭니다. </p>
   </td> 
  </tr>

</tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 개인 작업 요청 만들기

1. 사용자의 프로필 페이지로 이동하거나, 보기 액세스 권한이 있는 다른 사용자의 프로필 페이지로 이동합니다.

   >[!TIP]
   >
   >Workfront 관리자는 사용자가 액세스 수준을 구성할 때 특정 사용자가 표시되지 않도록 할 수 있습니다.

1. 헤더의 사용자 이름 오른쪽에 있는 **추가 메뉴** ![](assets/more-menu.png)을(를) 클릭합니다.
1. **작업 보내기** 요청을 클릭합니다.
**사용자에게 작업 요청 보내기** 상자가 표시됩니다.

   ![](assets/personal-task-box.png)
1. 다음 정보를 업데이트합니다.

   * **작업 이름**: 임시 작업 요청 또는 개인 작업의 이름입니다.
   * **설명**: 작업에 대한 설명을 추가합니다.
   * **할당 대상**: 선택한 사용자의 이름이 기본적으로 표시됩니다. 사용자 또는 팀을 더 추가할 수 있습니다.
   * **기한**: 이 작업을 완료하려는 날짜입니다. 기본적으로 오늘 날짜입니다. 과거의 날짜는 선택할 수 없습니다.
   * **시간**: 이 작업을 완료하는 데 필요한 시간입니다. 기본적으로 현재 시간입니다.

1. 작업 요청을 저장하려면 **요청 보내기**&#x200B;를 클릭하십시오.

   작업 요청은 Workfront에서 개인 작업으로 저장되고 홈 영역의 할 일 위젯에 추가됩니다.

   <!--this last step will need to be updated when they fix this functionality and the work requests you create for others actually go to their To do widget instead of yours-->

## 개인 작업 찾기

다음 영역에서 개인 태스크를 찾을 수 있습니다.

* 홈 영역의 할 일 위젯입니다. 자세한 내용은 [홈 영역에서 작업 항목 및 프로젝트 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)를 참조하십시오.

* 개인 작업 보고서 또는 목록. 작업 보고서 또는 목록에 개인 작업 필터를 빌드하고 적용할 수 있습니다. 자세한 내용은 [필터: 개인 작업](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md)을 참조하세요.





