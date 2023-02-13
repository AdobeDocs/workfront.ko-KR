---
product-area: projects
navigation-topic: task-duration
title: 단순 기간 유형으로 작업의 계획 시간 및 기간 업데이트
description: 기본적으로 Adobe Workfront은 계획 시간의 양을 기준으로 단순 기간 유형으로 작업 기간을 계산합니다. 그러나 Workfront의 특정 영역에서 계획 시간 및 단순 기간 작업의 기간을 수동으로 편집할 수도 있습니다.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# 단순 기간 유형으로 작업의 계획 시간 및 기간 업데이트

기본적으로 Adobe Workfront은 계획 시간의 양을 기준으로 단순 기간 유형으로 작업 기간을 계산합니다. 그러나 Workfront의 특정 영역에서 계획 시간 및 단순 기간 작업의 기간을 수동으로 편집할 수도 있습니다.

단순 기간 유형 인라인이나 지정 영역의 태스크 레벨에서 태스크의 계획 시간 및 기간을 편집할 수 있습니다.

인라인 정보 편집에 대한 자세한 내용은 [Adobe Workfront의 목록에서 인라인 편집 항목](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

이 문서에서는 지정 영역에서 태스크 레벨의 단순 기간 유형으로 태스크에 대한 계획 시간 및 기간을 갱신하는 방법에 대해 설명합니다.

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
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>작업에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>작업에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 단순 기간 유형으로 작업의 계획 시간 및 기간 업데이트

>[!IMPORTANT]
>
>단순 기간 작업에 대해 지속 시간을 수동으로 업데이트한 후 Workfront에서는 계획 시간을 기반으로 기간 계산을 중지합니다.

고급 지정 상자에서 단순 기간 유형으로 작업의 계획 시간 및 기간을 편집하려면

1. 작업 목록에서 기간 유형을 변경할 작업 이름을 클릭합니다.
1. 다음 중 하나를 수행하십시오.

   * 을(를) 클릭합니다. **자세히** 아이콘 ![](assets/qs-more-icon-on-an-object.png) 작업 이름 옆의 **편집**, 그런 다음 **지정**.
   * 을(를) 클릭합니다. **지정 대상** 또는 작업 헤더의 지정 영역에 있는 지정 이름을 클릭한 다음 **고급**.

1. 에 대한 합계 값을 입력합니다. **계획 시간** 모든 지정(예: 10시간) 총 계획 시간 수는 태스크에 지정된 모든 자원 간에 균등하게 분배됩니다.
1. (선택 사항) 태스크에 지정된 각 자원의 계획 시간 을 수동으로 조정합니다. 자원에 개별적으로 지정된 새 시간을 반영하도록 태스크 갱신에 대한 총 계획 시간 수
1. 작업에 대한 값을 입력합니다 **기간**&#x200B;예: 2일

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. **저장**&#x200B;을 클릭합니다.
