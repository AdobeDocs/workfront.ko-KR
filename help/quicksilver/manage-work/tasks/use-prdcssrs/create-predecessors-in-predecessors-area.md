---
product-area: projects
navigation-topic: use-predecessors
title: 선행 작업 영역을 사용하여 선행 관계 만들기
description: 선행 작업(또는 선행 작업)을 사용하여 다른 작업에 의존하는 작업을 시작 또는 완료하도록 연결할 수 있습니다. 예를 들어 초대장(선행 작업)을 보내기 전에 파티(종속 작업)를 호스팅하지 않으려는 경우
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# 선행 작업 영역을 사용하여 선행 관계 만들기

선행 작업(또는 선행 작업)을 사용하여 다른 작업에 의존하는 작업을 시작 또는 완료하도록 연결할 수 있습니다. 예를 들어 초대장(선행 작업)을 보내기 전에 파티(종속 작업)를 호스팅하지 않으려는 경우

이 문서에서는 작업 내에서 선행 작업 탭을 사용하여 선행 작업을 설정하는 방법을 보여 줍니다.

작업 목록에서 선행 작업을 설정하는 방법에 대한 자세한 내용은 [작업 목록에서 선행 관계 만들기](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

다음 Adobe Workfront 영역에서 작업 선행 작업을 볼 수 있습니다.

* 종속 작업의 선행 작업 섹션에서
* 간트 차트
* 선행 작업 열의 작업 목록

선행자에 대한 자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

## 작업에 대한 선행 작업 만들기

1. 종속 작업으로 지정할 작업으로 이동한 다음 **선행 작업** 왼쪽 패널에 표시됩니다.

   을(를) 클릭하여 **자세히 표시**, 그런 다음 **선행 작업**.

1. 클릭 **+선행 항목 추가**.
1. (선택 사항) 교차 프로젝트 전임자를 추가하려면 **상위 프로젝트** 다른 프로젝트가 있는 필드에 선행 작업으로 원하는 작업 또는 작업의 이름을 입력합니다.

   프로젝트 간 선행 작업 추가에 대한 자세한 내용은 [프로젝트 간 선행 작업 만들기](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. 선행 작업으로 지정할 작업 또는 작업의 이름을 입력합니다.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. 선택 **종속성 유형**.

   작업 종속성 유형에 대한 자세한 내용은 [작업 종속성 유형 개요](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 을(를) 지정합니다 **지연** 일 단위 금액입니다.

   지연 유형에 대한 자세한 내용은 다음을 &#x200B; 참조하십시오 [지연 유형 개요](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. 선택 **강제 적용** 두 작업 간에 이전 관계를 적용하려는 경우

   이전 버전 실행에 대한 자세한 내용은 [선행 작업 적용](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. **저장**&#x200B;을 클릭합니다.
