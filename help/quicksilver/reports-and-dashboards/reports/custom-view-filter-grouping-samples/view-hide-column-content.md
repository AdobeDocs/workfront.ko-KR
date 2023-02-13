---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 열 내용 숨기기'
description: 보기의 열에서 정보를 숨길 수 있습니다. 열의 텍스트 모드를 수정하여 이 작업을 수행할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 보기: 열의 내용 숨기기

보기의 열에서 정보를 숨길 수 있습니다. 열의 텍스트 모드를 수정하여 이 작업을 수행할 수 있습니다.

>[!TIP]
>
>* 숨겨진 열을 사용하여 보기에 표시하지 않을 특정 개체를 기준으로 정렬할 수 있습니다.\
   >  예를 들어 작업 보기에서 작업 번호별로 정렬하고 보기에서 작업 번호 정보를 숨길 수 있습니다. 이 경우 열에서 참조되는 개체는 보기를 정렬하는 데 도움이 되지만, 해당 개체의 정보는 보기에 표시되지 않습니다.
>* 열을 숨길 때는 열의 정보가 숨겨지지만 열은 여전히 뷰에 있습니다.
>


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

## 예: 작업 보기에서 작업 번호 열을 정렬 및 숨깁니다.

1. 작업 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 클릭 **열 추가** 작업 번호 입력 시작 **이 열에 표시** 필드를 선택한 다음 목록에 표시될 때 선택합니다.

1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역을 마우스로 가리킨 다음 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>이 코드에서 열을 숨기는 중요한 변경 사항은 다음과 같습니다.

   ```
   displayname
   ```

   이 줄은 비어 있어야 합니다.

   ```
   valuefield
   ```

   이 항목은 *value*, 및 는 비어 있어야 합니다.

   ```
   width
   ```

   : 필드에 따라 값 가 있어야 합니다 *0* 또는 *1*.

1. 클릭 **저장**, 그런 다음 **보기 저장**.
