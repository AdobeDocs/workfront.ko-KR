---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''보기: 증명 링크가 있는 문서 보고서'
description: '''보기: 증명 링크가 있는 문서 보고서'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 40c7142574c3491b7bdf8799c287db1c3f7e9e8c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 보기: 증명 링크가 있는 문서 보고서

이 문서 보기에서는 문서의 현재 버전 증명에 대한 링크를 삽입할 수 있습니다.

![](assets/view-document-with-proof-link-350x92.png)

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

## 증명 링크가 있는 문서 보고서 보기

이 뷰를 적용하려면 다음을 수행합니다.

1. 문서 목록으로 이동합니다.
1. 에서 **보기** 드롭다운 메뉴에서 **새 보기**.

1. 클릭 **열 추가**.
1. 클릭 **텍스트 모드로 전환**.
1. 텍스트 모드 영역을 마우스로 가리킨 다음 **텍스트를 편집하려면 클릭하십시오.**.
1. 에서 찾을 텍스트를 제거합니다. **텍스트 모드** 상자를 열고 다음 코드로 바꿉니다.

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >&quot;도메인&quot;을 실제 Workfront 도메인으로 바꿉니다. 예를 들어 회사의 Workfront url이 *Company.my.workfront.com*, 도메인은 &quot;Company&quot;입니다.

1. 클릭 **저장**, 그런 다음 **보기 저장**.
1. 보기의 이름을 입력한 다음 를 클릭합니다 **보기 저장**.
1. (선택 사항) 증명이 있는 문서만 표시하려면 다음을 수행하여 필터를 추가합니다.

   1. 을(를) 클릭합니다. **필터** 드롭다운 메뉴를 클릭한 다음 **새 필터**.
   1. 클릭 **필터 규칙 추가** 증명 소유자 입력을 시작한 다음 **증명 소유자 ID** 목록에 표시됩니다.
   1. 선택 **비어 있지 않음** 필터 수정자에 사용됩니다.
   1. 클릭 **필터 저장**&#x200B;를 입력한 다음 필터 이름을 입력하고 **필터 저장**.

1. 문서의 마지막 버전 증명에 액세스하려면 [증명 링크] 열의 링크를 클릭합니다.
