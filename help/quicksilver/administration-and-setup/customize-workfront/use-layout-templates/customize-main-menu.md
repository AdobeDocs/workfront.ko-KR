---
title: 레이아웃 템플릿을 사용하여 메인 메뉴 사용자 정의
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 사용자가 Workfront에서 메인 메뉴를 열 때 표시되는 옵션을 구성할 수 있습니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 4%

---

# 레이아웃 템플릿을 사용하여 메인 메뉴 사용자 정의

<!--Audited: 01/2024-->

Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 사용자가 Workfront에서 메인 메뉴를 열 때 표시되는 옵션을 구성할 수 있습니다.

![메인 메뉴 옵션](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>사용자가 볼 수 있는 메인 메뉴 옵션은 라이선스 유형과 액세스 수준에서 구성된 설정에 따라 다릅니다. 이 레이아웃 템플릿을 사용할 일부 사용자에게는 여기에서 선택한 일부 옵션이 표시되지 않을 수 있습니다. 자세한 내용은 [액세스 수준 및 권한이 함께 작동하는 방식](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) 및 [각 객체 유형에 대한 기능에 대한 구성 가능한 액세스](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md).

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td><p>현재:플랜</p>
   또는
   <p>새로운 기능: 표준</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.</p>
    <p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*액세스 요구 사항에 대한 자세한 내용은 다음을 참조하십시오. [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 메인 메뉴 사용자 정의

1. 에 설명된 대로 레이아웃 템플릿에서 작업 시작 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 클릭 **메인 메뉴 설정** 템플릿의 오른쪽 상단 모서리에서 참조할 수 있습니다.

   주 메뉴 상자가 열리면 템플릿의 주 메뉴에 현재 표시된 영역과 추가할 수 있는 항목을 볼 수 있습니다. 추가할 수 있는 모든 항목은 다음과 같습니다.
   * 홈

     >[!TIP]
     >
     >기본적으로 홈 영역 외에 기본 메뉴의 내 업데이트 영역을 포함하는 프로필과 연결된 레이아웃 템플릿이 없는 경우 기본 메뉴의 홈 아이콘에는 검토 라이선스 사용자(현재 라이선스 계획)의 내 업데이트 영역이 표시됩니다.

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
     >시나리오 플래너에는 추가 라이센스가 필요합니다. Workfront 시나리오 플래너에 대한 자세한 내용은 다음을 참조하십시오. [시나리오 플래너 개요](../../../scenario-planner/scenario-planner-overview.md).

   * 팀
   * 사용자

     >[!NOTE]
     >
     >현재 라이선스 모델에서 플랜 라이선스가 있는 사용자 또는 새 라이선스 모델에서 Standard 라이선스가 있는 사용자만 사용자 영역을 볼 수 있습니다. ![](assets/users-icon-in-main-menu.png) 기본 메뉴 아래의 제품에서 사용할 수 있습니다.

   * 요청
   * 타임시트
   * 문서
   * 템플릿
   * 분석
   * 증명
   * 목표

     >[!NOTE]
     >
     >목표에 대해서는 추가 라이센스가 필요합니다. Workfront 목표에 대한 자세한 내용은 다음을 참조하십시오. [Adobe Workfront 목표 개요](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * 내 업데이트
   * 보드
   * 블루프린트

1. 다음 중 하나를 수행합니다.

   * 숨기기 ![](assets/remove-icon---x-in-circle.png) **활성 항목** 표시하지 않으려는 경우
   * 표시 ![](assets/add-icon-plus-in-circle.png) **사용 가능한 항목** 기본 메뉴에 표시할 수 있습니다.
   * 드래그 ![](assets/move-icon---dots.png) **활성 항목** 메인 메뉴의 표시 순서를 변경합니다.

1. 클릭 **완료**.

   다음을 클릭할 수도 있습니다. **취소** 언제든지 변경 사항을 취소하려면 을 클릭합니다.

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
