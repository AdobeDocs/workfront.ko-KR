---
title: 레이아웃 템플릿을 사용하여 더 보기 메뉴 사용자 지정
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 레이아웃 템플릿을 사용하여 사용자가 Adobe Workfront에서 프로젝트, 작업, 문제, 포트폴리오 및 프로그램 개체를 볼 때 추가 메뉴(3점 메뉴)를 클릭할 때 표시되는 옵션을 결정할 수 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bee0117d-a15b-494a-833a-179a42ae4f74
source-git-commit: 665b15170805feba2b55850faf1b73cdc0416305
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 6%

---

# 레이아웃 템플릿을 사용하여 기타 메뉴 사용자 지정

레이아웃 템플릿을 사용하여 사용자가 Adobe Workfront에서 프로젝트, 작업, 문제, 포트폴리오 및 프로그램 개체를 볼 때 추가 메뉴(3점 메뉴)를 클릭할 때 표시되는 옵션을 결정할 수 있습니다.

![프로젝트에 대한 추가 메뉴 샘플링](assets/more-menu-display-for-project.png)

레이아웃 템플릿 만들기에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)을 참조하십시오.

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md)을 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.</p>
        <p>그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Workfront에서 영역에 대한 기타 메뉴 맞춤화

1. [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)에 설명된 대로 레이아웃 템플릿 작업을 시작합니다.
1. **사용자에게 표시되는 항목 사용자 지정** 드롭다운 메뉴에서 기타 메뉴를 사용자 지정할 개체 형식 이름 또는 Workfront 영역을 클릭합니다.
1. **메뉴 옵션 선택**&#x200B;을 클릭합니다.
1. **메뉴 옵션 선택** 상자에서 다음 중 하나를 수행하여 선택한 Workfront 영역 또는 개체 유형에 대한 기타 메뉴에서 사용자에게 표시될 내용을 결정합니다.

   * 왼쪽 패널에서 섹션을 표시하거나 숨기려면 **표시** ![표시 아이콘](assets/add-secondary-nav-item.png) 또는 **숨기기** ![숨기기 아이콘](assets/delete-secondary-nav-item.png) 아이콘을 클릭합니다. **표시** 또는 **숨기기** 아이콘이 없는 항목은 숨길 수 없습니다.

   * 왼쪽 패널에서 순서를 변경하려면 ![이동 아이콘](assets/move-icon---dots.png)을 끕니다.

1. **완료**&#x200B;를 클릭합니다.
