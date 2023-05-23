---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 승인 상태의 항목만 표시'
description: 현재 승인 보류 중인 특정 상태의 항목만 표시할 수 있습니다. 승인 상태가 있는 다른 모든 오브젝트에 대해서도 동일하게 작동합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# 필터: 승인 상태의 항목만 표시

현재 승인 보류 중인 특정 상태의 항목만 표시할 수 있습니다. 승인 상태가 있는 다른 모든 오브젝트에 대해서도 동일하게 작동합니다.

다음 객체를 승인 상태에 배치할 수 있습니다.

* 작업
* 문제
* 프로젝트

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>필터 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 승인 상태의 항목만 표시

1. 예를 들어 프로젝트 목록에 대해 사용자 지정할 필터로 이동합니다.
1. 클릭 **필터 규칙 추가** 대상: **상태** 목록의 개체 필드.\
   예를 들어 프로젝트 보고서에서 을 추가합니다 **계획과 동일한 상태**, 상태의 프로젝트만 표시하려는 경우 **계획 - 승인 보류 중**.

1. 클릭 **텍스트 모드로 전환**.
1. 수정

   ```
   status
   ```

   추가하여 행 **:A** 3자로 된 상태 키:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. 클릭 **완료**, 그런 다음 **필터 저장**.

   계획 - 승인 보류 중 상태인 프로젝트만 목록에 표시됩니다.
