---
title: 프로젝트에 요금 카드 첨부
description: 프로젝트에 요금 카드를 첨부하면 위치별 모든 역할과 관련 청구 요금이 프로젝트에 추가됩니다.
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 프로젝트에 요금 카드 첨부

{{highlighted-preview-article-level}}

요금 카드는 위치에 따라 작업 역할당 여러 청구 요금을 저장합니다. 각각 청구 요금이 다른 파리에 본사를 둔 디자이너와 뉴욕에 본사를 둔 두 번째 디자이너 역할이 있을 수 있습니다. 하지만 요금 카드의 작업 역할에는 위치가 필요하지 않습니다. 요금 카드의 작업 역할(및 가능한 위치)에 대한 청구 요금에는 유효 날짜도 포함될 수 있습니다.

프로젝트에 요금 카드를 첨부하면 위치별 모든 역할과 관련 청구 요금이 프로젝트에 추가됩니다.

>[!NOTE]
>
>요금 카드를 첨부하면 프로젝트의 기존 청구 요금이 무시됩니다.

프로젝트의 요금 카드에서 직접 청구 요금을 편집할 수 있습니다. 기본 요금 카드에 저장된 요금에는 영향을 주지 않습니다.

비율 카드 만들기에 대한 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

프로젝트에 대한 작업 역할 청구 요율 대체 및 프로젝트 수익 계산에 대한 일반 정보는 다음을 참조하십시오. [작업 역할 청구 요금 재정의 및 프로젝트의 수익 계산에 대한 개요](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>현재 플랜: 표준</p><p>또는</p><p>레거시 플랜: 플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>작업 역할에 대한 관리 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 권한으로 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 프로젝트에 요금 카드 첨부

1. 프로젝트로 이동합니다.
1. 클릭 **청구 요금** 왼쪽 패널에서 먼저 다음을 클릭해야 할 수 있습니다 **더 보기**.
1. 클릭 **청구 요금 추가 > 요금 카드 첨부**.

   요금 카드 첨부 페이지가 열립니다. 자세한 내용은 [등급 카드 관리](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. 프로젝트에 추가할 요금 카드를 선택하고 **첨부**.

   요금 카드 및 모든 작업 역할 요금이 청구 요금 목록에 추가됩니다.

   ![등급 카드가 프로젝트에 추가됨](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >청구 요금 목록에서 요금 카드에서 가져온 하나 이상의 작업 역할을 제거할 수 있습니다. 프로젝트에서 작업 역할 청구 요율을 제거해도 기본 요율 카드에서 제거되지 않습니다.

