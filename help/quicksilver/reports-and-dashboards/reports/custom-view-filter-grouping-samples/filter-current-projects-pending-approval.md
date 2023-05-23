---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 승인 보류 중인 현재 프로젝트 표시'
description: 다음 프로젝트 필터는 현재 - 승인 보류 중 상태의 프로젝트를 표시합니다. 여기서 로그인한 사용자는 프로젝트 스폰서이거나 Portfolio 관리자입니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 필터: 승인 보류 중인 현재 프로젝트 표시

다음 프로젝트 필터는 현재 - 승인 보류 중 상태의 프로젝트를 표시합니다. 여기서 로그인한 사용자는 프로젝트 스폰서이거나 Portfolio 관리자입니다.

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

## 승인 보류 중인 현재 프로젝트 필터링

이 필터를 적용하려면:

1. 프로젝트 목록으로 이동합니다.
1. 다음에서 **필터** 드롭다운 메뉴에서 다음을 선택합니다. **새 필터**.

1. 클릭&#x200B;**텍스트 모드로 전환**.
1. 다음에서 **보고서에 대한 필터 규칙 설정** 다음 코드를 복사하여 붙여넣습니다.
   <pre>status=CUR:A<br>스폰서 ID=$$USER.ID<br>또는:a:status=CUR:A<br>또는:a:포트폴리오:ownerID=$$USER.ID</pre>

1. 클릭 **필터 저장**.
