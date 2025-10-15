---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 승인 상태의 항목만 표시'
description: 현재 승인 보류 중인 특정 상태의 항목만 표시할 수 있습니다. 승인 상태가 있는 다른 모든 오브젝트에 대해서도 동일하게 작동합니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 필터: 승인 상태의 항목만 표시

<!--Audited: 10/2024-->

현재 승인 보류 중인 특정 상태의 항목만 표시할 수 있습니다. 승인 상태가 있는 다른 모든 오브젝트에 대해서도 동일하게 작동합니다.

다음 객체를 승인 상태에 배치할 수 있습니다.

* 작업
* 문제
* 프로젝트

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>필터 수정을 위한 기여자 또는 요청 </p>
   <p>표준 또는 보고서 수정 계획</p>
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

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 승인 상태의 항목만 표시

1. 프로젝트 목록으로 이동합니다.
1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.
1. **프로젝트: 상태**&#x200B;별로 필터링하도록 선택한 다음 목록에서 필터링할 상태를 선택합니다.

   예를 들어, **계획 - 승인 보류 중** 상태인 프로젝트만 표시하려면 프로젝트 보고서에 **Status Equal Planning**&#x200B;을(를) 추가하십시오.
1. **텍스트 모드**&#x200B;를 클릭합니다.
1. 상태의 3자리 키에 `status`을(를) 추가하여 **:A** 줄을 수정합니다.
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. **적용** > **새 이름으로 저장**&#x200B;을 클릭합니다.

   계획 - 승인 보류 중 상태인 프로젝트만 목록에 표시됩니다.
