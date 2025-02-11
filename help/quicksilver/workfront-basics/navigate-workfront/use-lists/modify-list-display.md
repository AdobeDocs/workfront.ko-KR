---
navigation-topic: use-lists
title: 목록 표시 방법 수정
description: ' [!DNL Adobe Workfront]에서 목록을 표시하는 방법을 사용자 지정할 수 있습니다. 목록을 보는 다른 사용자에게는 변경 사항이 표시되지 않습니다.'
feature: Get Started with Workfront
author: Nolan
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# 목록 표시 방법 수정

<!--Audited: 11/2024-->

[!DNL Adobe Workfront]에서 목록을 표시하는 방법을 사용자 지정할 수 있습니다. 목록을 보는 다른 사용자에게는 변경 사항이 표시되지 않습니다.

다음과 같은 사용자 정의를 수행할 수 있습니다.

* 표시되는 항목 수
* 열 너비 또는 순서
* 그룹화를 확장할지 축소할지 여부

>[!NOTE]
>
>[!DNL Workfront]에서 로그아웃하거나 브라우저를 닫으면 위의 표시 변경 내용이 되돌아갑니다. 이러한 변경 사항은 8시간 후에 되돌릴 수도 있습니다.

위의 임시 사용자 지정 외에도, 로그아웃하거나 브라우저를 닫은 후에도 [!DNL Workfront]이(가) 유지하는 목록의 정렬 기준 열을 조정할 수도 있습니다. 그러나 다른 사용자가 목록 보기에서 정렬 옵션을 편집하면 이전 정렬 선택은 유지되지 않습니다.

목록에 표시되는 정보를 수정하는 방법에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>기여자 이상 </p></li>
   </ul>

<p>현재:</p>
   <ul><li><p>요청 이상</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>목록이 있는 영역에 대한 [!UICONTROL 보기] 액세스 권한</p> <p>예를 들어 프로젝트의 보기를 수정하려면 프로젝트에 대한 [!UICONTROL 보기] 액세스 권한이 필요합니다.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>목록에 적용된 보기에 대한 [!UICONTROL 보기] 이상 권한</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 목록 수정

1. [!DNL Workfront]에서 수정할 목록으로 이동합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (선택 사항 및 조건부) 목록의 그룹화가 축소되어 추가 정보를 보려면 원하는 그룹화를 클릭하여 목록을 확장하고 나열된 정보를 표시합니다.

   또는

   모든 그룹화를 확장하려면 열 머리글에서 확인란 오른쪽에 있는 화살표를 클릭합니다.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (선택 사항 및 조건부) 특정 개수의 항목을 화면에 표시하려면 화면의 오른쪽 하단에 있는 **[!UICONTROL 표시]** 드롭다운 메뉴를 클릭한 다음 **100**, **250**, **500**, **[!UICONTROL 모두]** 또는 **2000** 항목을 표시하도록 선택하십시오.

   ![페이지의 목록 번호](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >기본적으로 업데이트된 목록에 대해서는 2,000개 항목이 표시되고 이전 목록에 대해서는 100개 항목이 표시됩니다. 목록에 항목이 2,000개를 초과하는 경우 모든 항목을 한 페이지에 표시할 수 없습니다.
   >
   >
   >오브젝트에 서식이 지정된 텍스트 필드가 있는 큰 목록에서 최상의 성능을 얻으려면 이 숫자를 250으로 제한하는 것이 좋습니다.
   >
   >
   >두 목록 유형에 대한 자세한 내용은 문서 [목록 시작 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)에서 [업데이트된 목록과 기존 목록의 차이점](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 섹션을 참조하십시오.

   목록의 결과는 페이지당 선택한 항목 수를 표시하도록 페이지가 지정됩니다. 뒤로 및 앞으로 화살표를 클릭하거나 특정 페이지를 선택하여 다른 페이지의 결과에 액세스할 수 있습니다.

1. 열 너비의 크기를 조정하려면 2개의 열을 구분하는 선 위로 마우스를 가져간 다음 클릭하여 원하는 너비로 끕니다.

   브라우저에서 캐시를 지우거나 열의 크기를 수동으로 다시 조정할 때까지 열의 크기가 조정됩니다.

1. 목록의 열 순서를 바꾸려면 열 머리글 위로 마우스를 가져가 손 도구를 표시한 다음 를 클릭하여 열을 표시할 위치로 끕니다.

   페이지를 새로 고칠 때까지 열의 위치가 저장됩니다.

   목록에 있는 열의 너비와 순서를 사용자 지정하는 방법에 대한 자세한 내용은 문서 [열 너비와 순서 수정](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)을 참조하십시오.

1. 목록의 정렬 순서를 조정하려면 열 머리글을 클릭하여 선택한 다음 키보드에서 CMD 키([!DNL Mac]의) 또는 CTRL 키([!DNL Windows]의)를 누른 채 최대 2개의 추가 열 머리글을 선택하여 정렬합니다.

   목록은 선택한 각 열을 선택한 순서대로 정렬합니다.

   목록의 수정 사항이 모두 즉시 저장됩니다.

   >[!NOTE]
   >
   >[!UICONTROL 설정]의 [!UICONTROL 그룹] 영역에서 그룹을 정렬하는 경우 목록 정렬 방법을 변경할 때 그룹 및 해당 하위 그룹의 계층 보기가 분리되지 않습니다. 하위 그룹은 상위 그룹과 함께 유지됩니다. 목록은 먼저 최상위 그룹별로 정렬됩니다. 그런 다음 각 상위 그룹 아래에서 동일한 수준에 있는 하위 그룹 목록이 함께 정렬됩니다.
