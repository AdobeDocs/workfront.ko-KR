---
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-workfront-proofing-viewer
title: 증명 뷰어에서 증명 비교
description: 두 증명에 대한 병렬 비교를 볼 수 있습니다. 동일한 증명의 두 버전 또는 완전히 다른 두 개의 증명일 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d4ec0c53-1451-4475-aa38-2319c6432936
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# 증명 뷰어에서 증명 비교

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

두 증명에 대한 병렬 비교를 볼 수 있습니다. 동일한 증명의 두 버전 또는 완전히 다른 두 개의 증명일 수 있습니다.

## 증명 버전 비교 {#compare-proof-versions}

1. 비교할 여러 버전이 있는 증명을 엽니다.
1. 표시되는 증명 뷰어의 왼쪽 상단 모서리에서 증명 이름을 클릭합니다. 그런 다음 표시되는 버전 목록에서 열고 비교할 버전 옆에 있는 **비교** 아이콘을 클릭합니다.

   ![증명 비교](assets/compare-proofs-choose-version-350x115.jpg)

   증명이 나란히 표시되고 새 버전이 왼쪽에 표시됩니다.

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Separate breadcrumbs above each proof allow you to view and go to the work item associated with the proof:</p>
   -->

   <!--
   <p class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/compare-proofs-breadcrumbs-350x148.jpg" style="width: 350;height: 148;"> </p>
   -->

1. [비교 도구 사용](#use-the-compare-tools)을 사용하여 계속합니다.

## 별도의 증명 비교 {#compare-separate-proofs}

두 개의 개별 증명을 비교할 수 있습니다.

* [ [!DNL Workfront]에서 개별 증명 비교](#compare-separate-proofs-in-workfront)
* [ [!DNL Workfront Proof]에서 개별 증명 비교](#compare-separate-proofs-in-workfront-proof)

### [!DNL Workfront]에서 개별 증명 비교 {#compare-separate-proofs-in-workfront}

[!DNL Workfront] 내의 문서 목록에서 개별 증명을 비교하는 방법에 대한 자세한 내용은 [증명 비교](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md) 문서의 [서로 다른 두 증명 비교](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md#comparing-two-proofs-from-a-document-list) 섹션을 참조하십시오.

### [!DNL Workfront Proof]에서 개별 증명 비교 {#compare-separate-proofs-in-workfront-proof}

>[!NOTE]
>
>비교하는 증명은 폴더 구조 내에서 동일한 폴더 및 동일한 수준의 계층에 있어야 합니다. 폴더를 사용하여 비교하려는 증명을 그룹화하는 방법에 대한 자세한 내용은 [증명 뷰어에서 여러 증명을 사용하여 작업](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/work-with-multiple-proofs.md)을 참조하십시오.

1. 증명 뷰어에서 비교할 증명 중 하나를 엽니다.
1. **[!UICONTROL 비교 모드]** 아이콘을 클릭합니다.

   ![proof_compare_icon.png](assets/proof-compare-icon.png)\
   보기 영역이 반으로 분할되고 증명 뷰어의 왼쪽과 오른쪽에 증명이 모두 표시됩니다.

   ![Compare_proofs-versions.png](assets/compare-proofs-versions-350x180.png)

1. 왼쪽이나 오른쪽에 있는 증명 위에 있는 [!UICONTROL 폴더] 아이콘을 클릭하여 동일한 폴더 내에 있는 다른 증명을 나열합니다.

   ![Folder_icons_when_comparing_in_proofing_viewer.png](assets/folder-icons-when-comparing-in-proofing-viewer-350x121.png)

1. 목록에서 비교하려는 증명 이름을 현재 증명 뷰어에 열려 있는 증명과 클릭합니다.

   ![Comparing_proofs-list_of_proofs_in_folder.png](assets/comparing-proofs-list-of-proofs-in-folder-350x89.png)

   두 증명이 모두 나타납니다.

1. [비교 도구 사용](#use-the-compare-tools)을 사용하여 계속합니다.

## 비교 도구 사용 {#use-the-compare-tools}

증명 뷰어는 증명을 효과적이고 효율적으로 비교하기 위한 다양한 도구를 제공한다.

* [증명 자동 비교](#auto-compare-proofs)
* [오버레이에서 증명 비교](#compare-proofs-in-an-overlay)
* [동시 탐색 비교](#simultaneous-navigation-comparison)

### 증명 자동 비교 {#auto-compare-proofs}

자동 비교 는 두 정적 증명 또는 비디오 증명 간에 픽셀별로 비교합니다. 감지된 모든 차이는 왼쪽의 증명에서 빨간색으로 강조 표시됩니다.

대화형 증명을 비교할 때는 자동 비교를 사용할 수 없습니다.

두 증명을 자동 비교하려면 다음을 수행합니다.

1. 다음 방법 중 하나로 증명 비교를 시작합니다.

   * 동일한 증명의 두 버전을 비교합니다(이 문서에서 [증명 버전 비교](#compare-proof-versions) 참조).
   * 두 개의 개별 증명 비교(이 문서에서 [개별 증명 비교](#compare-separate-proofs) 참조).

1. **[!UICONTROL 자동 비교]** 아이콘을 클릭합니다.

   ![proof_autocompare_icon.png](assets/proof-autocompare-icon-31x32.png)

   두 증명 간의 모든 차이는 왼쪽의 증명에서 빨간색으로 강조 표시됩니다.

1. (선택 사항) **[!UICONTROL 전환]** 아이콘을 클릭하여 오른쪽의 증명에 차이가 표시되도록 활성 면을 변경합니다. 기본적으로 왼쪽의 증명에 차이가 표시됩니다.

   ![proof_autocompare_changeactive.png](assets/proof-autocompare-changeactive.png)

1. (선택 사항) **[!UICONTROL 색상]** 아이콘을 클릭하여 차이를 강조 표시할 때 사용되는 색상 및 불투명도를 변경합니다.

   ![proof_compare_color.png](assets/proof-compare-color.png)

### 오버레이에서 증명 비교 {#compare-proofs-in-an-overlay}

오버레이 비교를 사용하면 두 증명을 하나의 증명으로 보면서 증명의 중앙 아래에 수직 구분선을 제공하여 두 정적 증명 간의 차이점을 볼 수 있습니다. 수직 분할기에서 증명을 이동할 때 차이가 표시됩니다.

>[!NOTE]
>
>비디오 또는 대화형 증명을 비교할 때는 오버레이 비교를 사용할 수 없습니다.

오버레이 비교를 활성화하려면:

1. 다음 방법 중 하나로 증명 비교를 시작합니다.

   * 동일한 증명의 두 버전을 비교합니다(이 문서에서 [증명 버전 비교](#compare-proof-versions) 참조).
   * 두 개의 개별 증명 비교(이 문서에서 [개별 증명 비교](#compare-separate-proofs) 참조).

1. **[!UICONTROL 오버레이]** 아이콘을 클릭합니다.

   ![proof_compare_overlay_icon.png](assets/proof-compare-overlay-icon.png)

   두 증명은 증명 중앙의 세로 구분선이 있는 단일 증명으로 표시됩니다.

1. 다음 중 하나를 수행합니다.

   * 수직 분할기에서 증명을 패닝합니다. 패닝할 때 세로 구분선의 왼쪽에 증명이 표시되고 오른쪽의 증명이 오른쪽에 표시됩니다.
   * 세로 구분선을 왼쪽과 오른쪽으로 이동합니다. 구분선을 이동하면 세로 구분선의 왼쪽에 증명이 표시되고 오른쪽의 증명이 오른쪽에 표시됩니다.

### 동시 탐색 비교 {#simultaneous-navigation-comparison}

증명을 비교할 때 기본적으로 동시 탐색이 활성화됩니다. 정적 증명과 정적 증명을 비교하거나 비디오 증명과 비디오 증명을 비교할 때 사용할 수 있습니다. 정적 증명과 비디오 증명을 비교할 때는 사용할 수 없습니다.

**정적 증명:** 정적 증명에 대해 활성화하면 패닝 또는 스크롤할 때 동시 탐색이 두 증명에 대한 확대/축소 수준 및 위치를 잠급니다. 증명에 여러 페이지가 포함되어 있고 동시 탐색이 활성화된 경우 한 증명에서 페이지를 변경하면 다른 증명에서 페이지가 변경됩니다.

**비디오 증명:** 비디오 증명에서 활성화된 경우 동시 탐색은 두 증명 타임라인의 시간 차이를 기억합니다.

동시 탐색이 아직 활성화되지 않은 경우 활성화하려면 다음을 수행합니다.

1. 다음 방법 중 하나로 증명 비교를 시작합니다.

   * 동일한 증명의 두 버전을 비교합니다(이 문서에서 [증명 버전 비교](#compare-proof-versions) 참조).
   * 두 개의 개별 증명 비교(이 문서에서 [개별 증명 비교](#compare-separate-proofs) 참조).

1. **[!UICONTROL 동시 탐색]** 아이콘을 클릭합니다.

   ![proof_compare_simultaneous_icon.png](assets/proof-compare-simultaneous-icon.png)

1. (선택 사항) 언제든지 **[!UICONTROL 재설정]** 아이콘을 클릭하여 확대/축소 레벨 및 위치(정적 증명의 경우) 또는 타임라인(비디오 증명의 경우)을 재설정합니다.

   ![proof_compare_simultaneous_reset.png](assets/proof-compare-simultaneous-reset.png)

## 비교 모드 종료

1. 증명의 왼쪽 위 모서리에 있는 (x) 아이콘을 클릭하여 더 이상 보지 않을 증명을 닫습니다.

   ![proof_compare_exit.png](assets/proof-compare-exit-350x163.png)

   닫지 않은 증명이 증명 뷰어에 열려 있는 상태로 유지됩니다.
