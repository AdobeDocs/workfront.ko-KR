---
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 계획자 찾기
description: '(이 문서는 다음 문서에서 제공됨: 문서가 라이브로 제공되면 해당 컨텐츠에 초안 생성: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 리소스 계획자 찾기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

자원 계획자를 사용하여 프로젝트에 대한 자원 할당을 관리할 수 있습니다. 프로젝트의 업무 사례 영역에서 여러 프로젝트에 대한 자원 계획자에 동시에 액세스하거나 한 프로젝트에 대해 액세스할 수 있습니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

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
   <td> <p>검토 이상<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>글로벌 영역에서 자원 계획자를 찾기 위한 계획 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 관리에 대한 액세스 이상 보기</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 사용자에 대한 권한 보기 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

사용을 시작하기 전에 Resource Planner에 액세스하고 작업하기 위한 모든 전제 조건을 충족하는지 확인합니다. 이렇게 하면 자원 예산 책정을 시작하기 전에 자원 계획자가 올바른 정보를 표시해야 합니다.

리소스 플래너 사전 요구 사항에 대한 자세한 내용은 [리소스 계획 시작](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## 리소스 계획자 찾기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

여러 프로젝트에 대한 리소스를 예산을 책정할 것인지 아니면 한 프로젝트에만 투자할 것인지에 따라 Workfront의 두 영역에서 리소스 계획자를 찾을 수 있습니다.

* [여러 프로젝트에 자원 계획자 사용](#use-the-resource-planner-for-multiple-projects)
* [프로젝트 하나에 자원 계획자 사용](#use-the-resource-planner-for-one-project)

### 여러 프로젝트에 자원 계획자 사용 {#use-the-resource-planner-for-multiple-projects}

여러 프로젝트에 대해 자원 계획자를 사용하는 경우 자원에 대한 할당 번호는 여러 프로젝트의 숫자를 나타냅니다.

자원 영역에서 계획자 섹션에 액세스하려면

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

1. 클릭 **리소스**. 기본적으로 계획자가 표시됩니다.  Resource Planner의 예산 책정 자원에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 및 역할 보기를 사용하는 자원 계획자의 예산 자원](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 왼쪽 패널을 마우스로 가리킨 다음 을 클릭합니다 **리소스 풀**.\
   리소스 풀 만들기에 대한 내용은 [리소스 풀 만들기](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### 프로젝트 하나에 자원 계획자 사용 {#use-the-resource-planner-for-one-project}

한 프로젝트에 대해 자원 계획자를 사용하는 경우 자원에 대한 할당 번호는 선택한 프로젝트에 대한 숫자를 나타냅니다.

1. 리소스를 예산을 편성할 프로젝트로 이동합니다.
1. 클릭 **비즈니스 사례** 왼쪽 패널에 표시됩니다.
1. 로 스크롤합니다. **리소스 예산 책정** 비즈니스 사례 섹션
1. 클릭 **리소스 예산 책정 편집** 프로젝트에 리소스 풀을 추가하고 리소스 예산을 책정하는 작업을 시작합니다.

   >[!TIP]
   >
   >프로젝트에 연관된 자원 풀이 없는 경우 Business Case의 Resource Budgeting 영역에서만 리소스 풀을 추가할 수 있습니다. 프로젝트에 이미 리소스 풀이 있는 경우 기본적으로 풀의 사용자와 해당 작업 역할이 리소스 예산 책정 영역에 표시됩니다.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   하나의 프로젝트에 대한 예산 책정 리소스에 대한 내용은 문서를 참조하십시오 [비즈니스 사례의 예산 자원](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
