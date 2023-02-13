---
product-area: resource-management
navigation-topic: resource-planning
title: 자원 계획자에서 예산 책정 일자 조정
description: Resource Planner에서 자원을 설정한 후 자원의 초과 할당이 있는 경우 예산책정된 시간, FTE 또는 비용을 다른 시간 프레임으로 이동하여 가능한 시나리오를 탐색할 수 있습니다. 이러한 시나리오의 결과에 따라 예산 책정된 시간, FTE 또는 비용을 조정할 수 있습니다.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# 자원 계획자에서 예산 책정 일자 조정

Resource Planner에서 자원을 설정한 후 자원의 초과 할당이 있는 경우 예산책정된 시간, FTE 또는 비용을 다른 시간 프레임으로 이동하여 가능한 시나리오를 탐색할 수 있습니다. 이러한 시나리오의 결과에 따라 예산 책정된 시간, FTE 또는 비용을 조정할 수 있습니다.

초과 할당은 자원의 예산책정된 시간, FTE 또는 비용이 사용 가능한 시간, FTE 또는 비용보다 높을 때 나타날 수 있습니다. 이렇게 하면 음수 순 값이 생성됩니다.

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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>리소스 계획자의 우선순위 및 예산 시간 편집에 대한 액세스 권한을 포함하는 리소스 관리에 대한 액세스 편집</p> <p>재무 데이터, 프로젝트 및 사용자에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 기능을 사용하여 예산을 책정하려는 프로젝트에 대한 권한을 관리합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 예산 책정 일자 조정

1. 리소스 계획자로 이동하여 를 선택합니다 **프로젝트별 보기**.

   >[!NOTE]
   >
   >프로젝트별 자원 계획자를 조회할 때만 예산책정된 일자 조정 옵션을 사용할 수 있습니다.

1. 프로젝트 이름을 마우스로 가리킨 다음, **자세히** 메뉴 아래의 제품에서 사용할 수 있습니다.
1. 클릭 **예산 책정 날짜 조정**.\
   프로젝트 할당 타임라인이 표시됩니다.\
   현재 시간 예산책정된 기간은 예산 충돌이 있는 경우 주황색으로 강조 표시되고 충돌이 없는 경우에는 파란색으로 강조 표시됩니다.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. 강조 표시된 기간을 다른 시간으로 끌어다 놓아 선택한 프로젝트에 대한 예산 충돌이 없는 위치를 파악합니다. 네트 값이 양수인 기간을 찾으면 강조 표시된 시간 프레임이 파란색으로 변경됩니다.
1. 프로젝트 할당 타임라인의 오른쪽 위 모서리에 있는 &quot;x&quot;를 클릭하여 닫습니다.
1. 프로젝트의 기존 타임라인에서 예산책정된 시간을 제거하고 가장 사용 가능한 시간을 보여 주는 타임라인에 추가합니다.
1. **저장**&#x200B;을 클릭합니다.
1. (조건부 및 선택 사항) 예산 충돌이 없는 기간이 프로젝트 타임라인을 벗어나는 경우 프로젝트 이름을 클릭하여 프로젝트에 액세스합니다.
1. (조건부 및 선택 사항) **프로젝트 편집**&#x200B;를 편집한 다음 **계획 시작 날짜** 또는 **계획 완료 일자** 예산 편성에 충돌하지 않고 기간 동안 프로젝트의 타임라인을 수정하려면\
   프로젝트 편집에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md).

1. (조건부 및 선택 사항) **변경 내용 저장**.
1. Resource Planner로 돌아가서 예산책정 작업 시간, FTE 또는 비용을 예산 충돌 없이 기간 내에 다시 입력합니다.
1. **저장**&#x200B;을 클릭합니다.
