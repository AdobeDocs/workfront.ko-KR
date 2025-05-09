---
product-area: projects
navigation-topic: use-predecessors
title: 전임 작업 시행
description: 전임 작업은 다른 작업이 완료에 종속되는 작업입니다. 전임 작업 관계는 작업의 시작 및 완료 날짜에 영향을 주며 최종적으로 프로젝트의 타임라인에 영향을 줍니다.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 전임 작업 시행

<!-- Audited: 2/2024 -->

전임 작업은 다른 작업이 완료에 종속되는 작업입니다. 전임 작업 관계는 작업의 시작 및 완료 날짜에 영향을 주며 최종적으로 프로젝트의 타임라인에 영향을 줍니다.

전임 작업에 대한 자세한 내용은 [작업 전임 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)를 참조하십시오.

작업 간의 전임 작업 관계를 설정하여 종속 작업의 시작 또는 완료가 전임 작업의 시작 또는 완료에 따라 달라지는 방식을 정의합니다. 이 작업은 다양한 종속성 유형을 사용하여 수행됩니다.

종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)를 참조하십시오.

## 강제 전임 작업 개요

>[!IMPORTANT]
>
>전임 작업 관계를 준수하도록 전임 작업을 적용해야 합니다. 전임 작업을 적용하지 않으면 종속 작업은 종속성 유형에 관계없이 전임 작업의 시작 및 완료와 독립적으로 시작 및 완료될 수 있습니다.

프로젝트에 전임 작업을 설정할 때 전임 작업 관계를 적용할 수 있습니다.

전임 작업이 적용되면 전임 작업이 완료되기 전에 후임 작업을 시작할 수 없습니다. 예를 들어, 태스크 A와 태스크 B 간에 완료-시작 관계를 적용하면 태스크 A가 완료됨으로 표시될 때까지 태스크 B를 시작할 수 없습니다(상태는 신규 상태로 유지되어야 하고 완료율은 0%로 유지되어야 함). 관계 적용은 모든 전임 작업 유형에 적용됩니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
      <p>새로운 기능: 표준</p> 
      <p>또는</p>
      <p>현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td><p>작업 및 프로젝트에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 작업 수준에서 전임 작업 적용

1. 전임 작업을 적용할 후임 작업으로 이동합니다.
1. 왼쪽 패널에서 **전임 작업**&#x200B;을 클릭한 다음 **전임 작업 추가**&#x200B;를 클릭합니다.
1. (조건부) 프로젝트 간 전임 작업을 추가하려면 **상위 프로젝트** 필드에서 프로젝트 이름을 제거하고 다른 프로젝트로 바꾸십시오.
1. **작업** 필드에 전임 작업 이름을 지정하십시오.
1. 이 두 작업 사이에 **종속성 유형**&#x200B;을(를) 지정하십시오.

   기본 **종속성 유형**&#x200B;은(는) **마침-시작**&#x200B;입니다.

1. 전임 작업을 적용하려면 **적용됨** 필드를 선택하십시오.
1. **저장**&#x200B;을 클릭합니다.

## 작업 목록에 전임 작업 적용

1. 프로젝트의 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **표준 보기**&#x200B;를 선택합니다.

1. 전임 작업으로 지정할 작업의 수를 기록해 둡니다.
1. 전임 작업을 적용할 후임 작업을 찾습니다.
1. **전임 작업** 열에서 전임 작업의 수를 입력하고 그 뒤에 &quot;e&quot;를 입력합니다. 예를 들어 작업 번호 1을 선택한 작업에 전임 작업으로 추가하려면 &quot;1e&quot;를 입력합니다.
1. Enter 를 클릭하여 작업에 대한 전임 작업 정보를 저장합니다.

   ![전임 작업_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
