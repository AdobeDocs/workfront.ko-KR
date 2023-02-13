---
content-type: reference
product-area: reporting
keywords: 감사,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: "계산된 사용자 지정 필드 예: 필드의 편집 기록 표시"
description: 사용자가 정기적으로 사용자 지정 필드를 업데이트하며 필드에 수행된 모든 변경 내용과 변경 사항이 발생한 날짜의 로그를 캡처하려는 경우 계산된 사용자 지정 필드에서 이 정보를 캡처할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# 계산된 사용자 지정 필드 예: 필드의 편집 기록 표시

사용자가 정기적으로 사용자 지정 필드를 업데이트하며 필드에 수행된 모든 변경 내용과 변경 사항이 발생한 날짜의 로그를 캡처하려는 경우 계산된 사용자 지정 필드에서 이 정보를 캡처할 수 있습니다.

다음 예는 를 빌드하는 방법을 보여 줍니다 *지침 기록 편집* 계산된 필드 : *지침*.

>[!TIP]
>
>단일 행 텍스트 필드뿐만 아니라 모든 유형의 사용자 지정 필드에 대해 이 예제를 따를 수 있습니다.

이렇게 하면 다음과 같은 작업이 수행됩니다. 

* 제한 *지침 기록 편집* 필드를 최신 2000자로 변경하여 Workfront 데이터베이스 제한 내에 남아 있습니다.
* 현재 값이 *지침* 필드의 앞과 일치합니다 *지침 기록 편집* 값; 이 변수는 이 비어 있다고 간주하며 그렇지 않으면 다음을 수행합니다. 

   * 일치하는 경우 *지침 기록 편집* 있는 그대로
   * 일치하지 않으면 가 바뀝니다 *지침 기록 편집* 에서 최신 값으로 *지침* 필드, 뒤에 현재 날짜(괄호, 세로 막대 및 이전)가 옵니다 *지침 기록 편집*: 이전 값과 입력한 날짜를 유지합니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 라이선스*</p> </td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>사용자 지정 Forms에 대한 관리 액세스</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>사용자 지정 양식에 대한 권한 관리 </p> <p>자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">사용자 지정 양식 공유</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## 전제 조건

필드의 편집 내역을 표시하는 계산된 필드를 사용자 지정 양식에 추가하려면 먼저 다음을 수행해야 합니다.

* 사용자 지정 양식 만들기
* 사용자 지정 양식에 캡처할 기록을 가진 필드를 추가합니다

## 필드의 편집 기록 표시

1. 계산된 필드를 추가할 사용자 지정 양식으로 이동합니다.

1. 예를 들어 단일 행 텍스트 사용자 지정 필드를 만들려면 다음을 수행하십시오.

   1. 클릭 **단일 행 텍스트 필드**.
   1. 을(를) 지정합니다 **레이블** 사용자 지정 필드의 경우(예: ) *지침*.
   1. 클릭 **애플리**.

1. 선택 **필드 추가**&#x200B;를 선택하고 을 선택합니다. **계산된 지표** 계산된 사용자 지정 필드를 양식에 추가하려면
1. 을(를) 지정합니다 **레이블** 를 입력합니다. *지침 기록 편집*.

   이 필드는 사용자가 만든 첫 번째 필드(*지침*).

1. 클릭 **저장 + 닫기**.
1. 이제 필드를 두 개 추가한 양식 이름을 클릭하여 다시 엽니다.
1. 계산된 사용자 지정 필드를 클릭합니다 *지침 기록 편집,* 그런 다음 계산 상자에 다음을 복사하여 붙여넣습니다.
1. 에서 **계산** 필드에서 사용자 지정 필드에 다음 계산을 지정합니다.

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (권장) 같은 계산을 **지침** 양식에서 계산된 필드의 필드입니다.
1. 확인  **텍스트** 에서 선택됨 **형식** 계산된 사용자 지정 필드의 형식을 텍스트로 지정하는 필드입니다.

   기본값입니다.

1. 클릭 **저장+닫기**.

   이제 사용자 지정 양식을 개체에 첨부한 다음 다른 사용자가 *지침* 필드, *지침 편집 기록&quot; 필드에는 최신 값이 표시되고, 그 뒤에는 현재 날짜가 괄호 안에 표시되고, 세로 막대가 표시됩니다. 추가 변경이 있는 경우 동일한 방식으로 이 정보에 추가됩니다.

   위의 계산에서 *지침* 단일 행 텍스트 필드의 정확한 이름과 함께 추적하려는 내역을 추적할 수 있습니다. *지침 기록 편집* 을 사용하여 계산된 필드의 정확한 이름을 지정합니다.
