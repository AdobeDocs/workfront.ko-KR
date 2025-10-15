---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '보고서를 실행할 때 오류 메시지: ''현재 로그인되어 있지 않습니다.'''
description: '''현재 로그인하지 않음'' 오류 메시지에 대해 알아봅니다.'
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 6%

---

# 보고서를 실행할 때 오류 메시지: &quot;현재 로그인되어 있지 않습니다.&quot;

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
   <td> <p>보고서에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 문제

보고서를 실행하거나 대시보드에 표시할 때 다음 오류가 반환됩니다.\
*다시 시도해 보십시오. 현재 로그인되어 있지 않습니다.*

보고서에 결과가 표시되지 않습니다.

## 원인

보고서는 현재 비활성화된 사용자로 실행되도록 설정되어 있습니다.

## 솔루션

보고서 설정을 변경하려면 보고서에 대한 관리 권한이 있어야 합니다.\
보고서를 조정하고 결과를 보려면 다음 작업을 수행하십시오.

1. 보고서로 이동합니다.
1. **보고서 작업** > **편집** > **보고서 설정**&#x200B;을 클릭합니다.

1. **액세스 권한:** 필드에서 이 보고서 실행에서 활성 사용자의 이름을 지정하십시오.\
   또는\
   **액세스 권한:** 필드가 비어 있는 상태로 이 보고서 실행

1. **완료**&#x200B;를 클릭합니다.
1. **저장 및 닫기**&#x200B;를 클릭합니다.\
   이 보고서를 실행할 때 오류가 다시 나타나지 않아야 합니다.
