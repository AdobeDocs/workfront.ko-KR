---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 시스템 전체 필터, 보기 및 그룹화 만들기, 편집 및 공유
description: 기본 필터, 보기 및 그룹화를 만든 다음 조직의 사용자가 사용할 수 있도록 할 수 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 4fbf88c544cd56887e6f6f36d7aabfa0668a2a05
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# 시스템 전체 필터, 보기 및 그룹화 만들기, 편집 및 공유

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

필터, 보기 및 그룹화를 만들어 조직의 시스템 전체 사용자가 사용할 수 있도록 할 수 있습니다.

이 문서에 설명된 대로 시스템 전체 필터, 보기 및 그룹화를 만들면 공유한 사용자가 해당 목록을 볼 때 활용할 수 있습니다. 사용자는 사용자가 만든 필터, 보기 및 그룹화를 기반으로 고유한 필터, 보기 및 그룹화를 만들 수 있지만 직접 변경할 수는 없습니다.

사용자가 만드는 시스템 전체 필터, 보기 및 그룹화는 Adobe Workfront이 시스템에서 자동으로 만드는 기본 필터, 보기 및 그룹화와 다릅니다. 이러한 기본 필터, 보기 및 그룹화는 편집하거나 삭제할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
   <td><p>새로운 기능: [!UICONTROL Standard]</p>
   또는
   <p>현재: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL 시스템 관리자]</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 필터, 보기 또는 그룹화 만들기

{{step-1-to-setup}}


1. **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음 **[!UICONTROL 필터]**, **[!UICONTROL 보기]** 또는 **[!UICONTROL 그룹화]** 중 하나를 클릭합니다.

1. 필터, 보기 또는 그룹화를 만드는 경우 **[!UICONTROL 필터 추가]**, **[!UICONTROL 보기 추가]** 또는 **[!UICONTROL 그룹화 추가]**&#x200B;를 클릭한 다음 새 필터, 보기 또는 그룹화를 연결할 개체 형식을 선택합니다.

   또는

   기존 필터, 보기 또는 그룹화를 편집하는 경우 해당 필터를 선택한 다음 **[!UICONTROL 편집]** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.

1. 필터, 보기 또는 그룹화를 구성합니다.

   사용 가능한 옵션에 대한 자세한 내용은 다음 문서 중 하나를 참조하십시오.

   * [필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [!UICONTROL Adobe Workfront][&#128279;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)의 보기 개요
   * [[!UICONTROL Adobe Workfront]의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 왼쪽 아래 모서리 근처에 있는 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

시스템의 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 할 수 있습니다. 다른 사용자와 필터, 보기 또는 그룹화를 공유하는 방법에 대한 자세한 내용은 이 문서의 [사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 만들기](#make-filters-views-or-groupings-available-to-users) 섹션을 참조하십시오.


## 모든 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 설정 {#make-filters-views-or-groupings-available-to-users}

시스템에서 필터, 보기 또는 그룹화를 표시하거나 숨기도록 선택할 수 있습니다. 표시되는 필터는 시스템 전체에서 모든 사용자가 사용할 수 있습니다. 이 설정은 레이아웃 템플릿을 포함한 전체 시스템에 대해 온/오프 스위치처럼 작동합니다.

특정 사용자에게서 필터, 보기 또는 그룹화를 숨기려면 시스템 전체에서 끄지 않고 레이아웃 템플릿을 사용하는 것이 좋습니다.

>[!NOTE]
>
>* 사용자가 필터, 보기 또는 그룹화를 적극적으로 사용하고 관리자가 비활성화하는 경우 새 필터, 보기 또는 그룹화를 선택할 때까지 사용자는 계속 액세스할 수 있습니다. 새 버전을 선택하면 더 이상 숨겨진 상태로 되돌릴 수 없습니다.
>* 레이아웃 템플릿을 통해 모든 필터, 보기 및 그룹화가 제한되거나 시스템 전체에서 비활성화되는 경우 시스템에 표시되는 항목이 있으므로 기본 옵션이 표시됩니다.

필터, 보기 또는 그룹화를 표시하거나 숨기려면:

{{step-1-to-setup}}

1. **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음 **[!UICONTROL 필터]**, **[!UICONTROL 보기]** 또는 **[!UICONTROL 그룹화]** 중 하나를 클릭합니다.

1. (조건부) 사용자가 사용할 수 있도록 할 필터, 보기 또는 그룹화를 선택한 다음 **[!UICONTROL 시스템 전체에서 사용]**&#x200B;을 클릭합니다.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >대부분의 사용자가 사용할 수 있는 필터, 보기 또는 그룹화는 유지하지만 다른 사용자는 숨기려면 레이아웃 템플릿을 사용할 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)을 참조하십시오.

1. (조건부) 사용자로부터 숨기려는 필터, 보기 또는 그룹화를 선택한 다음 **[!UICONTROL 시스템 전체에서 사용 안 함]**&#x200B;을 클릭합니다. 이제 필터, 보기 또는 그룹화가 레이아웃 템플릿과 시스템 전체의 사용자 모두에서 숨겨집니다.


## 특정 사용자와 사용자 정의 필터, 보기 또는 그룹화 공유

다음 단계에서는 [!UICONTROL 설정]의 [!UICONTROL 인터페이스] 영역에서 공유 대화 상자를 사용하여 특정 사용자와 사용자 지정 필터, 보기 및 그룹화를 공유하는 방법을 설명합니다. 본인 또는 다른 사용자가 만든 필터, 보기 및 그룹화에 대한 보기 또는 관리 액세스 권한을 부여할 수 있습니다. 시스템 기본값을 사용자와 공유할 수 없습니다.


{{step-1-to-setup}}

1. **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음 **[!UICONTROL 필터]**, **[!UICONTROL 보기]** 또는 **[!UICONTROL 그룹화]** 중 하나를 클릭합니다.

1. 공유할 필터, 보기 또는 그룹화를 선택한 다음 **[!UICONTROL 공유]** 아이콘 ![공유 아이콘](assets/share-icon.png)을 클릭합니다.
1. 필터, 보기 또는 그룹화를 공유할 특정 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력한 다음 드롭다운 목록에 표시될 때 이름을 클릭합니다.

   공유에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

1. 사용자, 팀, 역할, 그룹 또는 회사 이름 옆에 있는 **보기** 또는 **관리**&#x200B;를 선택하세요. 권한을 미세 조정하려면 슬라이더 아이콘을 클릭하고 권한을 조정합니다.

   ![권한 미세 조정](assets/fine-tune-permissions.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다. 지정한 사용자는 이제 연결된 개체 유형을 볼 때 필터, 보기 또는 그룹화를 상호 작용할 수 있습니다.


## 필터, 보기 및 그룹화 삭제

{{step-1-to-setup}}

1. **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음 **[!UICONTROL 필터]**, **[!UICONTROL 보기]** 또는 **[!UICONTROL 그룹화]** 중 하나를 클릭합니다.

1. 목록에서 하나 이상의 항목을 선택한 다음 **[!UICONTROL 삭제]** 아이콘 ![삭제 아이콘](assets/delete.png)을 클릭합니다.

1. 표시되는 **삭제** 대화 상자에서 **예, 삭제**&#x200B;을 클릭합니다.
