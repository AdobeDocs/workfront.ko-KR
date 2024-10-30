---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 시간 동안 프로젝트 스폰서'
description: 이 시간 그룹화는 시간이 기록된 프로젝트의 스폰서에 의해 시간을 구성합니다. 시간 그룹화에 대한 표준 Report Builder 인터페이스는 프로젝트 스폰서 필드에 대한 매핑을 제공하지 않습니다. 이 필드에 액세스하려면 텍스트 모드 인터페이스를 사용해야 합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: bc99e303047b989b972974b398420a9180e40874
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 그룹화: 시간 동안 프로젝트 스폰서

<!--Audited: 10/2024-->

이 시간 그룹화는 시간이 기록된 프로젝트의 스폰서에 의해 시간을 구성합니다. 시간 그룹화에 대한 표준 Report Builder 인터페이스는 프로젝트 스폰서 필드에 대한 매핑을 제공하지 않습니다. 이 필드에 액세스하려면 텍스트 모드 인터페이스를 사용해야 합니다.

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## 프로젝트 스폰서별로 시간 그룹화

이 그룹화를 적용하려면:

1. 시간 목록으로 이동합니다.
1. **그룹화** 드롭다운 메뉴에서 **새 그룹화**&#x200B;을 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. 표시되는 영역에서 텍스트를 제거하고 다음 코드로 대체합니다.

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. **완료**&#x200B;를 클릭합니다.
1. 그룹화 이름을 업데이트한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
