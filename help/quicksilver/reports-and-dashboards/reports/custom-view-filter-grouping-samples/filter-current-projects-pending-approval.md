---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 승인 보류 중인 현재 프로젝트 표시'
description: 다음 프로젝트 필터는 현재 - 승인 보류 중 상태의 프로젝트를 표시합니다. 여기서 로그인한 사용자는 프로젝트 스폰서이거나 Portfolio 관리자입니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 필터: 승인 보류 중인 현재 프로젝트 표시

<!--Audited: 10/2024-->

다음 프로젝트 필터는 현재 - 승인 보류 중 상태의 프로젝트를 표시합니다. 여기서 로그인한 사용자는 프로젝트 스폰서이거나 Portfolio 관리자입니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 승인 보류 중인 현재 프로젝트 필터링

이 필터를 적용하려면:

1. 프로젝트 목록으로 이동합니다.
1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.

1. **텍스트 모드**&#x200B;를 클릭합니다.
1. 표시된 영역에서 다음 코드를 복사하여 붙여넣습니다.
   <pre>상태=CUR:A<br>스폰서ID=$$USER.ID<br>OR:a:상태=CUR:A<br>OR:a:포트폴리오:소유자ID=$$USER.ID</pre>

1. **적용** > **새 이름으로 저장**&#x200B;을 클릭합니다.
