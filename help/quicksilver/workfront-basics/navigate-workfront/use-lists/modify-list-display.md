---
navigation-topic: use-lists
title: 목록이 표시되는 방식 수정
description: in [!DNL Adobe Workfront]를 사용하여 목록이 표시되는 방식을 사용자 지정할 수 있습니다. 목록을 보는 다른 사용자는 변경 사항을 볼 수 없습니다.
feature: Get Started with Workfront
author: Lisa
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# 목록이 표시되는 방식 수정

in [!DNL Adobe Workfront]를 사용하여 목록이 표시되는 방식을 사용자 지정할 수 있습니다. 목록을 보는 다른 사용자는 변경 사항을 볼 수 없습니다.

다음 사용자 지정을 만들 수 있습니다.

* 표시되는 항목 수
* 열 너비 또는 순서
* 그룹 확장 또는 축소 여부

>[!NOTE]
>
>위에서 변경한 내용은 [!DNL Workfront] 또는 브라우저를 닫습니다. 8시간 후에 이러한 변경 사항을 되돌릴 수도 있습니다.

위의 임시 사용자 지정 외에도 목록을 정렬할 열을 조정할 수 있습니다. [!DNL Workfront] 브라우저를 로그아웃하거나 닫아도 유지됩니다. 그러나 다른 사용자가 목록 보기에서 정렬 옵션을 편집하면 이전 정렬 선택이 유지되지 않습니다.

목록에 표시되는 정보를 수정하는 방법에 대한 자세한 내용은 [보고 요소: 필터, 보기 및 그룹화](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>목록이 있는 영역에 대한 [!UICONTROL 보기] 액세스</p> <p>예를 들어 프로젝트의 보기를 수정하려면 프로젝트에 대한 [!UICONTROL 보기] 액세스 권한이 필요합니다.</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우<br>자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>목록에 적용된 보기에 대한 [!UICONTROL 보기] 이상 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 목록이 표시되는 방식 수정

1. 의 목록으로 이동합니다. [!DNL Workfront] 수정할 수 있습니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (선택 사항 및 조건부) 목록의 그룹화가 축소되어 추가 정보를 보려면 원하는 그룹을 클릭하여 목록을 확장하고 목록에 나열된 정보를 표시합니다.

   또는

   모든 그룹을 확장하려면 열 헤더에서 확인란 오른쪽에 있는 화살표를 클릭합니다.

   ![expand_groups__1_.png](assets/expand-groupings--1--350x227.png)

1. (선택 사항 및 조건부) 화면에 특정 개수의 항목을 표시하려면 **[!UICONTROL 표시]** 화면의 오른쪽 아래 모서리에 있는 드롭다운 메뉴를 선택한 다음 표시를 선택합니다 **100년**, **250년**, **500년**, **[!UICONTROL 모두]**, 또는 **2000년** 항목.

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >기본적으로 업데이트된 목록에 2,000개의 항목이 표시되고, 기존 목록에 100개의 항목이 표시됩니다. 목록에 2,000개 이상의 항목이 포함되어 있으면 한 페이지에 모든 항목을 표시할 수 없습니다.
   >
   >
   >개체에 서식이 지정된 텍스트 필드가 들어 있는 큰 목록의 성능을 최상으로 유지하려면 이 수를 250개로 제한하는 것이 좋습니다.
   >
   >
   >2가지 목록 유형에 대한 자세한 내용은 섹션을 참조하십시오 [업데이트된 목록과 기존 목록 간의 차이점](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 기사 [에서 목록 시작 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   목록 결과는 페이지당 선택한 항목 수를 표시하기 위해 페이지 매김됩니다. 이전 및 이전 화살표를 클릭하거나 특정 페이지를 선택하여 다른 페이지의 결과에 액세스할 수 있습니다.

1. 열 너비의 크기를 조정하려면 두 열을 구분하는 선 위로 마우스를 가져간 다음 클릭하여 원하는 너비로 드래그합니다.

   이 열은 브라우저에서 캐시를 지우거나 수동으로 다시 크기를 조정할 때까지 크기가 조정됩니다.

1. 목록에서 열을 재정렬하려면 열 머리글 위로 마우스를 가져가 손 도구를 표시한 다음 을 클릭하여 열을 표시할 위치로 드래그합니다.

   열의 위치는 페이지를 새로 고칠 때까지 저장됩니다.\
   목록의 열 너비와 순서 사용자 지정에 대한 자세한 내용은 문서를 참조하십시오 [열 너비 및 순서 수정](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. 목록의 정렬 순서를 조정하려면 열 헤더를 클릭하여 선택한 다음 Cmd 키를 누른 채 [!DNL Mac]) 또는 CTRL 키(켜짐) [!DNL Windows])을 키보드 위에 표시하고 정렬할 최대 2개의 추가 열 헤더를 선택합니다.

   선택한 열 순서대로 선택된 각 열로 목록이 정렬됩니다.

   목록에 대한 모든 수정 사항이 즉시 저장됩니다.

   >[!NOTE]
   >
   >에서 그룹을 정렬하는 경우 [!UICONTROL 그룹] 영역 [!UICONTROL 설정]를 지정하는 방법을 변경해도 그룹 및 해당 하위 그룹의 계층 보기가 중단되지 않습니다. 하위 그룹은 상위 그룹과 함께 유지됩니다. 목록은 먼저 최상위 그룹별로 정렬됩니다. 그런 다음 각 상위 그룹 아래에서 동일한 수준에 있는 하위 그룹 목록이 함께 정렬됩니다.
