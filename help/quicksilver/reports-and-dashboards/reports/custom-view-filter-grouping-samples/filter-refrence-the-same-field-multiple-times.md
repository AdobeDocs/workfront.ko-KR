---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 동일한 필드(''AND'' 문)를 참조하는 여러 필터 규칙을 만듭니다.'
description: 표준 모드 인터페이스에서 동일한 필드를 참조하는 여러 필터를 만들려고 할 때(AND 한정자 사용) 보고서를 저장하고 Report Builder를 종료하면 필터 중 하나가 삭제됩니다.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 필터: 동일한 필드(&quot;AND&quot; 문)를 참조하는 여러 필터 규칙을 만듭니다.

<!--Audited: 10/2024-->

표준 모드 인터페이스에서 동일한 필드를 참조하는 여러 필터를 만들려고 할 때(AND 한정자 사용) 보고서를 저장하고 Report Builder를 종료하면 필터 중 하나가 삭제됩니다.

**예:** 이름에 &quot;녹색&quot;이라는 단어는 들어 있지만 &quot;빨간색&quot;이라는 단어는 들어 있지 않은 작업만 볼 수 있습니다. Adobe Workfront에서는 동일한 필드(작업 이름)를 참조하지만 다른 수정자를 사용하고 다른 값을 참조하므로 표준 모드 인터페이스를 사용하여 다음 필터 규칙을 저장할 수 없습니다.

* 작업 이름 > 포함 > 녹색
* 작업 이름 > 포함하지 않음 > 빨간색

그러나 텍스트 모드를 사용하여 이 필터를 만들 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>필터 수정을 위한 기여자 또는 요청 </p>
   <p>표준 또는 보고서 수정 계획</p>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 동일한 필드를 참조하는 여러 필터 규칙 만들기

1. 작업 목록으로 이동합니다.
1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.
1. **텍스트 모드**&#x200B;를 클릭합니다.
1. 표시된 상자에 다음 코드를 추가합니다.

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >유사한 필터를 빌드하려면 먼저 첫 번째 문을 빌드합니다. For example:
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >필요한 횟수만큼 명령문을 복사하여 붙여넣습니다. 그런 다음 동일한 필드(여기서는 &quot;name&quot;)를 참조하는 데 필요한 만큼 문을 추가하고 추가 문을 다음과 같이 수정할 수 있습니다.
   >
   >1. 복사된 두 줄 앞에 &quot;AND:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot; 등이 있습니다. 각 새 필드에 대해 가능한 값입니다.
   >1. 필드 줄을 새 필드 값으로 바꿉니다(&quot;=&quot; 기호 뒤).
   >1. 수정자 라인(_Mod)을 새 수정자로 바꿉니다.
   >   
   >이 문은 대/소문자를 구분합니다.

1. **적용**&#x200B;을 클릭한 다음 **새 이름으로 저장**&#x200B;을 클릭합니다.
