---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "보고서를 실행할 때 오류 메시지: '현재 로그인되어 있지 않습니다.'"
description: 이 문서 - EDIT ME의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 4%

---

# 보고서를 실행할 때 오류 메시지: &quot;현재 로그인되어 있지 않습니다.&quot;

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
   <td> <p>보고서에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제

보고서를 실행하거나 대시보드에 표시할 때 다음 오류가 반환됩니다.\
*다시 시도해 보겠습니다. 현재 로그인되어 있지 않습니다.*

보고서에 결과가 표시되지 않습니다.

## 원인

보고서는 현재 비활성화된 사용자로 실행되도록 설정되어 있습니다.

## 솔루션

보고서 설정을 변경하려면 보고서에 대한 관리 권한이 있어야 합니다.\
보고서를 조정하고 결과를 보려면 다음을 수행하십시오.

1. 보고서로 이동합니다.
1. 클릭 **보고서 작업** > **편집** > **보고서 설정**.

1. 에서 활성 사용자의 이름을 지정합니다. **다음 액세스 권한으로 이 보고서를 실행합니다.** 필드.\
   또는\
   을(를) 종료하십시오. **다음 액세스 권한으로 이 보고서를 실행합니다.** 필드를 비워 둡니다.

1. 클릭 **완료**.
1. 클릭 **저장 + 닫기**.\
   이 보고서를 실행할 때 오류가 다시 나타나지 않습니다.
