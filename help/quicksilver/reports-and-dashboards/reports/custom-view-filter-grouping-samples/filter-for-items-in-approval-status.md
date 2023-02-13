---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 승인 상태에 항목만 표시'
description: 현재 승인 보류 중인 특정 상태의 항목만 표시할 수 있습니다. 승인 상태가 있는 다른 객체에도 동일하게 작동합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# 필터: 승인 상태의 항목만 표시

현재 승인 보류 중인 특정 상태의 항목만 표시할 수 있습니다. 승인 상태가 있는 다른 객체에도 동일하게 작동합니다.

승인 상태에 다음 객체를 배치할 수 있습니다.

* 작업
* 문제
* 프로젝트

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
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 승인 상태에 항목만 표시

1. 예를 들어 프로젝트 목록에 대해 사용자 지정할 필터로 이동합니다.
1. 클릭 **필터 규칙 추가** 대상 **상태** 목록의 개체 필드입니다.\
   예를 들어 프로젝트 보고서에서 을 추가합니다 **Status Equal Planning**&#x200B;를 설정하는 경우, **계획 - 승인 보류 중**.

1. 클릭 **텍스트 모드로 전환**.
1. 수정

   ```
   status
   ```

   추가 **: A** 상태의 3자로 된 키:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. 클릭 **완료**, 그런 다음 **필터 저장**.

   목록에는 Planning - Pending Approval 상태의 프로젝트만 표시됩니다.
