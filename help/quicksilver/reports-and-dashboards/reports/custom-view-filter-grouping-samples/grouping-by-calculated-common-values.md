---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '그룹화: 그룹화에 있는 모든 개체에 공통되는 계산된 값으로 목록 결과를 구성합니다.'
description: 0~25, 26~50, 51~75, 75~99 및 100 범위에서 완료율별로 그룹화된 작업을 볼 수 있습니다. 텍스트 모드를 사용하여 그룹화를 만들어 이 작업을 수행할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# 그룹화: 그룹화에 있는 모든 객체에 공통되는 계산된 값으로 목록 결과를 구성합니다.

0~25, 26~50, 51~75, 75~99 및 100 범위에서 완료율별로 그룹화된 작업을 볼 수 있습니다. 텍스트 모드를 사용하여 그룹화를 만들어 이 작업을 수행할 수 있습니다.

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
   <td> <p>그룹화 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 그룹화 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 그룹화의 모든 객체에 공통되는 계산된 값으로 목록 결과를 구성합니다.

작업 목록에 이 그룹화를 적용하려면 다음을 수행합니다.

1. 작업 목록으로 이동합니다.
1. **그룹화**&#x200B;드롭다운 메뉴에서 **새 그룹화**&#x200B;을 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
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

1. **완료**&#x200B;를 클릭한 다음 **그룹화 저장**&#x200B;을 클릭합니다.
