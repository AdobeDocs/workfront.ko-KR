---
product-area: documents
navigation-topic: approvals
title: 그룹화된 승인 검토
description: 홈 또는 Frame.io 뷰어의 내 승인 위젯에서 그룹화된 승인으로 모든 문서를 검토하고 결정할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: e62ae215bcc7ea42701d6eb92cf43f531a6afc0d
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 3%
---

# 그룹화된 승인 검토

그룹화된 승인에 할당되면 그룹의 모든 문서가 함께 표시되므로 각 문서에 대해 결정을 내릴 수 있습니다. 모든 문서에 대해 한 번에 승인 또는 변경을 요청하거나 각 문서에 대해 개별적으로 결정을 내릴 수 있습니다.

하나 이상의 문서가 여러 단계로 그룹화된 승인에서 **작업 필요**&#x200B;로 표시된 경우 그룹의 모든 문서에 승인된 결정이 있을 때까지 그룹이 다음 단계로 이동할 수 없습니다. 자세한 내용은 [여러 단계로 그룹화된 승인 중 단일 문서에 대한 &quot;작업 필요&quot; 결정 해결](#resolve-a-needs-work-decision-on-a-single-document-in-a-multi-stage-grouped-approval)을 참조하십시오.



>[!IMPORTANT]
>
>조직에서 Adobe 클라우드 스토리지를 사용하는 경우 Workfront의 문서에 액세스할 때 새 문서 영역이 표시됩니다. 그룹화된 승인은 새 문서 영역에서만 사용할 수 있습니다. Adobe 클라우드 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 패키지</td>
   <td> <p>Adobe 클라우드 스토리지를 사용하여 승인을 관리하는 모든 워크플로우 패키지</p> </td>
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
   <td> <p>승인과 연관된 객체에 대한 보기 이상의 액세스 권한</p></td>
  </tr>
  <tr>
   <td role="rowheader">개체 권한</td>
   <td> <p>승인과 연관된 오브젝트에 대한 이상 권한 보기</p></td>
  </tr>
 </tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 홈의 내 승인 위젯에서 그룹화된 승인 검토

홈의 내 승인 위젯은 모든 문서를 함께 처리할 수 있도록 문서를 하나의 승인으로 그룹화합니다.

>[!NOTE]
>
>홈 페이지에 내 승인 위젯을 추가해야 할 수 있습니다. 자세한 내용은 [홈에서 위젯 추가, 편집 또는 제거](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)를 참조하세요.

1. Adobe Workfront의 왼쪽 위 모서리에 있는 **홈** 아이콘을 클릭한 다음 **내 승인** 위젯을 찾습니다.

1. 그룹화된 승인을 엽니다. 그룹의 모든 문서가 함께 나열되며 그룹의 항목 수가 맨 위에 표시됩니다.

1. 다음 중 하나를 사용하여 결정을 내립니다.

   * **모두 승인됨으로 표시**: 그룹의 모든 문서에 대해 승인된 결정을 한 번에 기록합니다.
   * **모든 작업 필요 표시**: 그룹의 모든 문서에 대한 작업 필요 결정을 한 번에 기록합니다.
   * **의사 결정**: 단일 문서에 대해 개별적으로 결정 별도로 결정하려는 각 문서에 대해 이 작업을 반복합니다.


   ![내 승인 위젯이 승인 그룹화됨](assets/my-approvals-group.png)

## Frame.io 뷰어에서 그룹화된 승인 검토

Frame.io 뷰어에는 그룹의 모든 문서가 함께 표시되므로 각 문서를 빠르게 결정하거나 문서를 열어 자세히 검토할 수 있습니다.

1. 검토 전자 메일 알림으로 이동하여 **검토로 이동**&#x200B;을 클릭하거나 홈의 **내 승인** 위젯에서 그룹화된 승인을 엽니다.

1. 다음 중 하나를 수행하십시오.

   * 그룹 페이지에서 문서를 열지 않고 직접 각 문서에 대해 빠른 결정을 내릴 수 있습니다.
   * 문서를 클릭하여 열고 주석 또는 마크업을 추가한 다음 화살표를 사용하여 그룹의 다음 문서로 이동합니다. 문서 카운터(예: **1/2**)는 그룹의 위치를 표시합니다.

   Frame.io 뷰어의 주석 달기 및 마크업에 대한 자세한 내용은 [Frame.io 뷰어로 검토 및 승인](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)을 참조하십시오.

1. 각 문서에 대한 결정 선택:

   * **승인됨**: 문서를 변경할 필요가 없으며 사용할 준비가 되었습니다.
   * **작업 필요**: 문서를 변경해야 하며 사용할 준비가 되지 않았습니다.

   결정에 대한 자세한 내용은 [문서 결정 상태 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)를 참조하십시오.

   ![frame.io 뷰어가 그룹화된 승인](assets/frame-group-approval.png)

## 추가 리소스

이 문서에서는 문서 그룹 검토에 대한 정보를 다룹니다. 단일 문서에 대한 의사 결정, 마크업 추가 등에 대한 자세한 내용은

* [Workfront에서 문서 승인](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/approve-a-document.md)
* [Workfront에서 문서 검토](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-a-document.md)
* [Frame.io 뷰어로 검토 및 승인](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)