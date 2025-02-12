---
product-area: resource-management
navigation-topic: resource-planning
title: 리소스 플래너에서 예산 책정 일자 조정
description: 리소스 플래너에서 예산을 책정한 후 리소스에 대한 초과 할당이 있는 경우 예산 시간, FTE 또는 비용을 다른 시간대로 이동하여 가정 시나리오를 살펴볼 수 있습니다. 이러한 시나리오의 결과를 기반으로 예산 시간, FTE 또는 비용을 조정할 수 있습니다.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

# 리소스 플래너에서 예산 책정 일자 조정

리소스 플래너에서 예산을 책정한 후 리소스에 대한 초과 할당이 있는 경우 예산 시간, FTE 또는 비용을 다른 시간대로 이동하여 가정 시나리오를 살펴볼 수 있습니다. 이러한 시나리오의 결과를 기반으로 예산 시간, FTE 또는 비용을 조정할 수 있습니다.

초과 할당은 자원의 예산 시간, FTE 또는 비용이 가용 시간, FTE 또는 비용보다 높을 때 나타날 수 있습니다. 음수 순 값을 생성합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
    <td><p>새로 만들기: 모두</p>
       <p>또는</p>
       <p>현재: Pro 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>리소스 플래너에서 우선순위 및 예산 시간 편집에 대한 액세스 권한이 포함된 리소스 관리에 대한 액세스 편집</p> <p>재무 데이터, 프로젝트 및 사용자에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 관리 기능으로 예산을 책정하려는 프로젝트에 대한 권한을 관리합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 예산 책정 일자 조정

1. 리소스 플래너로 이동하고 **프로젝트별 보기**&#x200B;를 선택합니다.

   >[!NOTE]
   >
   >프로젝트별 리소스 플래너를 볼 때만 예산 일자 조정 옵션을 사용할 수 있습니다.

1. 프로젝트 이름 위로 마우스를 가져간 다음 **자세히** 메뉴를 클릭합니다.
1. **예산 책정 날짜 조정**&#x200B;을 클릭합니다.\
   프로젝트 할당 타임라인이 표시됩니다.\
   현재 시간이 예산으로 책정된 시간대는 예산 충돌이 있는 경우 주황색으로, 충돌이 없는 경우 파란색으로 강조 표시됩니다.

   ![예산 책정 날짜 조정](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. 강조 표시된 시간대를 다른 시간으로 끌어다 놓아 선택한 프로젝트에 대해 예산 충돌이 없는 위치를 이해합니다. [순] 값이 양수인 시간대를 찾으면 강조 표시된 시간대가 파란색으로 바뀝니다.
1. 프로젝트 할당 타임라인의 오른쪽 위 모서리에 있는 &quot;x&quot;를 클릭하여 닫습니다.
1. 프로젝트의 기존 타임라인에서 예산 시간을 제거하고 가장 많은 가용성을 보여주는 타임라인에 추가합니다.
1. **저장**&#x200B;을 클릭합니다.
1. (조건부 및 선택 사항) 예산 충돌이 없는 시간대가 프로젝트의 타임라인을 벗어나는 경우 프로젝트 이름을 클릭하여 프로젝트에 액세스합니다.
1. (조건부 및 선택 사항) **프로젝트 편집**&#x200B;을 클릭한 다음 **계획된 시작 일자** 또는 **계획된 완료 일자**&#x200B;를 편집하여 예산 충돌이 없는 기간에 대한 프로젝트의 타임라인을 수정합니다.\
   프로젝트 편집에 대한 자세한 내용은 문서 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md)을 참조하세요.

1. (조건부 및 선택 사항) **변경 내용 저장**&#x200B;을 클릭합니다.
1. 리소스 플래너로 돌아가서 예산 충돌 없이 시간대에 예산 시간, FTE 또는 비용을 다시 입력합니다.
1. **저장**&#x200B;을 클릭합니다.
