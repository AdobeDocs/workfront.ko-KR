---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 복사
description: 새 프로젝트 템플릿을 처음부터 새로 만드는 대신, 기존 템플릿을 복사하고 필요한 경우 변경할 수 있습니다.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# 프로젝트 템플릿 복사

새 프로젝트 템플릿을 처음부터 새로 만드는 대신, 기존 템플릿을 복사하고 필요한 경우 변경할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>템플릿에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>템플릿에 대한 보기 이상의 권한</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.


## 템플릿 복사 관련 고려 사항

다음 항목은 항상 기존 프로젝트에서 새 프로젝트에 복사됩니다.

* 템플릿 작업
* 템플릿 작업 기본 정보(작업 기본 승인 프로세스, 작업 기본 사용자 지정 Forms)
* 사용자 정의 양식
* 위험
* 대기열 설정 정보
* Portfolio 및 프로그램
* 승인
* 문서
* 원래 템플릿 작업의 일 수가 새 템플릿으로 전송됩니다. 필요한 경우 템플릿 작업의 일자를 업데이트하려면 템플릿의 시작 또는 완료 일자(예약 모드에 따라)를 변경해야 합니다.

다음 항목은 기존 프로젝트에서 새 프로젝트로 복사되지 않습니다.

* 청구 요금
* 사용자 댓글

## 템플릿 복사

1. 복사할 템플릿으로 이동합니다.
1. **자세히** 메뉴 ![](assets/qs-more-icon-on-an-object.png)을(를) 클릭한 다음 **복사**&#x200B;를 클릭합니다.
1. **새 템플릿 이름** 필드에 템플릿 이름을 지정하십시오.

   기본적으로 새 이름은 **`<original template name>`의 복사본**&#x200B;입니다.

1. **작업 및 템플릿에 대한 사용자 할당 유지**: 이 옵션을 선택하여 원래 템플릿의 모든 작업 및 템플릿 할당을 새 템플릿으로 전달합니다.
1. 템플릿의 복사본을 만들려면 **저장**&#x200B;을 클릭하십시오.
