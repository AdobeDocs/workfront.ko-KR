---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 포트폴리오 삭제 및 비활성화
description: Portfolio은 Adobe Workfront의 프로젝트 또는 프로그램 컬렉션입니다. 시스템과 관련이 없는 포트폴리오를 삭제하거나 비활성화할 수 있습니다.
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 포트폴리오 삭제 및 비활성화

Portfolio은 의 프로젝트 또는 프로그램 컬렉션입니다. [!DNL Adobe Workfront]. 시스템과 관련이 없는 포트폴리오를 삭제하거나 비활성화할 수 있습니다.

포트폴리오를 삭제하는 대신 더 이상 향후 프로젝트와 연결할 필요가 없는 포트폴리오는 비활성화하여 현재 포트폴리오 및 해당 프로그램과 연결된 프로젝트에 대한 내역 정보를 유지하는 것이 좋습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스*</td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 Portfolio에 대한 [!UICONTROL 편집] 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 변경할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>포트폴리오에 대한 [!UICONTROL 관리] 권한 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 포트폴리오 삭제 및 비활성화 개요

포트폴리오 삭제 또는 비활성화 여부를 결정할 때 다음 사항을 고려하십시오.

* 포트폴리오를 삭제하면 포트폴리오와 연결된 프로그램이 삭제됩니다.

  >[!IMPORTANT]
  >
  >포트폴리오를 삭제할 수 있도록 프로그램에 대한 권한이 필요하지 않습니다.

* 포트폴리오를 삭제해도 포트폴리오와 연결된 프로젝트는 삭제되지 않습니다.
* 삭제된 포트폴리오는 복구할 수 없습니다.
* 포트폴리오를 비활성화하면 프로젝트를 만들 때 더 이상 포트폴리오 및 해당 프로그램의 이름을 프로젝트에 할당할 수 없습니다.

## 포트폴리오 비활성화

포트폴리오를 비활성화해도 다음에서 액세스할 수 있습니다 [!UICONTROL Portfolio] 영역이지만 사용자가 프로젝트에 추가하려고 할 때 포트폴리오 목록에 더 이상 표시되지 않습니다.

>[!NOTE]
>
>다음 방법에 따라 [!DNL Workfront] 또는 그룹 관리자가 레이아웃 템플릿을 구성합니다. [!UICONTROL Portfolio] 영역에 표시되지 않을 수 있음 [!UICONTROL 메인 메뉴]. 자세한 내용은 [레이아웃 템플릿을 사용하여 메인 메뉴 사용자 정의](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront].

1. 클릭 **[!UICONTROL Portfolio]** .
1. 포트폴리오의 이름을 클릭합니다.
1. 기타 메뉴 클릭 ![](assets/more-icon.png) 포트폴리오 이름의 오른쪽에 있는 **[!UICONTROL Portfolio 비활성화]**.

## 포트폴리오 삭제

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront 오른쪽 상단에 있습니다.

1. 클릭 **[!UICONTROL Portfolio]** .
1. 포트폴리오를 선택한 다음 **[!UICONTROL 삭제]**&#x200B; [!UICONTROL 삭제] 아이콘 ![](assets/delete.png).
1. 표시되는 상자에서 **[!UICONTROL 예, 삭제합니다.]** 확인할 수 있습니다.
