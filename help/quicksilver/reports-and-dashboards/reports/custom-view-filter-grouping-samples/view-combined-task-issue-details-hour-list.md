---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 시간 목록의 결합된 작업 및 문제 세부 정보'
description: 이 시간 보기에는 sharecol 태그를 사용하여 작업 및 문제 이름 열과 작업 및 문제 계획된 시간이 결합됩니다. 시간 입력은 작업 또는 문제에만 속할 수 있으므로 두 개체가 동시에 같은 열에 나타날 수 없습니다. 보기의 각 행은 작업 또는 문제의 정보로 채워집니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# 보기: 시간 목록의 결합된 작업 및 문제 세부 정보

이 시간 보기에는 작업 및 문제 이름 열과 을 사용한 작업 및 문제 계획 시간이 결합됩니다.

```
sharecol
```

태그에 가깝게 배치하십시오. 시간 입력은 작업 또는 문제에만 속할 수 있으므로 두 개체가 동시에 같은 열에 나타날 수 없습니다. 보기의 각 행은 작업 또는 문제의 정보로 채워집니다.

에 대해 자세히 알아보려면

```
sharecol
```

태그에 [보기: 하나의 공유 열에 있는 여러 열의 병합 정보](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)를 참조하십시오.\
![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

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

## 시간 목록에서 결합된 작업 및 문제 세부 정보 보기

이 보기를 적용하려면:

1. 시간 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 열을 제외한 모든 열을 제거하십시오.
1. 나머지 열의 머리글을 클릭한 다음 **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭하세요**.
1. **텍스트 모드** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.
   <pre>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=100<br>column.2.description=작업 또는 문제<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=task:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=task<br>column.link.valuecode=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task).string(name)<br>column.2.name=Task 또는 Issue<br>column.2.querysort=task:name<br>column.2.sharecol=true<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=task:name<br>column.2.valuefield=HTML HTML<br>column.2.width=100<br>column.3.descriptionkey=optask<br>column.link.linkproperty.0.name=ID{24 3.link.linkproperty.0.valuefield=opTask:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=opTask:objCode<br>column.3.link.valuefield=val<br>column.3.linkedname=optask<br>column.3.listsort=nested(opTask).string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask:name<br>column.shortview=false4}column.stretch <br>column.3.valuefield=opTask:name<br>column.3.valueformat=column<br>column.3.width=1<br>column.4.valuefield=task:work<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueformat=doubleAsInt<br>column.4.namekey=view.relatedcolumn<br>column.4.querysort=task:work<br>column.4.textmode=true<br>column.4.namekeyargkey.0=task<br>column.namekeyargkey.1=work<br>column.displayname=계획된 노력<br>열.5.displayname=계획된 노력<br>열.5.viewalias=opTask:workrequired<br>열.5.linkedname=opTask<br>열.5.valuefield=opTask:workRequired<br>열.5.valueformat=compound<br>열.5.querysort=opTask:workRequired<br>열.5.namekeyargkey.0=opTask<br>열.5.namekeyargkey.1=workrequired<br>열.5.namekey=view.relatedcolumn{5.textmode=true<br>열.6 tionkey=hours<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(hours)<br>column.6.namekey=hours.abbr<br>column.6.querysort=hours<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=hours<br>column.6.valueformat=doubleAsString<br>column.6.width=7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.listsort=AtDateAsAt date(entryDate)<br>column.7.namekey=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valuefield=entryDate<br>column.7.valueformat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.8.listsort=string(description)<br>column.8.namekey=description.abbr<br>column.83.column.8 shortview=false<br>column.8.stretch=0<br>column.8.valuefield=description<br>column.8.valueformat=HTML<br>column.8.width=150<br><br><br><br><br></pre>

1. **보기 저장**&#x200B;을 클릭합니다.
