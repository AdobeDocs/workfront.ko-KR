---
product-area: documents
navigation-topic: approvals
title: 새 문서 버전 업로드 및 승인 요청
description: 새 문서 버전을 업로드하고 Adobe Workfront의 다른 사용자에게 승인을 요청할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 2%

---

# 새 문서 버전 업로드 및 승인 요청

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

이전 검토에서 문서가 &quot;작업 필요&quot;로 표시되어 있는 경우, 원본 문서에 새 버전을 업로드하고 다른 버전의 승인을 시작할 수 있습니다. 새 버전의 문서를 업로드하면 이전 버전이 잠깁니다.

새 버전의 파일 이름이 이전 버전의 파일 이름과 다른 경우 Workfront에 새 파일 이름으로 문서가 표시됩니다.

미결 승인이 있는 문서에 새 버전을 추가하면 이전 버전의 승인이 &quot;철회됨&quot;으로 표시됩니다. 일부 참가자가 아직 결정을 내리지 않았더라도 기존 승인 절차는 종료된다.

최신 문서 버전을 삭제하면 이전 버전이 잠긴 상태로 유지됩니다. 이전 버전을 편집해야 하는 경우 수동으로 잠금을 해제해야 합니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>요청 이상</p>
   <p>기여자 이상</p>
   <p>Frame.io 통합을 사용하는 경우 승인 워크플로를 만들려면 표준 라이선스가 있어야 합니다.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문서와 연관된 객체에 대한 액세스 편집</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 드래그 앤 드롭을 사용하여 프로덕션 환경에 새 버전을 추가합니다.

>[!NOTE]
>
>드래그 앤 드롭은 Internet Explorer에서 작동하지 않습니다.


문서에 대한 또 다른 검토 및 승인이 필요한 경우 Workfront에서 새 문서 버전을 만들 수 있습니다.

이전 참여자, 새 참여자 또는 두 가지 모두를 혼합하여 추가할 수 있습니다. 문서 세부 정보 페이지에서 이전 버전 및 참여자에 대한 정보를 볼 수 있습니다.

새 버전을 추가하려면 다음을 수행하십시오.

1. Workfront의 문서로 이동합니다.
1. 이전 문서 위에 새 파일을 끌어다 놓습니다. 이렇게 하면 새 버전이 자동으로 만들어집니다.

1. 문서 업로드가 완료되면 문서를 선택한 다음 **문서 세부 정보**&#x200B;를 클릭합니다.
   ![문서 세부 정보 페이지 열기](assets/open-doc-details.png)


1. 왼쪽 패널에서 **승인**&#x200B;을 클릭한 다음 **추가**&#x200B;를 클릭합니다.

1. 모든 이전 참가자를 추가하려면 **모두 추가**&#x200B;를 클릭하세요. 필요에 따라 새 참여자를 추가하거나 이전 참여자를 제거할 수도 있습니다.


1. 기존 승인 템플릿을 추가하려면 템플릿 버튼을 클릭하고 템플릿 이름을 입력하십시오.

   >[!TIP]
   >
   >   표준 라이선스가 있는 사용자는 설정 영역에서 재사용 가능한 승인 템플릿을 만들 수 있습니다. 자세한 내용은 [문서에 대한 승인 워크플로 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)를 참조하십시오.


1. (선택 사항) 승인 기한을 설정합니다. 사용자와 팀은 지정된 기한 24시간 전에 이메일로 72시간 전에 알림을 받습니다.

1. 모든 검토자와 승인자를 추가했으면 **요청 제출**&#x200B;을 클릭합니다. 참가자에게는 이메일을 통해 알림이 전송됩니다.

   ![승인을 위해 새 버전을 제출](assets/add-previous-participants.png)





<div class="preview">

## 드래그 앤 드롭을 사용하여 이전 문서 영역의 미리보기 환경에 새 버전을 추가합니다

조직이 Workfront 스토리지에 있는 경우 Workfront의 문서에 액세스할 때 기존 문서 영역이 표시됩니다. Workfront 스토리지에 대한 자세한 내용은 [Workfront 스토리지와 Adobe 엔터프라이즈 스토리지 비교](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)를 참조하십시오.

>[!NOTE]
>
>드래그 앤 드롭은 Internet Explorer에서 작동하지 않습니다.


문서에 대한 또 다른 검토 및 승인이 필요한 경우 Workfront에서 새 문서 버전을 만들 수 있습니다.

이전 참여자, 새 참여자 또는 두 가지 모두를 혼합하여 추가할 수 있습니다. 문서 세부 정보 페이지에서 이전 버전 및 참여자에 대한 정보를 볼 수 있습니다.

새 버전을 추가하려면 다음을 수행하십시오.

1. Workfront의 문서로 이동합니다.
1. 이전 문서 위에 새 파일을 끌어다 놓습니다. 이렇게 하면 새 버전이 자동으로 만들어집니다.

1. 문서 업로드가 완료되면 문서를 선택하여 문서 요약 패널을 엽니다. 여기에서는 패널 상단에 버전 번호가 표시됩니다.
   ![문서 세부 정보 페이지 열기](assets/open-doc-details.png)


1. 아래로 스크롤하여 **승인** 섹션으로 이동합니다.

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



1. (선택 사항) 기존 승인 템플릿을 추가하려면 대화 상자의 왼쪽에서 템플릿을 선택합니다.

   >[!TIP]
   >
   >   표준 라이선스가 있는 사용자는 설정 영역에서 재사용 가능한 승인 템플릿을 만들 수 있습니다. 자세한 내용은 [문서에 대한 승인 워크플로 템플릿 만들기](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)를 참조하십시오.



1. 필요한 단계 및 참가자를 모두 추가했으면 **승인 요청**&#x200B;을 클릭합니다.

   승인 워크플로가 시작되고 승인자는 새 문서 버전에 대한 승인이 필요하다는 알림을 받습니다. 이전 문서 버전이 잠기고 이전 버전에서 미결 승인이 철회됩니다.

   ![승인 요청](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->



</div>

