---
product-area: documents
navigation-topic: approvals
title: 문서 승인 워크플로 만들기
description: Adobe Workfront에서 문서에 대한 다른 사용자의 승인을 요청할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 3%

---

# 문서 승인 워크플로 만들기

Adobe Workfront에서 문서에 대한 다른 사용자 또는 팀의 승인을 요청하거나 승인할 필요 없이 문서를 검토하도록 요청할 수 있습니다.

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
   <td> <p>기존 Workfront 스토리지를 사용하여 승인을 관리하는 모든 Workfront 패키지</p>
<p>Adobe 엔터프라이즈 스토리지를 사용하여 승인을 관리하는 모든 워크플로우 패키지</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td>  
   <td>
   <p>기여자 이상</p>
   <p>검토 이상</p>
   <p>Frame.io 통합을 사용하는 경우 승인 워크플로를 만들려면 표준 라이선스가 있어야 합니다.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트, 작업, 문제, 템플릿, 포트폴리오, 프로그램, 보고서, 대시보드 및 캘린더, 문서에 대한 보기 또는 상위 액세스 권한</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>액세스 또는 승인 요청과 연결된 개체에 대한 액세스 관리 </p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기존 문서 영역의 요약 패널에서 승인 워크플로를 만듭니다

조직이 Workfront 스토리지에 있는 경우 Workfront의 문서에 액세스할 때 기존 문서 영역이 표시됩니다. Workfront 스토리지에 대한 자세한 내용은 [Workfront 스토리지와 Adobe 엔터프라이즈 스토리지 비교](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)를 참조하십시오.

승인 워크플로를 만들려면 다음 작업을 수행하십시오.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 필요한 문서를 클릭하면 해당 문서에 대한 [문서 요약] 패널이 열립니다.

1. 버전 드롭다운에서 승인을 생성할 문서 버전을 선택합니다. 기본적으로 최신 버전이 선택됩니다.

1. **승인** 섹션까지 아래로 스크롤한 다음 **워크플로 만들기**&#x200B;를 클릭합니다.


1. 다음 세부 정보를 입력합니다.

   <table>
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
   <td><strong>기한(선택 사항)</strong></td>
   <td>승인에 대한 기한을 설정하십시오. 사용자와 팀은 지정된 기한으로부터 24시간 전에 이메일로 72시간 전에 알림을 받습니다.</td>
   </tr>
   </table>

1. (선택 사항) 이전 단계를 반복하여 필요에 따라 단계를 더 추가합니다.

   >[!NOTE]
   >
   >여러 단계를 추가하면 승인 워크플로가 단계가 나열된 순서로 진행됩니다. 필요한 모든 결정이 이루어지면 다음 단계가 시작되고 이전 단계가 잠깁니다.

   ![문서 세부 정보](assets/new-stage.png)


## 새 문서 영역의 요약 패널에서 승인 워크플로를 만듭니다.

조직에서 엔터프라이즈 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. 엔터프라이즈 스토리지에 대한 자세한 내용은 [엔터프라이즈 스토리지 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

승인 워크플로우를 만들려면 다음 작업을 수행하십시오.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 문서를 클릭한 다음 페이지 오른쪽에 있는 승인 아이콘을 클릭합니다.

   ![문서 요약에 승인자 추가](assets/approvals-icon-new.png)

1. **워크플로 만들기**&#x200B;를 클릭한 후 다음 세부 정보를 입력하십시오.

   <table>
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
   <td><strong>기한(선택 사항)</strong></td>
   <td>승인에 대한 기한을 설정하십시오. 사용자와 팀은 지정된 기한으로부터 24시간 전에 이메일로 72시간 전에 알림을 받습니다.</td>
   </tr>
   </table>

1. (선택 사항) 이전 단계를 반복하여 필요에 따라 단계를 더 추가합니다.

   >[!NOTE]
   >
   >여러 단계를 추가하면 승인 워크플로가 단계가 나열된 순서로 진행됩니다. 필요한 모든 결정이 이루어지면 다음 단계가 시작되고 이전 단계가 잠깁니다.

   ![문서 세부 정보](assets/new-stage.png)



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
