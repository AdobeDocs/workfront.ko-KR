---
product-area: documents
navigation-topic: approvals
title: 문서에 대한 승인 워크플로 템플릿 만들기
description: 승인 템플릿을 만들어 승인 프로세스를 간소화할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 9%

---

# 문서에 대한 승인 워크플로 템플릿 만들기

Workfront 설정 영역에서 Standard 라이선스를 가진 사용자는 재사용 가능한 승인 템플릿을 만들 수 있습니다. 승인 템플릿이 생성되면 프로젝트, 작업 또는 문제의 문서 영역에 있는 자산에 적용할 수 있습니다.

>[!IMPORTANT]
>
>이 문서의 내용은 특정 계정에만 사용할 수 있는 업데이트된 문서 승인 기능에 적용됩니다. 표준 승인 프로세스에 대한 자세한 내용은 [작업 승인](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)에 나열된 문서를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>표준</p> 
   <p>플랜</p>
   </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++
ß

## 승인 템플릿 만들기

{{step-1-to-setup}}

1. 왼쪽 패널에서 **검토 및 승인** > **승인 템플릿**&#x200B;을 클릭합니다.
1. 페이지 오른쪽에서 **새 템플릿**&#x200B;을 클릭합니다.

1. 다음 세부 정보를 입력합니다.

   <table>
     <tr>
   <td><strong>템플릿 이름</strong></td>
   <td>템플릿 이름을 추가합니다. </td>
   </tr>
   <tr>
   <td><strong>단계 이름</strong></td>
   <td>단계 이름을 추가합니다. <em>초기 검토</em> 또는 <em>최종 승인</em>과 같이 이름을 좀 더 설명적인 이름으로 변경할 수 있습니다.</td>
   </tr>
   <tr>
   <td><strong>이름 또는 이메일 추가</strong></td>
   <td>승인자 또는 검토자로 추가할 사용자 또는 팀 이름을 입력하십시오. 검토자만 있는 경우 알림을 받고 검토를 완료할 수 있는 옵션이 있지만 결정이 필요하거나 수행되지 않습니다.</td>
   </tr>
   <tr>
   <td><strong>한 가지 결정 필요(선택 사항)</strong></td>
   <td>가장 먼저 결정을 내리는 사람이 단계를 완료합니다.</td>
   </tr>
   <tr>
   <td><strong>기한까지 남은 근무일</strong></td>
   <td>단계가 활성화된 후 승인이 만료될 때까지 남은 근무일 수를 선택합니다.</td>
   </tr>
   </table>

1. (선택 사항) 이전 단계를 반복하여 필요에 따라 단계를 더 추가합니다.

   >[!NOTE]
   >
   >여러 단계를 추가하면 승인 워크플로가 단계가 나열된 순서로 진행됩니다. 필요한 모든 결정이 이루어지면 다음 단계가 시작되고 이전 단계가 잠깁니다.

   ![문서 세부 정보](assets/new-stage.png)

1. **저장**&#x200B;을 클릭합니다.

템플릿이 생성되면 프로젝트, 작업 또는 문제의 문서 영역에 있는 문서에 적용하여 Workfront에서 공식 검토 및 승인 프로세스를 시작할 수 있습니다.



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
