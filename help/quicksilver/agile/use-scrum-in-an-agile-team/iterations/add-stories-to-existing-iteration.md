---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 기존 반복에 스토리 추가
description: 다양한 방법으로 반복에 스토리를 추가할 수 있습니다.
author: Jenny
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 3%

---

# 기존 반복에 스토리 추가

다음 방법 중 하나로 반복에 스토리를 추가할 수 있습니다.

* [애자일 백로그 관리[!UICONTROL 의 ]백로그에서 반복 또는 ](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board)Kanban[ 보드로 스토리 이동](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) 섹션에 설명된 대로 반복이 만들어진 후 백로그에서

* 개별 작업 또는 문제의 [!UICONTROL 세부 정보] 페이지에서
* 작업 또는 문제 목록에서
* 보고서에서
* 대시보드에서

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p> 
   <p>작업 이상</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>스토리가 있는 프로젝트에 대한 액세스 관리 </td> 
  </tr>
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 스토리를 추가하는 것이 작업 날짜에 미치는 영향 이해

기본적으로 기존 작업을 반복에 추가하면 작업의 [!UICONTROL 계획된 시작 일자] 및 [!UICONTROL 계획된 완료 일자]가 다음과 같이 설정됩니다.

### 작업 [!UICONTROL 계획된 시작 일자]

* 이 작업에서는 다음과 같은 경우 반복의 시작 일자를 사용합니다.

   * 프로젝트에 [!UICONTROL 계획된 시작 일자]가 설정되어 있지 않습니다.
   * 프로젝트의 [!UICONTROL 계획된 시작 일자]가 반복의 시작 일자인 *이전* 또는 *날짜*&#x200B;입니다.

* 작업은 다음과 같은 경우 프로젝트의 [!UICONTROL 계획된 시작 일자]를 사용합니다.

   * 프로젝트의 [!UICONTROL 계획된 시작 일자]는 반복의 시작 일자 *이후*&#x200B;입니다.

### 작업 [!UICONTROL 계획된 완료 일자]

* 이 작업에서는 다음과 같은 경우 반복의 종료 일자를 사용합니다.

   * 프로젝트에 [!UICONTROL 계획된 완료 일자]가 설정되어 있지 않습니다.
   * 프로젝트의 [!UICONTROL 계획된 시작 일자]는 반복의 시작 일자 *이전 또는*&#x200B;이거나 프로젝트의 [!UICONTROL 계획된 완료 일자]는 반복의 종료 일자 *이전 또는*&#x200B;입니다.

* 작업은 다음과 같은 경우 프로젝트의 [!UICONTROL 계획된 완료 일자]를 사용합니다.

   * 프로젝트의 [!UICONTROL 계획된 시작 일자]는 반복의 시작 일자 *이후*&#x200B;이고 프로젝트의 [!UICONTROL 계획된 완료 일자]는 반복의 종료 일자 *이후*&#x200B;입니다.

개별 스크럼 팀이 반복 날짜가 아닌 프로젝트 날짜를 기본적으로 사용하도록 구성할 수 있습니다. 자세한 내용은 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) 문서의 [반복에 작업 항목을 추가할 때 날짜가 적용되는 방법 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md) 섹션을 참조하십시오.

## 기존 반복에 스토리 추가

프로젝트에 대한 관리 액세스 권한이 있는 경우 모든 반복에 작업 또는 문제를 추가할 수 있습니다. 작업 또는 문제를 반복으로 이동할 때는 다음 사항을 염두에 두십시오.

* 여러 팀을 추가하면 작업 또는 문제가 한 팀의 반복에만 표시될 수 있습니다. 아래 3단계에서 선택하는 반복입니다.
* 작업 또는 문제가 애자일 팀에 할당되고 다른 팀의 반복으로 이동한 경우 팀 할당이 변경되지 않습니다.
* 작업 또는 문제가 팀에 할당되지 않은 경우 작업 또는 문제가 반복을 소유한 팀에 할당됩니다.
* 반복에 상위 작업을 추가할 수 없습니다. 하위 작업을 추가하면 상위 작업이 스크럼 보드에 스윔레인으로 표시됩니다.

>[!IMPORTANT]
>
>작업이 반복으로 이동한 후에는 [!UICONTROL 기간 유형] 또는 [!UICONTROL 작업 제한]을 업데이트할 수 없습니다. [!UICONTROL 기간 유형]이(가) [!UICONTROL 단순]&#x200B;(으)로 설정되고 [!UICONTROL 작업 제한]이(가) [!UICONTROL 고정 날짜]&#x200B;(으)로 설정되어 작업 타임라인을 반복의 타임라인과 일관되게 유지합니다.

1. 반복에 추가할 작업 또는 문제를 엽니다.
또는
반복에 추가할 작업 또는 문제가 포함된 프로젝트, 보고서 또는 대시보드로 이동합니다. 그런 다음 작업 또는 문제를 하나 이상 선택합니다.

1. **[!UICONTROL 자세히]** ![추가 아이콘](assets/more-icon.png) > **[!UICONTROL 반복에 추가]**를 클릭합니다.
애자일이 아닌 팀에 할당된 작업 또는 문제를 할당할 수 없습니다.

1. **[!UICONTROL 다음에 추가]** 상자에서 반복 이름을 입력하고 목록에 나타나면 선택합니다.

   >[!NOTE]
   >
   >기존 반복에서 새 반복으로 스토리를 이동할 수 있습니다.

1. **[!UICONTROL 추가를 클릭합니다]**.
