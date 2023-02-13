---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 기존 반복에 스토리 추가
description: 여러 가지 방법으로 반복에 스토리를 추가할 수 있습니다.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 기존 반복에 스토리 추가

다음과 같은 방법으로 반복에 스토리를 추가할 수 있습니다.

* 다음에 설명된 대로 반복을 작성한 후 백로그에서 [백로그에서 반복 또는 [!UICONTROL 간판] 보드](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) 섹션 [애자일 백로그 관리](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* 에서 [!UICONTROL 세부 사항] 개별 작업 또는 문제의 페이지
* 작업 또는 문제 목록에서
* 보고서에서
* 대시보드에서

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
   <td> <p>[!UICONTROL Worker] 이상</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>스토리가 있는 프로젝트에 대한 [!UICONTROL Manage] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 스토리 추가가 작업 날짜에 미치는 영향 이해

기본적으로 기존 작업을 이터레이션에 추가할 때는 [!UICONTROL 계획 시작 날짜] 및 [!UICONTROL 계획 완료 일자] 는 다음과 같이 설정됩니다.

### 작업 [!UICONTROL 계획 시작 날짜]

* 다음과 같은 경우 이터링의 시작 날짜를 사용합니다.

   * 프로젝트에 [!UICONTROL 계획 시작 날짜] 설정합니다.
   * 프로젝트의 [!UICONTROL 계획 시작 날짜] is *이전* 또는 *on* 이터레이션의 시작 날짜입니다.

* 작업은 프로젝트의 [!UICONTROL 계획 시작 날짜] 설정:

   * 프로젝트의 [!UICONTROL 계획 시작 날짜] is *after* 이터레이션의 시작 날짜입니다.

### 작업 [!UICONTROL 계획 완료 일자]

* 다음과 같은 경우 이터링의 종료 날짜를 사용합니다.

   * 프로젝트에 [!UICONTROL 계획 완료 일자] 설정합니다.
   * 프로젝트의 [!UICONTROL 계획 시작 날짜] is *또는* 이터레이션의 시작 날짜 또는 프로젝트 [!UICONTROL 계획 완료 일자] is *또는* 이터레이션의 종료 날짜입니다.

* 작업은 프로젝트의 [!UICONTROL 계획 완료 일자] 설정:

   * 프로젝트의 [!UICONTROL 계획 시작 날짜] is *after* 반복의 시작 날짜 및 프로젝트의 [!UICONTROL 계획 완료 일자] is *after* 이터레이션의 종료 날짜입니다.

반복 날짜가 아닌 기본적으로 프로젝트 날짜를 사용하도록 개별 스크럼 팀을 구성할 수 있습니다. 자세한 내용은 섹션을 참조하십시오 [작업 항목을 이터레이션에 추가할 때 날짜가 적용되는 방식을 구성합니다](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 기사 [스크럼 구성](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## 기존 반복에 스토리 추가

작업 또는 문제와 직접 반복에 스토리를 추가하려면 다음을 수행합니다.

>[!IMPORTANT]
>
>작업이 반복으로 이동되면 업데이트할 수 없습니다 [!UICONTROL 기간 유형] 또는 [!UICONTROL 작업 제한]. [!UICONTROL 기간 유형] 가 로 설정되어 있습니다. [!UICONTROL 단순] 및 [!UICONTROL 작업 제한] 가 로 설정되어 있습니다. [!UICONTROL 고정 날짜] 작업 타임라인을 반복 타임라인과 일관되게 유지하기 위해

### 작업 또는 문제 탭에서 다음을 수행합니다

프로젝트에 대한 액세스 관리 권한이 있는 경우 모든 작업이나 문제를 반복에 추가할 수 있습니다. 작업이나 문제를 반복으로 이동할 때는 다음 사항을 염두에 두십시오.

* 여러 팀을 추가하는 경우 작업이나 문제가 한 팀의 반복에만 표시될 수 있습니다. 아래 3단계에서 선택한 반복입니다.
* 작업이나 문제가 민첩한 팀에 할당되어 다른 팀의 반복으로 이동하는 경우 팀 할당은 변경되지 않습니다.
* 작업이나 문제가 팀에 할당되지 않은 경우 반복을 담당하는 팀에 작업이나 문제가 할당됩니다.
* 반복에 상위 작업을 추가할 수 없습니다. 하위 작업을 추가하면 상위 작업이 스크럼 보드에 수영선으로 나타납니다.

1. 반복에 추가할 작업이나 문제가 포함된 프로젝트, 보고서 또는 대시보드로 이동합니다.
1. 하나 이상의 작업이나 문제를 선택합니다.
1. 클릭 **[!UICONTROL 자세히]** ![](assets/more-icon.png) > **[!UICONTROL 반복에 추가]**.\
   민첩하지 않은 팀에 할당된 작업이나 문제를 할당할 수 없습니다.

1. 에서 **[!UICONTROL 스토리 추가]** 상자에 이터레이션의 이름을 입력합니다.

   >[!NOTE]
   >
   >기존 이터레이션에서 새 이터레이션으로 스토리를 이동할 수 있습니다.

1. 작업을 추가하는 경우 **[!UICONTROL 스토리 추가]**.\
   또는\
   문제를 추가하는 경우 **[!UICONTROL 문제 추가]**.
