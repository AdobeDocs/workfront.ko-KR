---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '계산된 사용자 정의 필드 예: 문제 사용자 정의 양식에 문제 작성자의 관리자 표시'
description: 계산된 사용자 정의 필드를 사용하면 문제에 첨부된 사용자 정의 양식에 문제 작성자의 관리자 이름을 표시할 수 있습니다. 동일한 명령문을 사용하여 프로젝트, 문제 및 기타 개체에 대해 유사한 계산된 필드를 작성할 수 있습니다.
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 계산된 사용자 정의 필드 예: 문제 사용자 정의 양식에 문제 작성자의 관리자 표시

계산된 사용자 정의 필드를 사용하면 문제에 첨부된 사용자 정의 양식에 문제 작성자의 관리자 이름을 표시할 수 있습니다. 동일한 명령문을 사용하여 프로젝트, 문제 및 기타 개체에 대해 유사한 계산된 필드를 작성할 수 있습니다.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront 패키지</p> </td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront 라이선스</p> </td> 
   <td>
      <p>표준</p>
      <p>플랜</p></td>
  </tr> 
  <tr> 
   <td><p>액세스 수준 구성</p></td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr> 
  <tr> 
   <td> <p>개체 권한</p> </td> 
   <td> <p>사용자 정의 양식 편집에 대한 액세스 권한을 가지고 양식이 첨부된 오브젝트에 대한 액세스 기여</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 문제 사용자 정의 양식에 문제 작성자의 관리자 표시

다음 단계에서는 문제를 만든 사용자의 관리자 이름을 캡처할 수 있는 문제 사용자 정의 양식에 대해 계산된 필드를 만드는 방법을 보여줍니다. 예를 들어 작업, 프로젝트 또는 포트폴리오를 생성한 사용자의 관리자 이름을 캡처하려는 경우에는 프로세스가 동일합니다.

1. 문제 사용자 정의 양식을 만들고 계산된 필드를 추가합니다.

   사용자 정의 양식을 만들고 계산된 필드를 추가하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

   * [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. 다음 텍스트 모드 코드를 복사하여 사용자 정의 양식의 **계산** 필드에 붙여넣습니다.

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >사용자 정의 필드 계산은 대/소문자를 구분합니다.

1. **완료**&#x200B;를 클릭한 다음 **저장 + 닫기**&#x200B;를 클릭합니다.

   문제를 만든 사용자의 관리자는 필드가 포함된 양식을 문제에 첨부할 때 계산된 필드에 표시됩니다.
