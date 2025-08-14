---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 포트폴리오 삭제 및 비활성화
description: 포트폴리오는 Adobe Workfront에 있는 프로젝트 또는 프로그램의 컬렉션입니다. 시스템과 관련이 없는 포트폴리오를 삭제하거나 비활성화할 수 있습니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 8a4668a568fde2ca7ee26714caae3cd33efe4eda
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 1%

---

# 포트폴리오 삭제 및 비활성화

<!--Audited: 2/2024-->

포트폴리오는 [!DNL Adobe Workfront]에 있는 프로젝트 또는 프로그램의 컬렉션입니다. 시스템과 관련이 없는 포트폴리오를 삭제하거나 비활성화할 수 있습니다.

포트폴리오를 삭제하는 대신 더 이상 향후 프로젝트와 연결할 필요가 없는 포트폴리오는 비활성화하여 현재 포트폴리오 및 해당 프로그램과 연결된 프로젝트에 대한 내역 정보를 유지하는 것이 좋습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL 계획]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트 및 포트폴리오에 대한 [!UICONTROL 편집] 액세스</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>포트폴리오에 대한 [!UICONTROL 관리] 권한 </p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 포트폴리오 삭제 및 비활성화 개요

포트폴리오 삭제 또는 비활성화 여부를 결정할 때 다음 사항을 고려하십시오.

* 포트폴리오를 삭제하면 포트폴리오와 연결된 프로그램이 삭제됩니다.

  >[!IMPORTANT]
  >
  >포트폴리오를 삭제할 수 있도록 프로그램에 대한 권한이 필요하지 않습니다.

* 포트폴리오를 삭제해도 포트폴리오와 연결된 프로젝트는 삭제되지 않습니다.
* 삭제된 포트폴리오는 복구할 수 없습니다.
* 포트폴리오를 비활성화하면 프로젝트를 만들 때 더 이상 포트폴리오 및 해당 프로그램의 이름을 프로젝트에 할당할 수 없습니다.
* 이미 프로젝트에 첨부된 포트폴리오를 비활성화해도 프로젝트에서 제거되지 않습니다. 프로젝트에서 비활성화된 포트폴리오를 제거하는 경우 프로젝트에 다시 첨부하려면 먼저 다시 활성화해야 합니다.

## 포트폴리오 비활성화

포트폴리오를 비활성화해도 [!UICONTROL 포트폴리오] 영역에서 계속 액세스할 수 있지만 사용자가 포트폴리오를 프로젝트에 추가하려고 하면 포트폴리오 목록에 더 이상 표시되지 않습니다.

>[!NOTE]
>
>[!DNL Workfront] 또는 그룹 관리자가 레이아웃 템플릿을 구성하는 방법에 따라 [!UICONTROL 포트폴리오] 영역이 [!UICONTROL 주 메뉴]에 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 기본 메뉴 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)을 참조하십시오.

{{step1-click-main-menu}}

1. **[!UICONTROL 포트폴리오]** 를 클릭합니다.
1. 포트폴리오의 이름을 클릭합니다.
1. 포트폴리오 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL Portfolio 비활성화]**를 클릭합니다.
포트폴리오가 즉시 비활성화됩니다.
1. (선택 사항) 포트폴리오 이름의 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-icon.png)를 클릭한 다음 **[!UICONTROL Portfolio 활성화]**&#x200B;를 클릭하여 다시 활성화합니다.

## 포트폴리오 삭제

{{step1-to-portfolios}}

1. 다음 중 하나를 수행하십시오.

   * 목록에서 포트폴리오를 선택한 다음 **[!UICONTROL 삭제]** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.
   * 포트폴리오를 클릭하여 열고 포트폴리오 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-icon.png)를 클릭한 다음 **Portfolio 삭제**&#x200B;를 클릭합니다.
1. 확인하려면 **[!UICONTROL 예, 삭제]**&#x200B;를 클릭하세요.

   포트폴리오가 삭제되며 복구할 수 없습니다.
