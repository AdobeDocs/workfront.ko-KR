---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 작업을 들여써서 작업에 상위-하위 관계 표시'
description: 작업 목록에 사용자 정의 보기를 추가하고 목록을 내보내기 전에 이 보기를 선택하여 내보낸 작업 목록에서 상위-하위 관계를 구분할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 2%

---

# 보기: 작업을 들여써서 작업의 상위-하위 관계를 표시합니다.

작업 목록에 사용자 정의 보기를 추가하고 목록을 내보내기 전에 이 보기를 선택하여 내보낸 작업 목록에서 상위-하위 관계를 구분할 수 있습니다.

![](assets/parent-child-indented-custom-view-350x94.png)

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

## 작업을 들여써서 작업에 상위-하위 관계 표시

1. 내보낼 작업 목록이 있는 프로젝트로 이동합니다.
1. **보기** 드롭다운 메뉴를 클릭하고 **새 보기**&#x200B;를 선택합니다.

1. 화면 왼쪽 상단 모서리에서 필터 이름을 지정합니다.
1. **작업 이름** 열 머리글을 클릭합니다.

1. 오른쪽 상단에서 **텍스트 모드로 전환**&#x200B;을 선택합니다.
1. 텍스트 상자의 아무 곳이나 클릭하여 텍스트를 편집하고 기존 텍스트를 모두 제거합니다.
1. 다음 텍스트를 붙여넣습니다.


```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
```

1. **저장**&#x200B;을 클릭합니다.
1. **보기 저장**&#x200B;을 클릭합니다.
