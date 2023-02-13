---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "계산된 사용자 지정 필드 예: 문제 사용자 지정 양식에 문제 작성자의 관리자를 표시합니다."
description: 계산된 사용자 지정 필드를 사용하면 문제에 첨부된 사용자 지정 양식에 문제 작성자의 관리자 이름을 표시할 수 있습니다. 동일한 구문을 사용하여 프로젝트, 문제 및 기타 개체에 대해 유사한 계산된 필드를 작성할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 계산된 사용자 지정 필드 예: 문제 사용자 지정 양식에 문제 작성자의 관리자를 표시합니다.

계산된 사용자 지정 필드를 사용하면 문제에 첨부된 사용자 지정 양식에 문제 작성자의 관리자 이름을 표시할 수 있습니다. 동일한 구문을 사용하여 프로젝트, 문제 및 기타 개체에 대해 유사한 계산된 필드를 작성할 수 있습니다.

>[!TIP]
>
>다른 고객의 추가 사용자 지정 텍스트 모드 예제에 대한 자세한 내용은 [텍스트 모드 보고](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) 커뮤니티 사이트에 대한 주제입니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront 라이선스*</p> </td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>액세스 수준 구성*</td> 
   <td> <p>사용자 지정 양식에 대한 관리 액세스<br>액세스 수준에서 관리자 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>개체 권한</p> </td> 
   <td> <p>사용자 지정 양식 편집에 대한 액세스 권한과 함께 양식이 첨부된 객체에 대한 액세스 권한을 제공합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제 사용자 지정 양식에 문제 작성자의 관리자를 표시합니다

다음 단계는 문제를 만든 사용자의 관리자의 이름을 캡처할 수 있는 문제 사용자 지정 양식에 대해 계산된 필드를 만드는 방법을 보여줍니다. 작업, 프로젝트, 포트폴리오 등을 생성한 사용자의 관리자의 이름을 캡처하려면 프로세스가 동일합니다.

1. 문제 사용자 지정 양식을 만들고 계산된 필드를 추가합니다.

   사용자 지정 양식 만들기 및 여기에 계산된 필드 추가에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 다음 텍스트 모드 코드를 복사하여 **계산** 사용자 지정 양식의 필드:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >사용자 지정 필드 계산은 대/소문자를 구분합니다.

1. 클릭 **완료**, 그런 다음 **저장 + 닫기**.

   문제를 만든 사용자의 관리자가 필드가 포함된 양식이 문제에 첨부된 경우 계산된 필드에 표시됩니다.
