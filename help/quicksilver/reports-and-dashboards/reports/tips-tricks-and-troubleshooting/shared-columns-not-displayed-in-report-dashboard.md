---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 공유 열의 데이터가 대시보드 보고서에 표시되지 않음
description: 보고서를 여러 열 대시보드 레이아웃에 배치하면 공유 열의 데이터가 표시되지 않지만 단일 열 레이아웃에는 표시됩니다. 줄 바꿈도 재정의됩니다.
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 1%

---

# 공유 열의 데이터가 대시보드 보고서에 표시되지 않음

## 문제

보고서를 여러 열 대시보드 레이아웃에 배치하면 공유 열의 데이터가 표시되지 않지만 단일 열 레이아웃에는 표시됩니다. 줄 바꿈도 재정의됩니다.

## 원인

열로 표시된 열만

```
shortview=true
```

대시보드 레이아웃에 왼쪽/오른쪽 분할 또는 왼쪽/중간/오른쪽 분할이 설정되면 보고서의 대시보드 보기에 포함됩니다.

## 솔루션

보고서에 사용된 보기에 액세스하고 텍스트 모드를 엽니다. 자세한 내용은 [텍스트 모드를 사용하여 보기 편집](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)을 참조하십시오. 공유/병합된 열에 사용된 열을 포함하여 보고서의 모든 열에 레이블을 지정합니다.

```
shortview=true
```

. 그러면 보고서 열이 대시보드에 제대로 표시됩니다.
