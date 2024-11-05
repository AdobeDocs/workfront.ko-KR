---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '보기: 증명에 대한 링크가 있는 문서 보고서'
description: '보기: 증명에 대한 링크가 있는 문서 보고서'
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---

# 보기: 증명에 대한 링크가 있는 문서 보고서

<!--Audited: 11/2024-->

이 문서 보기에서는 문서의 현재 버전 증명에 대한 링크를 삽입할 수 있습니다.

![](assets/view-document-with-proof-link-350x92.png)

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
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>필터를 수정하는 기여자 </p></li>
   <li><p>보고서를 수정하는 표준</p></li> </ul>

<p>현재:</p>
   <ul><li><p>필터 수정 요청 </p></li>
   <li><p>보고서 수정 계획</p></li> </ul></td> 
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

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 증명에 대한 링크가 있는 문서 보고서 보기

이 보기를 적용하려면:

1. 문서 목록으로 이동합니다.
1. **보기** 드롭다운 메뉴에서 **새 보기**&#x200B;를 선택합니다.
1. **열 추가**&#x200B;를 클릭합니다.
1. **텍스트 모드로 전환**&#x200B;을 클릭한 다음 **텍스트 모드 편집**&#x200B;을 클릭합니다.
1. **텍스트 모드 편집** 상자에서 찾은 텍스트를 제거하고 다음 코드로 바꿉니다.

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

1. **완료**&#x200B;를 클릭한 다음 **보기 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 보기 이름을 업데이트한 다음 **보기 저장**&#x200B;을 클릭합니다.
1. (선택 사항) 증명이 포함된 문서만 표시하려면 다음을 수행하여 필터를 추가합니다.

   1. **필터** 드롭다운 메뉴를 클릭한 다음 **새 필터**&#x200B;을 클릭합니다.
   1. **필터 규칙 추가**&#x200B;를 클릭하고 &quot;증명 소유자&quot;를 입력한 다음 목록에 표시될 때 **증명 소유자 ID**&#x200B;를 선택합니다.
   1. 필터 수정자에 대해 **Is Not Blank**&#x200B;을(를) 선택합니다.
   1. **필터 저장**&#x200B;을 클릭합니다.
   1. (선택 사항) 필터 이름을 업데이트한 다음 **필터 저장**&#x200B;을 클릭합니다.

1. 증명 링크 열의 링크를 클릭하여 문서의 마지막 버전에 대한 증명에 액세스합니다.
