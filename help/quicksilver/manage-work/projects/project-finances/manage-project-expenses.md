---
product-area: projects
navigation-topic: financials
title: 프로젝트 비용 관리
description: 비용 생성 및 관리 프로세스는 프로젝트 및 태스크 관련 비용 모두에 대해 동일합니다. 업무 사례에서 프로젝트에 추가되는 모든 비용은 계획 비용으로 비용 탭에 추가됩니다. 비즈니스 사례에 대한 자세한 내용은 프로젝트에 대한 비즈니스 사례 만들기 문서를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 1%

---

# 프로젝트 비용 관리

비용 생성 및 관리 프로세스는 프로젝트 및 태스크 관련 비용 모두에 대해 동일합니다. 업무 사례에서 프로젝트에 추가되는 모든 비용은 계획 비용으로 비용 탭에 추가됩니다. 비즈니스 사례에 대한 자세한 내용은 문서를 참조하십시오 [프로젝트에 대한 비즈니스 사례 생성](../../../manage-work/projects/define-a-business-case/create-business-case.md).

모든 작업 및 프로젝트의 총 비용 금액이 프로젝트의 총 비용에 기여합니다. 비용 계획 금액은 프로젝트의 계획 원가에 기여하며, 실제 비용 금액은 프로젝트의 실제 원가에 기여합니다.

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

## 경비 추가

1. 비용을 입력할 프로젝트로 이동합니다.\
   작업에 비용을 추가하려면 태스크로 이동합니다. 
1. 클릭 **표시**** 자세히** **비용.**
1. 클릭 **비용을 추가합니다.**
해당 
**비용 추가** 대화 상자가 표시됩니다.
1. 다음을 업데이트합니다.

   * **설명:** 비용에 대한 설명입니다.

   * **비용 유형:** (필수) 비용을 가장 잘 설명하는 범주를 선택합니다.
   * **작업:** 이 비용과 관련된 작업의 이름을 입력한 다음 드롭다운 목록에 나타나면 클릭합니다.
   * **계획 금액:** 비용에 대한 계획된 예산 금액입니다.\
      이는 프로젝트의 예산 비용에 영향을 줍니다.

   * **실제 금액:** 비용 실제 비용의 금액입니다.\
      이는 프로젝트의 실제 원가에 영향을 줍니다.

   * **계획 일자:** 비용이 발생할 것으로 예상되는 날짜입니다. 필드에 날짜를 입력하고 *mm/dd/yy* 서식을 지정하거나 달력 아이콘을 클릭할 수 있습니다  ![](assets/calendar-icon.png) 날짜를 동적으로 선택합니다.

   * **지불 날짜:** 비용이 지불된 날짜입니다.
   * **청구가능:** 이 비용을 청구하려면 이 옵션을 선택합니다. 청구 레코드를 생성할 때 비용을 청구 가능한 것으로 분류하는 것이 중요합니다.
   * **환급 가능:** 비용을 상환해야 하는 경우 이 옵션을 선택합니다. 그러면 비용이 상환된 후에 그 비용을 상환으로 표시할 수 있습니다.

1. 선택 **사용자 지정 양식** 필요한 추가 정보를 지정합니다. 비용과 연결하려면 먼저 사용자 지정 양식을 만들어야 합니다. 활성 사용자 지정 양식만 목록에 표시됩니다. 사용자 지정 양식 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 클릭 **변경 사항을 저장합니다.**

## 비용 삭제

1. 비용을 삭제할 프로젝트로 이동합니다.
1. 클릭&#x200B;**보기****자세히**&#x200B;를 클릭한 다음 **비용.**
1. 삭제할 비용을 선택한 다음 **삭제** ![삭제](assets/delete.png).

1. 클릭 **예, 삭제합니다.** 삭제를 확인하는 중입니다. 
