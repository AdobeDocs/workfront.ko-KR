---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 개인 작업 만들기
description: 개인 작업은 사용자가 홈 영역에서 직접 생성하는 사용자, 자신 또는 할 일 항목에 보내는 임시 작업 요청입니다. Workfront은 임시 작업 요청을 저장하고 항목을 개인 작업으로 수행합니다.
author: Lisa
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: a1081b7ce0877b08f9546ab57cfac3f2a580ea76
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# 개인 작업 만들기

<!--Audited: 10/2024-->

개인 작업은 사용자에게 보내거나 직접 보내거나 추가하는 임시 작업 요청입니다.

Adobe Workfront은 임시 작업 요청을 저장하고 Windows가 각 사용자에 대해 자동으로 만드는 사용자의 개인 프로젝트에서 항목을 개인 작업으로 처리합니다.

다음은 사용자의 개인 프로젝트 특성입니다.

* Workfront의 모든 사용자에게는 &quot;&lt; 사용자의 전체 이름>&#39;s Tasks&quot;라는 개인 프로젝트가 있습니다. 예를 들어 &quot;John Smith의 작업&quot;입니다.
* 각 사용자의 개인 프로젝트는 검색에 표시되지 않고 숨겨집니다.
* 사용자가 비활성화된 경우에도 개인 프로젝트를 삭제할 수 없습니다.
* 개인 프로젝트의 상태는 항상 현재입니다. 개인 프로젝트는 완료하거나 취소할 수 없습니다.
* 모든 개인 작업은 사용자 개인 프로젝트에 저장됩니다.
* 필요한 경우 개인 작업을 다른 프로젝트로 이동할 수 있습니다.

다음과 같은 방법으로 개인 작업을 만들 수 있습니다.

* 홈 영역에서 할 일 항목 만들기

  자세한 내용은 [홈 영역에서 작업 항목 및 프로젝트 만들기](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)를 참조하십시오.

* 사용자 프로필 페이지에서 개인 작업 요청을 만들어 다른 사용자에게 보내기
* 사용자 프로필 페이지에서 개인 작업 요청을 직접 만들어 보냅니다.

이 문서에서는 사용자 프로필 페이지에서 사용자 또는 사용자에 대한 개인 작업 요청을 만드는 방법에 대해 설명합니다.

개인 작업을 추가하는 방법에 관계없이 Workfront의 동일한 영역에서 찾을 수 있습니다. 자세한 내용은 이 문서의 [개인 작업 찾기](#locate-personal-tasks) 섹션을 참조하십시오.

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
   <p>새로운 기능: 다른 사용자에게 요청을 보내는 표준. 모든 사용자는 자신을 위해 작업 요청을 만들 수 있습니다.</p> 
   <p>현재: 다른 사용자에게 요청을 보낼 계획입니다. 모든 사용자는 자신을 위해 작업 요청을 만들 수 있습니다.</p>
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

1. 사용자의 프로필 페이지로 이동하거나, 보기 권한이 있는 다른 사용자의 프로필 페이지로 이동합니다.

   >[!TIP]
   >
   >Workfront 관리자가 특정 사용자가 액세스 수준을 구성할 때 특정 사용자를 못하도록 차단할 수 있습니다.

1. **헤더에서 사용자 이름 오른쪽에 있는 자세히 메뉴를** ![](assets/more-menu.png) 클릭합니다.
1. **작업 요청 보내기**를 클릭합니다.
**사용자에게 작업 요청 보내기** 상자가 표시됩니다.

   ![](assets/personal-task-box.png)
1. 다음 정보를 업데이트합니다.

   * **작업 이름**: 임시 작업 요청 또는 개인 작업의 이름입니다.
   * **설명**: 작업에 대한 설명을 추가합니다.
   * **할당 대상**: 선택한 사용자의 이름이 기본적으로 표시됩니다. 사용자 또는 팀을 더 추가할 수 있습니다.
   * **기한**: 이 작업을 완료하려는 날짜입니다. 기본적으로 오늘 날짜입니다. 과거의 날짜는 선택할 수 없습니다.
   * **시간**: 이 작업을 완료하는 데 필요한 시간입니다. 기본적으로 현재 시간입니다.

1. 작업 요청을 저장하려면 **요청 보내기**&#x200B;를 클릭하십시오.

   작업 요청은 Workfront에서 개인 작업으로 저장되며 홈 영역에서 사용자의 할 일 위젯에 추가됩니다. 작업 요청을 자신에게 보내면 홈 의 할 일 위젯에 표시됩니다.


## 개인 작업 찾기

다음 영역에서 개인 작업을 찾을 수 있습니다.

* 개인 요청 수신을 받은 사용자 홈 영역에 있는 To-dos 위젯

  자세한 내용은 홈 영역에서](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) 작업 항목 및 프로젝트 만들기 항목을 [참조하세요.

* 개인 작업 보고서 또는 목록입니다. 개인 작업 필터를 작성하고 작업 보고서 또는 목록에 적용하여 개인 작업만 표시하고 프로젝트 작업을 제외할 수 있습니다.

  자세한 내용은 [필터: 개인 작업](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md)을 참조하세요.
