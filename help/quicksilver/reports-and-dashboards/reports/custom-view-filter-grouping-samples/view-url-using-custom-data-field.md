---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 사용자 지정 데이터 필드를 사용하는 외부 URL'
description: 작업 보기에서 "사용자 지정 URL"이라는 계산된 사용자 지정 필드를 사용하여 내부 사용자 지정 URL에 대한 링크를 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# 보기: 사용자 지정 데이터 필드를 사용하는 외부 URL

내부 사용자 지정 URL에 대한 링크를 **계산된 사용자 지정 필드** 에서 &quot;사용자 지정 URL&quot;로 이름이 지정됨 **작업 보기**.

이렇게 하면 뷰의 특정 개체에서 보고서에서 직접 애플리케이션의 특정 영역에 빠르게 연결할 수 있습니다.

계산된 사용자 지정 필드를 만들 때 먼저 필드를 만든 다음 보기를 만들어야 합니다.

다음 섹션은 작업에 대한 계산된 사용자 지정 필드의 예입니다. 사용자 지정 필드를 사용자 지정 URL이라고 합니다. 사용자 지정 보기에는 필드의 값과 **URL** 작업 필드입니다.

동일한 단계를 사용하여 사용자 정의 양식이 있는 시스템의 모든 개체에 대해 유사한 계산된 사용자 정의 필드와 사용자 정의 보기를 만들 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## &quot;사용자 지정 URL&quot; 계산된 사용자 지정 필드를 만듭니다

계산된 사용자 지정 필드 만들기에 대한 자세한 내용은 문서를 참조하십시오 [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

사용자 지정 양식을 만들 수 있는 액세스 권한이 있는 경우 &quot;사용자 지정 URL&quot;이라는 작업에 대해 계산된 사용자 지정 필드를 만들 수 있습니다. 이 필드는 **개요** 하위 탭 내 **작업 세부 사항** 탭.

1. 계산된 사용자 지정 필드를 만듭니다.
1. 계산 필드에 다음 코드를 입력합니다.

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&quot;)

1. 바꾸기 &quot;`<domain>`&quot;에는 대괄호 없이 실제 도메인 이름을 사용합니다.

   해당

   ```
   /overview
   ```

   이 URL의 부분에서는 링크를 **개요** 작업 왼쪽 패널의 섹션에 있습니다.

1. 작성 후 **계산된 사용자 지정 필드**&#x200B;를 첨부합니다. **사용자 지정 양식** 이 필드를 Adobe Workfront의 여러 작업에 추가하여 새 보기에 표시할 작업을 수행합니다.

## 작업의 &quot;사용자 지정 URL&quot; 및 &quot;URL&quot; 필드를 표시하는 보기를 만듭니다

작업 **보기** 아래 예에서는 **계산된 사용자 지정 필드** 에 대한 직접 링크로 &quot;사용자 지정 URL&quot;을 호출했습니다. **개요** 작업 내의 하위 탭&#x200B;**세부 사항** 탭과 **URL** 작업의 필드입니다.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

이 보기를 사용자 지정하는 방법은 다음과 같습니다.

1. 작업 목록으로 이동합니다.
1. 를 확장합니다. **보기** 작업 목록 맨 위에 있는 드롭다운
1. 클릭 **보기 사용자 지정**.
1. 첫 번째 열을 제외하고 보기 내의 모든 열을 제거합니다.
1. 첫 번째 열의 헤더를 클릭합니다.
1. 클릭 **텍스트 모드로 전환** 인터페이스 오른쪽 상단 모서리에서 을(를) 클릭합니다.
1. 클릭 **텍스트를 편집하려면 클릭하십시오.**.
1. 아래의 텍스트 모드를 하나의 열에 붙여넣습니다.\
   이 예제에서는 &#39;column.1&#39;입니다. &#39;사용자 지정 URL&#39; 필드에 값을 작업의 링크로 표시합니다 **개요**. &#39;Column.2.&#39; 에 저장된 값을 표시합니다. **URL 필드** Analytics JavaScript에서 액세스 권한을 부여합니다.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.value.format= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valufield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=사용자 지정 URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(사용자 지정 URL)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(사용자 지정 URL)<br>column.1.name=사용자 지정 URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=사용자 지정 URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.description-key=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 클릭 **보기 저장**.
