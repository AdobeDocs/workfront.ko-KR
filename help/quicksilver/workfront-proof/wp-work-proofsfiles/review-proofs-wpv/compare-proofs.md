---
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-workfront-proofing-viewer
title: 교정 뷰어에서 증명 비교
description: 두 개의 증명을 나란히 비교할 수 있습니다. 두 버전의 동일한 증명 또는 두 개의 완전히 분리된 증명이 될 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d4ec0c53-1451-4475-aa38-2319c6432936
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# 교정 뷰어에서 증명 비교

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

두 개의 증명을 나란히 비교할 수 있습니다. 두 버전의 동일한 증명 또는 두 개의 완전히 분리된 증명이 될 수 있습니다.

## 증명 버전 비교 {#compare-proof-versions}

1. 비교하려는 여러 버전이 있는 증명을 엽니다.
1. 표시되는 교정 뷰어의 왼쪽 위 모서리에서 증명 이름을 클릭합니다. 그런 다음 표시되는 버전 목록에서 **비교** 아이콘을 클릭하여 비교할 버전 옆의 아이콘을 클릭합니다.

   ![](assets/compare-proofs-choose-version-350x115.jpg)

   증명을 나란히 표시하고 왼쪽에 최신 버전이 표시됩니다.

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Separate breadcrumbs above each proof allow you to view and go to the work item associated with the proof:</p>
   -->

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/compare-proofs-breadcrumbs-350x148.jpg" style="width: 350;height: 148;"> </p>
   -->

1. 계속 [비교 도구 사용](#use-the-compare-tools).

## 별도의 증명 비교 {#compare-separate-proofs}

두 개의 개별 증명을 비교할 수 있습니다.

* [에서 개별 증명 비교 [!DNL Workfront]](#compare-separate-proofs-in-workfront)
* [에서 개별 증명 비교 [!DNL Workfront Proof]](#compare-separate-proofs-in-workfront-proof)

### 에서 개별 증명 비교 [!DNL Workfront] {#compare-separate-proofs-in-workfront}

내에서 문서 목록과 별도의 증명을 비교하는 방법에 대한 정보 [!DNL Workfront]를 참조하고 [두 개의 다른 증명 비교](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md#comparing-two-proofs-from-a-document-list) 의 섹션 [증명 비교](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md) 문서.

### 에서 개별 증명 비교 [!DNL Workfront Proof] {#compare-separate-proofs-in-workfront-proof}

>[!NOTE]
>
>비교하는 증명은 폴더 구조 내에서 동일한 폴더 및 동일한 수준의 계층 구조에 있어야 합니다. 폴더를 사용하여 비교하려는 증명을 그룹화하는 방법에 대한 자세한 내용은 [교정 뷰어에서 여러 증명 작업](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/work-with-multiple-proofs.md)

1. 교정 뷰어에서 비교할 증명 중 하나를 엽니다.
1. 을(를) 클릭합니다. **[!UICONTROL 비교 모드]** 아이콘.

   ![prop_compare_icon.png](assets/proof-compare-icon.png)\
   상기 뷰 영역은 반으로 분할되고, 상기 증명 표시부는 상기 교정 뷰어 좌우에 각각 표시된다.

   ![Compare_증명-versions.png](assets/compare-proofs-versions-350x180.png)

1. 을(를) 클릭합니다. [!UICONTROL 폴더] 같은 폴더 내에 다른 증명을 나열하려면 왼쪽이나 오른쪽에 있는 증명 위에 아이콘을 클릭합니다.

   ![Folder_icons_when_comparing_in_proofing_viewer.png](assets/folder-icons-when-comparing-in-proofing-viewer-350x121.png)

1. 목록에서 언어 교정 뷰어에서 현재 열려 있는 증명과 비교할 증명 이름을 클릭합니다.

   ![Comparing_증명-list_of_증명_in_folder.png](assets/comparing-proofs-list-of-proofs-in-folder-350x89.png)

   두 증명 모두 표시됩니다.

1. 계속 [비교 도구 사용](#use-the-compare-tools).

## 비교 도구 사용 {#use-the-compare-tools}

교정 뷰어는 증명을 효과적이고 효율적으로 비교하는 다양한 도구를 제공한다.

* [자동 비교 증명](#auto-compare-proofs)
* [오버레이에서 증명 비교](#compare-proofs-in-an-overlay)
* [동시 탐색 비교](#simultaneous-navigation-comparison)

### 자동 비교 증명 {#auto-compare-proofs}

자동 비교는 두 정적 또는 비디오 증명 간에 픽셀별로 비교됩니다. 감지된 모든 차이는 왼쪽의 증표에 빨간색으로 강조 표시됩니다.

대화형 증명을 비교할 때에는 자동 비교를 사용할 수 없습니다.

두 증명을 자동으로 비교하려면:

1. 다음 방법 중 하나로 증명을 비교할 수 있습니다.

   * 동일한 증명의 두 버전을 비교합니다(참조: [증명 버전 비교](#compare-proof-versions) 참조).
   * 두 개의 개별 증명을 비교합니다(참조). [별도의 증명 비교](#compare-separate-proofs) 참조).

1. 을(를) 클릭합니다. **[!UICONTROL 자동 비교]** 아이콘.

   ![prop_autocompare_icon.png](assets/proof-autocompare-icon-31x32.png)

   두 증명 간의 차이점은 왼쪽의 증식에서 빨간색으로 강조 표시됩니다.

1. (선택 사항) **[!UICONTROL 스위치]** 아이콘 을 클릭하여 오른쪽의 증명에 차이가 표시되도록 활성 측면을 변경합니다. 기본적으로 왼쪽에 증표에 차이가 표시됩니다.

   ![prop_autocompare_changeactive.png](assets/proof-autocompare-changeactive.png)

1. (선택 사항) **[!UICONTROL 색상]** 아이콘을 클릭하여 차이를 강조 표시할 때 사용되는 색상 및 불투명도를 변경합니다.

   ![prop_compare_color.png](assets/proof-compare-color.png)

### 오버레이에서 증명 비교 {#compare-proofs-in-an-overlay}

오버레이 비교를 통해 두 증명을 하나의 증명으로 보고 증명 가운데 아래에 세로 구분선을 표시하여 두 정적 증명 간의 차이점을 볼 수 있습니다. 세로 구분선을 따라 증명을 이동할 때 차이가 표시됩니다.

>[!NOTE]
>
>비디오 또는 대화형 증명을 비교할 때에는 오버레이 비교를 사용할 수 없습니다.

오버레이 비교를 활성화하려면

1. 다음 방법 중 하나로 증명을 비교할 수 있습니다.

   * 동일한 증명의 두 버전을 비교합니다(참조: [증명 버전 비교](#compare-proof-versions) 참조).
   * 두 개의 개별 증명을 비교합니다(참조). [별도의 증명 비교](#compare-separate-proofs) 참조).

1. 을(를) 클릭합니다. **[!UICONTROL 오버레이]** 아이콘.

   ![prop_compare_overlay_icon.png](assets/proof-compare-overlay-icon.png)

   증명 두 개는 증명 가운데 아래에 세로 구분선이 표시되어 있습니다.

1. 다음 중 하나를 수행합니다.

   * 세로 구분선 위로 증명을 패닝합니다. 패닝할 때 세로 구분선의 왼쪽에 증명이 표시되고 오른쪽에는 증거가 표시됩니다.
   * 세로 구분선을 좌우로 이동합니다. 구분선을 이동하면 세로 구분선의 왼쪽에 증명이 표시되고 오른쪽에는 오른쪽이 증명됩니다.

### 동시 탐색 비교 {#simultaneous-navigation-comparison}

증명을 비교할 때 기본적으로 동시 탐색이 활성화됩니다. 정적 증명과 정적 증명을 비교하거나 비디오 증명과 비디오 증명을 비교할 때 사용할 수 있습니다. 정적 증명과 비디오 증명을 비교할 때에는 사용할 수 없습니다.

**정적 증명:** 정적 증명에서 활성화되면 패닝하거나 스크롤할 때 동시에 탐색에서는 두 증명을 확대/축소 수준과 위치로 잠급니다. 증명에 여러 페이지가 포함되어 있고 동시 탐색을 사용할 수 있는 경우, 한 증명의 페이지를 변경하면 다른 증명에서 페이지가 변경됩니다.

**비디오 증명:** 비디오 증명에서 활성화되면 동시 탐색은 두 증명 타임라인의 시간 차이를 기억합니다.

아직 활성화되지 않은 경우 동시 탐색을 활성화하려면

1. 다음 방법 중 하나로 증명을 비교할 수 있습니다.

   * 동일한 증명의 두 버전을 비교합니다(참조: [증명 버전 비교](#compare-proof-versions) 참조).
   * 두 개의 개별 증명을 비교합니다(참조). [별도의 증명 비교](#compare-separate-proofs) 참조).

1. 을(를) 클릭합니다. **[!UICONTROL 동시 탐색]** 아이콘.

   ![prop_compare_concurrent_icon.png](assets/proof-compare-simultaneous-icon.png)

1. (선택 사항) **[!UICONTROL 재설정]** 언제든지 아이콘을 사용하여 확대/축소 레벨 및 위치(정적 증명용)나 타임라인(비디오 증명)을 재설정할 수 있습니다.

   ![prop_compare_concurrent_reset.png](assets/proof-compare-simultaneous-reset.png)

## 비교 모드 종료

1. 증명의 왼쪽 위 모서리에 있는 (x) 아이콘을 클릭하여 더 이상 보지 않을 증명을 닫습니다.

   ![prop_compare_exit.png](assets/proof-compare-exit-350x163.png)

   닫지 않은 증명은 교정 뷰어에서 열려 있습니다.
