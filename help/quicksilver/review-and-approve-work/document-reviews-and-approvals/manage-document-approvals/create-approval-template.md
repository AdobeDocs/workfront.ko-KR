---
product-area: documents
navigation-topic: approvals
title: 문서에 대한 승인 워크플로 템플릿 만들기
description: 승인 템플릿을 만들어 승인 프로세스를 간소화할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
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
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 684
ht-degree: 2%

---

# 문서에 대한 승인 워크플로 템플릿 만들기

Workfront 설정 영역에서 Standard 라이선스를 가진 사용자는 재사용 가능한 승인 템플릿을 만들 수 있습니다. 승인 템플릿을 만들면 오브젝트의 문서 영역에 있는 에셋에 적용할 수 있습니다.
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
   <td><p>기존 Workfront 스토리지를 사용하여 승인을 관리하는 모든 Workfront 패키지</p>
<p>Adobe 클라우드 스토리지를 사용하여 승인을 관리하는 모든 워크플로우 패키지</p> </td> 
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

<!--
## Create an Approval Template in Production

{{step-1-to-setup}}

1. In the left panel, click **Review and Approval** > **Approval Templates**.
1. Click **New Template** on the right side of the page. 

1. Fill in the following details:

   <table>
     <tr>
   <td><strong>Template name</strong></td>
   <td>Add a template name. </td>
   </tr>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Workdays until due date</strong></td>
   <td>Choose how many workdays until the approval is due after a stage is activated.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)
    
1. Click **Save**.

Once the template is created, it can be applied to documents in the Documents area of an object to begin the formal review and approval process in Workfront.
-->

## 승인 템플릿 만들기

승인 템플릿 대화 상자는 항상 고급 모드에서 열립니다. 템플릿에 대한 기본 모드는 없습니다. 템플릿에서 최대 30개의 병렬 경로를 구성하고 총 100개의 단계를 포함할 수 있습니다. 각 경로는 독립적으로 실행되며 하나 이상의 순차적 단계를 포함할 수 있습니다.

승인 템플릿을 만들려면 다음 작업을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **검토 및 승인** > **승인 템플릿**&#x200B;을 클릭합니다.

1. 페이지 오른쪽에서 **새 템플릿**&#x200B;을 클릭합니다.

1. **템플릿 이름**&#x200B;을(를) 추가합니다.

1. 경로 1의 단계 1에 대한 세부 정보 입력:

   <table>
   <tr>
   <td><strong>단계 이름</strong></td>
   <td>단계 이름은 기본적으로 <em>단계 1</em>, <em>단계 2</em> 등으로 지정됩니다. <em>초기 검토</em> 또는 <em>최종 승인</em>과 같이 보다 설명적인 단계로 단계 이름을 바꾸십시오.</td>
   </tr>
   <tr>
   <td><strong>이름 또는 이메일 추가(선택 사항)</strong></td>
   <td>승인자 또는 검토자로 추가할 사용자 또는 팀 이름을 입력하십시오. 템플릿에서 참가자는 선택 사항입니다. 문서에 템플릿을 적용할 때 추가할 수 있습니다.<p>참고: 검토자 또는 승인자는 동일한 에셋에서 한 번에 하나의 진행 단계에만 할당할 수 있습니다. 여러 병렬 단계가 동시에 열려 있는 경우 동일한 사람을 둘 이상의 단계에 추가할 수 없습니다.</p></td>
   </tr>
   <tr>
   <td><strong>필요한 결정은 단 하나입니다(선택 사항).</strong></td>
   <td>가장 먼저 결정을 내리는 사람이 단계를 완료합니다.</td>
   </tr>
   <tr>
   <td><strong>기한까지 근무일(선택 사항)</strong></td>
   <td>스테이지가 열린 후 완료되는 데 소요되는 작업일 수를 선택합니다. 각 경로의 첫 번째 단계도 절대 기한을 지원합니다. 경로의 각 후속 스테이지는 상대적 기한만 지원합니다.</td>
   </tr>
   <tr>
   <td><strong>사용자 지정 메시지 추가(선택 사항)</strong></td>
   <td><strong>사용자 지정 메시지 추가</strong> 텍스트 상자에 메시지를 입력하십시오. 템플릿이 문서에 적용되면 메시지가 승인 이메일 알림과 Workfront의 승인 탭에 표시됩니다.<p>두 번째 단계를 추가하면 기본적으로 <strong>모든 단계에서 이 메시지 표시</strong>가 선택됩니다. 모든 단계에서 동일한 메시지를 사용하도록 선택한 상태로 둡니다. 각 단계에 대해 다른 메시지를 사용하려면 <strong>모든 단계에서 이 메시지 표시</strong>의 선택을 취소한 다음 각 단계의 <strong>사용자 지정 메시지 추가</strong> 텍스트 상자에 단계별 메시지를 입력하십시오.</p></td>
   </tr>
   </table>

   ![단계 추가](assets/add-stage.png)

1. (선택 사항) 경로에 다른 단계를 추가하려면 **단계 추가**&#x200B;를 클릭합니다. 경로 내의 단계는 나열된 순서대로 순차적으로 실행됩니다. 단계의 모든 필수 결정이 이루어지면 해당 경로의 다음 단계가 시작되고 이전 단계가 잠깁니다. 한 경로에서 다른 경로로 단계를 이동할 수는 없지만 경로 내의 단계를 재정렬할 수는 있습니다. 각 경로에는 서로 다른 스테이지 수가 있을 수 있습니다.

1. (선택 사항) **병렬 경로**&#x200B;에서 **경로 추가**&#x200B;를 클릭하여 다른 경로를 추가합니다. 새 경로는 하나의 빈 단계로 시작하여 선택한 경로가 됩니다. 경로의 순서를 변경할 수 없습니다.

   ![병렬 경로 추가](assets/add-path.png)

1. (선택 사항) 경로의 이름을 바꾸려면 경로 레이블을 마우스로 가리키고 연필 아이콘을 클릭한 다음 새 이름을 입력합니다. 경로를 제거하려면 경로 레이블을 마우스로 가리킨 다음 휴지통 아이콘을 클릭합니다. **경로 1**&#x200B;을(를) 제거할 수 없으며 경로 내의 단계가 잠겨 있거나 완료된 경우에만 다른 경로를 제거할 수 있습니다.

1. (선택 사항) 모든 경로와 단계를 지우고 다시 시작하려면 오른쪽 상단의 **재설정**&#x200B;을 클릭합니다.

1. **저장**&#x200B;을 클릭합니다.

템플릿이 생성되면 객체의 문서 영역에 있는 문서에 적용하여 Workfront에서 공식 검토 및 승인 프로세스를 시작할 수 있습니다.

<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
