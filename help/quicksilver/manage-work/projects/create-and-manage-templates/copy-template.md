---
product-area: templates
navigation-topic: templates-navigation-topic
title: 프로젝트 템플릿 복사
description: 처음부터 프로젝트 템플릿을 작성할 수 있을 뿐만 아니라, 기존 템플릿을 복사하여 수정할 수도 있습니다.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 1926500c76e4f9cfdac829f8d9f0cdfa6231e31d
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 2%

---

# 프로젝트 템플릿 복사

<!--Audited: 5/2025-->

처음부터 프로젝트 템플릿을 제작하는 것 외에도 Adobe Workfront에서 기존 템플릿을 복사하고 수정할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td><p>새로운 기능: 표준</p> 
   <p>현재: 플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>템플릿에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>템플릿에 대한 보기 이상의 권한</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 템플릿 복사 관련 고려 사항

다음 항목은 항상 기존 템플릿에서 새 템플릿으로 복사됩니다.

* 템플릿 작업
* 템플릿 작업 기본 정보(작업 기본 승인 프로세스, 작업 기본 사용자 지정 Forms)
* 사용자 정의 양식
* 위험
* 대기열 설정 정보
* Portfolio 및 프로그램
* 승인
* 문서
* 원래 템플릿 작업의 일 수가 새 템플릿으로 전송됩니다. 필요한 경우 템플릿 작업의 일자를 업데이트하려면 템플릿의 시작 또는 완료 일자(예약 모드에 따라)를 변경해야 합니다.

다음 항목은 기존 템플릿에서 새 템플릿으로 복사되지 않습니다.

* 결제 요율
* 사용자 댓글

## 템플릿 복사

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. 복사할 템플릿으로 이동합니다.
1. 헤더의 템플릿 이름 오른쪽에 있는 **자세히** 메뉴 ![자세히 아이콘](assets/qs-more-icon-on-an-object.png)을 클릭한 다음 **복사**&#x200B;를 클릭합니다.

   **템플릿 복사** 상자가 열립니다.

   ![템플릿 상자 복사](assets/copy-template-box.png)

1. **새 템플릿 이름** 필드에 템플릿 이름을 지정하십시오.

   기본적으로 Workfront은 `Copy of Original template name` 형식에 따라 새 이름을 설정합니다.

1. 원래 템플릿에서 새 템플릿으로 모든 작업 및 템플릿 할당을 이전하려면 **작업 및 템플릿에 대한 사용자 할당 유지** 옵션을 선택하십시오. 템플릿 작업 할당, 템플릿 소유자 및 스폰서가 복사된 템플릿으로 전송됩니다.
1. 템플릿의 복사본을 만들려면 **저장**&#x200B;을 클릭하십시오.

   Workfront의 템플릿 영역에 있는 템플릿 목록에 새 템플릿이 표시됩니다.
