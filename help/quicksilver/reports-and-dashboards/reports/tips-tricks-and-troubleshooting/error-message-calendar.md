---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '캘린더에 오류 메시지: ''이 캘린더에는 비활성화된 사용자의 보기 권한이 있습니다.'''
description: '''이 캘린더에는 비활성화된 사용자의 보기 권한이 있습니다.'' 오류 메시지에 대해 알아봅니다.'
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%

---

# 캘린더에 오류 메시지: &quot;이 캘린더에는 비활성화된 사용자의 보기 권한이 있습니다.&quot;

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
     <p>표준</p>
     <p>작업 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드, 캘린더에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>캘린더에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 문제

공유된 캘린더에 액세스할 때 다음 오류가 표시됩니다. 

*이 캘린더에는 비활성화된 사용자의 보기 권한이 있습니다. 관리자에게 캘린더 권한을 수정하도록 하십시오.*

## 원인

이 캘린더를 만든 사용자(원래 소유자)는 비활성화된 사용자입니다. 

## 솔루션

다음과 같은 방법으로 이 문제를 해결할 수 있습니다.

1. 원래 달력을 복사합니다. 캘린더를 복사하면 캘린더의 소유자가 됩니다. 복사된 캘린더에는 원래 캘린더의 모든 정보가 표시됩니다.\
   일정 복사에 대한 자세한 내용은 [일정 보고서 복사](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md)를 참조하세요.

1. 복사된 캘린더를 원래 캘린더와 동일한 사용자와 공유합니다. 모든 사용자는 새 캘린더에 동일한 정보를 볼 수 있습니다.
1. (선택 사항 및 조건부) 원래 달력을 관리할 수 있는 권한이 있는 경우 달력 공유 영역에서 달력을 공유하는 다른 모든 사용자를 제거합니다. 이렇게 하면 잘못된 달력을 표시하려는 사용자의 혼동을 피할 수 있습니다.
