---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: FTE 가용성의 사용자 직무 역할 백분율'
description: 사용자 목록 보기에 열을 추가하여 사용자 프로필에 정의된 대로 사용자와 연결된 작업 역할 목록과 각 작업 역할에 대한 FTE 가용성 비율을 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 보기: FTE 가용성의 사용자 작업 역할 백분율

사용자 목록 보기에 열을 추가하여 사용자와 연관된 작업 역할 목록과 사용자 프로필에 정의된 대로 각 작업 역할에 대한 FTE 가용성 비율을 표시할 수 있습니다.

사용자의 FTE 사용 가능 비율을 정의하는 방법에 대한 자세한 내용은 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

![사용자_with_percent_avialbility_per_역할.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 플랜*</td> 
   <td> <p>어떤</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 라이선스*</td> 
   <td> <p>보기 수정 요청 </p>
   <p>보고서를 수정하기 위한 플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 보기 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정할 수 있는 방법에 대한 자세한 내용은 사용자 지정 액세스 수준</a> 만들기 또는 수정을 참조하십시오<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">개체 사용 권한</td> 
   <td> <p>보고서에 대한 사용 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 객체</a>에 대한 액세스 요청을 참조하십시오 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;사용 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 보기 사용자 직무 FTE 가용성의 백분율

1. 사용자 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 미리 보기** 영역에서 **열 추가**&#x200B;를 클릭합니다.

1. 새로운 열의 머리글을 클릭한 다음, 텍스트 모드로&#x200B;**전환을 클릭하십시오**.
1. 텍스트 모드 영역 위에 마우스를 놓고 [텍스트를&#x200B;**편집하려면 클릭]을 클릭합니다**.
1. 텍스트 모드&#x200B;**상자에서 찾은**&#x200B;텍스트를 제거 후 다음 코드로 바꿉니다.
   <pre>displayname=역할 시간 백분율<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=반복<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. **저장** 클릭한 다음 **저장 보기**.

1. (선택 사항) 보기 이름을 지정한 다음 저장 보기&#x200B;**클릭합니다**.
