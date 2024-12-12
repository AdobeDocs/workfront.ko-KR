---
product-area: projects
navigation-topic: financials
title: 프로젝트 수준 청구 요율을 회사 수준 청구 요율로 재정의
description: 프로젝트 수준 청구 요율을 회사 수준 청구 요율로 재정의
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# 프로젝트 수준 청구 요율을 회사 수준 청구 요율로 재정의

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

프로젝트 수준 청구 요금 대신 회사 수준 청구 요금을 사용하도록 프로젝트를 구성할 수 있습니다.

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
   <td>프로젝트 및 재무 데이터에 대한 액세스 편집</td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>재무 관리 권한으로 프로젝트에 대한 권한 관리</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 회사 수준 청구 요금 대체 옵션 활성화

회사가 프로젝트와 연결되어 있고 이 옵션이 활성화된 경우 회사 수준의 청구 요율 변경은 프로젝트에 설정된 청구 요율을 재정의합니다.

사용자가 프로젝트의 재무를 수동으로 다시 계산할 때 회사 수준의 청구 요금에 대한 모든 변경 사항이 적용됩니다. 청구됨으로 표시되지 않는 한 과거 수익 계산도 무시됩니다.

1. 프로젝트로 이동합니다.
1. 헤더의 프로젝트 이름 옆에 있는 **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭합니다.
1. **재무** 섹션에서 **회사 수준의 청구 요금이 프로젝트 수준의 청구 요금을 재정의할 수 있도록 허용**&#x200B;을(를) 설정합니다.

   >[!CAUTION]
   >
   >청구됨으로 표시되지 않는 한 이 옵션을 활성화하면 과거 수익 계산이 재정의됩니다. 청구 기록을 생성하여 과거 수익 계산을 보존할 수 있습니다. 자세한 내용은 문서 [청구 기록 만들기](../../../manage-work/projects/project-finances/create-billing-records.md)를 참조하십시오.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

## 회사 수준 청구 요율을 업데이트하고 프로젝트에 적용

프로젝트에 대해 회사 수준 청구 요금 대체 옵션을 활성화한 후, 회사 청구 요금에 대한 변경 사항은 재정이 다시 계산될 때마다 프로젝트에 적용됩니다.

>[!NOTE]
>
>회사 수준의 청구 요율을 업데이트하려면 사용자는 액세스 수준에서 회사에 액세스할 수 있어야 합니다.

{{step-1-to-setup}}

1. **회사**&#x200B;를 클릭합니다.
1. 회사 수준 청구 요금 대체를 활성화한 프로젝트와 연관된 회사의 이름을 클릭합니다.
1. 왼쪽 패널에서 **청구 요금**&#x200B;을 클릭합니다.
1. 기존 작업 역할에 대한 **회사 청구 요금** 및 시작/종료 날짜를 업데이트한 다음 Enter 키를 누르십시오.

   새 일자 유효 회사 청구 요율을 추가하려면 작업 역할에 대한 청구 요율을 선택하고 **편집**&#x200B;을 클릭합니다. 날짜 유효 회사 청구 요금에 대한 자세한 내용은 [회사 수준에서 작업 역할 청구 요금 재정의](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)를 참조하십시오.

1. 하나 이상의 프로젝트에 대한 회사 비율을 갱신하려면 다음 중 하나를 수행합니다.

   * 여러 프로젝트:

      1. 프로젝트 목록으로 이동합니다.
      1. 업데이트하려는 프로젝트에 맞춰 확인란을 선택합니다.
      1. **편집**&#x200B;을 클릭합니다.
      1. 설정 섹션에서 **비용 및 수익 다시 계산** 옵션을 사용하도록 설정합니다.
      1. **변경 내용 저장**&#x200B;을 클릭합니다.

   * 단일 프로젝트:

      1. 회사 수준 청구 요율 재정의를 활성화한 프로젝트로 이동합니다.
      1. 헤더의 프로젝트 이름 옆에 있는 **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png)을(를) 클릭한 다음 **재무 다시 계산**&#x200B;을 클릭합니다.
