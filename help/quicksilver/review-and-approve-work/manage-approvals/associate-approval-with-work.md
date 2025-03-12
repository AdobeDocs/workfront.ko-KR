---
product-area: projects
navigation-topic: approvals
title: 신규 또는 기존 승인 프로세스를 작업과 연결
description: 이 문서에서는 승인 프로세스를 작업 항목과 연결하는 방법에 대해 설명합니다. 승인을 증명 또는 문서와 연결하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: e02a593ddca923067eb61f838a7ade17e7fc3652
workflow-type: tm+mt
source-wordcount: '1917'
ht-degree: 0%

---

# 신규 또는 기존 승인 프로세스를 작업과 연결

이 문서에서는 승인 프로세스를 작업 항목과 연결하는 방법에 대해 설명합니다. 승인을 증명 또는 문서와 연결하는 방법에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [자동화된 워크플로로 고급 증명 만들기](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [문서 승인 요청](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

Adobe Workfront에서 글로벌 또는 일회용 승인 프로세스를 작업 항목과 연결할 수 있습니다. 다음과 같은 시나리오가 있습니다.

* 기존 글로벌 승인 프로세스를 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업과 연결합니다. 일부 전역 승인 프로세스는 시스템의 모든 그룹에서 사용할 수 있습니다. 그룹 수준 글로벌 승인 프로세스는 특정 그룹에만 사용할 수 있습니다.
* 일회용 승인 프로세스를 만들고 기존 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업과 연결합니다.

>[!NOTE]
>
>이 문서에서는 &quot;글로벌 승인 프로세스&quot;라는 용어를 사용하여 &quot;일회용 승인 프로세스&quot;와 구분합니다. 글로벌 승인 프로세스를 반복적으로 사용할 수 있습니다.
>
>&quot;그룹 수준 글로벌 승인 프로세스&quot;란 특정 그룹에만 연관된 상태 및 항목에 대해 반복적으로 사용할 수 있는 승인 프로세스를 말합니다.

승인 프로세스에 대한 일반적인 정보는 [승인 프로세스 개요](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)를 참조하십시오.

글로벌 승인 프로세스를 만드는 방법에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>작업 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>프로젝트, 작업, 문제 또는 템플릿에 대한 액세스 이상 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업, 문제 또는 템플릿에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체 </a>에 대한 액세스 요청 을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

+++

## 승인 프로세스를 작업 항목과 연결하는 것에 대한 고려 사항

아래에 설명된 고려 사항 외에 Workfront의 승인 프로세스에 대한 일반적인 고려 사항을 다시 참조하는 것이 좋습니다. 자세한 내용은 [승인 프로세스 개요](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)를 참조하십시오.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* 승인 프로세스를 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업과 연결하려면 먼저 해당 작업을 만들어야 합니다.
* 전달된 상태의 항목에 승인 프로세스를 첨부할 때 현재 항목이 있는 경우 승인 프로세스가 트리거되지 않고 승인자에게 알림이 전송되지 않습니다.

  **예:** 작업이 완료 상태이고 완료 상태와 연결된 승인 프로세스를 첨부하면 승인이 트리거되지 않습니다.

* 항목의 첫 번째 상태에 승인 프로세스를 첨부할 때(작업 및 프로젝트에 대한 템플릿 사용, 문제에 대한 대기열 설정 설정 사용 또는 새 작업에 대한 프로젝트의 작업 설정 정의 사용) 제출된 승인이 회수되면 승인 프로세스가 무시됩니다. 이 경우 승인자는 알림을 받지 않습니다.

  승인 회수에 대한 자세한 내용은 [승인 보기](../../review-and-approve-work/manage-approvals/view-approvals.md)를 참조하십시오.

  >[!TIP]
  >
  >작업 또는 문제의 첫 번째 상태는 신규입니다. 프로젝트의 첫 번째 상태는 시스템의 프로젝트 환경 설정에서 Workfront 관리자가 선택한 상태입니다. 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)을 참조하십시오.

* 승인 프로세스와 오브젝트의 연결은 오브젝트의 업데이트 영역에 기록되지 않습니다.
* 승인 프로세스를 상위 작업과 연결할 수 없습니다.
* 사용자, 팀 또는 역할을 승인자로 추가해도 해당 승인과 연관된 오브젝트에 대한 권한이 자동으로 부여되지 않습니다. 이 사용자는 승인 단계가 트리거될 때 오브젝트에 대한 권한을 받습니다. 그렇지 않으면 승인 결정을 내리기 전에 객체를 공유해야 합니다.

다음 섹션에서는 승인 프로세스를 프로젝트, 작업 또는 문제에 연결하는 다양한 방법에 대해 설명합니다.

## 글로벌 승인 프로세스를 작업 항목과 연결 {#associate-a-global-approval-process-with-a-work-item}

글로벌 승인 프로세스를 작업 항목(프로젝트, 작업, 문제, 템플릿, 템플릿 작업)과 연결할 수 있습니다.

속한 그룹 또는 시스템의 모든 그룹과 공유되는 한 모든 글로벌 승인 프로세스에 액세스할 수 있습니다.

<!--The global approval process must be available to the group associated with the work item or to all groups in the system.-->

>[!NOTE]
>
>템플릿에 프로젝트 승인 프로세스를 첨부하고 템플릿 작업에 작업 승인 프로세스를 첨부할 수 있습니다. 이렇게 하면 누군가가 템플릿을 사용하여 프로젝트를 만들 때 승인 프로세스가 프로젝트 또는 작업 승인 프로세스가 됩니다. 템플릿 또는 템플릿 작업에 연결된 일회성 승인 프로세스는 프로젝트 및 작업에 대한 일회성 승인 프로세스로 유지됩니다.

Workfront 관리자가 시스템의 모든 그룹에 대한 전역 승인 프로세스를 구성하는 방법과 그룹 관리자가 그룹에 대한 승인을 만드는 방법에 대한 자세한 내용은 [작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)를 참조하십시오.

>[!NOTE]
>
>특정 요구 사항에 맞게 글로벌 승인 프로세스를 수정할 수도 있습니다. 자세한 내용은 이 문서의 [특정 개체에서 사용할 전역 승인 프로세스 수정](#modify-a-global-approval-process-for-use-on-a-specific-object) 섹션을 참조하십시오.

기존 글로벌 승인 프로세스를 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업과 연결하려면

1. 승인 프로세스를 연결할 작업 항목으로 이동합니다.
1. 왼쪽 패널에서 **승인**&#x200B;을 클릭합니다.

   **자세히 표시**&#x200B;를 클릭한 다음 **승인**&#x200B;을 클릭해야 할 수 있습니다.

   ![작업에 대한 승인 섹션](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![기존 승인 사용 또는 단일 사용 승인 만들기](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   선택한 승인 프로세스가 표시됩니다.

1. **기존 사용** 드롭다운 메뉴를 확장하고 기존 승인 프로세스를 선택합니다.

   ![승인 메뉴](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   선택한 승인 프로세스가 표시됩니다.

   ![기존 승인이 작업에 첨부됨](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. **저장**&#x200B;을 클릭합니다.
1. (선택 사항) 항목에 첨부한 기존 승인을 수정하려면 승인 프로세스 편집 을 클릭합니다. 이렇게 하면 전역 승인 프로세스가 일회용 승인 프로세스로 변경됩니다. 자세한 내용은 이 문서의 [특정 개체에서 사용할 전역 승인 프로세스 수정](#modify-a-global-approval-process-for-use-on-a-specific-object) 섹션을 참조하십시오.

## 특정 오브젝트에서 사용할 전역 승인 프로세스 수정 {#modify-a-global-approval-process-for-use-on-a-specific-object}

[작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)에 설명된 대로 Workfront 관리자 또는 그룹 관리자가 사용할 전역 승인 프로세스를 만듭니다.

항목에 첨부된 글로벌 승인 프로세스를 수정하는 것은 일회용 승인 프로세스를 수정하는 것과 동일합니다.

연결된 프로젝트, 작업 또는 문제의 특정 요구 사항에 맞게 글로벌 승인 프로세스를 수정할 수 있습니다.

>[!IMPORTANT]
>
>글로벌 승인 프로세스를 수정하면 단일 사용 승인 프로세스가 되어 수정한 객체에서만 사용할 수 있습니다. 글로벌 승인 프로세스는 변경되지 않습니다.
>
>글로벌 승인 프로세스를 수정할 때 다음 제한 사항을 고려하십시오.
>
>* 승인 프로세스를 연관시키는 프로젝트, 작업 또는 문제에 대해서만 승인 프로세스가 수정됩니다.
>* 관리자가 원래 글로벌 승인 프로세스에 대해 변경한 내용은 수정한 글로벌 승인 프로세스를 반영하지 않습니다.
>

항목에 이미 첨부된 승인 프로세스를 수정하려면

1. 프로젝트, 작업 또는 문제에 글로벌 승인 프로세스를 추가합니다.

   지침은 이 문서의 [전역 승인 프로세스를 작업 항목과 연결](#associate-a-global-approval-process-with-a-work-item) 섹션을 참조하십시오.

   >[!IMPORTANT]
   >
   >승인을 추가할 때 **저장**&#x200B;을 클릭해야 합니다.

1. 글로벌 승인 프로세스가 추가되면 승인 페이지의 오른쪽 상단에 있는 **편집**&#x200B;아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다. 이 작업은 전역 또는 그룹 수준의 승인 프로세스를 일회용 승인 프로세스로 전환합니다.
1. 기존 승인 프로세스를 변경합니다. 자세한 내용은 이 문서의 [일회용 승인 프로세스를 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업과 연결](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) 섹션을 참조하십시오.
1. **저장**&#x200B;을 클릭한 다음 **저장**&#x200B;을 다시 클릭하여 전역 승인 프로세스를 이 개체에서만 사용할 수 있는 단일 사용 승인 프로세스로 전환할지 확인합니다.

## 일회용 승인 프로세스를 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업에 연결 {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

특정 프로젝트, 작업 또는 문제에서만 사용할 일회용 승인 프로세스를 만들 수 있습니다.

템플릿에서 만든 프로젝트 및 작업에서 사용할 수 있도록 일회용 승인 프로세스를 템플릿 또는 템플릿 작업과 연결할 수도 있습니다.

>[!NOTE]
>
>단일 사용 승인 프로세스를 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업에 대한 시스템 수준 또는 그룹 수준 상태와 연결할 수 있습니다. Workfront 상태에 대한 자세한 내용은 [상태 만들기 또는 편집](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)을 참조하세요.

이러한 방식으로 승인 프로세스를 만들면 요구 사항에 맞는 사용자 지정 승인 프로세스를 만들 수 있습니다. 그러나 승인 프로세스는 향후에 다른 작업 항목과 연결할 수 없습니다.

또는 특정 품목에 대한 글로벌 승인 프로세스를 수정할 수 있으며 이는 일회용 승인 프로세스가 됩니다. 자세한 내용은 이 문서에서 [특정 개체에 사용할 전역 승인 프로세스 수정](#modify-a-global-approval-process-for-use-on-a-specific-object) 섹션을 참조하십시오.

일회용 승인 프로세스를 만들려면 다음 작업을 수행하십시오.

1. 승인 프로세스를 연결할 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업으로 이동합니다.
1. 왼쪽 패널에서 **승인**&#x200B;을 클릭합니다.

   **자세히 표시** > **승인**&#x200B;을 클릭해야 할 수 있습니다.

   ![작업에 대한 승인 섹션](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. **일회용 만들기**&#x200B;를 클릭합니다.

   ![승인 메뉴](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. 문서 [작업 항목에 대한 승인 프로세스 만들기](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)의 &quot;작업 항목에 대한 시스템 수준 또는 그룹 수준 글로벌 승인 프로세스 만들기&quot; 섹션에서 6단계부터 시작하는 단계를 완료합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >일회용 승인 프로세스를 첨부하면 템플릿 및 템플릿 작업의 편집 상자 안에 있는 승인 프로세스 필드에 &quot;`<Custom>`&quot;(으)로 표시됩니다. 템플릿 또는 템플릿 작업 편집에 대한 자세한 내용은 다음 문서를 참조하십시오.
   >
   >* [프로젝트 템플릿 편집](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   >* [템플릿 작업 편집](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## 작업 항목에서 승인 프로세스 제거 또는 삭제

전역 또는 그룹 수준 승인 프로세스를 제거하거나 이전에 연결된 프로젝트, 작업 또는 문제에서 일회용 승인 프로세스를 삭제할 수 있습니다.

다음과 같은 시나리오가 있습니다. 

* 글로벌 또는 그룹 수준 승인 프로세스를 제거해도 승인이 삭제되지 않습니다. 이 승인은 나중에 사용할 수 있습니다.
* 단일 사용자 승인 프로세스를 삭제하면 Workfront에서 삭제되며 복구할 수 없습니다.

작업 항목에서 승인 프로세스를 제거하거나 삭제하려면

1. 이전에 추가한 승인 프로세스를 제거할 프로젝트, 작업, 문제, 템플릿 또는 템플릿 작업으로 이동합니다.
1. 왼쪽 패널에서 **승인**&#x200B;을 클릭합니다.

   **자세히 표시** > **승인**&#x200B;을 클릭해야 할 수 있습니다.

   ![작업에 대한 승인 섹션](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. 항목과 연결된 승인 유형에 따라 승인 섹션의 오른쪽 상단에 있는 다음 아이콘 중 하나를 클릭합니다.

   * 전역 또는 그룹 수준 승인을 위한 **제거**&#x200B;아이콘 ![제거 아이콘](assets/remove-icon---x-in-circle.png).
   * 일회성 승인을 위한 **삭제**&#x200B;아이콘 ![삭제 아이콘](assets/delete.png).

1. 확인하려면 **제거** 또는 **삭제**&#x200B;를 클릭하세요.

   승인 프로세스가 작업 항목에서 제거됩니다.

## 승인 프로세스를 작업 항목에 자동으로 연결

다음 워크플로우를 사용하여 승인 프로세스를 작업 항목과 자동으로 연결할 수 있습니다.

* 프로젝트 및 작업의 경우 템플릿을 사용하여 승인 프로세스를 연결할 수 있습니다. 템플릿 승인 탭 또는 템플릿 작업 승인 탭에 기존 승인 프로세스를 첨부할 수 있습니다. 기존 승인을 작업 항목과 연결하는 방법에 대한 자세한 내용은 이 문서에서 [전역 승인 프로세스를 작업 항목과 연결](#associate-a-global-approval-process-with-a-work-item)을 참조하십시오.
* 기존 프로젝트에 대한 새 작업의 경우 프로젝트 편집 상자의 작업 설정 영역에서 글로벌 승인 프로세스 또는 그룹 수준 글로벌 승인 프로세스를 연결할 수 있습니다. 자세한 내용은 문서 [프로젝트 편집](../../manage-work/projects/manage-projects/edit-projects.md)의 &quot;작업 설정&quot; 섹션을 참조하십시오.
* 문제의 경우 기존 승인 프로세스를 요청 대기열과 연결하여 프로젝트에 추가된 모든 새 문제와 승인을 연결할 수 있습니다. 요청 큐 구성에 대한 자세한 내용은 [요청 큐 만들기](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하십시오.
