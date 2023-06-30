---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열의 오브젝트에 대한 링크 제거'
description: 뷰에 표시되는 일부 객체는 기본적으로 객체의 세부내용 페이지에 연결됩니다. 예를 들어, 프로젝트 이름을 표시하는 열은 프로젝트에 대한 링크이고, 사용자 이름을 표시하는 열은 사용자의 프로필 페이지에 대한 링크입니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 5480d6b5e97c4c2e21080bb92ffe255f60ed6f60
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# 보기: 열의 오브젝트에 대한 링크 제거

뷰에 표시되는 일부 객체는 기본적으로 객체의 세부내용 페이지에 연결됩니다. 예를 들어, 프로젝트 이름을 표시하는 열은 프로젝트에 대한 링크이고, 사용자 이름을 표시하는 열은 사용자의 프로필 페이지에 대한 링크입니다.

모든 보기에 표시되는 열의 텍스트 모드를 사용하여 이 링크를 제거할 수 있습니다.

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

## 예: 작업 보기의 작업 이름 열에서 작업에 대한 링크 제거:

1. 작업 목록으로 이동합니다.
1. 다음에서 **보기** 드롭다운 메뉴, 클릭 **새 보기** 새 보기를 만듭니다.

   또는

   다음을 클릭합니다. **편집 아이콘** ![](assets/edit-icon.png)

   기존 뷰를 편집하려면 뷰를 선택합니다.

1. 클릭 **열 추가** 새 열을 추가합니다.

   또는

   오브젝트에 대한 링크가 있는 기존 열을 클릭합니다.

1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 다음 **텍스트를 편집하려면 클릭**.
1. 에서 찾은 텍스트 제거 **텍스트 모드** 확인란을 선택하고 다음 코드로 바꿉니다.
   <pre>displayname=작업 이름<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueexpression={name}</strong><br>valueformat=Compound</pre>

   >[!TIP]
   >
   >다음을 조정하여 다른 개체에 대해 유사한 코드를 사용할 수 있습니다.
   >
   >* 바꾸기 **valuefield** 코드 줄 **valueexpression** 중괄호 안에 동일한 이름을 등호 뒤에 포함시킵니다.
   >* 다음으로 시작하는 모든 줄 제거 `link.` 열의 원본 텍스트에서 가져옵니다. 예를 들어 다음 줄을 모두 제거합니다.
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. 클릭 **저장**, 그런 다음 **보기 저장**.
