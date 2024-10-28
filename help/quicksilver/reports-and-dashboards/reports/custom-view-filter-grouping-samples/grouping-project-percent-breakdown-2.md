---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 프로젝트 백분율 분류 2'
description: '이 사용자 지정 프로젝트 그룹에서는 완료율 값 범위로 그룹화된 프로젝트를 표시할 수 있습니다. 분류는 0~10%, 11~20%, 21~30% 등 10% 포인트 단위의 완료율 값을 표시합니다.'
author: Nolan
feature: Reports and Dashboards
exl-id: 7845fd66-8304-4154-8630-e72482cd753f
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 그룹화: 프로젝트 백분율 분류 2

<!--Audited: 10/2024-->

이 사용자 정의 프로젝트 그룹에서는 완료율 값 범위로 그룹화된 프로젝트를 표시할 수 있습니다. 분류는 0~10%, 11~20%, 21~30% 등 10% 포인트 증가의 완료율 값을 표시합니다.

다음 그룹화는 완료율 값별로 프로젝트를 이러한 그룹화 중 하나로 구성합니다.

* 0%
* 1-10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![percent_complete_breakdown_for_projects_in_10__increments.png](assets/percent-complete-breakdown-350x94.png)

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

## 프로젝트 비율 분류별 그룹화

이 그룹화를 적용하려면:

1. 프로젝트 목록으로 이동합니다.
1. **그룹화** 드롭다운 메뉴에서 **새 그룹화**&#x200B;을 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. 상자의 텍스트를 제거하고 사용 가능한 공간에 다음 코드를 붙여넣습니다.

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=11,"1-10 %",IF({percentComplete}<=21,"11-20 %",IF({percentComplete}<=31,"21-30 %",IF({percentComplete}<41,"31-40 %",IF({percentComplete}<51,"41-50 %",IF({percentComplete}<61,"51-60 %",IF({percentComplete}<71,"61-70 %",IF({percentComplete}<81,"71-80 %",IF({percentComplete}<91,"81-90 %",IF({percentComplete}<100,"91-99 %","100 %")))))))))))
   textmode=true
   ```

1. **완료** > **그룹화 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 그룹화 이름을 업데이트한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
