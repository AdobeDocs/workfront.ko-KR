---
product-area: documents
navigation-topic: approvals
title: 문서 승인 요청
description: Adobe Workfront에서 문서에 대해 관리자나 다른 사용자에게 승인을 요청할 수 있습니다. 시스템 보안 환경 설정에 설명된 대로 Workfront 관리자가 이 기능을 활성화한 경우 Workfront 계정이 없는 사람에게 문서 승인을 요청할 수도 있습니다.
author: Courtney
feature: Work Management
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 문서 승인 요청

Adobe Workfront에서 문서에 대해 관리자나 다른 사용자에게 승인을 요청할 수 있습니다. 에 설명된 대로 Workfront 관리자가 이 기능을 활성화한 경우 Workfront 계정이 없는 사람에게 문서 승인을 요청할 수도 있습니다 [시스템 보안 환경 설정 구성](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

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
   <td> <p>검토 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트, 작업, 문제, 템플릿, Portfolio, 프로그램, 보고서, 대시보드 및 달력, 문서에 대한 액세스 권한을 보거나 그 이상의</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>요청 액세스 또는 승인과 연관된 객체에 대한 보기 또는 더 높은 액세스 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문서 승인 요청

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**.
1. 필요한 문서를 찾습니다.

1. 아래로 스크롤하여 **승인** 요약 섹션에서 다음을 입력하여 **승인자 추가** 텍스트 상자 이름이나 이메일 외부 사용자별로 Workfront 사용자를 추가할 수 있습니다.

1. Adobe Workfront 관리자가 다음에 설명된 대로 Workfront을 사용하지 않는 사람과 공동 작업하는 기능을 활성화한 경우 [시스템 보안 환경 설정 구성](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)에는 포함할 이메일 주소를 입력할 수 있습니다.

   팀이나 그룹에서 승인을 요청할 수 없습니다.

1. 이전 단계를 반복하여 다른 승인자를 추가합니다.

## 새 버전에 대한 승인을 다시 제출합니다.

새 버전을 업로드할 때 문서 승인 결정은 자동으로 재설정되지 않습니다. 예를 들어, 변경 사항이 포함된 문서가 승인되면 지정된 변경 사항이 있는 새 버전을 업로드하더라도 결정 시 &quot;변경 내용&quot;이 표시됩니다. 승인을 수동으로 다시 제출하는 경우 새 버전에 대한 결정을 지울 수 있습니다.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**.
1. 필요한 문서를 찾습니다.

1. 아래로 스크롤하여 **승인** 요약 섹션에서 자세히 아이콘을 클릭한 다음 다시 제출을 클릭합니다.

   ![](assets/nwe-resubmit-approval-350x149.png)

## 문서 승인 요청 삭제

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**.
1. 필요한 문서를 찾습니다.

1. 아래로 스크롤하여 **승인** 요약 섹션에서 **자세히** 승인자 이름이 있는 인라인 메뉴를 선택하고 을 선택합니다 **삭제**.

   승인 요청이 제거되고 승인자가 더 이상 승인이 필요하지 않다는 알림을 받습니다. 승인 관련 공유 액세스 권한도 제거됩니다.

## 승인자에게 미리 알림 보내기

승인자가 피드백을 기다리고 있음을 알리는 메시지를 보내어 문서에 서명할 수 있습니다.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**.
1. 필요한 문서를 찾습니다.

1. 아래로 스크롤하여 **승인** 요약 섹션에서 **자세히** 승인자 이름이 있는 인라인 메뉴를 선택하고 을 선택합니다 **알림**.

   승인자는 승인이 아직 보류 중임을 알리는 알림을 받습니다. 전자 메일 미리 알림을 받을 수도 있습니다.
