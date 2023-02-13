---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 기본 필터, 보기 및 그룹 만들기, 편집 및 공유
description: 기본 필터, 보기 및 그룹화를 만든 다음 조직의 사용자가 사용할 수 있도록 할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# 기본 필터, 보기 및 그룹 만들기, 편집 및 공유

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

기본 필터, 보기 및 그룹화를 만든 다음 조직의 사용자가 사용할 수 있도록 할 수 있습니다.

이 문서에 설명된 대로 기본 필터, 보기 및 그룹화를 만들면 이러한 필터와 공유하는 사용자는 목록을 볼 때 이를 활용할 수 있습니다. 사용자는 만드는 필터, 보기 및 그룹화를 기반으로 만들 수 있지만 직접 만들 수는 없습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 필터, 보기 또는 그룹화 만들기

{{step-1-to-setup}}

1. 필터를 만들거나 편집 중인지 여부에 따라 다음 중 하나를 수행합니다.

   * 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 필터]**.

   * 클릭 **[!UICONTROL 인터페이스] >** **[!UICONTROL 보기 횟수]**.

   * 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 그룹화]**.

1. 필터, 보기 또는 그룹을 만드는 경우 **[!UICONTROL 필터 추가]**, **[!UICONTROL 보기 추가]**, 또는 **[!UICONTROL 그룹화 추가]**&#x200B;그런 다음 새 필터, 뷰 또는 그룹을 연결할 객체 유형을 선택합니다.

   또는

   기존 필터, 보기 또는 그룹을 편집하는 경우 필터를 선택한 다음 **[!UICONTROL 편집]** 아이콘 ![편집 아이콘](assets/edit-icon.png).

1. 필터, 보기 또는 그룹을 구성합니다.

   사용 가능한 옵션에 대한 자세한 내용은 다음 문서 중 하나를 참조하십시오.

   * [의 필터 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [의 보기 개요 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [의 그룹화 개요 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 클릭 **[!UICONTROL 저장]** 왼쪽 아래 모퉁이에서.

시스템의 사용자가 필터, 보기 또는 그룹을 사용할 수 있도록 만들 수 있습니다. 다른 사용자와 필터, 보기 또는 그룹화를 공유하는 방법에 대한 자세한 내용은 섹션을 참조하십시오 [사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 설정](#make-filters-views-or-groupings-available-to-users) 참조하십시오.


## 레이아웃 템플릿에서 사용할 수 있는 필터, 보기 또는 그룹화를 표시하거나 숨깁니다

레이아웃 템플릿에서 필터, 보기 또는 그룹화를 표시하거나 숨기도록 선택할 수 있습니다. 시스템 전체에서 모든 사용자가 볼 수 있는 필터를 사용할 수 있습니다. 레이아웃 템플릿을 사용하여 특정 사용자 또는 그룹에 대해 표시되는 필터를 숨길 수 있습니다.

>[!NOTE]
>
>사용자가 필터, 보기 또는 그룹을 사용하고 관리자가 비활성화하는 경우 새 필터, 보기 또는 그룹을 선택할 때까지 사용자는 여전히 액세스할 수 있습니다. 새 필터, 보기 또는 그룹을 선택하면 더 이상 숨겨진 필터, 보기 또는 그룹으로 되돌릴 수 없습니다.

레이아웃 템플릿에서 사용할 수 있는 필터, 보기 또는 그룹화를 표시하거나 숨기려면:

1. 클릭 **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음, 다음 중 하나를 클릭합니다. **[!UICONTROL 필터]**, **[!UICONTROL 보기 횟수]**, 또는 **[!UICONTROL 그룹화]**.

1. (조건부) 사용자가 사용할 수 있도록 하려는 필터, 보기 또는 그룹을 선택한 다음 를 클릭합니다 **[!UICONTROL 시스템 전체 사용]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >대부분의 사용자가 필터, 보기 또는 그룹을 사용할 수 있도록 유지하지만 다른 사용자로부터 숨기려면 레이아웃 템플릿을 사용할 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 필터, 보기 및 그룹화 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (조건부) 사용자로부터 숨기려는 필터, 보기 또는 그룹을 선택한 다음 **[!UICONTROL 시스템 전체 사용 안 함]**. 비활성화하면 필터, 보기 또는 그룹화는 시스템 내의 사용자와 레이아웃 템플릿에서 숨겨집니다.


## 모든 사용자가 필터, 보기 또는 그룹화를 사용할 수 있도록 설정 {#make-filters-views-or-groupings-available-to-users}

이러한 단계는 필터, 보기 및 그룹화를 [!UICONTROL 공유] 대화 상자 [!UICONTROL 인터페이스] 영역 [!UICONTROL 설정]. 이 설정은 레이아웃 템플릿을 포함하여 전체 시스템의 켜기/끄기 스위치처럼 작동합니다.

{{step-1-to-setup}}

1. 클릭 **[!UICONTROL 인터페이스]**&#x200B;를 클릭한 다음, 다음 중 하나를 클릭합니다. **[!UICONTROL 필터]**, **[!UICONTROL 보기 횟수]**, 또는 **[!UICONTROL 그룹화]**.

1. 사용자가 사용할 수 있도록 할 필터, 보기 또는 그룹을 선택한 다음 **[!UICONTROL 공유]** 아이콘 ![공유 아이콘](assets/share-icon.png) 열다 [!UICONTROL 필터 액세스], [!UICONTROL 액세스 보기], 또는 [!UICONTROL 그룹화 액세스] 양식.
1. (조건부) 시스템의 모든 사용자가 필터, 보기 또는 그룹을 사용할 수 있도록 하려면 **[!UICONTROL 기어]** 드롭다운 메뉴 ![](assets/gear-menu-for-sharing-items.png)를 클릭한 다음 **[!UICONTROL 시스템 전체에 표시]**. 이제 시스템의 모든 사용자가 필터, 보기 또는 그룹을 볼 수 있습니다.

   또는

   필터, 보기 또는 그룹화를 공유할 특정 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력하고 드롭다운 목록에 표시될 이름을 클릭합니다.

   공유에 대한 자세한 내용은 [개체에 대한 권한 공유 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   지정한 사용자는 연결된 객체 유형을 볼 때 기본 필터, 보기 또는 그룹화가 표시됩니다.

## 필터, 보기 및 그룹화 삭제

{{step-1-to-setup}}

1. 필터, 보기 또는 그룹을 삭제하는지 여부에 따라 다음 중 하나를 수행합니다.

   * 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 필터]**

   * 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 보기 횟수]**

   * 클릭 **[!UICONTROL 인터페이스]** > **[!UICONTROL 그룹화]**

1. 목록에서 항목을 하나 이상 선택한 다음 **[!UICONTROL 삭제]** 아이콘 ![삭제 아이콘](assets/delete.png).
1. 필터, 보기 또는 그룹화 구성에 대한 자세한 내용은 다음 문서 중 하나를 참조하십시오.

   * [의 필터 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [의 보기 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [의 그룹화 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
