---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 사용자 정의 데이터 필드를 사용하는 외부 URL'
description: 작업 보기에서 "사용자 지정 URL"이라는 계산된 사용자 지정 필드를 사용하여 내부 사용자 지정 URL에 대한 링크를 표시할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 보기: 사용자 지정 데이터 필드를 사용하는 외부 URL

<!--Audited: 11/2024-->

**작업 보기**&#x200B;에서 &quot;사용자 지정 URL&quot;이라는 **계산된 사용자 지정 필드**&#x200B;를 사용하여 내부 사용자 지정 URL에 대한 링크를 표시할 수 있습니다.

이렇게 하면 보기의 특정 오브젝트에서 보고서에서 바로 애플리케이션의 특정 영역에 빠르게 연결할 수 있습니다.

계산된 사용자 정의 필드를 만들 때 먼저 필드를 만든 다음 보기를 만들어야 합니다.

다음 섹션은 작업에 대한 계산된 사용자 정의 필드의 예입니다. 사용자 지정 필드를 사용자 지정 URL이라고 합니다. 사용자 지정 보기에는 작업의 **URL** 필드와 필드 값이 표시됩니다.

동일한 단계를 사용하여 사용자 정의 양식이 있는 시스템의 모든 객체에 대해 유사한 계산된 사용자 정의 필드 및 사용자 정의 보기를 만들 수 있습니다.

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
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p> 현재: 
   <ul>
   <li>보기 수정 요청</li> 
   <li>보고서 수정 계획</li>
   </ul>
     </p>
     <p> 신규: 
   <ul>
   <li>보기를 수정하는 기여자</li> 
   <li>보고서를 수정하는 표준</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## &quot;사용자 정의 URL&quot; 계산된 사용자 정의 필드 만들기

계산된 사용자 지정 필드를 만드는 방법에 대한 자세한 내용은 [양식에 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

사용자 정의 양식을 만들 수 있는 액세스 권한이 있는 경우 &quot;사용자 정의 URL&quot;이라는 작업에 대해 계산된 사용자 정의 필드를 만들 수 있습니다. 이 필드는 **작업 세부 정보** 탭의 **개요** 하위 탭으로 바로 연결됩니다.

1. 계산된 사용자 정의 필드를 만듭니다.
1. [계산] 필드에 다음 코드를 입력합니다.

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;)

1. 대괄호 없이 &quot;`<domain>`&quot;을(를) 실제 도메인 이름으로 바꾸십시오. 이 URL의 `/overview` 부분이 작업 왼쪽 패널의 **개요** 섹션으로 링크를 보냅니다.

1. **계산된 사용자 정의 필드**&#x200B;을(를) 만든 후 이 필드가 포함된 **사용자 정의 양식**&#x200B;을(를) 새 보기에 표시할 Adobe Workfront의 여러 작업에 첨부합니다.

## 작업의 &quot;사용자 지정 URL&quot; 및 &quot;URL&quot; 필드를 표시하는 보기를 만듭니다.

아래 예제의 작업 **보기**&#x200B;에는 &quot;사용자 지정 URL&quot;이라는 **계산된 사용자 지정 필드**&#x200B;이(가) 작업&#x200B;**세부 정보** 탭의 **개요** 하위 탭과 작업의 **URL** 필드에 대한 직접 링크로 표시됩니다.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

이 보기를 사용자 지정하려면:

1. 작업 목록으로 이동합니다.
1. 작업 목록 맨 위에 있는 **보기** 드롭다운을 확장합니다.
1. **보기 사용자 지정**&#x200B;을 클릭합니다.
1. 첫 번째 열을 제외하고 보기 내의 모든 열을 제거합니다.
1. 첫 번째 열의 헤더를 클릭합니다.
1. **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 텍스트를 제거하고 다음 코드로 바꿉니다.


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   이 예제에서는 &#39;column.1&#39;을 사용합니다. 행은 &#39;사용자 지정 URL&#39; 필드의 값을 작업의 **개요** 섹션(&#39;column.2&#39;)에 대한 링크로 표시합니다. 작업의 **URL 필드**&#x200B;에 저장된 값을 표시합니다.

1. **완료** > **보기 저장**&#x200B;을 클릭합니다.
