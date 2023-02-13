---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "달력에 오류 메시지: '이 달력에 비활성화된 사용자의 보기 권한이 있습니다.'"
description: 이 문서 - EDIT ME의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 6%

---

# 달력에 오류 메시지: &quot;이 달력에 비활성화된 사용자의 보기 권한이 있습니다.&quot;

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>계획, 작업</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>일정에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제

사용자와 공유된 달력에 액세스할 때 다음 오류가 표시됩니다. 

*이 캘린더에는 비활성화된 사용자의 보기 권한이 있습니다. 관리자에게 캘린더 권한을 수정하도록 하십시오.*

## 원인

이 달력을 만든 사용자(원래 소유자)는 비활성화된 사용자입니다. 

## 솔루션

다음과 같은 방법으로 이 문제를 해결할 수 있습니다.

1. 원래 달력을 복사합니다. 달력을 복사하면 달력의 소유자가 됩니다. 복사한 달력은 원래 달력의 모든 정보를 표시해야 합니다.\
   달력 복사에 대한 자세한 내용은 [달력 보고서 복사](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. 복사한 일정을 원래 캘린더와 동일한 사용자와 공유합니다. 모든 사용자에게 새 달력에 동일한 정보가 표시됩니다.
1. (선택 사항 및 조건부) 원래 달력을 관리할 권한이 있으면 달력 공유 영역에서 캘린더가 공유되는 다른 모든 사용자를 제거합니다. 따라서 사용자가 잘못된 달력을 표시하려고 할 때 혼동을 없앨 수 있습니다.
