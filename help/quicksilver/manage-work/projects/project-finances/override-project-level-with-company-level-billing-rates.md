---
product-area: projects
navigation-topic: financials
title: 프로젝트 수준 청구 요율을 회사 수준 청구 요율로 재정의
description: 프로젝트 수준 청구 요율을 회사 수준 청구 요율로 재정의
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 72511f98e05c160e2ca69def8aa3a929ed62bb40
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 프로젝트 수준 청구 요율을 회사 수준 청구 요율로 재정의

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

프로젝트 수준 청구 요금 대신 회사 수준 청구 요금을 사용하도록 프로젝트를 구성할 수 있습니다.

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 권한으로 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 회사 수준 청구 요금 대체 옵션 활성화

회사가 프로젝트와 연결되어 있고 이 옵션이 활성화된 경우 회사 수준의 청구 요율 변경은 프로젝트에 설정된 청구 요율을 재정의합니다.

사용자가 프로젝트의 재무를 수동으로 다시 계산할 때 회사 수준의 청구 요금에 대한 모든 변경 사항이 적용됩니다. 청구됨으로 표시되지 않는 한 과거 수익 계산도 무시됩니다.

1. 프로젝트로 이동합니다.
1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) 헤더에서 프로젝트 이름 옆에 있는 을(를) 클릭한 다음 을(를) 클릭합니다. **편집**.
1. 다음에서 **재무** 섹션, 활성화 **회사 수준의 청구 요금이 프로젝트 수준의 청구 요금을 재정의할 수 있도록 허용**.

   >[!CAUTION]
   >
   >청구됨으로 표시되지 않는 한 이 옵션을 활성화하면 과거 수익 계산이 재정의됩니다. 청구 기록을 생성하여 과거 수익 계산을 보존할 수 있습니다. 자세한 내용은 이 문서 를 참조하십시오. [청구 기록 만들기](../../../manage-work/projects/project-finances/create-billing-records.md)

1. 클릭 **변경 내용 저장**.

## 회사 수준 청구 요율을 업데이트하고 프로젝트에 적용

프로젝트에 대해 회사 수준 청구 요금 대체 옵션을 활성화한 후, 회사 청구 요금에 대한 변경 사항은 재정이 다시 계산될 때마다 프로젝트에 적용됩니다.

>[!NOTE]
>
>회사 수준의 청구 요율을 업데이트하려면 사용자는 액세스 수준에서 회사에 액세스할 수 있어야 합니다.

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **설정**.
1. 클릭 **회사**.
1. 회사 수준 청구 요금 대체를 활성화한 프로젝트와 연관된 회사의 이름을 클릭합니다.
1. 클릭 **청구 요금** 왼쪽 패널에서
1. 업데이트 **회사 청구 요금** 기존 작업 역할의 시작/종료 날짜를 클릭한 다음 Enter 키를 누릅니다.

   새 일자 유효 회사 청구 단가를 추가하려면 작업 역할에 대한 청구 단가를 선택하고 **편집**. 유효 회사 청구 요금에 대한 자세한 내용은 [회사 수준에서 작업 역할 청구 요금 재정의](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. 하나 이상의 프로젝트에 대한 회사 비율을 갱신하려면 다음 중 하나를 수행합니다.

   * 여러 프로젝트:

      1. 프로젝트 목록으로 이동합니다.
      1. 업데이트하려는 프로젝트에 맞춰 확인란을 선택합니다.
      1. 클릭 **편집**.
      1. 설정 섹션에서 다음을 활성화합니다. **비용 및 수익 재계산** 옵션을 선택합니다.
      1. 클릭 **변경 내용 저장**.

   * 단일 프로젝트:

      1. 회사 수준 청구 요율 재정의를 활성화한 프로젝트로 이동합니다.
      1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) 헤더에서 프로젝트 이름 옆에 있는 을(를) 클릭한 다음 을(를) 클릭합니다. **재무 다시 계산**.
