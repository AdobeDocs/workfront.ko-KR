---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 캔버스 대시보드에서 보고서 데이터 그룹화
description: 보고서 결과를 그룹으로 구성합니다. 보고서 유형에 따라 그룹화가 다르게 작동합니다.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 4%
---
# 캔버스 대시보드에서 보고서 데이터 그룹화

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 이 단계에서 기능 일부가 완전하지 않거나 의도한 대로 작동하지 않을 수 있습니다. Canvas Dashboards Beta 개요 문서의 [피드백 제공](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) 섹션에 있는 지침에 따라 경험에 대한 피드백을 제출하십시오.<br>
>가능한 버그 또는 기술 문제에 대한 피드백이 있는 경우 Workfront 지원에 티켓을 제출하십시오. 자세한 내용은 [고객 지원 센터에 문의](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)를 참조하세요.<br>
>다음 클라우드 공급자에서는 이 Beta를 사용할 수 없습니다.
>
>* Amazon Web Services에 대한 자체 키 가져오기
>* Azure
>* Google Cloud 플랫폼

그룹화는 보고서 결과를 구성하여 관련 레코드가 함께 표시되도록 합니다. 그룹화가 작동하는 방식은 보고서 유형에 따라 다르므로, 이 문서에는 각 보고서 유형에 대해 별도의 섹션이 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>Any </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td> 
<p>표준</p> 
<p>플랜</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td><p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td><p>대시보드에 대한 권한 관리</p>
  </td> 
  </tr>
</tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
+++

## 전제 조건

데이터를 그룹화하려면 먼저 대시보드에 보고서가 있거나 보고서를 작성하고 있어야 합니다. 자세한 내용은 [캔버스 대시보드 만들기](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)를 참조하세요.

## 테이블 보고서의 행 그룹화

테이블 보고서에서 그룹화는 보고서 자체의 행을 구성합니다.

1. **구성** 대화 상자에서 왼쪽 패널의 **그룹 설정** 아이콘을 클릭합니다.

1. **그룹화 추가**&#x200B;를 클릭한 다음 그룹화할 필드를 선택합니다. 오른쪽 미리보기에 그룹화가 나타납니다.

1. (선택 사항) 더 많은 그룹화를 추가하려면 반복하십시오.

## 차트 및 KPI 보고서에서 드릴다운 그룹화 구성

차트 및 KPI 보고서에서는 기본 시각화를 그룹화하지 않습니다. 대신 뷰어가 값으로 드릴다운할 때 드릴다운 테이블이 어떻게 그룹화되는지 구성합니다.

1. **구성** 대화 상자에서 왼쪽 패널의 **드릴다운 그룹 설정** 아이콘을 클릭합니다.

1. **그룹화 추가**&#x200B;를 클릭한 다음 드릴다운 테이블을 그룹화할 필드를 선택합니다.

## 피벗 테이블 보고서에서 세그먼트 구성

피벗 테이블 보고서는 그룹화를 사용하지 않습니다. 대신 최대 2개의 세그먼트를 정의합니다. 이 세그먼트는 피벗의 지표를 그룹화하고 총계한 범주입니다.

1. **구성** 대화 상자에서 왼쪽 패널의 **세그먼트** 아이콘을 클릭합니다.

1. **세그먼트 추가**&#x200B;를 클릭한 다음 원하는 필드를 선택합니다. 세그먼트는 미리보기에 열로 나타납니다.

1. (선택 사항) 두 번째 세그먼트를 추가하려면 반복합니다. 최대 2개의 세그먼트를 추가할 수 있습니다.

## 대시보드에서 그룹화된 데이터 보기

보고서 뷰어는 그룹화된 데이터를 확장, 축소 및 정렬할 수 있습니다. 자세한 내용은 [캔버스 대시보드 사용](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)에서 [그룹화된 데이터가 있는 보고서 보기](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data)를 참조하십시오.
