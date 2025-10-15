---
product-area: documents
navigation-topic: approvals
title: 문서 승인 요청
description: Adobe Workfront에서 문서에 대한 관리자 또는 다른 사용자의 승인을 요청할 수 있습니다. 시스템 보안 환경 설정 구성에 설명된 대로 Workfront 관리자가 이 기능을 활성화한 경우 Workfront 계정이 없는 사람들로부터 문서 승인을 요청할 수도 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 2503b6e628e4860a5652c620d8e4d0eea2414443
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

# 문서 승인 요청

Adobe Workfront에서 문서에 대한 관리자 또는 다른 사용자의 승인을 요청할 수 있습니다. [시스템 보안 환경 설정 구성](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)에 설명된 대로 Workfront 관리자가 이 기능을 활성화한 경우 Workfront 계정이 없는 사람에게 문서 승인을 요청할 수도 있습니다.

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
   <p>기여자 이상</p>
   <p>검토 이상</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트, 작업, 문제, 템플릿, 포트폴리오, 프로그램, 보고서, 대시보드 및 캘린더, 문서에 대한 보기 또는 상위 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 또는 승인 요청과 연결된 개체에 대한 액세스 관리 </p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 문서 승인 요청

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.
1. 필요한 문서를 찾습니다.

1. 요약의 **승인** 섹션까지 아래로 스크롤한 다음 **승인자 추가** 텍스트 상자에 입력을 시작합니다. 이름별로 Workfront 사용자를 추가하거나 이메일로 외부 사용자를 추가할 수 있습니다.

1. [시스템 보안 환경 설정 구성](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)에 설명된 대로 Adobe Workfront 관리자가 Workfront을 사용하지 않는 사람과 공동 작업을 수행하는 기능을 활성화한 경우, 해당 사용자를 포함하도록 전자 메일 주소를 입력할 수 있습니다.

   팀 또는 그룹에서 승인을 요청할 수 없습니다.

1. 다른 승인자를 추가하려면 이전 단계를 반복하십시오.

## 새 버전에 대한 승인 다시 제출

새 버전을 업로드할 때 문서 승인 결정이 자동으로 재설정되지 않습니다. 예를 들어 문서에 변경 사항이 적용되면 지정된 변경 사항이 있는 새 버전을 업로드하더라도 결정에 &quot;변경 사항&quot;이 결정으로 표시됩니다. 승인을 수동으로 다시 제출하는 경우 새 버전에 대한 결정을 지울 수 있습니다.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.
1. 필요한 문서를 찾습니다.

1. 요약에서 **승인** 섹션까지 아래로 스크롤하고 자세히 아이콘을 클릭한 다음 다시 제출을 클릭합니다.

   ![승인 다시 제출](assets/nwe-resubmit-approval-350x149.png)

## 문서 승인 요청 삭제

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.
1. 필요한 문서를 찾습니다.

1. 요약의 **승인** 섹션까지 아래로 스크롤한 다음 승인자 이름으로 인라인된 **기타** 메뉴를 클릭하고 **삭제**&#x200B;를 선택합니다.

   승인 요청이 제거되고 승인자가 더 이상 승인이 필요하지 않다는 알림을 받습니다. 승인 관련 공유 액세스도 제거됩니다.

## 승인자에게 미리 알림 보내기

문서를 승인자에게 피드백 대기 중임을 알리는 메시지를 보낼 수 있습니다.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 **문서**&#x200B;을(를) 선택합니다.
1. 필요한 문서를 찾습니다.

1. 요약의 **승인** 섹션까지 아래로 스크롤한 다음 승인자 이름으로 인라인된 **기타** 메뉴를 클릭하고 **미리 알림**&#x200B;을 선택합니다.

   승인자는 승인이 아직 보류 중임을 알리는 알림을 받습니다. 활성화된 경우 이메일 미리 알림을 받을 수도 있습니다.
