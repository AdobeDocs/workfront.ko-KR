---
product-area: resource-management
navigation-topic: resource-planning
title: 링크와 리소스 플래너 사용자 보기 공유
description: Adobe Workfront은 대시보드에 외부 페이지로 포함할 수 있는 리소스 플래너의 사용자 보기에 대한 고유 URL을 생성하거나 새 브라우저 탭에서 별도로 열 수 있습니다. 이 기능은 리소스 조달 영역에 직접 액세스할 수 없는 사용자와 리소스 플래너 정보를 공유할 때 유용합니다.
author: Lisa
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# 링크와 리소스 플래너 사용자 보기 공유

Adobe Workfront은 대시보드에 외부 페이지로 포함할 수 있는 리소스 플래너의 사용자 보기에 대한 고유 URL을 생성하거나 새 브라우저 탭에서 별도로 열 수 있습니다. 이 기능은 리소스 조달 영역에 직접 액세스할 수 없는 사용자와 리소스 플래너 정보를 공유할 때 유용합니다.

![](assets/rp-user-view-with-link-highlight-350x49.png)

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
    <td><p>새로 만들기: 모두</p>
       <p>또는</p>
       <p>현재: Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>리소스 관리, 프로젝트 및 사용자에 대한 보기 이상의 액세스 권한</p> <p>재무 데이터에 대한 액세스를 보고 비용 정보를 봅니다.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>리소스 플래너에 표시할 프로젝트에 대한 이상의 권한 보기</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


리소스 플래너의 사용자 보기에 대한 고유 URL을 생성할 때 다음 사항을 고려하십시오.

* 사용자 보기에 대해서만 고유한 URL을 가져올 수 있습니다. 프로젝트 또는 역할 보기에 URL을 생성하는 옵션이 없습니다.
* 작업 및 검토 라이선스가 부여된 사용자를 포함하여 다른 사용자와 URL을 공유할 수 있습니다.\
  리소스 플래너의 정보를 다른 사용자와 공유하려면 리소스 플래너에 있는 URL에서 다른 사용자를 볼 수 있는 액세스 권한이 있어야 합니다.
* URL을 다른 사용자와 공유할 때 다음 정보가 저장됩니다.

   * 기간 유형(주, 월, 분기).
   * 적용하는 필터입니다.
   * 표시 유형(시간 또는 FTE).

리소스 플래너의 사용자 보기에서 고유 URL을 가져와서 다른 사용자와 공유하려면 다음 작업을 수행하십시오.

{{step1-to-resourcing}}

1. **사용자별 보기**&#x200B;를 선택합니다.
1. (선택 사항) 리소스 플래너에서 정보를 확인할 기간을 선택합니다. 다음 중에서 선택합니다.

   * 주
   * 월
   * 분기

1. (선택 사항) **FTE** 또는 **시간**&#x200B;을(를) 기준으로 정보를 볼지 여부를 선택합니다.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. (선택 사항) 리소스 플래너에 필터를 적용합니다.\
   필터를 적용하는 방법에 대한 자세한 내용은 [리소스 플래너의 필터 정보](../../resource-mgmt/resource-planning/filter-resource-planner.md) 를 참조하십시오.

1. **하이퍼링크** 아이콘을 클릭합니다.\
   ![RP_Storm_generate_URL_with_copy_URL_link.png](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. **URL 복사**&#x200B;를 클릭합니다.\
   사용자 보기에서 리소스 플래너의 고유 URL을 클립보드에 복사합니다.

1. (선택 사항) 다음 중 하나를 수행합니다.  

   * URL을 다른 애플리케이션에 붙여넣어 다른 사용자에게 보냅니다.\
     사용자 보기에서 리소스 플래너를 보려면 사용자가 Workfront에 로그인해야 합니다.
   * 새 브라우저 탭이나 창을 열고 복사한 링크를 붙여넣은 다음 키보드에서 Enter 키를 클릭하여 리소스 플래너를 새 탭이나 창에서 엽니다.
   * 다음을 수행합니다.

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. **보고**>**대시보드**>**새 대시보드**>**외부 페이지 추가**&#x200B;로 이동합니다.

      1. 클립보드에 복사한 링크를 **URL** 필드에 붙여 넣습니다.
      1. **저장**&#x200B;을 클릭한 다음 **저장 + 닫기**&#x200B;를 클릭합니다.\
         이렇게 하면 URL이 대시보드에 임베드되고 리소스 플래너의 사용자 보기가 별도의 대시보드에 표시됩니다.

1. (선택 사항) URL을 대시보드에 삽입한 경우 레이아웃 템플릿에 추가하거나 리소스 관리 영역에 대한 액세스 권한이 없는 다른 사용자와 공유할 수 있습니다.\
   레이아웃 템플릿에 대시보드를 추가하는 방법에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)를 참조하십시오.\
   대시보드 공유에 대한 자세한 내용은 [대시보드 공유](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) 를 참조하십시오.\
   공유 URL을 볼 때 사용자는 리소스 플래너에 원래 적용한 설정으로 정보를 볼 수 있습니다. 공유 URL을 보려면 Workfront에 로그인해야 합니다.\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
