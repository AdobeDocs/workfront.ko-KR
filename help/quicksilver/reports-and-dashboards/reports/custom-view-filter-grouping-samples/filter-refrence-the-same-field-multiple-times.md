---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "필터: 동일한 필드('AND' 문)를 참조하는 여러 필터 규칙을 만듭니다."
description: 표준 모드 인터페이스에서 동일한 필드를 참조하는 여러 필터를 만들려고 할 때(AND 한정자 사용) 보고서를 저장하고 Report Builder를 종료하면 필터 중 하나가 삭제됩니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# 필터: 동일한 필드(&quot;AND&quot; 문)를 참조하는 여러 필터 규칙을 만듭니다.

표준 모드 인터페이스에서 동일한 필드를 참조하는 여러 필터를 만들려고 할 때(AND 한정자 사용) 보고서를 저장하고 Report Builder를 종료하면 필터 중 하나가 삭제됩니다.

**예:** 이름에 &quot;녹색&quot;이라는 단어는 들어 있지만 &quot;빨간색&quot;이라는 단어는 들어 있지 않은 작업만 볼 수 있습니다. Adobe Workfront에서는 동일한 필드(작업 이름)를 참조하지만 다른 수정자를 사용하고 다른 값을 참조하므로 표준 모드 인터페이스를 사용하여 다음 필터 규칙을 저장할 수 없습니다.

* 작업 이름 > 포함 > 녹색
* 작업 이름 > 포함하지 않음 > 빨간색

그러나 텍스트 모드를 사용하여 이 필터를 만들 수 있습니다.

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
   <td> <p>필터 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 동일한 필드를 참조하는 여러 필터 규칙 만들기

1. 작업 목록으로 이동합니다.
1. 다음에서 **필터** 드롭다운 메뉴에서 다음을 선택합니다. **새 필터**.
1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역 위로 마우스를 가져간 다음 **텍스트를 편집하려면 클릭**.
1. 보고서에 대한 필터 규칙 설정 영역에서 다음 코드를 추가합니다.

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
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >필요한 횟수만큼 명령문을 복사하여 붙여넣습니다. 그런 다음 동일한 필드(여기서는 &quot;name&quot;)를 참조하는 데 필요한 만큼 문을 추가하고 추가 문을 다음과 같이 수정할 수 있습니다.
   >
   >1. 복사된 두 줄 앞에 &quot;AND&quot;:1:&quot;, &quot;및:2:&quot;, &quot;및:3:&quot;, 각 새 필드에 대해 가능한 값.
   >1. 필드 줄을 새 필드 값으로 바꿉니다(&quot;=&quot; 기호 뒤).
   >1. 수정자 라인(_Mod)을 새 수정자로 바꿉니다.

   >   
   >이 문은 대/소문자를 구분합니다.

1. 클릭 **완료**, 그런 다음 **필터 저장**.
