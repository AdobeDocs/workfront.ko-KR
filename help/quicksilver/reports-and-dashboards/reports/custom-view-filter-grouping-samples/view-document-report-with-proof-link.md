---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 증명에 대한 링크가 있는 문서 보고서'
description: '보기: 증명에 대한 링크가 있는 문서 보고서'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# 보기: 증명에 대한 링크가 있는 문서 보고서

이 문서 보기에서는 문서의 현재 버전 증명에 대한 링크를 삽입할 수 있습니다.

![](assets/view-document-with-proof-link-350x92.png)

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

## 증명에 대한 링크가 있는 문서 보고서 보기

이 보기를 적용하려면:

1. 문서 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.

1. **열 추가**&#x200B;를 클릭합니다.
1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. 텍스트 모드 영역 위로 마우스를 가져간 후 **텍스트를 편집하려면 클릭**&#x200B;합니다.
1. **텍스트 모드** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >&quot;내 도메인&quot;을 실제 Workfront 도메인으로 바꿉니다. 예를 들어 회사의 Workfront url이 *Company.my.workfront.com*&#x200B;인 경우 도메인은 &quot;Company&quot;입니다.

1. **저장**&#x200B;을 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
1. 보기의 이름을 입력한 다음 **보기 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 증명이 포함된 문서만 표시하려면 다음을 수행하여 필터를 추가합니다.

   1. **필터** 드롭다운 메뉴를 클릭한 다음 **새 필터**&#x200B;을 클릭합니다.
   1. **필터 규칙 추가**&#x200B;를 클릭하고 증명 소유자를 입력한 다음 목록에 표시될 때 **증명 소유자 ID**&#x200B;를 선택합니다.
   1. 필터 수정자에 대해 **Is Not Blank**&#x200B;을(를) 선택합니다.
   1. **필터 저장**&#x200B;을 클릭하고 필터 이름을 입력한 다음 **필터 저장**&#x200B;을 클릭합니다.

1. 증명 링크 열의 링크를 클릭하여 문서의 마지막 버전에 대한 증명에 액세스합니다.
