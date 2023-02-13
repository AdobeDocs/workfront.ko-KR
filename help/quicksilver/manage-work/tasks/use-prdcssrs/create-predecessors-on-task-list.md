---
product-area: projects
navigation-topic: use-predecessors
title: 작업 목록에서 선행 관계 만들기
description: 선행 작업(또는 선행 작업)을 사용하여 다른 작업에 의존하는 작업을 시작 또는 완료하도록 연결할 수 있습니다. 예를 들어 초대장(선행 작업)을 보내기 전에 파티(종속 작업)를 호스팅하지 않으려는 경우
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# 작업 목록에서 선행 관계 만들기

선행 작업(또는 선행 작업)을 사용하여 다른 작업에 의존하는 작업을 시작 또는 완료하도록 연결할 수 있습니다. 예를 들어 초대장(선행 작업)을 보내기 전에 파티(종속 작업)를 호스팅하지 않으려는 경우

이 문서에서는 작업 목록에서 선행 작업을 만드는 방법을 보여 줍니다.

다음 Adobe Workfront 영역에서 작업 선행 작업을 볼 수 있습니다.

* 선행 작업 열의 작업 목록
* 간트 차트
* 종속 작업의 선행 작업 섹션에서

자세한 내용은 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>작업 및 프로젝트에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업 및 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 선행 작업 만들기

1. 프로젝트로 이동합니다.
1. 클릭 **작업** 왼쪽 패널에 표시됩니다.
1. 현재 보기에 **전임자** 열.

   보기에 선행 작업 열이 표시되지 않으면 해당 보기로 변경하거나 열에 열을 추가합니다.

1. 종속 작업으로 지정할 작업을 선택합니다.
1. 의 내부를 클릭합니다. **선행 작업** 열.
1. 선택한 작업의 선행 작업으로 지정할 작업 번호를 입력한 다음 키를 누릅니다 **Enter 키**.

   선행 작업이 완료된 것으로 표시되면 선행 작업 아이콘이 녹색으로 바뀝니다. 종속 작업이 작업을 수행할 준비가 되었음을 나타냅니다.

   선행 작업 열에서 사용할 수 있는 관계 유형에 대한 자세한 내용은 선행 작업 열을 참조하십시오 [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [작업 선행 작업 개요](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 이전 세부 정보 보기

작업 목록에서 선행 작업에 대한 세부 정보를 빠르게 볼 수 있습니다.

1. 작업 목록에서 이전 번호를 마우스로 가리키면 **선행 작업** 열.

   선행 작업의 세부 사항이 표시된 상자가 표시됩니다.

   ![이전 정보](assets/predecessor-details-in-task-list.png)

   다음 세부 정보가 표시됩니다.

   **이전 이름:** 참조되고 있는 선행 작업의 이름입니다. 선행 작업의 작업 번호가 포함됩니다. 작업 이름을 클릭하여 엽니다. 위의 예에서 전임자는 프로덕션/실행/게재입니다.

   **프로젝트 이름:** 이전 프로젝트가 있는 프로젝트의 이름입니다. 이전 프로젝트가 작업과 동일한 프로젝트에 속하는 경우, 또는 이전 프로젝트가 다른 프로젝트에 속하는 경우 교차 프로젝트로 식별됩니다. 위의 예에서 프로젝트 이름은 Digital Asset Production (Integrated) - Project입니다. 프로젝트 간 선행 작업에 대한 자세한 내용은 [프로젝트 간 선행 작업 만들기](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   프로젝트 세부 정보를 확장하여 프로젝트의 계획 시작 및 종료 날짜, 조건, 상태, 완료% 및 소유자를 볼 수 있습니다. 그런 다음 교차 프로젝트의 경우 **프로젝트 를 참조하십시오** 프로젝트를 엽니다.

   **ID:** 이전 프로젝트가 있는 프로젝트의 참조 번호입니다.

   **계획된 시작:** 선행 작업의 계획 시작 날짜입니다.

   **예정된 종료:** 선행 작업의 계획 완료 일자입니다.

   **선행 작업 수:** 참조되는 전임자의 선행 작업 수입니다. 위의 예에서 참조되는 이전 모델에는 1개의 이전 제품이 있습니다.

   **상속자 수:** 참조되는 선행 작업의 후속 작업(또는 종속) 수입니다. 위의 예에서, 참조되는 이전 모델에는 1개의 후속 제품이 있습니다.
