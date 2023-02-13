---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '계산된 사용자 지정 필드 예: 사용자 지정 양식에 상태 타임스탬프 표시'
description: 다음 계산된 필드는 객체 상태가 진행 중(INP)으로 표시된 날짜를 표시합니다. 문제, 작업 또는 프로젝트에 대해 계산된 사용자 지정 필드에 동일한 정보를 사용할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 계산된 사용자 지정 필드 예: 사용자 지정 양식에 상태 타임스탬프 표시

다음 계산된 필드는 객체 상태가 진행 중(INP)으로 표시된 날짜를 표시합니다. 문제, 작업 또는 프로젝트에 대해 계산된 사용자 지정 필드에 동일한 정보를 사용할 수 있습니다.

>[!NOTE]
>
>개체의 상태가 INP로 변경된 다음 다른 상태로 변경된 다음 다시 INP로 돌아오면 Adobe Workfront은 첫 번째 변경 내용의 타임스탬프만 INP에 캡처합니다.

## 액세스 요구 사항

다음 항목이 있어야 합니다.

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront 라이선스*</p> </td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>보고서, 대시보드 및 달력 만들기에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>개체 권한</strong> </p> </td> 
   <td> <p>양식이 첨부된 개체의 권한을 관리합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.<br>대시보드 권한에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">보고서, 대시보드 및 달력 공유 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 전제 조건

필드의 편집 내역을 표시하는 계산된 필드를 사용자 지정 양식에 추가하려면 먼저 사용자 지정 양식을 만들어야 합니다.

## 사용자 지정 양식에 상태 타임스탬프 표시

1. 필드를 추가할 사용자 지정 양식으로 이동합니다.
1. 클릭 **계산된 지표** 계산된 사용자 지정 필드를 양식에 추가하려면
1. 입력 **레이블** 사용자 지정 필드의 경우(예: ) *상태 타임스탬프 사용자 지정 필드*.
1. 클릭 **완료**&#x200B;를 클릭한 다음 **저장+닫기**.
1. 사용자 지정 양식을 다시 연 다음 새 양식을 선택합니다 **상태 타임스탬프 사용자 지정 필드** 클릭합니다.
1. 에서 **계산** 상자에서 사용자 지정 필드에 대해 다음 계산을 복사하여 붙여넣습니다.

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >이 계산은 모든 객체 및 모든 상태에 대해 동일합니다. 이 계산에서는 개체 상태에 대한 상태 이름이 아니라 항상 세 글자 키를 사용해야 합니다.
   >
   >상태 키에 대한 자세한 내용은 [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 클릭 **저장+닫기**.

   이제 상태 타임스탬프 사용자 지정 필드에 대해 보고하거나 다른 계산, 보고서 또는 사용자 지정 필드에서 사용할 수 있습니다.
