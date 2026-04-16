---
title: 프로젝트에 비율 카드 첨부
description: 프로젝트에 요금 카드를 첨부하면 위치별 모든 역할과 관련 청구 요금이 프로젝트에 추가됩니다.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 3%

---

# 프로젝트에 요금 카드 첨부

요금 카드는 속성을 기준으로 작업 역할당 여러 청구 요금을 저장합니다. 예를 들어, 각각 청구 요금이 다른 에이전시에 할당되지 않은 Designer(파리 기반, 에이전시 A), 다른 Designer(파리 기반, 에이전시 B), 세 번째 Designer(뉴욕 기반)의 작업 역할이 있을 수 있습니다. 하지만 비율 카드의 작업 역할에는 속성이 필요하지 않습니다. 속성은 보다 세부적인 비율을 설정하는 도구 역할을 합니다. 요금 카드의 청구 요금도 날짜 유효일 수 있으므로 지정된 날짜에 요금이 시작되고 종료됩니다.

프로젝트에 요금 카드를 첨부하면 모든 역할과 관련 청구 요금이 프로젝트에 추가됩니다.

>[!NOTE]
>
>요금 카드를 첨부하면 프로젝트의 기존 요금 카드 청구 요금이 무시됩니다. 프로젝트에 직접 추가된 청구 요금 무시는 제거되지 않습니다.

등급 카드 만들기에 대한 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)를 참조하십시오.

프로젝트의 작업 역할 청구 요율 재정의 및 프로젝트 수익 계산에 대한 일반 정보는 [프로젝트의 청구 요율 재정의 및 수익 계산 개요](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)를 참조하십시오.

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
   <td>프로젝트, 재무 데이터 및 등급 카드에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td>개체 권한</td> 
   <td>청구 요금 편집 권한으로 프로젝트에 대한 권한 관리</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트에 요금 카드 첨부

1. 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **요금**&#x200B;을 클릭한 다음 **청구**&#x200B;를 선택합니다.
1. **청구 요금 추가 > 요금 카드 첨부**&#x200B;를 클릭합니다.

   **요금 카드 첨부** 상자가 열립니다. 목록에서 요금 카드를 검색할 수 있습니다.

   ![요금 카드 상자 첨부](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >요금 카드의 그룹 및 회사는 이 목록에서 필터로 사용됩니다. 프로젝트에는 그룹 및 회사 필드도 포함되어 있으므로 Workfront은 이러한 값을 사용하여 사용 가능한 비율 카드 목록을 시스템 전체의 모든 비율 카드가 아닌 프로젝트 컨텍스트와 관련된 비율카드로 좁힙니다.
   >
   >일치 항목이 정확할 필요는 없습니다. 프로젝트의 그룹/회사 구성에 따라 빈 그룹 및/또는 회사 값이 있는 등급 카드가 여전히 표시될 수 있습니다. 예를 들어, 프로젝트에 선택한 그룹이 있지만 회사가 비어 있는 경우, 비율 카드의 회사가 다르거나 비어 있더라도 해당 그룹과 관련된 비율 카드가 표시될 수 있습니다.

1. 프로젝트에 추가할 요금 카드를 선택하고 **첨부**&#x200B;를 클릭합니다.

   요금 카드 및 모든 작업 역할 요금이 청구 요금 목록에 추가됩니다.

   ![등급 카드가 프로젝트에 추가됨](assets/rate-card-on-project.png)

## 프로젝트에서 비율 카드 제거

프로젝트에서 비율 카드를 제거하면 해당 작업의 모든 역할 비율이 제거됩니다. 요금제에서 가져온 프로젝트에서는 개별 요금을 제거할 수 없습니다.

프로젝트에 직접 추가된 사용자 또는 작업 역할에 대한 청구 요율 무시는 전체 요율 카드를 제거하지 않고 제거할 수 있습니다.

1. 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **요금**&#x200B;을 클릭한 다음 **청구**&#x200B;를 선택합니다.
1. **제거** 아이콘 ![제거 아이콘](assets/remove-icon.png)을 클릭합니다.
1. 확인 메시지에서 **확인**&#x200B;을 클릭하여 요금 카드를 제거합니다.

