---
product-area: projects
navigation-topic: use-predecessors
title: 선행 작업 적용
description: 선행 작업은 다른 작업이 완료에 종속되는 작업입니다. 선행 관계는 작업의 시작 및 완료 날짜에 영향을 주며 결과적으로 프로젝트의 타임라인에 영향을 줍니다.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# 선행 작업 적용

선행 작업은 다른 작업이 완료에 종속되는 작업입니다. 선행 관계는 작업의 시작 및 완료 날짜에 영향을 주며 결과적으로 프로젝트의 타임라인에 영향을 줍니다.

선행자에 대한 자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

작업 간의 선행 관계를 설정하여 종속 작업의 시작 또는 완료가 이전 작업의 시작 또는 완료에 따라 어떻게 달라지는지를 정의합니다. 이 작업은 다른 종속성 유형을 사용하여 수행됩니다.

종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## 적용된 이전 버전 개요

>[!IMPORTANT]
>
>전임자의 관계가 존중되도록 하기 위해서는 전임자들을 강제해야 한다. 선행자가 적용되지 않으면 종속 작업은 종속성 유형에 관계없이 선행자의 시작 및 종료와 독립적으로 시작 및 완료할 수 있습니다.

프로젝트에 선행 작업을 설정할 때 이전 관계를 적용할 수 있습니다.

전임자가 집행되면 전임자가 완료되기 전에 후속 작업을 시작할 수 없습니다. 예를 들어, 태스크 A와 태스크 B의 완료-시작 관계를 적용하면 태스크 B가 완료 상태로 표시될 때까지 태스크 B를 시작할 수 없습니다(상태는 신규 상태로, 완료율은 0%로 유지되어야 함). 관계 적용은 모든 이전 유형에 적용됩니다.

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 작업 수준에서 선행 작업 적용

1. 이전 작업을 수행하려는 후속 작업으로 이동합니다.
1. 클릭 **선행 작업** 왼쪽 패널에서 **선행 작업 추가**. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **선행 작업**.
1. (조건부) 교차 프로젝트 전임자를 추가하려면 **상위 프로젝트** 필드를 만들어 다른 프로젝트로 바꿉니다.
1. 선행 작업 또는 작업의 이름을 **작업** 필드.
1. 을(를) 지정합니다. **종속성 유형** 이 두 작업 사이에 있을 수 있습니다.

   기본값 **종속성 유형** is **완료 시작**.

1. 을(를) 선택합니다 **강제 적용** 전임자를 집행하기 위한 분야.
1. **저장**&#x200B;을 클릭합니다.

## 작업 목록에서 선행 작업 적용

1. 프로젝트의 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **표준 보기**.

1. 당신이 전임자로 지정할 작업의 수를 정신 있게 기록하라.
1. 선행 작업을 적용할 후속 작업을 찾습니다.
1. 에서 **선행 작업** 열에서 선행 작업 번호 입력 후 &quot;e&quot; 입력 시작 예를 들어, &quot;1e&quot;를 입력하여 선택된 작업의 선행 작업으로 작업 번호 1을 추가합니다.
1. 작업에 대한 이전 정보를 저장하려면 Enter 키를 누릅니다.

   ![npr_forced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
