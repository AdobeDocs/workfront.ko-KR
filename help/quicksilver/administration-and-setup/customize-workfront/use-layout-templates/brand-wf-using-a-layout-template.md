---
title: 레이아웃 템플릿을 사용한 Adobe Workfront 브랜드
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 특정 그룹, 팀, 작업 역할 및 사용자에 대해 상단 탐색 영역 및 메인 메뉴의 로고를 사용자 정의할 수 있습니다. 이는 자체 브랜딩이 있는 대규모 조직의 그룹에 특히 유용합니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용한 Adobe Workfront 브랜드

<!--Audited: 09/2024-->

>[!IMPORTANT]
>
>이 페이지에 설명된 프로시저는 [!DNL Adobe Experience Cloud]에 아직 온보딩되지 않은 조직에만 적용됩니다.
>
> 조직이 [!DNL Adobe Experience Cloud]에 온보딩된 경우 브랜딩을 사용할 수 없습니다.

레이아웃 템플릿을 사용하여 특정 그룹, 팀, 작업 역할 및 사용자에 대해 상단 탐색 영역 및 메인 메뉴의 로고를 사용자 정의할 수 있습니다. 이는 자체 브랜딩이 있는 대규모 조직의 그룹에 특히 유용합니다.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

>[!NOTE]
>
>[Adobe Workfront 인스턴스 브랜딩](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)에 설명된 대로 Workfront 관리자는 시스템 수준에서 전체 조직에 대해 동일한 브랜딩 사용자 지정을 수행할 수 있습니다. 그러나 레이아웃 템플릿의 브랜딩은 시스템 수준 브랜딩을 무시합니다.
><!--
>Maybe add a section about deleting these 2 settings to revert to default branding?
>-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>새로운 기능: 표준</p>
  <p> 현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레이아웃 템플릿을 사용한 Adobe Workfront 브랜드

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.
1. **사용자에게 표시되는 항목 사용자 지정** 아래의 아래쪽 화살표 ![](assets/dropdown-arrow.png)을(를) 클릭한 다음 **브랜딩**&#x200B;을(를) 클릭합니다.
1. 이 레이아웃 템플릿이 할당된 사용자를 위해 브랜딩 이미지로 Workfront을 사용자 정의하려면 다음 중 하나를 변경하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>홈 아이콘 <span style="font-weight: normal;">(위쪽 탐색 영역의 맨 왼쪽에 표시됨)</span>에 브랜딩합니다.</p> </td> 
      <td> <p><strong>위쪽 탐색 영역</strong> 섹션의 <strong>홈 아이콘</strong>에서 상자의 아무 곳이나 클릭한 다음 로고 이미지를 찾아 선택합니다. 또는 이미지를 상자로 드래그합니다.</p> <p>이미지를 자르려면 스크롤 컨트롤을 사용하고 이미지를 지정된 공간 내에서 원하는 위치로 드래그합니다.</p> <p>120 x 120 이미지를 사용하는 것이 좋습니다. GIF, JPG, PNG, SVG 형식 중 하나일 수 있습니다.</p> <p>이 아이콘은 사용자가 PDF 파일로 내보내는 보고서, 목록, 대시보드 및 게재된 보고서에도 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>주 메뉴 <img src="assets/main-menu-icon.png"> 로고 <span style="font-weight: normal;"> 브랜딩(주 메뉴의 오른쪽 위 모서리에 표시)</span></p> </td> 
      <td> <p> <p> <p><strong>위쪽 탐색 영역</strong> 섹션의 <strong>기본 메뉴 로고</strong>에서 상자의 아무 곳이나 클릭한 다음 로고 이미지를 찾아 선택합니다. 또는 이미지를 상자로 드래그합니다.</p> <p>이미지를 자르려면 스크롤 컨트롤을 사용하고 이미지를 지정된 공간 내에서 원하는 위치로 드래그합니다.</p> <p>300 x 120픽셀 이미지를 사용하는 것이 좋습니다. GIF, JPG, PNG, SVG 형식 중 하나일 수 있습니다.</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**&#x200B;을 클릭합니다.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.
