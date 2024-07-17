---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 기본 필터, 보기 및 그룹화 만들기, 편집 및 공유
description: 기본 필터, 보기 및 그룹화를 만든 다음 조직의 사용자가 사용할 수 있도록 할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# 기본 필터, 보기 및 그룹화 만들기, 편집 및 공유

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

기본 필터, 보기 및 그룹화를 만든 다음 조직의 사용자가 사용할 수 있도록 할 수 있습니다.

이 문서에 설명된 대로 기본 필터, 보기 및 그룹화를 만들면 공유하는 사용자는 목록을 볼 때 활용할 수 있습니다. 사용자는 사용자가 만든 필터, 보기 및 그룹화를 기반으로 고유한 필터, 보기 및 그룹화를 만들 수 있지만 직접 만든 필터, 보기 및 그룹화는 변경할 수 없습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 필터, 보기 또는 그룹화 만들기

{{step-1-to-setup}}

1. 필터, 보기 또는 그룹화 생성 또는 편집 여부에 따라 다음 중 하나를 수행하십시오.

   * **[!UICONTROL 인터페이스]** > **[!UICONTROL 필터]**&#x200B;를 클릭합니다.

   * **[!UICONTROL 인터페이스] >** **[!UICONTROL 보기]**&#x200B;를 클릭합니다.

   * **[!UICONTROL 인터페이스]** > **[!UICONTROL 그룹화]**&#x200B;를 클릭합니다.

1. 필터, 보기 또는 그룹화를 만드는 경우 **[!UICONTROL 필터 추가]**, **[!UICONTROL 보기 추가]** 또는 **[!UICONTROL 그룹화 추가]**&#x200B;를 클릭한 다음 새 필터, 보기 또는 그룹화를 연결할 개체 형식을 선택합니다.

   또는

   기존 필터, 보기 또는 그룹화를 편집하는 경우 해당 필터를 선택한 다음 **[!UICONTROL 편집]** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

1. 필터, 보기 또는 그룹화를 구성합니다.

   사용 가능한 옵션에 대한 자세한 내용은 다음 문서 중 하나를 참조하십시오.

   * [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)의 [보기 개요
   * [[!UICONTROL Adobe Workfront]의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 왼쪽 아래 모서리 근처에 있는 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

시스템의 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 할 수 있습니다. 다른 사용자와 필터, 보기 또는 그룹화를 공유하는 방법에 대한 자세한 내용은 이 문서의 [사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 만들기](#make-filters-views-or-groupings-available-to-users) 섹션을 참조하십시오.


## 레이아웃 템플릿에서 사용할 수 있는 필터, 보기 또는 그룹화 표시 또는 숨기기

레이아웃 템플릿에서 필터, 보기 또는 그룹화를 표시하거나 숨기도록 선택할 수 있습니다. 표시된 필터는 시스템 전체에서 모든 사용자가 사용할 수 있습니다. 레이아웃 템플릿을 사용하여 특정 사용자 또는 그룹에 대해 표시되는 필터를 숨길 수 있습니다.

>[!NOTE]
>
>사용자가 필터, 보기 또는 그룹화를 적극적으로 사용하고 관리자가 비활성화하는 경우 새 필터, 보기 또는 그룹화를 선택할 때까지 사용자는 계속 액세스할 수 있습니다. 새 필터, 보기 또는 그룹화를 선택한 후에는 더 이상 숨겨진 필터, 보기 또는 그룹화로 되돌릴 수 없습니다.

레이아웃 템플릿에서 사용할 수 있는 필터, 보기 또는 그룹화를 표시하거나 숨기려면 다음을 수행하십시오.

1. **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음 **[!UICONTROL 필터]**, **[!UICONTROL 보기]** 또는 **[!UICONTROL 그룹화]** 중 하나를 클릭합니다.

1. (조건부) 사용자가 사용할 수 있도록 할 필터, 보기 또는 그룹화를 선택한 다음 **[!UICONTROL 시스템 전체에서 사용]**&#x200B;을 클릭합니다.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >대부분의 사용자가 사용할 수 있는 필터, 보기 또는 그룹화는 유지하지만 다른 사용자는 숨기려면 레이아웃 템플릿을 사용할 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

1. (조건부) 사용자에게 숨기려는 필터, 보기 또는 그룹화를 선택한 다음 **[!UICONTROL 시스템 전체에서 사용 안 함]**&#x200B;을 클릭합니다. 비활성화되면 시스템 내의 사용자는 물론 레이아웃 템플릿에서도 필터, 보기 또는 그룹화가 숨겨집니다.


## 모든 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 설정 {#make-filters-views-or-groupings-available-to-users}

다음 단계에서는 [!UICONTROL 설정]의 [!UICONTROL 인터페이스] 영역에 있는 [!UICONTROL 공유] 대화 상자에서 필터, 보기 및 그룹화를 사용할 수 있도록 설정하는 방법을 설명합니다. 이 설정은 레이아웃 템플릿을 포함한 전체 시스템에 대해 온/오프 스위치처럼 작동합니다.

{{step-1-to-setup}}

1. **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음 **[!UICONTROL 필터]**, **[!UICONTROL 보기]** 또는 **[!UICONTROL 그룹화]** 중 하나를 클릭합니다.

1. 사용자가 사용할 수 있는 필터, 보기 또는 그룹화를 선택한 다음 **[!UICONTROL 공유]** 아이콘 ![공유 아이콘](assets/share-icon.png)을 클릭하여 [!UICONTROL 필터 액세스], [!UICONTROL 보기 액세스] 또는 [!UICONTROL 그룹화 액세스] 양식을 엽니다.
1. (조건부) 시스템의 모든 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 하려면 **[!UICONTROL 톱니바퀴]** 드롭다운 메뉴 ![](assets/gear-menu-for-sharing-items.png)을(를) 클릭한 다음 **[!UICONTROL 시스템 전체에 표시]**&#x200B;를 클릭합니다. 이제 시스템의 모든 사용자가 필터, 보기 또는 그룹화를 볼 수 있습니다.

   또는

   필터, 보기 또는 그룹화를 공유할 특정 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   공유에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 지정한 사용자가 연결된 개체 유형을 볼 때 기본 필터, 보기 또는 그룹화를 볼 수 있습니다.

## 필터, 보기 및 그룹화 삭제

{{step-1-to-setup}}

1. 필터 삭제, 보기 또는 그룹화 여부에 따라 다음 중 하나를 수행하십시오.

   * **[!UICONTROL 인터페이스]** > **[!UICONTROL 필터]**&#x200B;를 클릭합니다

   * **[!UICONTROL 인터페이스]** > **[!UICONTROL 보기]**&#x200B;를 클릭합니다

   * **[!UICONTROL 인터페이스]** > **[!UICONTROL 그룹화]**&#x200B;를 클릭합니다

1. 목록에서 하나 이상의 항목을 선택한 다음 **[!UICONTROL 삭제]** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.
1. 필터, 보기 또는 그룹화 구성에 대한 자세한 내용은 다음 문서 중 하나를 참조하십시오.

   * [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [ [!DNL Adobe Workfront]의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [ [!DNL Adobe Workfront]의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
