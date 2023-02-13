---
product-area: resource-management
navigation-topic: resource-planning
title: 링크와 리소스 계획자 사용자 보기 공유
description: Adobe Workfront은 대시보드에 외부 페이지로 포함할 수 있는 리소스 계획자의 사용자 보기에 대한 고유 URL을 생성하거나 새 브라우저 탭에서 별도로 열 수 있습니다. 이 기능은 리소스 영역에 직접 액세스할 수 없는 사용자와 리소스 계획자 정보를 공유할 때 유용합니다.
author: Alina
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 링크와 리소스 계획자 사용자 보기 공유

Adobe Workfront은 대시보드에 외부 페이지로 포함할 수 있는 리소스 계획자의 사용자 보기에 대한 고유 URL을 생성하거나 새 브라우저 탭에서 별도로 열 수 있습니다. 이 기능은 리소스 영역에 직접 액세스할 수 없는 사용자와 리소스 계획자 정보를 공유할 때 유용합니다.

![](assets/rp-user-view-with-link-highlight-350x49.png)

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 관리, 프로젝트 및 사용자에 대한 액세스 권한 보기 이상</p> <p>재무 데이터에 대한 액세스를 보고 비용 정보를 조회합니다. </p> <p><b>참고</b> 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>리소스 계획자에 표시할 프로젝트에 대한 보기 또는 더 높은 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.


리소스 계획자의 사용자 뷰에 대한 고유 URL을 생성할 때는 다음 사항을 고려하십시오.

* 사용자 보기에 대해서만 고유 URL을 가져올 수 있습니다. URL 생성 옵션이 프로젝트 또는 역할 보기에 없습니다.
* Work 및 Review 라이선스가 있는 사용자를 포함하여 다른 사용자와 URL을 공유할 수 있습니다.\
   사용자와 공유하는 URL에서 리소스 플래너의 정보를 보려면 다른 사용자를 볼 수 있는 액세스 권한이 있어야 합니다.
* 다른 사용자와 URL을 공유할 때 다음 정보가 저장됩니다.

   * 기간 유형(주, 월, 분기)입니다.
   * 적용하는 필터.
   * 표시 유형(시간 또는 FTE)입니다.

리소스 플래너의 사용자 뷰에서 고유한 URL을 가져와 다른 사용자와 공유하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **리소스**.
1. 에서 을(를) 선택합니다. **사용자별 보기**.
1. (선택 사항) 자원 계획자에서 정보를 조회할 기간을 선택합니다. 다음 중에서 선택합니다.

   * 주
   * 월
   * 분기

1. (선택 사항) 정보를 볼 것인지 여부를 선택합니다 **FTE** 또는 **시간**.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. (선택 사항) 리소스 계획자에 필터를 적용합니다.\
   필터 적용에 대한 자세한 내용은 [리소스 계획자에서 정보 필터링](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. 을(를) 클릭합니다. **하이퍼링크** 아이콘.\
   ![RP_Storm_generate_URL_with_copy_URL_link.png](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. 클릭 **URL 복사**.\
   이렇게 하면 사용자 보기에서 리소스 플래너의 고유 URL이 클립보드에 복사됩니다.

1. (선택 사항) 다음 중 하나를 수행합니다.  

   * URL을 다른 애플리케이션에 붙여 넣어 다른 사용자에게 보냅니다.\
      사용자 보기에서 리소스 계획자를 보려면 Workfront에 로그인해야 합니다.
   * 새 브라우저 탭이나 창을 열고 복사한 링크를 붙여넣은 다음, 키보드에서 Enter 키를 눌러 새 탭이나 창에서 Resource Planner를 엽니다.
   * 다음을 수행합니다.

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. 이동 **보고**>**대시보드**>**새 대시보드**>**외부 페이지 추가.**

      1. 클립보드로 복사한 링크를 **URL** 필드.
      1. 클릭 **저장**, 그런 다음 **저장 + 닫기**.\
         그러면 URL이 대시보드에 포함되고 리소스 계획자의 사용자 보기가 별도의 대시보드에 표시됩니다.

1. (선택 사항) URL을 대시보드에 포함시킨 경우 레이아웃 템플릿에 추가하거나 리소스 관리 영역에 액세스할 수 없는 다른 사용자와 공유하는 것이 좋습니다.\
   레이아웃 템플릿에 대시보드를 추가하는 방법에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   대시보드 공유에 대한 자세한 내용은 [대시보드 공유](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   공유 URL을 볼 때 사용자는 처음에 Resource Planner에 적용한 설정으로 정보를 볼 수 있습니다. 공유 URL을 보려면 Workfront에 로그인해야 합니다.\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
