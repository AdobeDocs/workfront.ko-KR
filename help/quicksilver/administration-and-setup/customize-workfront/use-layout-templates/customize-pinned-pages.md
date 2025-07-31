---
title: 레이아웃 템플릿을 사용하여 고정된 페이지 사용자 지정
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 레이아웃 템플릿에서 사용자가 Adobe Workfront의 맨 위에서 항상 사용할 수 있도록 하려는 페이지를 고정할 수 있습니다. 메인 메뉴 또는 대시보드를 통해 액세스하는 페이지일 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: 0e7000597e2347bff0bc626d21aa9a6c9a839c0b
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 4%

---

# 레이아웃 템플릿을 사용하여 고정된 페이지 사용자 지정

레이아웃 템플릿에서 사용자가 Adobe Workfront의 맨 위에서 항상 사용할 수 있도록 하려는 페이지를 고정할 수 있습니다. 기본 메뉴 ![기본 메뉴 아이콘](assets/main-menu-icon.png) 또는 사용 가능한 경우 기본 메뉴 ![기본 메뉴 아이콘](assets/main-menu-icon-left-nav.png)을 통해 액세스하는 페이지나 대시보드일 수 있습니다.

사용자가 직접 추가한 핀은 레이아웃 템플릿에 추가한 핀 오른쪽에 표시됩니다.

페이지 고정에 대한 자세한 내용은 [페이지를 고정하여 작업 영역을 사용자 지정](../../../workfront-basics/the-new-workfront-experience/pin-pages.md)을 참조하십시오.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
      <p>신규:</p>
         <ul>
         <li><p>표준</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>플랜</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레이아웃 템플릿을 사용하여 페이지 고정

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.
1. **위쪽 탐색 영역**&#x200B;에서 **새 핀 추가**&#x200B;를 클릭합니다.

1. 표시되는 드롭다운 메뉴에서 다음 중 하나를 수행합니다.

   * 다음 영역 중에서 선택합니다.

      * 캘린더
      * 대시보드
      * 문서
      * 목표
      * 홈
      * 내 업데이트
      * 포트폴리오
      * 프로그램
      * 프로젝트
      * 보고서
      * 요청
      * 리소스 조달
      * 시나리오
      * 팀
      * 템플릿
      * 타임시트
      * 사용자
      * 블루프린트
      * 계획 수립

     >[!IMPORTANT]
     >
     >목표, 시나리오 및 계획 영역을 보려면 추가 라이센스가 필요합니다.
     >
     >* Workfront 목표에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../../workfront-goals/goal-management/wf-goals-overview.md)를 참조하십시오.
     >
     >* Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 플래너 개요](../../../scenario-planner/scenario-planner-overview.md)를 참조하십시오.
     >
     >* Workfront Planning에 대한 자세한 내용은 [Adobe Workfront Planning 개요](/help/quicksilver/planning/general/planning-overview.md)를 참조하십시오.

   * **대시보드 추가**&#x200B;를 클릭합니다
      * <!--**Quick link name**-->**사용자 지정 이름** 필드에 수사적 이름을 입력하십시오.
      * **대시보드 추가** 필드 <!-- dropdown for existing or canvas dashboard, called "Choose a dashboard" now -->에서 대시보드를 선택하십시오.
      * **추가**&#x200B;를 클릭합니다.

1. 다른 페이지를 고정하려면 이전 단계를 반복합니다.

1. (선택 사항) 핀을 이동하려면 핀 위로 마우스를 가져간 후 핀 이름 옆에 있는 기타 메뉴 아이콘 ![기타 아이콘](assets/more-icon.png)을 클릭한 다음 **왼쪽으로 이동** 또는 **오른쪽으로 이동**&#x200B;을 클릭하여 선택한 방향으로 핀을 이동하거나 **맨 앞으로 이동**&#x200B;을 클릭하여 핀을 맨 왼쪽 위치로 이동합니다.

1. (선택 사항) 핀 이름을 바꾸려면 핀 위로 마우스를 가져간 후 핀 이름 옆에 있는 기타 메뉴 아이콘 ![기타 아이콘](assets/more-icon.png)을 클릭한 다음 **핀 이름 바꾸기**&#x200B;를 클릭합니다. 새 이름을 입력한 다음 **저장**&#x200B;을 클릭합니다.

1. (선택 사항) 핀을 삭제하려면 핀 위로 마우스를 가져간 후 핀 이름 옆에 있는 기타 메뉴 아이콘 ![기타 아이콘](assets/more-icon.png)을 클릭한 다음 **핀 제거**&#x200B;를 클릭합니다.

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >언제든지 **저장**&#x200B;을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.
