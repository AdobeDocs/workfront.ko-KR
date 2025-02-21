---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열의 오브젝트에 대한 링크 제거'
description: 뷰에 표시되는 일부 객체는 기본적으로 객체의 세부내용 페이지에 연결됩니다. 예를 들어, 프로젝트 이름을 표시하는 열은 프로젝트에 대한 링크이고, 사용자 이름을 표시하는 열은 사용자의 프로필 페이지에 대한 링크입니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 보기: 열의 오브젝트에 대한 링크 제거

<!--Audited: 11/2024-->

뷰에 표시되는 일부 객체는 기본적으로 객체의 세부내용 페이지에 연결됩니다. 예를 들어, 프로젝트 이름을 표시하는 열은 프로젝트에 대한 링크이고, 사용자 이름을 표시하는 열은 사용자의 프로필 페이지에 대한 링크입니다.

모든 보기에 표시되는 열의 텍스트 모드를 사용하여 이 링크를 제거할 수 있습니다.

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


## 예: 작업 보기의 작업 이름 열에서 작업에 대한 링크 제거:

1. 작업 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 클릭하여 새 보기를 만듭니다.

   또는

   **편집 아이콘** ![편집 아이콘](assets/edit-icon.png) 클릭

   기존 뷰를 편집하려면 뷰를 선택합니다.

1. 새 열을 추가하려면 **열 추가**&#x200B;를 클릭하세요.

   또는

   오브젝트에 대한 링크가 있는 기존 열을 클릭합니다.

1. **텍스트 모드로 전환** > **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >다음을 조정하여 다른 개체에 대해 유사한 코드를 사용할 수 있습니다.
   >
   >* 코드의 `valuefield` 줄을 `valueexpression`(으)로 바꾸고 대괄호 안에 동일한 이름을 등호 뒤에 포함시킵니다.
   >* 열의 원래 텍스트에서 `link.`(으)로 시작하는 모든 줄을 제거하십시오. 예를 들어 다음 줄을 모두 제거합니다.
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.

