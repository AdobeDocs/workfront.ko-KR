---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 사용자 지정 데이터 필드를 사용하는 외부 URL'
description: 작업 보기에서 "사용자 지정 URL"이라는 계산된 사용자 지정 필드를 사용하여 내부 사용자 지정 URL에 대한 링크를 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 보기: 사용자 지정 데이터 필드를 사용하는 외부 URL

를 사용하여 내부 사용자 지정 URL에 대한 링크를 표시할 수 있습니다. **계산된 사용자 정의 필드** 에 &quot;사용자 지정 URL&quot;로 지정됨 **작업 보기**.

이렇게 하면 보기의 특정 오브젝트에서 보고서에서 바로 애플리케이션의 특정 영역에 빠르게 연결할 수 있습니다.

계산된 사용자 정의 필드를 만들 때 먼저 필드를 만든 다음 보기를 만들어야 합니다.

다음 섹션은 작업에 대한 계산된 사용자 정의 필드의 예입니다. 사용자 지정 필드를 사용자 지정 URL이라고 합니다. 사용자 지정 보기에는 필드의 값과 **URL** 작업용 필드입니다.

동일한 단계를 사용하여 사용자 정의 양식이 있는 시스템의 모든 객체에 대해 유사한 계산된 사용자 정의 필드 및 사용자 정의 보기를 만들 수 있습니다.

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
   <td> <p>보기 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## &quot;사용자 정의 URL&quot; 계산된 사용자 정의 필드 만들기

계산된 사용자 정의 필드를 만드는 방법에 대한 자세한 내용은 문서 를 참조하십시오 [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

사용자 정의 양식을 만들 수 있는 액세스 권한이 있는 경우 &quot;사용자 정의 URL&quot;이라는 작업에 대해 계산된 사용자 정의 필드를 만들 수 있습니다. 이 필드는 로 직접 연결됩니다. **개요** 하위 탭 내 **작업 세부 정보** 탭.

1. 계산된 사용자 정의 필드를 만듭니다.
1. [계산] 필드에 다음 코드를 입력합니다.

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. 바꾸기 &quot;`<domain>`대괄호 없이 실제 도메인 이름과 함께 사용할 수 있습니다.

   해당

   ```
   /overview
   ```

   이 URL의 부분은 링크를 **개요** 섹션에 설명을 추가합니다.

1. 을(를) 만든 후 **계산된 사용자 정의 필드**, 다음을 첨부합니다 **사용자 정의 양식** Adobe Workfront에서 새 보기에 표시할 몇 가지 작업에 대해 이 필드를 사용합니다.

## 작업의 &quot;사용자 지정 URL&quot; 및 &quot;URL&quot; 필드를 표시하는 보기를 만듭니다.

작업 **보기** 아래 예에는 **계산된 사용자 정의 필드** 에 대한 직접 링크로서 &quot;사용자 지정 URL&quot;이라고 함 **개요** 작업 내의 하위 탭&#x200B;**세부 사항** 탭과 **URL** 작업 필드.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

이 보기를 사용자 지정하려면:

1. 작업 목록으로 이동합니다.
1. 확장 **보기** 작업 목록 맨 위에 있는 드롭다운
1. 클릭 **보기 맞춤화**.
1. 첫 번째 열을 제외하고 보기 내의 모든 열을 제거합니다.
1. 첫 번째 열의 헤더를 클릭합니다.
1. 클릭 **텍스트 모드로 전환** 인터페이스의 오른쪽 상단 모서리에서 을 참조하십시오.
1. 클릭 **텍스트를 편집하려면 클릭**.
1. 아래의 텍스트 모드를 하나의 열에 붙여넣습니다.\
   이 예제에서는 &#39;column.1&#39;을 사용합니다. &#39;사용자 지정 URL&#39; 필드의 값을 작업의 링크로 표시 **개요**. &#39;열.2.&#39; 에 저장된 값을 표시합니다. **URL 필드** 작업.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=사용자 지정 URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(사용자 지정 URL)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(사용자 지정 URL)<br>column.1.name=사용자 지정 URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=Custom URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 클릭 **보기 저장**.
