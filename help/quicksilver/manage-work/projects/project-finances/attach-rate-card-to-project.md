---
title: 프로젝트에 비율 카드 첨부
description: 프로젝트에 요금 카드를 첨부하면 위치별 모든 역할과 관련 청구 요금이 프로젝트에 추가됩니다.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# 프로젝트에 요금 카드 첨부

{{highlighted-preview-article-level}}

요금 카드는 위치에 따라 작업 역할당 여러 청구 요금을 저장합니다. 각각 청구 요금이 다른 파리에 기반을 둔 Designer과 뉴욕에 기반을 둔 두 번째 Designer의 작업 역할이 있을 수 있습니다. 하지만 요금 카드의 작업 역할에는 위치가 필요하지 않습니다. 요금 카드의 작업 역할(및 가능한 위치)에 대한 청구 요금에는 유효 날짜도 포함될 수 있습니다.

프로젝트에 요금 카드를 첨부하면 위치별 모든 역할과 관련 청구 요금이 프로젝트에 추가됩니다.

>[!NOTE]
>
>요금 카드를 첨부하면 프로젝트의 기존 청구 요금이 무시됩니다.

프로젝트의 요금 카드에서 직접 청구 요금을 편집할 수 있습니다. 기본 요금 카드에 저장된 요금에는 영향을 주지 않습니다.

등급 카드 만들기에 대한 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)를 참조하십시오.

프로젝트의 작업 역할 청구 요율 재정의 및 프로젝트 수익 계산에 대한 일반 정보는 [작업 역할 청구 요율 재정의 개요 및 프로젝트의 수익 계산](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>작업 역할에 대한 관리 액세스</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>재무 관리 권한으로 프로젝트에 대한 권한 관리 </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 프로젝트에 요금 카드 첨부

1. 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **청구 요금**&#x200B;을 클릭합니다.
1. **청구 요금 추가 > 요금 카드 첨부**&#x200B;를 클릭합니다.

   요금 카드 첨부 페이지가 열립니다. 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)를 참조하십시오.

1. 프로젝트에 추가할 요금 카드를 선택하고 **첨부**&#x200B;를 클릭합니다.

   요금 카드 및 모든 작업 역할 요금이 청구 요금 목록에 추가됩니다.

   ![등급 카드가 프로젝트에 추가됨](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >청구 요금 목록에서 요금 카드에서 가져온 하나 이상의 작업 역할을 제거할 수 있습니다. 프로젝트에서 작업 역할 청구 요율을 제거해도 기본 요율 카드에서 제거되지 않습니다.
