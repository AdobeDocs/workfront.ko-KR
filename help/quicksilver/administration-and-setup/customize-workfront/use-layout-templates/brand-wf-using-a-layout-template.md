---
title: 레이아웃 템플릿을 사용하여 Adobe Workfront 브랜드
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Adobe Workfront 관리자 또는 그룹 관리자는 레이아웃 템플릿을 사용하여 위쪽 탐색 영역과 특정 그룹, 팀, 작업 역할 및 사용자에 대한 기본 메뉴에서 로고를 사용자 지정할 수 있습니다. 이 기능은 브랜딩이 고유한 대규모 조직의 그룹에 특히 유용합니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: 7b5b0fd95e39f37153e36abb4e3b8e738ac26d21
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 Adobe Workfront 브랜드

>[!IMPORTANT]
>
>이 페이지에 설명된 절차는 아직 온보딩되지 않은 조직에만 적용됩니다 [!DNL Adobe Experience Cloud].
>
> 조직에 온보딩된 경우 [!DNL Adobe Experience Cloud], 브랜딩을 사용할 수 없습니다.

레이아웃 템플릿을 사용하여 위쪽 탐색 영역과 특정 그룹, 팀, 작업 역할 및 사용자에 대한 기본 메뉴에서 로고를 사용자 지정할 수 있습니다. 이 기능은 브랜딩이 고유한 대규모 조직의 그룹에 특히 유용합니다.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

>[!NOTE]
>
>Workfront 관리자는 다음과 같이 시스템 수준에서 전체 조직에 대해 동일한 브랜딩 사용자 지정을 만들 수 있습니다. [Adobe Workfront 인스턴스 브랜딩](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md). 하지만 레이아웃 템플릿의 브랜딩은 시스템 수준 브랜딩을 무시합니다.
><!--
>Maybe add a section about deleting these 2 settings to revert to default branding?
>-->


## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 해당 그룹을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 레이아웃 템플릿을 사용하여 Adobe Workfront 브랜드

1. 에 설명된 대로 레이아웃 템플릿 작업을 시작합니다. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 아래쪽 화살표를 클릭합니다 ![](assets/dropdown-arrow.png) 아래에 **사용자에게 표시되는 항목 사용자 지정**&#x200B;를 클릭한 다음 **브랜딩**.
1. 이 레이아웃 템플릿을 지정한 사용자에 대한 브랜드 이미지를 사용하여 Workfront을 사용자 지정하려면 다음 중 하나를 변경합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>홈 아이콘 브랜딩 <span style="font-weight: normal;">(위쪽 탐색 영역의 맨 왼쪽에 표시)</span></p> </td> 
      <td> <p>에서 <strong>위쪽 탐색 영역</strong> 섹션 아래의 <strong>홈 아이콘</strong>을 클릭하고 상자에서 아무 곳이나 클릭한 다음 로고 이미지를 찾아 선택합니다. 또는 이미지를 상자로 드래그합니다.</p> <p>이미지를 자르려면 스크롤 컨트롤을 사용하고 지정된 공간 내에서 원하는 위치로 이미지를 드래그합니다.</p> <p>120 x 120 이미지를 권장합니다. 다음 형식을 사용할 수 있습니다. GIF, JPG, PNG, SVG.</p> <p>이 아이콘은 사용자가 PDF 파일로 내보내는 보고서, 목록, 대시보드 및 게재된 보고서에도 나타납니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>기본 메뉴 브랜딩 <img src="assets/main-menu-icon.png"> 로고 <span style="font-weight: normal;">(주 메뉴의 오른쪽 위 모서리에 표시)</span></p> </td> 
      <td> <p> <p> <p>에서 <strong>위쪽 탐색 영역</strong> 섹션 아래의 <strong>기본 메뉴 로고</strong>을 클릭하고 상자에서 아무 곳이나 클릭한 다음 로고 이미지를 찾아 선택합니다. 또는 이미지를 상자로 드래그합니다.</p> <p>이미지를 자르려면 스크롤 컨트롤을 사용하고 지정된 공간 내에서 원하는 위치로 이미지를 드래그합니다.</p> <p>300 x 120 픽셀 이미지를 권장합니다. 다음 형식을 사용할 수 있습니다. GIF, JPG, PNG, SVG.</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 완료한 경우 을 누릅니다 **저장**.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상태를 저장한 다음 나중에 계속 템플릿을 수정할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
