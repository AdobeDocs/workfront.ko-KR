---
product-area: projects
navigation-topic: financials
title: 프로젝트 경비 관리
description: 비용을 생성하고 관리하는 프로세스는 프로젝트 및 작업 관련 비용 모두에 대해 동일합니다. 비즈니스 사례에서 프로젝트에 추가된 모든 경비는 계획된 경비로 경비 탭에 추가됩니다. 비즈니스 사례에 대한 자세한 내용은 프로젝트에 대한 비즈니스 사례 만들기 문서를 참조하십시오.
author: Alina
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 1%

---

# 프로젝트 경비 관리

비용을 생성하고 관리하는 프로세스는 프로젝트 및 작업 관련 비용 모두에 대해 동일합니다. 비즈니스 사례에서 프로젝트에 추가된 모든 경비는 계획된 경비로 경비 탭에 추가됩니다. 비즈니스 사례에 대한 자세한 내용은 [프로젝트에 대한 비즈니스 사례 만들기](../../../manage-work/projects/define-a-business-case/create-business-case.md) 문서를 참조하십시오.

모든 작업 및 프로젝트의 총 경비 금액이 프로젝트의 총 비용에 기여합니다. 경비의 계획된 금액은 사업의 계획된 비용에 기여하고, 경비의 실제 금액은 사업의 실제 비용에 기여한다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>작업 이상 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트 및 재무 데이터에 대한 액세스 편집</p> <p><b>참고</b> </p>
   <p> 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>재무 보기 또는 관리 권한이 있는 프로젝트에 대한 Contribute 이상의 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 경비 추가

1. 비용을 입력하려는 프로젝트로 이동합니다.\
   작업에 경비를 추가하려면 작업으로 이동하십시오. 
1. **자세히 표시**&#x200B;를 클릭한 다음 **경비**&#x200B;를 클릭합니다.
1. **경비 추가** 를 클릭합니다.
**경비 추가** 대화 상자가 표시됩니다.
1. 다음 내용을 업데이트합니다.

   * **설명:** 비용에 대한 설명입니다.

   * **경비 유형:**(필수) 경비를 가장 잘 설명하는 범주를 선택하십시오.
   * **작업:** 이 비용과 관련된 작업의 이름을 입력한 다음 드롭다운 목록에 나타나면 해당 이름을 클릭합니다.
   * **계획된 금액:** 경비의 계획된 예산 금액입니다.\
     이는 프로젝트의 예산 비용에 영향을 줍니다.

   * **실제 금액:** 실제 비용이 소요된 금액입니다.\
     이는 프로젝트의 실제 비용에 영향을 줍니다.

   * **계획된 일자:** 비용이 발생할 예상 일자입니다. *mm/dd/yy* 형식을 사용하여 필드에 날짜를 입력하거나 달력 아이콘을 클릭할 수 있습니다  ![](assets/calendar-icon.png)을(를) 클릭하고 날짜를 동적으로 선택합니다.

   * **지급일:** 경비가 지급된 날입니다.
   * **청구 가능:** 이 비용을 청구하려면 이 옵션을 선택하십시오. 청구 기록을 생성할 때 경비를 청구 가능으로 분류하는 것이 중요합니다.
   * **정산 가능:** 경비를 정산해야 하는 경우 이 옵션을 선택하십시오. 그런 다음 경비가 상환된 후 경비를 상환된 것으로 표시할 수 있습니다.

1. **사용자 정의 양식**&#x200B;을(를) 선택하고 필요한 추가 정보를 지정하십시오. 사용자 정의 양식을 비용과 연결하려면 먼저 만들어야 합니다. 활성 사용자 정의 양식만 목록에 표시됩니다. 사용자 정의 양식 만들기에 대한 자세한 내용은 문서 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. **변경 내용 저장**&#x200B;을 클릭합니다.

## 비용 삭제

1. 경비를 삭제할 프로젝트로 이동합니다.
1. **자세히 표시**&#x200B;를 클릭한 다음 **경비**&#x200B;를 클릭합니다.
1. 삭제할 경비를 선택한 다음 **삭제** ![삭제](assets/delete.png)를 클릭합니다.

1. 삭제를 확인하려면 **예, 삭제**&#x200B;를 클릭하십시오.
