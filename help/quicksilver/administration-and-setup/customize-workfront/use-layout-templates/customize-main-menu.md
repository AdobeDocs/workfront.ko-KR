---
title: 레이아웃 템플릿을 사용하여 기본 메뉴 사용자 지정
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 사용자가 Workfront에서 기본 메뉴를 열 때 표시되는 옵션을 구성할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# 레이아웃 템플릿을 사용하여 기본 메뉴 사용자 지정

Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 사용자가 Workfront에서 기본 메뉴를 열 때 표시되는 옵션을 구성할 수 있습니다.

![기본 메뉴 옵션](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>사용자에게 표시되는 기본 메뉴 옵션은 라이선스 유형과 액세스 수준에서 구성되는 설정에 따라 다릅니다. 이 레이아웃 템플릿을 사용할 일부 사용자는 여기에서 선택하는 옵션을 모두 표시하지 않을 수 있습니다. 자세한 내용은 [액세스 수준 및 권한이 함께 작동하는 방법](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) 및 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스</strong></td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 해당 그룹을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 메뉴 사용자 정의

1. 에 설명된 대로 레이아웃 템플릿 작업을 시작합니다. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 클릭 **기본 메뉴 설정** 오른쪽 상단 근처에 있습니다.

   나타나는 기본 메뉴 상자에서 템플릿의 기본 메뉴에서 현재 활성화된 항목과 추가할 수 있는 항목을 볼 수 있습니다. 다음은 추가할 수 있는 모든 가능한 항목입니다.

   * 홈

      >[!TIP]
      >
      >기본 메뉴의 내 업데이트 영역을 포함하는 프로필과 연관된 레이아웃 템플릿이 없는 경우 기본적으로 홈 은 검토 라이선스 사용자를 위한 내 업데이트로 표시됩니다.

   * 포트폴리오
   * 프로그램
   * 프로젝트
   * 보고서
   * 대시보드
   * 캘린더
   * 리소스 조달
   * 시나리오

      >[!NOTE]
      >
      >시나리오 플래너는 새 Adobe Workfront 경험에서만 사용할 수 있으며 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 [시나리오 계획자 개요](../../../scenario-planner/scenario-planner-overview.md).

   * 팀
   * 사용자

      >[!NOTE]
      >
      >계획 라이센스가 있는 사용자만 사용자를 볼 수 있습니다 ![](assets/users-icon-in-main-menu.png) 를 클릭합니다.

   * 요청
   * 타임시트
   * 문서
   * 템플릿
   * 분석
   * 증명
   * 목표

      >[!NOTE]
      >
      >이 경우 추가 라이센스가 필요합니다. Workfront 목표에 대한 자세한 내용은 [Adobe Workfront 목표 개요](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * 내 업데이트
   * 보드
   * 블루프린트

1. 다음 중 하나를 수행합니다.

   * 숨기기 ![](assets/remove-icon---x-in-circle.png) **활성 항목** 표시되지 않을 경우
   * 표시 ![](assets/add-icon-plus-in-circle.png) **사용 가능한 항목** 기본 메뉴에 표시할 구성 요소
   * 드래그 ![](assets/move-icon---dots.png) **활성 항목** 기본 메뉴에서 표시 순서를 변경하려면

1. 클릭 **완료**.

   을 클릭할 수도 있습니다 **취소** 언제든지 변경 사항을 취소하려면

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 완료한 경우 을 누릅니다 **저장**.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상태를 저장한 다음 나중에 계속 템플릿을 수정할 수 있습니다.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
