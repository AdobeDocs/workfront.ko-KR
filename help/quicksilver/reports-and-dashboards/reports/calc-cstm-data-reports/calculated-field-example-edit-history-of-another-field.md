---
content-type: reference
product-area: reporting
keywords: 감사,추적,사용자 정의,필드
navigation-topic: calculate-custom-data-reports
title: '계산된 사용자 정의 필드 예: 필드의 편집 내역 표시'
description: 사용자가 사용자 정의 필드를 정기적으로 업데이트하며 필드에 대한 모든 변경 사항의 로그와 변경 사항이 발생한 날짜를 캡처하려는 경우 계산된 사용자 정의 필드에서 이 정보를 캡처할 수 있습니다.
author: Jenny
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 계산된 사용자 정의 필드 예: 필드의 편집 내역 표시

사용자가 사용자 정의 필드를 정기적으로 업데이트하며 필드에 대한 모든 변경 사항의 로그와 변경 사항이 발생한 날짜를 캡처하려는 경우 계산된 사용자 정의 필드에서 이 정보를 캡처할 수 있습니다.

다음 예제에서는 지침 편집 기록 계산 필드를 작성하여 지침이라는 한 줄 텍스트 필드에 대한 모든 변경 사항을 캡처하는 방법을 보여 줍니다.

>[!TIP]
>
>한 줄 텍스트 필드뿐만 아니라 모든 유형의 사용자 정의 필드에 대해 이 예제를 따를 수 있습니다.

이 작업은 다음 작업을 수행합니다.

* 지침 편집 기록 필드를 Workfront 데이터베이스 제한 이내로 유지하도록 가장 최근 2000자로 제한합니다.
* 지침 필드의 현재 값이 지침 편집 기록 값의 앞면과 일치하는지 확인합니다. 이 값은 비어 있다고 가정하고 그렇지 않으면 다음을 수행합니다.

   * 일치하는 경우 지침 작업 내역 편집 을 그대로 둡니다.
   * 일치하지 않으면 [지침 편집 기록] 필드를 [지침] 필드의 최신 값으로 바꾼 다음 괄호로 묶인 현재 날짜, 세로 막대 및 이전 값과 입력된 날짜를 유지하는 이전 [지침 편집 기록]으로 바꿉니다.

## 액세스 요구 사항

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
   <td> <p>사용자 지정 Forms에 대한 관리 액세스</p> </td> 
  </tr> 
  <tr> 
   <td> <p>개체 권한</p> </td> 
   <td> <p>사용자 정의 양식에 대한 권한 관리</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

필드의 편집 기록을 표시하는 계산된 필드를 사용자 정의 양식에 추가하려면 먼저 다음을 수행해야 합니다.

* 사용자 정의 양식 만들기
* 내역을 캡처할 필드를 사용자 정의 양식에 추가합니다

## 필드의 편집 내역 표시

1. 계산된 필드를 추가할 사용자 정의 양식으로 이동합니다.

1. 예를 들어 한 줄 텍스트 사용자 정의 필드를 만들려면 다음을 수행합니다.

   1. **한 줄 텍스트**&#x200B;를 클릭합니다.
   1. 사용자 지정 필드에 **Label**&#x200B;을(를) 지정하십시오. 예를 들어 이름을 &quot; Instructions&quot;로 지정할 수 있습니다.
   1. **적용**&#x200B;을 클릭합니다.

1. 양식에 계산된 사용자 지정 필드를 추가하려면 **계산됨**&#x200B;을(를) 클릭하십시오.
1. 계산된 사용자 지정 필드에 **Label**&#x200B;을(를) 지정하십시오. 예를 들어 이름을 &quot;Instructions Edit History&quot;로 지정할 수 있습니다.

   첫 번째 필드(&quot;지침&quot;)에 대한 변경 사항을 캡처하는 필드입니다.

1. **저장 후 닫기**&#x200B;를 클릭합니다.
1. 이제 두 필드를 추가한 양식 이름을 클릭하여 다시 엽니다.
1. 계산된 사용자 지정 필드 **내역 편집 지침**&#x200B;을 클릭한 다음 **계산** 상자에 다음을 복사하여 붙여 넣으십시오.

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (권장) 양식의 계산된 필드에서 **지침** 필드에 동일한 계산을 붙여 넣습니다.
1. 계산된 사용자 지정 필드의 서식을 텍스트로 지정하려면 **서식** 필드에서 **텍스트**&#x200B;을(를) 선택해야 합니다.

   이것이 기본값입니다.

1. **저장 후 닫기**&#x200B;를 클릭합니다.

   이제 사용자 정의 양식을 오브젝트에 첨부한 다음 누군가 **지침** 필드의 정보를 변경하면 **지침 편집 기록** 필드에 최신 값이 표시되고 그 뒤에 현재 날짜가 괄호 안에 표시되고 세로 막대가 표시됩니다. 추가 변경 사항이 있는 경우 동일한 방식으로 이 정보에 추가됩니다.

   위의 계산에서는 *지침*&#x200B;을(를) 추적할 한 줄 텍스트 필드의 정확한 이름으로 바꾸고, **지침 편집 기록**&#x200B;을(를) 계산된 필드의 정확한 이름으로 바꿀 수 있습니다.
