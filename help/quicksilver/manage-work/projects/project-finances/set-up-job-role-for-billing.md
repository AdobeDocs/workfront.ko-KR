---
content-type: overview
product-area: projects
navigation-topic: financials
title: 청구에 대한 작업 역할 설정
description: Workfront을 사용하면 사용자에게 기본 작업 역할과 다른 작업 역할의 비용을 청구할 수 있습니다. 이 기능은 개인이 다른 요금으로 청구되어야 하는 작업을 일시적으로 수행할 때 유용합니다.
author: Lisa
feature: Work Management
exl-id: d6e2947d-2f40-4591-b048-9a769caadf43
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 3%

---

# 청구에 대한 작업 역할 설정

Workfront을 사용하면 사용자에게 기본 작업 역할과 다른 작업 역할의 비용을 청구할 수 있습니다. 이 기능은 개인이 다른 요금으로 청구되어야 하는 작업을 일시적으로 수행할 때 유용합니다.

다음 두 가지 방법으로 청구에 대한 작업 역할을 할당할 수 있습니다.

* 프로젝트 수준: 전체 프로젝트에 대해 동일한 작업 역할로 개인에게 청구되어야 할 때 사용합니다.
* 발령 레벨에서: 특정 태스크에 대해 다르게 청구하고자 할 때 사용합니다.

>[!NOTE]
>
>* 청구에 대한 작업 역할은 사람(사용자)에게만 적용됩니다. 일반 작업 역할이나 자리 표시자에는 적용되지 않습니다.
>* 청구에 대한 작업 역할 추가는 비용이 아니라 청구 요금에만 영향을 줍니다.
>* 할당 수준 청구는 항상 프로젝트 수준 청구보다 우선합니다.

자세한 내용은 [수익 및 비용 계층 구조 개요](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) 및 [고급 할당 만들기](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md)를 참조하십시오.

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
   <td> 등급 카드에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td>프로젝트에 대한 권한 관리 </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 수준에서 청구에 대한 작업 역할 할당

프로젝트 청구에 대한 작업 역할을 생성하는 경우:

* 청구 역할은 해당 사용자에 대한 프로젝트 내의 모든 작업 및 할당에 적용됩니다.
* 청구는 선택한 작업 역할의 청구 요금을 사용하지만 비용은 여전히 사용자의 기본 역할을 따릅니다.

프로젝트 수준에서 청구에 대한 작업 역할을 할당하려면 다음을 수행합니다.

1. 프로젝트를 엽니다.
1. 왼쪽 패널에서 **청구용 리소스**&#x200B;를 클릭합니다.
1. 아직 표시되지 않은 경우 **대금 청구에 대한 작업 역할** 탭을 선택하십시오.
1. **추가 > 청구에 대한 작업 역할 추가**&#x200B;를 클릭합니다.
1. **청구에 대한 작업 역할 추가** 상자에서 **사용자**&#x200B;를 선택합니다.
1. 이 프로젝트에서 이 사용자에 대한 청구 작업 역할로 사용할 **작업 역할**&#x200B;을(를) 선택하십시오.
1. (선택 사항) **작업 역할 추가**&#x200B;를 클릭하여 청구용 작업 역할의 유효 날짜를 정의합니다. 작업 역할의 **시작** 및 **종료** 날짜를 입력하십시오.

[프로젝트 수준에서 청구에 대한 작업 역할 추가](assets/jrfb-project-level.png)

1. **작업 역할 추가**&#x200B;를 다시 클릭하여 다른 기간에 대한 추가 청구 역할을 지정하십시오.
1. **저장**&#x200B;을 클릭합니다.

### 프로젝트 수준의 예

>[!BEGINSHADEBOX]

John의 기본 작업 역할은 Designer 1입니다. 그 프로젝트에는 Designer의 상급자가 필요한데 John이 그 일을 맡고 있다.

프로젝트 수준에서 청구에 대한 작업 역할을 **선임 Designer**(으)로 설정합니다.

결과:

* 청구 수익은 선임 Designer 요금입니다.
* 원가는 Designer 1 원가율(John의 실제 원가율)입니다.

>[!ENDSHADEBOX]

## 할당 수준에서 청구에 대한 작업 역할 할당

발령에 대한 청구에 대한 작업 역할을 추가하면 이 설정은 해당 특정 발령에 대해서만 프로젝트 수준의 청구 역할을 재정의합니다.

지정 레벨에서 청구에 대한 작업 역할을 지정하려면

1. 프로젝트를 열고 작업을 찾습니다.
1. 작업의 **고급 할당**(으)로 이동합니다.

   자세한 내용은 [고급 할당 만들기](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md)를 참조하십시오.

1. 작업 할당 그리드에서 열 **청구에 대한 작업 역할**&#x200B;을(를) 찾습니다.
1. 서로 다른 청구를 원하는 각 발령에 대한 작업 역할을 선택합니다.

   >[!NOTE]
   >
   >프로젝트 레벨에서 청구에 대한 작업 역할이 지정된 경우 발령에 표시됩니다. **대금 청구에 대한 작업 역할** 필드를 클릭하고 할당에 사용할 다른 작업 역할을 선택할 수 있습니다.
   >정보 아이콘은 청구에 대한 작업 역할이 프로젝트 또는 할당 수준에서 정의되었는지 여부를 알려줍니다.

   ![할당 대금 청구에 대한 작업 역할](assets/jrfb-assignment-level.png)

### 할당 수준의 예

>[!BEGINSHADEBOX]

John의 기본 작업 역할은 Designer 1입니다. 프로젝트 수준에서 수석 Designer으로 청구되지만, 주도자 Designer 청구 요금이 필요한 특별한 작업이 한 가지 있습니다.

해당 발령에 대해서만 청구에 대한 작업 역할을 주도자 Designer으로 설정합니다.

결과:

* John의 다른 모든 작업은 Senior Designer으로 청구됨
* 이 한 작업은 주도자 Designer으로 청구됩니다.
* 비용은 Designer 1로 남음

>[!ENDSHADEBOX]
