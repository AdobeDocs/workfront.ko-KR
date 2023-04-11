---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront의 그룹화 개요
description: 그룹 을 추가하여 보고서 및 목록의 정보 레이아웃을 관리할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Adobe Workfront의 그룹화 개요

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

그룹 을 추가하여 보고서 및 목록의 정보 레이아웃을 관리할 수 있습니다.

다음과 같은 방법으로 보고서에 그룹화를 추가할 수 있습니다.

* 기존 그룹을 편집하여 그룹을 만들 수 있습니다.

   기존 그룹 사용자 지정에 대한 자세한 내용은 [기존 그룹화 편집](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* 처음부터 그룹화를 만들 수 있습니다.

   그룹을 처음부터 만드는 방법에 대한 자세한 내용은 [Adobe Workfront에서 그룹화 만들기](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

기본적으로 그룹화는 보고서나 목록에서 회색 또는 파란색 강조 표시로 표시됩니다. 보고서 또는 목록의 결과는 강조 표시 없이 개별 그룹 아래에 나열됩니다.

보고서에 최대 3개의 그룹을 추가할 수 있습니다. 매트릭스 보고서를 만들어 최대 4개의 그룹으로 정보를 구성할 수 있습니다. 매트릭스 보고서에 대한 자세한 내용은 [매트릭스 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

표준 그룹화 보고서에서 첫 번째 그룹화는 어두운 색이고 두 번째 및 세 번째 그룹화는 더 가볍습니다. 그룹화에 대한 강조 표시 색 또는 그룹핑 이름의 글꼴을 사용자 지정할 수 없습니다. 그룹화 이름 뒤에 괄호로 묶인 숫자는 해당 그룹화 아래에 있는 결과 수를 나타냅니다. 보고서가 여러 페이지에 걸쳐 있는 경우, *모두* 각 그룹화에서 결과에 대한 정확한 카운트를 얻기 위해 보고서나 목록의 결과를 가져옵니다.

![샘플 그룹화](assets/grouping-example-blue.png)

그룹화 작업 시 다음 사항을 고려하십시오.

* 기존 그룹의 정보를 사용자 지정할 수 있습니다. 그룹화를 볼 수 있는 모든 사용자도 변경 사항을 볼 수 있습니다.
* Workfront 관리자가 그룹을 만들려면 편집 필터, 보기 및 그룹화에 대한 액세스 권한을 부여해야 합니다.

   필터, 보기 및 그룹화에 대한 액세스 권한 부여에 대한 자세한 내용은 [필터, 보기 및 그룹화에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* 그룹화에 대한 권한 수준은 그룹화가 저장되는 방식을 나타냅니다. 원래 그룹을 생성한 경우에는 변경 사항을 저장할 수 있습니다. 그렇지 않으면 그룹화 버전을 저장하라는 메시지가 표시됩니다. 다른 사용자와 공유한 그룹을 변경하면 해당 그룹에도 영향을 줍니다.
* 공유된 그룹을 공유한 사용자가 관리 액세스 권한을 부여한 경우에만 사용자 지정할 수 있습니다. 그룹 공유에 대한 자세한 내용은 [필터, 보기 또는 그룹화 공유](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* 그룹화 인라인은 편집할 수 없습니다.
* 다중 선택 사용자 지정 필드(예: 확인란) 또는 여러 값을 가질 수 있는 필드(예: 리소스 관리자)별로 그룹화할 수 없습니다.

## 그룹화에 대한 추가 정보

그룹화 행의 각 열에 있는 값을 합산하여 그룹화를 사용할 때 보고서 정보를 추가로 관리할 수 있을 뿐만 아니라 그룹화의 필드별로 정보를 정렬할 수도 있습니다. 더 이상 필요하지 않은 그룹화를 제거할 수도 있습니다.

* [그룹화 단위의 값 합계](#aggregate-values-in-groupings)
* [그룹화 기준 정렬](#sort-by-a-grouping)
* [그룹화 제거](#remove-a-grouping)

### 그룹화 단위의 값 합계 {#aggregate-values-in-groupings}

보고서의 각 열에 있는 값을 요약하여 그룹핑 라인에서 보고서에 표시된 데이터를 집계할 수 있습니다. 그룹의 열 데이터 요약에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>다음 필드에 대한 값을 그룹화하면 상위 객체(예: 상위 작업)에 다음 예외가 적용됩니다.
>
>* 실제 시간(예: 계획/실제 노무비, 계획/실제 비용, 계획/실제 비용, 계획/실제 비용, 계획 시간)을 제외한 모든 숫자 및 통화 필드는 하위 태스크 및 독립형 태스크에 대한 값만 집계합니다. 상위 작업 또는 상위 항목에 대한 값을 집계하지 않습니다.
>* 실제 시간은 주 상위 및 독립형 작업의 값을 집계합니다. 상위 작업 또는 하위 작업의 상위 항목에 대한 숫자를 집계하지 않습니다.
>* 숫자 및 통화 값에 대한 사용자 지정 데이터 필드는 모든 작업을 집계합니다. 부모, 자녀, 부모의 부모 및 독립형 작업


### 그룹화 기준 정렬 {#sort-by-a-grouping}

그룹화는 정렬할 수 없습니다. 보기는 정렬할 수 있습니다. 그룹화에 캡처된 값으로 목록을 정렬하려면 뷰의 열 중 하나에 동일한 값을 포함하고 뷰에 정렬을 적용해야 합니다. 이렇게 하면 목록이 그룹화의 값별로 간접적으로 정렬됩니다(그룹화에도 캡처되는 뷰의 값별로 정렬). 보기 만들기 및 보기 내의 값별 정렬에 대한 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### 그룹화 제거 {#remove-a-grouping}

그룹을 제거하는 방법은 그룹을 처음 만들었는지 아니면 그룹이 사용자와 공유되었는지에 따라 다릅니다. 기본 그룹을 제거할 수 없습니다.

* **그룹을 만들고 제거한 경우**&#x200B;의 경우 Workfront 시스템에서 그룹이 제거됩니다. 그룹화는 이전에 공유한 모든 사용자가 더 이상 사용할 수 없습니다.
* **그룹이 사용자와 공유되어 제거되는 경우**&#x200B;를 채울 때만 그룹이 제거됩니다. 원래 만든 사용자와 공유된 다른 사용자는 여전히 해당 그룹에 액세스할 수 있습니다.

그룹 제거에 대한 자세한 내용은 문서를 참조하십시오 [필터, 보기 및 그룹화 제거](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
