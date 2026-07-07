---
product-area: documents
navigation-topic: approvals
title: 문서 승인 워크플로에 추가 승인자 또는 검토자 추가
description: 이미 보류 중인 승인이 있는 문서에 승인자 또는 검토자를 추가할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 82530b9b87f6865ec294adcdc601443ee48dcbcf
workflow-type: tm+mt
source-wordcount: 1130
ht-degree: 1%

---

# 문서 승인 워크플로에 추가 승인자 또는 검토자 추가

{{highlighted-preview}}

이미 보류 중인 승인이 있는 문서 승인 워크플로에 추가 승인자 또는 검토자를 추가할 수 있습니다.

>[!IMPORTANT]
>
>이 문서의 내용은 특정 계정에만 사용할 수 있는 업데이트된 문서 승인 기능에 적용됩니다. 표준 승인 프로세스에 대한 자세한 내용은 [작업 승인](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)에 나열된 문서를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>기존 Workfront 스토리지를 사용하여 승인을 관리하는 모든 Workfront 패키지</p>
<p>Adobe 클라우드 스토리지를 사용하여 승인을 관리하는 모든 워크플로우 패키지</p> </td> 
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
   <td> <p>프로젝트, 작업, 문제, 템플릿, 포트폴리오, 프로그램, 보고서, 대시보드, 캘린더 및 문서에 대한 보기 또는 상위 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>요청 액세스 또는 승인과 연관된 객체에 대한 액세스 권한 이상 보기 </p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++



## 프로덕션의 레거시 문서 영역에 승인자 또는 검토자를 추가합니다.

조직이 Workfront 스토리지에 있는 경우 Workfront의 문서에 액세스할 때 기존 문서 영역이 표시됩니다. Workfront 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소와 레거시 Workfront 저장소 간의 차이점](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)을 참조하십시오.

문서 요약에서 승인자 또는 검토자를 추가하려면

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 필요한 문서를 클릭하면 해당 문서에 대한 문서 요약 패널이 열립니다.

1. 버전 드롭다운 메뉴에서 승인자 또는 검토자를 추가하려는 문서 버전을 선택합니다. 기본적으로 최신 버전이 선택됩니다.

1. **승인** 섹션까지 아래로 스크롤한 다음 **워크플로 편집**&#x200B;을 클릭합니다.

   ![승인 워크플로 편집](assets/edit-approval-in-legacy.png)

1. 승인자 또는 검토자를 추가할 단계를 찾은 다음 텍스트 상자에 사용자 이름 또는 이메일을 추가합니다. 필요한 경우 전체 팀을 추가할 수도 있습니다.

1. 해당 이름이 추가되면 승인자 또는 검토자인지 여부를 선택합니다.

   ![승인자 또는 검토자 드롭다운](assets/choose-approver-or-reviewer.png)

1. 5-6단계를 반복하여 승인자 또는 검토자를 추가합니다.저장하면 추가된 참가자에게 문서에 대한 승인 또는 검토가 필요하다는 이메일 알림이 전송됩니다.

<div class="preview">

## 미리보기의 기존 문서 영역에 승인자 또는 검토자를 추가합니다.

조직이 Workfront 스토리지에 있는 경우 Workfront의 문서에 액세스할 때 기존 문서 영역이 표시됩니다. Workfront 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소와 레거시 Workfront 저장소 간의 차이점](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)을 참조하십시오.

문서 요약에서 승인자 또는 검토자를 추가하려면

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 필요한 문서를 클릭합니다. 해당 문서에 대한 문서 요약 패널이 열립니다.

1. 버전 드롭다운 메뉴에서 승인자 또는 검토자를 추가하려는 문서 버전을 선택합니다. 기본적으로 최신 버전이 선택됩니다.

1. **승인** 섹션까지 아래로 스크롤한 다음 **워크플로 편집**&#x200B;을 클릭합니다. 승인이 마지막으로 저장된 모드(단일 단계 승인의 경우 기본, 병렬 경로가 있는 다단계 승인 및 승인의 경우 고급)로 승인 요청 대화 상자가 열립니다.

1. 사용자, 팀 또는 이메일 추가:

   * 기본 모드에서 **이름 또는 전자 메일 추가** 필드에 이름 또는 전자 메일을 입력합니다.
   * 고급 모드에서 업데이트할 단계를 포함하는 경로를 선택한 다음 단계의 **이름 또는 전자 메일 추가** 필드에 이름 또는 전자 메일을 입력합니다.

1. 추가한 각 사용자에 대해 승인자인지 검토자인지 선택합니다.

   ![승인자 또는 검토자 드롭다운](assets/choose-reviewer-or-approver.png)

1. **저장**&#x200B;을 클릭합니다. 추가한 참가자에게는 문서에 대한 승인 또는 검토가 필요하다는 이메일 알림이 전송됩니다.

>[!TIP]
>
>기본 모드 승인을 다중 단계 또는 다중 경로 승인으로 다시 구성하려면 오른쪽 상단의 **고급으로 이동**&#x200B;을 클릭합니다. 기존 참가자는 경로 1, 단계 1로 유지됩니다. 저장한 후에는 다시 기본 모드로 전환할 수 없습니다. 자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

</div>

## 프로덕션의 새 문서 영역에 추가 승인자 또는 검토자 추가

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. Adobe 클라우드 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.


1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 문서를 클릭한 다음 페이지 오른쪽의 **승인** 아이콘을 클릭합니다.

   ![문서 요약에 승인자 추가](assets/approvals-icon-new.png)


1. **워크플로 편집**&#x200B;을 클릭합니다.

1. 승인자 또는 검토자를 추가할 단계를 찾은 다음 텍스트 상자에 사용자 이름 또는 이메일을 추가합니다. 필요한 경우 전체 팀을 추가할 수도 있습니다.

1. 해당 이름이 추가되면 승인자 또는 검토자인지 여부를 선택합니다.

   ![승인자 또는 검토자 드롭다운](assets/choose-approver-or-reviewer.png)

1. 5-6단계를 반복하여 승인자 또는 검토자를 추가합니다.저장하면 추가된 참가자에게 문서에 대한 승인 또는 검토가 필요하다는 이메일 알림이 전송됩니다.

<div class="preview">

## 미리보기의 새 문서 영역에 있는 문서 요약에서 승인자 또는 검토자를 추가합니다.

조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. Adobe 클라우드 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

문서 요약에서 승인자 또는 검토자를 추가하려면

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 문서를 클릭한 다음 페이지 오른쪽의 **승인** 아이콘을 클릭합니다.

   ![문서 요약에 승인자 추가](assets/approvals-icon-new.png)

1. **워크플로 편집**&#x200B;을 클릭합니다. 승인이 마지막으로 저장된 모드(단일 단계 승인의 경우 기본, 병렬 경로가 있는 다단계 승인 및 승인의 경우 고급)로 승인 요청 대화 상자가 열립니다.

1. 사용자, 팀 또는 이메일 추가:

   * 기본 모드에서 **이름 또는 전자 메일 추가** 필드에 이름 또는 전자 메일을 입력합니다.
   * 고급 모드에서 업데이트할 단계를 포함하는 경로를 선택한 다음 단계의 **이름 또는 전자 메일 추가** 필드에 이름 또는 전자 메일을 입력합니다.

1. 추가한 각 사용자에 대해 승인자인지 검토자인지 선택합니다.

   ![승인자 또는 검토자 드롭다운](assets/choose-reviewer-or-approver.png)

1. **저장**&#x200B;을 클릭합니다. 추가한 참가자에게는 문서에 대한 승인 또는 검토가 필요하다는 이메일 알림이 전송됩니다.

>[!TIP]
>
>기본 모드 승인을 다중 단계 또는 다중 경로 승인으로 다시 구성하려면 오른쪽 상단의 **고급으로 이동**&#x200B;을 클릭합니다. 기존 참가자는 경로 1, 단계 1로 유지됩니다. 저장한 후에는 다시 기본 모드로 전환할 수 없습니다. 자세한 내용은 [문서 승인 워크플로 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)를 참조하십시오.

</div>