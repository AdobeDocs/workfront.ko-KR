---
content-type: overview
product-area: projects
navigation-topic: financials
title: 초과 근무 비율 정의
description: 태스크에 대한 초과 근무 비율을 정의하여 태스크 지정에 대한 계획 수익 계산을 조정할 수 있습니다.
author: Lisa
feature: Work Management
source-git-commit: bf8dcc9dfa9697c8d212072bb511c57aa01e7529
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 6%

---

# 초과 근무 비율 정의

{{highlighted-preview-article-level}}

작업에 초과 근무 비율이 추가되면 해당 작업의 모든 할당에 적용됩니다. 해당 작업의 모든 계획된 시간을 곱하여 계획된 수익 계산에 영향을 줍니다.

동일한 작업 내의 할당에 대해서는 초과 근무 비율이 달라질 수 없습니다. 서로 다른 초과 근무 승수가 필요한 경우 상위 태스크에 별도의 하위 태스크를 생성해야 합니다.

>[!NOTE]
>
>초과 작업 비율을 초과 작업이 아닌 작업에 추가할 수 없도록 하는 유효성 검사가 없습니다.

## 계획된 수익에 대한 초과 작업 시간 계산

시스템은 먼저 표준 청구 요금 계층을 사용하여 청구 요금을 결정합니다. 자세한 내용은 [수익 및 비용 계층 구조 개요](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)를 참조하십시오.

작업에 초과 근무 비율이 있는 경우 계산은 다음과 같습니다.
계획된 수익 = 청구 요금 × 초과 근무 비율 × 계획된 시간

초과 근무 비율이 비어 있으면 계산은 다음과 같습니다.
계획된 수익 = 청구 요금 × 계획된 시간

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td>워크플로 얼티밋</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>표준</td> 
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td>작업, 프로젝트 및 재무 데이터에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td><p>청구 요금 편집이 포함된 작업에 대한 권한 관리</p>
     <p>프로젝트에 대한 상위 권한 기여</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

작업 수익 유형은 시간별 사용자 및 역할이어야 합니다. 자세한 내용은 [수익 및 비용 계층 구조 개요](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)를 참조하십시오.

레이아웃 템플릿에서 **초과 근무 비율** 필드를 사용하도록 설정해야 합니다.

1. 레이아웃 템플릿에서 **사용자에게 표시되는 항목 사용자 지정** 아래의 아래쪽 화살표를 클릭한 다음 **작업**&#x200B;을 클릭합니다.
1. **세부 정보** 섹션에서 **재무** 영역의 **초과 근무 비율** 필드를 선택합니다.

   자세한 내용은 [레이아웃 템플릿을 사용하여 세부 정보 보기 사용자 지정](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)을 참조하십시오.

## 작업에 대한 초과 근무 비율 정의

1. 편집할 작업으로 이동합니다.

   자세한 내용은 [작업 세부 정보 섹션의 작업 재무 관리](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md)를 참조하십시오.

1. 왼쪽 패널에서 **작업 세부 정보**&#x200B;를 클릭합니다.
1. **재무** 영역의 **초과 근무 비율** 필드에 초과 근무 승수를 입력합니다.
1. **변경 내용 저장**&#x200B;을 클릭합니다.

