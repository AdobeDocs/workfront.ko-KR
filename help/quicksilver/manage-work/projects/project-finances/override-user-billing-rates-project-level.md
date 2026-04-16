---
content-type: overview
product-area: projects
navigation-topic: financials
title: 프로젝트 수준에서 사용자 청구 요금 재정의
description: 이 문서에서는 프로젝트에 대한 시스템 사용자 청구 요율을 재정의하는 방법에 대해 설명합니다.
author: Lisa
feature: Work Management
exl-id: eb7dbb6f-a31c-4569-be54-9a151dcf4135
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 2%

---

# 프로젝트 수준에서 사용자 청구 요금 재정의

프로젝트 관리자는 특정 프로젝트의 사용자에 대한 청구 요금을 지정할 수 있습니다. 이 프로젝트 수준의 청구 요율은 이 사용자의 시스템 수준의 청구 요율을 무시합니다. Workfront은 시스템 수준 청구 요율을 사용하는 대신 사용자의 프로젝트 수준 청구 요율을 사용하여 수익을 계산합니다.

이 문서에서는 프로젝트에 대한 시스템 사용자 청구 요율을 재정의하는 방법에 대해 설명합니다.

프로젝트의 청구 요율 재정의 및 프로젝트 수익 계산에 대한 일반 정보는 [프로젝트의 청구 요율 재정의 및 수익 계산 개요](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)를 참조하십시오.

프로젝트의 수익 계산에 대한 자세한 내용은 [청구 및 수익 개요](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) 문서의 [수익 및 비용 계층 개요](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 및 [사용자 및 역할 할당에 따른 작업에 대한 수익 계산](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md) 섹션을 참조하십시오.

>[!NOTE]
>
>실제 매출의 경우, 청구됨으로 표시된 청구 기록에 추가된 시간에 적용되는 청구 요금은 청구 기록이 청구된 후에 발생하는 청구 요금 무시의 영향을 받지 않아야 합니다.

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
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p>
       <p><p>또한 다음 중 하나가 있어야 합니다.</p> 
        <ul> 
          <li> <p>시스템 관리자 액세스 수준입니다. </li> 
          <li> <p>액세스 수준의 <b>사용자</b> 설정이 <b>편집</b> 액세스로 구성되었으며, <b>만들기</b>와 <b>설정을 미세 조정</b> <b>에서 두 개의 </b>사용자 관리<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p>이 두 옵션 중 <b>사용자 관리자(그룹 사용자)</b>를 사용하도록 설정한 경우 사용자가 구성원인 그룹의 그룹 관리자여야 합니다.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td>재무 데이터 편집이 포함된 프로젝트에 대한 권한 관리 </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트 수준에서 사용자 청구 요금 재정의

프로젝트의 사용자 청구 요율을 재정의할 때 유효 일자를 지정할 수 있으며 각 일자 범위에는 다른 요율이 있습니다. 유효 일자를 지정하지 않으면 입력한 청구 단가 대체가 프로젝트의 전체 기간에 사용되어 수익을 계산합니다.

프로젝트에 대한 사용자 청구 요율을 재정의하려면

1. 청구 요율을 재정의할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **속도**&#x200B;를 클릭합니다. 먼저 **자세히 표시**&#x200B;를 클릭해야 할 수 있습니다.
1. 아직 선택하지 않은 경우 **청구** 탭을 클릭합니다.
1. **청구 요금 추가** > **새 사용자 청구 요금**&#x200B;을 클릭합니다.

   새 사용자 청구 요금 상자가 열립니다.

1. **사용자** 필드에서 청구 요금을 변경할 사용자를 선택합니다.
1. 청구 요금 재정의에 사용할 **통화**&#x200B;를 선택하십시오.
1. **청구 요금** 필드에 첫 번째 청구 요금 재정의를 입력합니다.
1. (선택 사항) 더 많은 청구 요금 재정의를 추가하려면 **날짜 유효 요금 추가**&#x200B;를 클릭합니다.
1. (조건부) 복수 청구 요금 대체를 추가하는 경우 각 행에 대해 다음 정보를 지정합니다.

   * **청구 요금**: 지정된 기간 동안의 청구 요금 값입니다.
   * **시작 날짜**: 청구 요금 재정의가 시작되는 날짜입니다.
   * **종료 날짜**: 청구 요금 재정의가 종료되는 날짜입니다.

   ![유효 날짜를 표시하는 새 사용자 청구 요금 상자](assets/new-user-billing-rate-on-project2.png)

   Workfront은 프로젝트의 매출을 계산할 때 이러한 시간대 동안 발생하는 시간에 재정의 사용자 비율을 적용합니다.

   Workfront을 사용하면 재정의 기간 사이에 간격을 둘 수 있지만, 의도적인지 확인하는 경고가 표시됩니다.

   첫 번째 대체 비율에 대해 시작 일자를 지정하거나 마지막 대체 비율에 대해 종료 일자를 지정하지 않아도 됩니다.

   청구 단가 재정의를 하나만 입력하는 경우 해당 단가는 프로젝트의 전체 기간에 적용됩니다. 날짜 효과 재정의를 여러 개 추가하는 경우 Workfront에서는 첫 번째 재정의가 종료 날짜 이전의 모든 시간에 적용되고 마지막 재정의는 시작 날짜 이후의 모든 시간에 적용된다고 가정합니다.

   Workfront에서는 첫 번째 재정의의 종료 날짜보다 오래된 날짜가 있는 모든 시간에 대해 첫 번째 재정의 비율이 적용되고, 마지막 재정의 시작 날짜보다 오래된 날짜가 있는 모든 시간에 대해 마지막 재정의 비율이 적용된다고 가정합니다.

   프로젝트의 계획된 시작 일자 전에 시간이 기록되는 경우 첫 번째 청구 요금이 사용됩니다.

   프로젝트의 계획된 완료 일자 이후 시간이 기록되는 경우 마지막 청구 요금이 사용됩니다.

1. **저장**&#x200B;을 클릭합니다.
