---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 목록 결과를 그룹 내의 모든 개체에 공통되는 계산된 값으로 구성합니다.'
description: 0-25, 26-50, 51-75, 75-99 및 100 범위에서 완료율 순으로 그룹화된 작업을 볼 수 있습니다. 텍스트 모드를 사용하여 그룹을 만들어 이 작업을 수행할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# 그룹화: 목록 결과를 그룹화 내의 모든 개체에 공통되는 계산된 값으로 구성합니다.

0-25, 26-50, 51-75, 75-99 및 100 범위에서 완료율 순으로 그룹화된 작업을 볼 수 있습니다. 텍스트 모드를 사용하여 그룹을 만들어 이 작업을 수행할 수 있습니다.

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

## 목록 결과를 그룹화 중인 모든 개체에 공통되는 계산된 값으로 구성합니다

작업 목록에 이 그룹을 적용하려면 다음을 수행합니다.

1. 작업 목록으로 이동합니다.
1. 에서 **그룹화**&#x200B;드롭다운 메뉴에서 **새 그룹화**.

1. 클릭 **텍스트 모드로 전환**.
1. 사용 가능한 공간에 다음 코드를 추가합니다.

   ```
   textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({
   ```

   ```
   percentComplete
   ```

   ```
   }>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete
   ```

1. 클릭 **완료**, 그런 다음 **그룹화 저장**.
