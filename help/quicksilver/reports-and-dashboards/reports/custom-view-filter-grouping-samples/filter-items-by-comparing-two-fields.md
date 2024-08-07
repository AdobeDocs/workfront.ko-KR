---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '필터: 두 필드를 비교하여 목록의 항목 제거'
description: 두 필드를 비교하여 목록에서 항목을 필터링할 수 있습니다. 예를 들어 작업의 실제 완료 일자가 계획된 완료 일자보다 큰 작업만 표시할 수 있습니다.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 필터: 두 필드를 비교하여 목록의 항목 제거

두 필드를 비교하여 목록에서 항목을 필터링할 수 있습니다. 예를 들어 작업의 실제 완료 일자가 계획된 완료 일자보다 큰 작업만 표시할 수 있습니다.

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
   <td> <p>필터 수정 요청 </p>
   <p>보고서 수정 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서 수정</p> <p>필터, 보기, 그룹화에 대한 액세스 권한을 편집하여 필터 수정</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 두 필드를 비교하여 항목 필터링

1. 작업 목록으로 이동합니다.
1. **필터** 드롭다운 메뉴에서 **새 필터**&#x200B;을(를) 선택합니다.

1. **필터 규칙 추가**&#x200B;를 클릭하고 **실제 완료 날짜** >**보다 큼** > **날짜 선택**&#x200B;을(를) 추가합니다.

   >[!TIP]
   >
   >사용 가능한 경우 선택한 필드에 사용할 필터 수정자를 선택합니다.

1. **텍스트 모드로 전환**&#x200B;을 클릭합니다.
1. **보고서에 대한 필터 규칙 설정** 영역에 다음 코드를 추가합니다.

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. **완료**&#x200B;를 클릭한 다음 **필터 저장**&#x200B;을 클릭합니다.
