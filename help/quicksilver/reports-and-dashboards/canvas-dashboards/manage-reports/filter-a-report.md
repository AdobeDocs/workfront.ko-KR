---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 캔버스 대시보드에서 보고서 필터링
description: 보고서에서 필터를 추가하거나 편집하여 캔버스 대시보드에 표시되는 데이터를 제어합니다.
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
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 5%
---
# 캔버스 대시보드에서 보고서 필터링

>[!IMPORTANT]
>
>캔버스 대시보드 기능은 현재 베타 단계에 참여하는 사용자만 사용할 수 있습니다. 이 단계에서 기능 일부가 완전하지 않거나 의도한 대로 작동하지 않을 수 있습니다. Canvas Dashboards Beta 개요 문서의 [피드백 제공](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) 섹션에 있는 지침에 따라 경험에 대한 피드백을 제출하십시오.<br>
>가능한 버그 또는 기술 문제에 대한 피드백이 있는 경우 Workfront 지원에 티켓을 제출하십시오. 자세한 내용은 [고객 지원 센터에 문의](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)를 참조하세요.<br>
>다음 클라우드 공급자에서는 이 Beta를 사용할 수 없습니다.
>
>* Amazon Web Services에 대한 자체 키 가져오기
>* Azure
>* Google Cloud 플랫폼

보고서를 작성하는 동안 및 그 이후 언제든지 표시할 데이터를 제어하기 위해 보고서를 필터링할 수 있습니다. 두 경우 모두 필터링 옵션과 비헤이비어가 동일합니다.

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

대시보드에 보고서가 있거나 빌드 중이어야 필터링할 수 있습니다. 자세한 내용은 [캔버스 대시보드 만들기](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)를 참조하세요.

## 보고서 필터 추가 또는 편집

보고서에서 필터를 추가하거나 편집하려면:

1. 보고서의 필터 패널을 엽니다.

   * 보고서를 작성하는 경우 **구성** 대화 상자의 왼쪽 패널에서 **필터** 아이콘을 클릭합니다.
   * 기존 보고서를 편집하는 경우 오른쪽 상단의 **자세히** 아이콘을 클릭하고 **편집**&#x200B;을 선택한 다음 **구성** 대화 상자에서 **필터** 패널을 클릭합니다.

1. **필터 편집**&#x200B;을 클릭합니다.

1. **조건 추가**&#x200B;를 클릭한 다음 조건을 정의합니다.

   * **필드 선택**&#x200B;을 클릭한 다음 필터링할 필드를 선택합니다.
   * 필드가 충족해야 하는 조건 종류를 정의하는 수정자를 선택합니다.
   * 수정자에 값이 필요한 경우 평가할 값을 입력하거나 선택합니다.

   ![조건 추가](assets/add-condition.png)

1. (선택 사항) 이전 단계를 반복하여 조건을 더 추가합니다.

1. (선택 사항) 다른 필터링 기준 집합을 추가하려면 **필터 그룹 추가**&#x200B;를 클릭합니다. 세트 사이의 기본 연산자는 AND입니다. 연산자를 클릭하여 OR로 변경합니다.

>[!NOTE]
>
>필드, 연산자, 와일드카드 및 특수 필터링 규칙의 전체 목록에 대해서는 [캔버스 대시보드에 대한 보고서 필터 참조](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md)를 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.
