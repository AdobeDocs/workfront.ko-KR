---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 전임 작업 세부 정보'
description: 이 작업 보기는 컬렉션 보기를 사용하여 작업의 전임 작업에 대한 세부 정보를 표시합니다. 컬렉션 뷰에서는 "일대다" 관계에 있는 개체에 대한 정보를 표시할 수 있습니다. 이 경우 각 작업(하나)에는 여러 개의 전임 작업(다)이 있을 수 있습니다. 이 보기에는 작업의 이름과 함께 전임 작업 이름, 전임 작업 프로젝트 이름, 전임 작업 계획된 완료 일자 및 전임 작업 상태가 표시됩니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 보기: 전임 작업 세부 정보

이 작업 보기는 컬렉션 보기를 사용하여 작업의 전임 작업에 대한 세부 정보를 표시합니다. 컬렉션 뷰에서는 &quot;일대다&quot; 관계에 있는 개체에 대한 정보를 표시할 수 있습니다. 이 경우 각 작업(하나)에는 여러 개의 전임 작업(다)이 있을 수 있습니다. 이 보기에는 작업의 이름과 함께 전임 작업 이름, 전임 작업 프로젝트 이름, 전임 작업 계획된 완료 일자 및 전임 작업 상태가 표시됩니다.

보고서에서 컬렉션 참조에 대한 자세한 내용은 [보고서에서 컬렉션 참조](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)를 참조하십시오.

![전임 작업_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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
   <td> <p>보기 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전임 작업 세부 정보 보기

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 머리글을 클릭한 다음 **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하세요**.
1. **텍스트 모드** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecessors Numbers &amp; Names<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(predecessors).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({predecessor}.{taskNumber},' - ',{predecessor}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=전임 작업 프로젝트 이름<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(전임 작업).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecessor}.{project}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=선행 작업 완료 날짜<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(선행 작업).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecessor}.{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=전임 작업 상태<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(전임 작업).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}.{status}<br>column.4.valueformat=HTML</pre>

1. **보기 저장**&#x200B;을 클릭합니다.
