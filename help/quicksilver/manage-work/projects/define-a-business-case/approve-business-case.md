---
navigation-topic: business-case-and-scorecards
title: 비즈니스 사례 승인
description: 프로젝트 요청에 대한 비즈니스 사례를 완료하고 실행한 후에는 비즈니스 사례를 승인해야 합니다. 조직의 워크플로우에 따라 다릅니다. 비즈니스 사례를 승인하지 않고 프로젝트를 시작할 수 있지만 Adobe Workfront 관리자 및 프로젝트 소유자는 이를 권장하지 않을 수 있습니다.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# 비즈니스 사례 승인

프로젝트 요청에 대한 비즈니스 사례를 완료하고 실행한 후에는 비즈니스 사례를 승인해야 합니다. 조직의 워크플로우에 따라 다릅니다. 비즈니스 사례를 승인하지 않고 프로젝트를 시작할 수 있지만 Adobe Workfront 관리자 및 프로젝트 소유자는 이를 권장하지 않을 수 있습니다. 

비즈니스 사례 완료 및 제출에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 비즈니스 사례 승인 개요

프로젝트의 비즈니스 사례를 승인할 때 다음 사항을 고려하십시오.

* 프로젝트에 대한 비즈니스 사례를 승인하려면 프로젝트에 대한 관리 권한이 있어야 합니다. 
* Home의 Approvals에 따라 Business Case가 승인되기를 기다리는 프로젝트를 볼 수 없습니다.
* 비즈니스 사례 승인이 필요한 개별 프로젝트로 수동으로 이동하여 승인 보류 중인지 확인해야 합니다. 프로젝트에 대한 비즈니스 사례를 승인해야 함을 알리는 Workfront 알림 메커니즘이 없습니다.
* 프로젝트 보고서를 작성하거나 연관된 포트폴리오에 액세스하여 비즈니스 사례 승인을 기다리는 프로젝트를 찾을 수 있습니다. 

   Portfolio에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 Portfolio 개요](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## 프로젝트 보고서를 작성하여 비즈니스 사례 승인

프로젝트에 대한 보고서를 작성하여 프로젝트 승인 시 필요한 비즈니스 사례를 확인할 수 있습니다. 

업무 사례의 승인 대기 중인 프로젝트에 대한 보고서를 작성하려면 다음을 수행하십시오.

1. 프로젝트에 대한 보고서를 만듭니다.

   보고서 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 을(를) 선택합니다 **보기** 보고서의 탭을 클릭한 다음 **열 추가**.

1. 에 &quot;Status&quot; 입력 시작 **이 열에 표시** 필드를 선택한 다음 목록에 이 필드가 나타나면 선택합니다.

    이 열에는 프로젝트의 상태가 표시됩니다.

1. 을(를) 선택합니다 **필터** 보고서의 탭을 클릭한 다음 **필터 규칙 추가**.

1. 에 &quot;Status&quot; 입력 시작 **프로젝트 표시** 필드를 선택한 다음 목록에 있으면 선택합니다.
1. 선택 **Equal** 필터 수정자에 사용됩니다.
1. 사용 가능한 필드에 &quot;Requested&quot;를 입력합니다. 

   이렇게 하면 보고서에 요청됨 상태의 프로젝트만 포함됩니다.

     ![request_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (선택 사항) **다른 필터 규칙 추가**.

   추가 필터를 추가하여 프로젝트 소유자, 프로젝트 스폰서 또는 Portfolio 소유자인 프로젝트만 표시할 수 있습니다.

   예를 들어 다음 필터 문을 사용할 수 있습니다. 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   프로젝트 스폰서로 지정된 프로젝트를 표시하려면

   ```
   Project Owner ID Equals $$USER.ID
   ```

   프로젝트 소유자로 지정된 프로젝트를 표시하려면

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   Portfolio 관리자로 지정된 위치를 표시합니다. 

1. 클릭 **저장+닫기**.

   보고서의 모든 프로젝트는 **요청**.

1. 보고서에서 프로젝트 이름을 클릭하여 엽니다.
1. 클릭 **비즈니스 사례** 왼쪽 패널에 표시됩니다.
1. 클릭 **승인** 또는 **거부** 비즈니스 사례 요약 영역에서 비즈니스 사례를 승인하거나 거부할 수 있습니다. 

   ![](assets/business-case-summary-with-rp-information--1-.png)

   프로젝트 상태가 (으)로 변경되었습니다. **승인됨** 비즈니스 사례가 승인되는 경우

   프로젝트 상태가 (으)로 변경되었습니다. **거부됨** 비즈니스 사례가 거부되는 경우

   >[!NOTE]
   >
   >비즈니스 사례 승인을 제출한 사용자에게 프로젝트 요청이 승인되었는지 또는 거부되었는지를 알리는 알림이 없습니다.

## 포트폴리오의 요청된 프로젝트에 액세스하여 비즈니스 사례 승인

요청된 프로젝트 검토에 대한 자세한 내용은 문서를 참조하십시오 [요청된 프로젝트 검토](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
