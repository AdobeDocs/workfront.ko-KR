---
title: 레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 맞춤화
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Workfront 관리자는 레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 드롭다운 메뉴에 나타나는 목록 컨트롤을 지정할 수 있습니다. 이러한 메뉴는 프로젝트의 작업 목록과 같은 Workfront 전체의 목록 위에 표시됩니다.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# 레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 맞춤화

Adobe Workfront 관리자는 레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 드롭다운 메뉴에 나타나는 목록 컨트롤을 지정할 수 있습니다. 이러한 메뉴는 프로젝트의 작업 목록과 같은 Workfront 전체의 목록 위에 표시됩니다.

![](assets/filter-view-grouping-layout-templates.png)

레이아웃 템플릿에 대한 자세한 내용은 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

그룹의 레이아웃 템플릿에 대한 자세한 내용은 [그룹의 레이아웃 템플릿 만들기 및 수정](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

레이아웃 템플릿을 구성한 후에는 다른 사용자가 변경 내용을 볼 수 있도록 사용자에게 할당해야 합니다. 사용자에게 레이아웃 템플릿을 할당하는 방법에 대한 자세한 내용은 [레이아웃 템플릿에 사용자 할당](../use-layout-templates/assign-users-to-layout-template.md).

## 액세스 요구 사항

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
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 수준에서 이러한 단계를 수행하려면 시스템 관리자 액세스 수준이 필요합니다.
그룹에 대해 이러한 작업을 수행하려면 해당 그룹의 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가적인 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 필터, 보기 및 그룹화 목록 컨트롤 사용자 지정:

1. 에 설명된 대로 레이아웃 템플릿에서 작업 시작 [레이아웃 템플릿 만들기 및 관리](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 아래쪽 화살표 클릭 ![](assets/down-arrow-blue.png) 아래에 **사용자에게 표시되는 항목 맞춤화**&#x200B;을 클릭한 다음 을 클릭합니다 **목록** 을 클릭하여 제품에서 사용할 수 있습니다.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. 아래쪽 화살표 클릭 ![](assets/down-arrow-blue.png) 아래에 **사용자 지정할 목록 선택**&#x200B;그런 다음 필터, 보기 및 그룹화 목록 컨트롤을 사용자 지정할 Workfront 개체 유형을 선택합니다.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >사용자 지정할 목록으로 프로젝트를 선택한 다음 필터 섹션에서 내가 진행 중인 프로젝트 또는 내가 소유한 프로젝트를 비활성화하면 사용자에게 해당 필터가 더 이상 표시되지 않거나 사용할 수 없습니다.
   >
   >* 필터 아이콘을 클릭할 때 표시되는 필터 목록에서 ![](assets/filter-nwepng.png) 목록 위:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* 프로젝트 영역 헤더의 헤더에서 다음을 수행합니다.
   >   
   >  ![](assets/disable-filter-pills.png)

1. (선택 사항) 레이아웃 템플릿에 대한 기본 필터, 보기 또는 그룹화를 변경하려면 필터, 보기 또는 그룹화 위로 마우스를 가져간 다음 **기본값으로 설정**.

   선택하는 기본값은 레이아웃 템플릿이 사용자에게 할당될 때 Workfront 전체의 목록에 표시되는 필터, 보기 및 그룹화 사용자를 결정합니다. 이러한 기본값을 변경하지 않으면 다음과 같이 모든 목록이 표시됩니다.

   * **필터**: 모두
   * **보기**: 표준(해당되는 경우, 일부 목록에 이 보기가 없음)
   * **그룹화**: 없음

   다른 기본값을 선택한 후 모두, 표준 및 없음 옵션을 숨길 수 있지만(5단계 참조) 삭제할 수는 없습니다.

   기본값으로 사용되는 다른 옵션은 삭제할 수 있지만 다른 기본값을 먼저 선택해야 합니다.

   필터, 보기 및 그룹화 삭제에 대한 자세한 내용은 [기본 필터, 보기 및 그룹화 만들기, 편집 및 공유](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. 다음과 같이 목록 컨트롤을 숨기고 추가합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">목록 컨트롤 숨기기</td> 
      <td> <p>숨기거나 표시할 목록 컨트롤 옆의 확인란을 선택 취소하거나 선택합니다.</p> <p>확인란이 흐리게 표시되면 해당 목록 컨트롤을 숨길 수 없습니다. 기본값 <img src="assets/default-pill.png"> 현재 기본값으로 구성된 설정을 숨길 수 없으므로 각 목록 컨트롤에 대한 설정은 흐리게 표시됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 지정 목록 컨트롤 추가</td> 
      <td> <p> 
        <ol> 
         <li value="1"> 클릭 <strong>필터 추가</strong>, <strong>보기 추가</strong>, 또는 <strong>그룹화 추가</strong> 필터, 보기 또는 그룹화 목록의 맨 아래. 표시되는 상자에서 이전에 조직에 대해 만든 기존 사용자 지정 목록 컨트롤의 이름을 입력한 다음 표시될 때 이름을 클릭합니다.</li> 
         <li value="2"> 레이아웃 템플릿에 대한 기본 필터, 보기 또는 그룹화로 새 사용자 지정 목록 컨트롤을 설정하려면 <strong>기본값으로 설정</strong>. </li> 
         <li value="3"> <p>클릭 <strong>추가</strong> 다 끝나면</p> <p><b>참고</b>: <p>사용자는 사용자 지정 목록 컨트롤을 자신의 목록에 추가할 수 있습니다. 레이아웃 템플릿에 사용자 지정 목록 컨트롤을 추가하면 목록 컨트롤이 추가되고 목록 컨트롤은 패널 아래쪽으로 이동하며, 목록 컨트롤은 대체되지 않습니다.</p> <p>이는 사용자 지정 목록 컨트롤이 있는 새 레이아웃 템플릿에 사용자를 할당하는 경우에도 마찬가지입니다. </p> <p>목록 컨트롤 사용자 지정에 대한 자세한 내용은 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">필터 개요</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Adobe Workfront의 보기 개요</a>, 및 <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Adobe Workfront의 그룹화 개요</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 레이아웃 템플릿을 계속 사용자 지정합니다.

   또는

   사용자 지정을 마쳤으면 **저장**.

   >[!TIP]
   >
   >언제든지 저장 을 클릭하여 진행 상황을 저장한 다음 나중에 템플릿을 계속 수정할 수 있습니다.
