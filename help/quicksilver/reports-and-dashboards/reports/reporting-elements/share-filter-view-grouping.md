---
product-area: reporting
navigation-topic: reporting-elements
title: 필터, 보기 또는 그룹화 공유
description: 다른 사용자와 볼 수 있는 액세스 권한이 있는 필터, 보기 및 그룹을 공유할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 1%

---

# 필터, 보기 또는 그룹화 공유

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

Adobe Workfront 관리자는 액세스 수준을 지정할 때 객체를 보거나 편집할 수 있는 액세스 권한을 사용자에게 부여합니다. 객체에 대한 액세스 권한 부여에 대한 자세한 내용은 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

사용자가 부여받은 액세스 레벨과 함께, 사용자가 생성한 특정 객체를 보거나 편집할 수 있는 권한을 부여할 수도 있습니다. 액세스 수준 및 권한에 대한 자세한 내용은 [액세스 수준 및 권한이 함께 작동하는 방법](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

다른 사용자와 볼 수 있는 액세스 권한이 있는 필터, 보기 및 그룹을 공유할 수 있습니다.

필터, 보기 또는 그룹이 사용자와 공유되면 해당 필터, 보기 또는 그룹을 목록에 적용할 수 있습니다. 액세스 권한에 따라, 수정하고 다른 사용자와 공유할 수 있습니다.

필터, 보기 또는 그룹을 만드는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront의 필터 개요](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 보기 이상의 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보기, 필터 또는 그룹화에 공유할 수 있는 액세스 권한이 있는 보기 또는 상위 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 필터, 보기 또는 그룹화 공유

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

선택 목록에서 필터를 공유하는 것은 필터를 공유하는 데 사용하는 인터페이스에 따라 다릅니다. 표준 또는 이전 필터 빌드 인터페이스 유형에 대한 자세한 내용은 [Adobe Workfront에서 필터 만들기 또는 편집](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

레거시 인터페이스에서만 보기 및 그룹화를 공유할 수 있습니다.

### 표준 빌더 인터페이스를 사용하여 필터 공유

프로젝트, 작업, 문제, 포트폴리오, 프로그램, 사용자, 템플릿 또는 그룹 목록에서 표준 인터페이스에서 필터를 공유할 수 있습니다. 필터에 대한 표준 빌더 인터페이스는 다른 객체나 보기 또는 그룹화에 사용할 수 없습니다.

표준 빌더 인터페이스를 사용하여 필터를 공유합니다.

1. 프로젝트, 작업 또는 문제 목록으로 이동합니다.
1. 을(를) 클릭합니다. **필터** 아이콘 ![필터 아이콘](assets/filter-nwepng.png).

   ![표준 필터 빌더](assets/new-filters-all-filter-types.png)

1. 다음 필터 목록을 검토하십시오.

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>즐겨찾기에 추가됨</strong></td>
   <td>즐겨찾기로 표시한 필터입니다. 필터를 즐겨찾으면 원래 위치가 필터 이름 아래에 표시되고, 즐겨찾기로 제거하지 않으면 원래 목록에서 숨겨집니다.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>저장됨</strong></td>
   <td>직접 빌드하고 저장한 필터.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>시스템 기본값</strong></td>
   <td>Workfront 시스템 기본 필터와 Workfront 관리자가 시스템 수준 또는 레이아웃 템플릿에서 필터 목록에 추가한 필터.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>나와 공유됨</strong></td>
   <td>다른 사용자가 만들고 공유했거나 시스템 전체에서 공유한 필터입니다.</td>
   </tr>
   </tbody>
   </table>

1. 보기 및 공유에 액세스할 수 있는 필터 위로 마우스를 가져간 다음 **자세히** 메뉴 ![추가 메뉴](assets/more-icon-spectrum.png)를 클릭한 다음 **공유**.

   ![추가 메뉴 옵션](assets/new-filters-more-menu-options-with-delete.png)

   필터 공유 상자가 표시됩니다.

1. 를 활성화합니다 **시스템 전체 보기** 설정 이렇게 하면 Workfront의 모든 사용자가 필터를 볼 수 있는 권한이 제공됩니다.

   >[!IMPORTANT]
   >
   >이 설정은 주의해서 사용하십시오. 모든 사용자에 대해 필터를 많이 추가하면 필터 경험이 복잡해지고 필터를 찾기가 더 어려워집니다.

   또는 에서 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력합니다 **액세스 권한 부여** 필드.

   ![필터 공유 상자](assets/new-filters-share-filter.png)

1. (선택 사항) 필터에 대한 권한을 편집할 엔티티 이름 옆에 있는 오른쪽 화살표 를 클릭한 다음, **보기** 또는 **관리** 선택 사항입니다. **보기** 는 기본값입니다.

   ![공유 권한](assets/new-filters-sharing-permissions.png)

1. (선택 사항) 다음 중 하나를 수행하여 엔티티에 대한 추가 권한을 활성화하거나 비활성화합니다.

   1. 클릭 **보기** 및 **공유** 선택 사항입니다. 기본적으로 활성화되어 있습니다.
   1. 클릭 **관리** 및 **공유** 또는 **삭제** 선택 사항입니다. 기본적으로 활성화되어 있습니다.

      >[!NOTE]
      >
      >삭제 옵션을 사용하여 액세스 관리를 활성화하면 필터를 소유하지 않더라도 이러한 사용자는 모든 사용자에서 필터를 삭제할 수 있습니다.
   >[!TIP]
   >
   >사용자는 액세스 수준보다 높은 권한을 받을 수 없습니다. 액세스 수준에서 편집 필터에 액세스할 수 없는 사용자는 필터를 관리할 권한을 받을 수 없습니다. Workfront이 이러한 사용자에 대한 관리 옵션을 비활성화하고 옵션이 흐리게 표시됩니다.

1. 클릭 **공유**. 필터는 지정한 엔터티와 공유됩니다.

   >[!TIP]
   >
   >그룹과 공유하면 그룹의 구성원 및 모든 하위 그룹에 대해 필터에 대한 권한이 제공됩니다.

   공유한 필터가 **나와 공유** 섹션에 나열된 상태로 남아 있습니다.

   ![나와 공유된 필터](assets/new-filters-shared-with-me.png)

### 기존 인터페이스를 사용하여 필터, 보기 및 그룹화를 공유할 수 있습니다

레거시 인터페이스의 필터, 보기 및 그룹화를 공유하는 것은 동일합니다.

1. 객체 목록이나 보고서로 이동합니다.
1. (조건부) 목록에서 **필터**, **보기**, 또는 **그룹화** 아이콘을 클릭한 다음 공유할 필터, 보기 또는 그룹을 마우스로 가리킨 다음 **자세히** 아이콘 ![자세히 아이콘](assets/more-icon.png), 그런 다음 **공유**.

   보고서에서 **필터**, **보기**, 또는 **그룹화** 드롭다운 메뉴에서 공유할 필터, 보기 또는 그룹을 선택합니다.

1. (조건부) 보고서에서 공유하는 경우 **필터**, **보기**, 또는 **그룹화** 드롭다운 메뉴를 다시 클릭한 다음 **공유 필터**, **공유 보기**, 또는 **공유 그룹화**.\
   다음 **필터 액세스**, **액세스 보기**, 또는 **그룹화 액세스** 대화 상자가 표시됩니다.

   ![공유 필터](assets/share-filter-people-box-nwe-350x458.png)

1. 공유할 사람에 따라 다음 중 하나를 완료하십시오.

   **개별 사용자, 팀, 역할, 그룹 또는 회사와 공유하려면 다음을 수행하십시오.** 제공된 필드에서 공유할 사용자, 팀, 역할, 그룹 또는 회사의 이름을 입력하고 드롭다운 목록에 표시되면 이름을 클릭합니다.\
   이 프로세스를 반복하여 여러 사용자, 팀, 역할, 그룹 또는 회사와 액세스 권한을 공유합니다.

   >[!TIP]
   >
   >그룹과 공유하면 그룹의 구성원 및 모든 하위 그룹의 필터, 보기 또는 그룹에 대한 권한이 제공됩니다.

   **시스템의 모든 사용자와 공유하려면** 을(를) 클릭합니다. **설정** 아이콘을 클릭한 다음 **시스템 전체에 표시**.\
   이 옵션을 사용하려면 관리자가 시스템 전체 공유 옵션을 선택해야 합니다. 자세한 내용은 문서를 참조하십시오 [사용자 정의 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) 및 [보고서, 대시보드 및 달력 공유](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (조건부) 개별 사용자, 팀, 역할, 그룹 또는 회사와 공유하는 경우 드롭다운 메뉴를 클릭하여 부여할 액세스 수준을 정의합니다.

   다음 옵션 중에서 선택할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>보기</strong></td> 
      <td> <p>공유 수신자가 공유 필터, 보기 또는 그룹화만 사용할 수 있도록 하려면 이 옵션을 선택합니다. 이 옵션을 선택하면 수신자는 공유 항목을 수정할 수 없습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>관리함</strong></td> 
      <td> <p>공유 수신자가 공유 필터, 보기 또는 그룹을 사용하고 수정할 수 있도록 하려면 이 옵션을 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>공유</strong></td> 
      <td> <p>클릭 <strong>고급 설정</strong>를 선택한 다음 을 선택하거나 선택을 취소합니다. <strong>공유</strong> 옵션을 선택합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. **저장**&#x200B;을 클릭합니다.

   필터, 보기 또는 그룹을 공유한 사용자는 **필터**, **보기**, 또는 **그룹화** 드롭다운 메뉴 또는 아이콘을 클릭하고 아래로 스크롤하여 **나와 공유** 섹션을 참조하십시오.


