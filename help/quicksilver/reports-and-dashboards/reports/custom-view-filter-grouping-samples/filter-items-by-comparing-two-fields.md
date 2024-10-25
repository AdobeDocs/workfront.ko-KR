---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 두 필드를 비교하여 목록의 항목 제거'
description: 두 필드를 비교하여 목록에서 항목을 필터링할 수 있습니다. 예를 들어 작업의 실제 완료 일자가 계획된 완료 일자보다 큰 작업만 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 4532e08bddf993426e9d4eed6f7f8bd638663188
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 필터: 두 필드를 비교하여 목록의 항목 제거

<!--Audited: 10/2024-->

두 필드를 비교하여 목록에서 항목을 필터링할 수 있습니다. 예를 들어 작업의 실제 완료 일자가 계획된 완료 일자보다 큰 작업만 표시할 수 있습니다.

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

## 두 필드를 비교하여 항목 필터링

1. 작업 목록으로 이동합니다.
1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.

1. **작업:실제 완료 날짜** > **다음보다 큼** > **날짜 선택**&#x200B;에 대한 필터를 추가합니다.

   >[!TIP]
   >
   >사용 가능한 경우 선택한 필드에 사용할 필터 수정자를 선택합니다.

1. **텍스트 모드**&#x200B;를 클릭합니다.
1. 표시된 영역에 다음 코드를 추가합니다.

   `actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt`

1. **적용** > **새 이름으로 저장**&#x200B;을 클릭합니다.
