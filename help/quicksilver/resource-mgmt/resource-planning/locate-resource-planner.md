---
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 플래너 찾기
description: '(이 문서의 결론은 다음과 같습니다. 라이브할 때 문서의 해당 내용 초안: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 리소스 플래너 찾기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

리소스 플래너를 사용하여 프로젝트에 대한 리소스 할당을 관리할 수 있습니다. 프로젝트의 비즈니스 사례 영역에서 동시에 또는 하나의 프로젝트에 대한 리소스 플래너에 액세스할 수 있습니다.

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>검토 이상<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>계획 이상을 수행하여 전역 영역에서 리소스 플래너를 찾습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 관리에 대한 액세스 이상 보기</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트 및 사용자에 대한 권한 보기 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

리소스 플래너 사용을 시작하기 전에 리소스 플래너에 액세스하고 리소스 플래너로 작업하기 위한 모든 전제 조건이 충족되는지 확인하십시오. 이렇게 하면 리소스 예산을 책정하기 전에 리소스 플래너에 올바른 정보가 표시되는지 확인합니다.

리소스 플래너 필수 구성 요소에 대한 자세한 내용은 [리소스 계획 시작](../../resource-mgmt/resource-planning/get-started-resource-planning.md)을 참조하세요.

## 리소스 플래너 찾기

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

여러 프로젝트에 대한 리소스 예산을 책정할 것인지 아니면 하나의 프로젝트에 대한 리소스 예산을 책정할 것인지에 따라 Workfront의 두 영역에서 리소스 플래너를 찾을 수 있습니다.

* [여러 프로젝트에 리소스 플래너 사용](#use-the-resource-planner-for-multiple-projects)
* [한 프로젝트에 리소스 플래너 사용](#use-the-resource-planner-for-one-project)

### 여러 프로젝트에 리소스 플래너 사용 {#use-the-resource-planner-for-multiple-projects}

여러 프로젝트에 리소스 플래너를 사용할 때 리소스에 대한 할당 번호는 여러 프로젝트의 번호를 나타냅니다.

리소스 조달 영역의 플래너 섹션에 액세스하려면 다음을 수행하십시오.

1. Adobe Workfront 오른쪽 상단의 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭합니다.

1. **리소스 조달**&#x200B;을 클릭합니다. 기본적으로 플래너가 표시됩니다.  리소스 플래너의 리소스 예산 책정에 대한 자세한 내용은 문서 [프로젝트 및 역할 보기를 사용하여 리소스 플래너의 리소스 예산](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)을 참조하십시오.

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 왼쪽 패널을 마우스로 가리킨 다음 **리소스 풀**&#x200B;을 클릭합니다.\
   리소스 풀 만들기에 대한 자세한 내용은 [리소스 풀 만들기](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)를 참조하십시오.

### 한 프로젝트에 리소스 플래너 사용 {#use-the-resource-planner-for-one-project}

한 프로젝트에 대해 리소스 플래너를 사용할 때 리소스의 할당 번호는 선택한 프로젝트에 대한 번호를 나타냅니다.

1. 리소스 예산을 책정할 프로젝트로 이동합니다.
1. 왼쪽 패널에서 **비즈니스 사례**&#x200B;를 클릭합니다.
1. 비즈니스 사례의 **리소스 예산 책정** 섹션으로 스크롤합니다.
1. 프로젝트에 리소스 풀을 추가하고 리소스 예산을 책정하려면 **리소스 예산 편성 편집**&#x200B;을 클릭하십시오.

   >[!TIP]
   >
   >프로젝트에 연결된 리소스 풀이 없는 경우 비즈니스 사례의 리소스 예산 책정 영역에만 리소스 풀을 추가할 수 있습니다. 프로젝트에 이미 리소스 풀이 있는 경우, 풀의 사용자와 해당 작업 역할이 기본적으로 리소스 예산 책정 영역에 표시됩니다.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   한 프로젝트의 리소스 예산 편성에 대한 자세한 내용은 [비즈니스 사례의 리소스 예산](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md) 문서를 참조하십시오.
