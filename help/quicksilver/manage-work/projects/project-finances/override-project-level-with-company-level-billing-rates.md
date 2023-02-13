---
product-area: projects
navigation-topic: financials
title: 회사 수준 청구 단가로 프로젝트 레벨 청구 비율 대체
description: 회사 수준 청구 단가로 프로젝트 레벨 청구 비율 대체
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 회사 수준 청구 단가로 프로젝트 레벨 청구 비율 대체

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

프로젝트 수준 청구 요금 대신 회사 수준 청구 비율을 사용하도록 프로젝트를 구성할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>Finance 관리 권한을 사용하여 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 회사 레벨 청구 비율 대체 옵션을 사용으로 설정합니다

회사가 프로젝트와 연관되어 있고 이 옵션이 활성화되면 회사 레벨 청구 단가를 변경하면 프로젝트에 설정된 청구 비율이 우선합니다.

사용자가 프로젝트에서 재무 상태를 수동으로 재계산하면 회사 수준 청구 비율에 대한 변경 사항이 적용됩니다. 내역 수익 계산도 청구됨으로 표시되지 않는 한 재정의됩니다.

1. 프로젝트로 이동합니다.
1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) 헤더에서 프로젝트 이름 옆에 있는 를 클릭합니다. **편집**.
1. 에서 **재무** 섹션에서 활성화 **회사 수준의 청구 요금이 프로젝트 수준의 청구 비율을 무효화하도록 허용**.

   >[!CAUTION]
   >
   >이 옵션을 활성화하면 청구로 표시되지 않는 한 내역 수익 계산을 무시합니다. 청구 레코드를 생성하여 내역 수익 계산을 유지할 수 있습니다. 자세한 내용은 문서를 참조하십시오 [청구 레코드 만들기](../../../manage-work/projects/project-finances/create-billing-records.md)

1. 클릭 **변경 내용 저장**.

## 회사 레벨 청구 비율을 갱신하고 프로젝트에 적용합니다

프로젝트에서 회사 레벨 청구 비율 대체 옵션을 활성화하면, 회사 청구 비율에 대한 변경 사항이 재무 재계산될 때마다 프로젝트에 적용됩니다.

>[!NOTE]
>
>사용자는 회사 수준의 청구 비율을 업데이트하려면 액세스 수준에서 회사에 액세스할 수 있어야 합니다.

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **설정**.
1. 클릭 **회사**.
1. 회사 레벨 청구 비율 대체를 활성화한 프로젝트와 연관된 회사 이름을 누릅니다.
1. 클릭 **청구 비율** 왼쪽 패널에 표시됩니다.
1. 기존 작업 역할에 대한 신규 청구 비율을 **회사 청구 비율** 필드를 입력한 다음 Enter 키를 누릅니다.
1. 하나 이상의 프로젝트에 대한 회사 비율을 갱신하려면 다음 중 하나를 수행합니다.

   * 여러 프로젝트:
   1. 프로젝트 목록으로 이동합니다.
   1. 업데이트할 프로젝트에 따라 확인란을 선택합니다.
   1. 클릭 **편집**.
   1. 설정 섹션에서 **비용 및 수익 재계산** 선택 사항입니다.
   1. 클릭 **변경 내용 저장**.
   * 단일 프로젝트:

      1. 회사 수준 청구 비율 대체를 활성화한 프로젝트로 이동합니다.
      1. 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png) 헤더에서 프로젝트 이름 옆에 있는 를 클릭하고 **재무 재계산**.
