---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 열에 있는 개체에 대한 링크 제거'
description: 기본적으로 객체의 세부 사항 페이지에 대한 보기 링크에 표시되는 일부 객체입니다. 예를 들어 프로젝트 이름 을 표시하는 열은 프로젝트에 대한 링크입니다. 사용자 이름을 표시하는 열은 사용자의 프로필 페이지에 대한 링크입니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# 보기: 열의 개체에 대한 링크 제거

기본적으로 객체의 세부 사항 페이지에 대한 보기 링크에 표시되는 일부 객체입니다. 예를 들어 프로젝트 이름 을 표시하는 열은 프로젝트에 대한 링크입니다. 사용자 이름을 표시하는 열은 사용자의 프로필 페이지에 대한 링크입니다.

모든 보기에 표시되는 열의 텍스트 모드를 사용하여 이 링크를 제거할 수 있습니다.

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

## 예: 작업 보기의 작업 이름 열에서 작업에 대한 링크를 제거합니다.

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기** 새 보기를 만들려면

   또는

   을(를) 클릭합니다. **편집 아이콘** ![](assets/edit-icon.png)

   기존 뷰를 편집하려면 뷰를 선택합니다.

1. 클릭 **열 추가** 새 열을 추가하려면

   또는

   객체에 대한 링크가 있는 기존 열을 클릭합니다.

1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역을 마우스로 가리킨 다음 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.

   <pre>displayname=작업 이름<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >다음을 조정하여 다른 개체에 유사한 코드를 사용할 수 있습니다.
   >
   >   
   >   
   >   * 바꾸기 **값** 코드 줄 **valueexpression** 등호 뒤에 중괄호 안에 포함된 동일한 이름을 유지합니다.
   >
   >     ```>   
   >     link.
   >     ```   >   
   >   
   >     from the original text of the column. For example, eliminate all the following lines:
   >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
   >
   >
   >



1. 클릭 **저장**, 그런 다음 **보기 저장**.
