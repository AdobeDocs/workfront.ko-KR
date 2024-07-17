---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 작업 비율 분류 1'
description: '이 사용자 지정 프로젝트 그룹에서는 완료율 값 범위로 그룹화된 프로젝트를 표시할 수 있습니다. 분류는 0~25%, 25~50% 등 25% 포인트 증가의 완료율 값을 보여 줍니다.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# 그룹화: 작업 비율 분류 1

이 사용자 정의 프로젝트 그룹에서는 완료율 값 범위로 그룹화된 프로젝트를 표시할 수 있습니다. 분류는 0~25%, 25~50% 등 25% 포인트 증가의 완료율 값을 보여 줍니다. 

다음 그룹화는 완료율 값별로 작업을 6개의 다른 그룹화로 구성합니다.

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25__breakdown_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>그룹화 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 그룹화 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 작업 비율 분류별 그룹화

이 그룹화를 적용하려면:

1. 작업 목록으로 이동합니다.
1. **그룹화** 드롭다운 메뉴에서 **새 그룹화**&#x200B;을 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. **보고서 그룹화** 영역에서 텍스트를 제거합니다.
1. 텍스트를 다음 코드로 바꿉니다.
   <pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF({percentComplete}&lt;100,"75-99 %","100 %")))))<br>group.0.valueformat=string</pre>

1. **그룹화 저장**&#x200B;을 클릭합니다.
