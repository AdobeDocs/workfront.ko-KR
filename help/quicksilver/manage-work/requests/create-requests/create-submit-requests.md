---
product-area: requests
navigation-topic: create-requests
title: Adobe Workfront 요청 만들기 및 제출
description: 계획된 작업은 프로젝트 및 작업으로 Adobe Workfront에 표시됩니다. 그러나 임의의 요청 형태로 계획되지 않은 작업이 언제든지 들어올 수 있는 환경에서 작업할 수 있습니다. Workfront은 요청 큐를 사용하여 이러한 유형의 환경을 수용할 수 있는 워크플로우를 제공합니다.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: b40ade1f1d7a9b81c654a274c5e8c872bf74b180
workflow-type: tm+mt
source-wordcount: '2337'
ht-degree: 2%

---

# Adobe Workfront 요청 만들기 및 제출

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE:&nbsp;If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

계획된 작업은 프로젝트 및 작업으로 Adobe Workfront에 표시됩니다. 그러나 임의의 요청 형태로 계획되지 않은 작업이 언제든지 들어올 수 있는 환경에서 작업할 수 있습니다. Workfront은 요청 큐를 사용하여 이러한 유형의 환경을 수용할 수 있는 워크플로우를 제공합니다. 

요청 큐에서 요청을 만든 후에는 완료할 요청을 할당하거나 작업 또는 프로젝트로 변환할 수 있습니다.\
문제를 작업 또는 프로젝트로 변환하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

다음과 같은 방법으로 요청을 만들 수 있습니다.

* 이 문서에 설명된 대로 처음부터 하십시오.
* 초안에서 자세한 내용은 [초안에서 요청 만들기](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* 기존 요청에서 복사본을 복사하고 제출함으로써 자세한 내용은 [요청 복사 및 제출](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## 액세스 요구 사항

<!--drafted for P&P - replace table: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p>여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오.

## 요청 큐 사용을 위한 사전 요구 사항

Workfront 관리자는 이 기능을 사용하기 전에 요청 큐 를 만들고 사용자가 사용할 수 있도록 해야 합니다. 계획자 라이센스가 있고 프로젝트 편집 및 특정 프로젝트에 대한 관리 권한이 있는 사용자도 요청 큐를 생성할 수 있습니다. 

요청 큐를 만드는 방법에 대한 자세한 내용은 문서를 참조하십시오 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

요청 큐의 다음 구성 요소를 만들어야 합니다.

* 도움말 요청 큐로 게시된 현재 상태의 프로젝트입니다.
* 대기열 주제.\
   자세한 내용은 문서를 참조하십시오 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* 라우팅 규칙.\
   자세한 내용은 문서를 참조하십시오 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (선택 사항) 항목 그룹.\
   자세한 내용은 문서를 참조하십시오 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (선택 사항) 사용자 지정 양식을 요청합니다.\
   자세한 내용은 문서를 참조하십시오 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (선택 사항) 승인 프로세스를 요청합니다.\
   자세한 내용은 문서를 참조하십시오 [작업 항목에 대한 승인 프로세스 생성](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Workfront 웹 앱에서 요청 만들기 및 초안 생성

Workfront 웹 앱에서 요청을 만들면 Workfront에서 요청을 제출하기 전에 초안으로 저장합니다. Workfront은 요청 큐를 선택하고 정보 입력을 시작하는 즉시 초안을 만듭니다.

요청 제출을 계속 하거나, 가능한 한 많은 정보를 완료하고 다른 위치로 이동하여 나중에 완료할 수 있습니다. Workfront은 초안 폴더에서 시작한 초안 요청을 저장합니다.

>[!IMPORTANT]
>
>초안으로 작업할 때 다음 사항을 고려하십시오.
>
>* Workfront은 초안 요청을 Workfront에 이메일이나 다른 애플리케이션을 사용하여 작성하는 것처럼 서드파티 애플리케이션에서 제출할 때 초안 요청을 만들지 않습니다. Workfront 웹 앱 외부에서 요청을 제출하면 요청이 제출됨 섹션에 저장됩니다.
>* 요청 큐의 구조가 변경되는 경우 더 이상 기존 초안에 액세스할 수 없습니다. 예를 들어, 큐 주제가 제거되거나 주제 그룹이 추가된 경우 저장된 초안에 더 이상 액세스할 수 없습니다.
>


기존 초안에서 요청을 만드는 방법에 대한 자세한 내용은 [초안에서 요청 만들기](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). 요청 초안 삭제에 대한 자세한 내용은 [요청 초안 삭제](../../../manage-work/requests/create-requests/delete-request-draft.md).

Workfront 웹 앱에서 요청을 만들려면: 

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단 모서리에서

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. 클릭  **요청**&#x200B;를 클릭한 다음 **새 요청** 페이지의 오른쪽 위 모서리에서 을(를) 클릭합니다.

   >[!TIP]
   >
   >* 요청 영역의 모든 섹션에서 새 요청 옵션에 액세스할 수 있습니다.
   >* 문제를 만들 수 있는 액세스 권한이 없으면 새 요청 옵션이 흐리게 표시됩니다.


1. (조건부) **요청 유형** 필드를 작성하고 다음 중 하나를 수행합니다.

   * 에서 **최근 경로** 섹션에서 최근에 요청 큐를 여는 데 사용한 경로를 선택합니다. 경로에는 최근에 제출한 요청 큐, 항목 그룹 및 큐 항목이 포함되어 있습니다. 기본적으로 마지막 세 경로가 표시됩니다.

      >[!NOTE]
      >
      >Workfront은 실제로 요청을 제출한 경우에만 경로를 저장합니다. 초안 요청에 대한 경로를 만들지 않습니다.

      ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * 에서 **요청 큐** 섹션에서 요청 큐를 선택합니다.
   * 이전에 액세스한 경로에 속하는 키워드를 입력하여 요청 큐를 검색합니다.

      예를 들어 &quot;Help Desk&quot;라는 이름의 항목 그룹 &quot;Location&quot;과 &quot;Remote&quot;라는 큐 항목이 있는 요청 큐가 있는 경우 경로 표시 요소에 &quot;remote&quot;를 입력하고 &quot;remote&quot;를 포함하는 모든 요청 큐를 입력할 수 있습니다.

      >[!TIP]
      >
      >특수 문자가 포함된 이름을 입력하면 문자 입력을 생략해도 요청 큐, 큐 항목 또는 주제 그룹이 표시됩니다.

      ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

      사용 가능한 요청 큐 목록 및 최근 경로는 결과에 강조 표시된 키워드가 포함된 경로만 포함하도록 동적으로 업데이트됩니다.

      검색 결과는 다음 영역 아래에 표시됩니다.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">요청 대기열</td> 
        <td>이름에 키워드를 포함하는 요청 큐</td> 
       </tr> 
       <tr> 
        <td role="rowheader">경로 요청</td> 
        <td> <p>요소 이름에 키워드를 포함하는 경로(요청 큐, 주제 그룹, 큐 주제 포함)</p> </td> 
       </tr> 
      </tbody> 
     </table>
   >[!TIP]
   >
   >* 처음 200개 요청 큐는 기본적으로 알파벳 순서로 표시됩니다.
   >* 요청 큐의 이름은 도움말 요청 큐로 게시된 프로젝트의 이름입니다.
   >* 선택한 요청 큐로 구성된 프로젝트의 설명이 요청 큐 이름의 오른쪽에 표시됩니다.

   >   
   >프로젝트를 도움말 요청 큐로 게시하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 에서 **새 요청** 양식에서 다음 중 하나를 수행합니다.

   * (조건부) 요청 유형 필드 아래에 표시되는 알림 메시지에서 사용 가능한 초안을 선택합니다.

      이 영역은 초안 제출 없이 초안을 저장한 경우에만 표시됩니다.

      세 개의 서로 다른 큐 항목에서 가장 최근 초안 세 개가 기본적으로 표시됩니다.

      ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * 선택한 큐에 새 요청 입력을 시작합니다.

      새 요청에 대한 정보를 입력하고 제목 필드에 요청 이름을 지정한 후 초안 섹션에 새 초안이 자동으로 저장됩니다.

1. (선택 사항) 요청 대기열에 항목 그룹이 포함되어 있는 경우, 첫 번째 드롭다운 필드에서 주제 그룹의 이름을 선택합니다. 그렇지 않으면 대기열 항목을 선택합니다.

   >[!TIP]
   항목 그룹 또는 대기열 항목을 마우스로 가리키면 설명 필드가 오른쪽에 표시됩니다. 여기에는 주제 그룹 또는 큐 주제에 대한 추가 정보가 포함되어 있습니다.
   ![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >

   요청 큐에 최대 10개의 주제 그룹 계층을 구축할 수 있습니다.\
   항목 그룹을 만드는 방법에 대한 자세한 내용은 문서를 참조하십시오 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 큐 항목 만들기에 대한 자세한 내용은 문서를 참조하십시오 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   초안 또는 이전 경로를 선택한 경우 항목 그룹 및 큐 주제가 이미 선택되어 있습니다. 필요한 경우 다른 항목을 선택할 수 있습니다.

1. Workfront 관리자가 활성화한 필드( **새 문제 필드** 섹션 **큐 세부 정보** 하위 탭에서 신규 요청을 실행할 때 다음 필드를 찾을 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>주제</strong> </td> 
      <td>요청 이름을 지정합니다. 필수 필드입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>설명</strong> </td> 
      <td>요청에 대한 설명을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>요청과 관련된 URL을 지정합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>우선 순위</strong> </td> 
      <td> <p>요청에 대한 우선 순위를 지정합니다. 우선 순위는 이 요청이 얼마나 빨리 해결되어야 한다고 생각하는지를 정의해야 합니다. 기본 옵션은 다음과 같습니다. </p> 
       <ul> 
        <li>없음</li> 
        <li>낮음 </li> 
        <li>기본</li> 
        <li>높음</li> 
        <li>긴급</li> 
       </ul> <p>시스템 관리자는 우선 순위 이름을 수정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>심각도</strong> </td> 
      <td> <p>요청의 심각도를 지정합니다. 제시간에 해결되지 않을 경우 심각도는 이 요청이 작업에 미치는 영향을 정의해야 합니다. 기본 옵션은 다음과 같습니다.</p> 
       <ul> 
        <li>표시용</li> 
        <li>혼란 야기</li> 
        <li>해결 방법이 있는 버그</li> 
        <li>해결 방법이 없는 버그</li> 
        <li>치명적인 오류</li> 
       </ul> <p>시스템 관리자는 심각도의 이름을 수정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 담당자</strong> </td> 
      <td>요청과 관련된 모든 질문을 처리할 주요 담당자이므로 요청의 기본 담당자는 기본적으로 사용자에게 표시됩니다. 그러나 다른 Workfront 사용자로 변경할 수 있습니다.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>할당</strong> </td> 
      <td> <p><span>요청을 지정할 활성 사용자, 작업 역할 또는 팀의 이름을 지정합니다.</span> </p> <p>팀을 하나만 지정할 수 있습니다.</p>

   <p> 요청 큐가 설정된 방법에 따라, 세 가지 리소스 대신 하나 또는 두 가지 유형의 리소스만 요청에 할당할 수 있습니다(예를 들어, 사용자에게만 요청을 할당할 수 있을 수 있습니다).</p>

   <p>라우팅 규칙이 요청 대기열에도 연결되어 있고 요청을 다른 리소스 유형(예: 팀)으로 자동 라우팅하는 경우, 요청(사용자)을 실행할 때 수동으로 지정하는 엔티티와 라우팅 규칙에 지정된 리소스(팀)에 모두 요청이 지정됩니다. </p>

   <p> 자세한 내용은 다음 문서를 참조하십시오.</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a> <br> </p> </li> 
      </ul> </p>

   <p><span>요청 대기열에 라우팅 규칙을 사용하여 해당 리소스로 자동 라우팅하는 것이 좋습니다.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>계획된 시간</strong> </td> 
      <td> <p>이 요청을 완료하는 데 걸리는 시간을 예측합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 시작 일자</strong> </td> 
      <td> <p>이 요청에서 작업할 날짜를 지정합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 완료 일자</strong> </td> 
      <td>이 요청을 확인할 날짜를 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태</strong> </td> 
      <td>새 요청의 기본 상태는 "New"입니다. 시스템 관리자가 이 상태의 이름을 변경했을 수 있습니다. 이 드롭다운 메뉴에서 상태를 다른 항목으로 변경할 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>문서</strong> </td> 
      <td> <p>요청에 문서를 추가합니다. </p> <p> 요청 큐의 설정 방식에 따라 문서 섹션이 사용자 지정 필드 전이나 후에 표시될 수 있습니다. </p> <p>Workfront에 업로드하는 문서는 초안 요청에서 24시간 동안 저장됩니다. 그런 다음 돌아가서 초안을 편집하고 제출할 때 다시 첨부해야 합니다. 다른 드라이브에서 연결된 문서는 초안으로 영구적으로 저장됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) Workfront 관리자가 사용자 지정 양식을 요청 큐 또는 큐 항목과 연결된 경우 사용자 지정 양식 내의 필드를 지정합니다.\
   사용자 지정 양식은 모든 Workfront 인스턴스에 대해 다릅니다. 
1. (선택 사항 및 조건부) 요청을 입력하는 동안 언제든지 [!UICONTROL **초안 취소**] 자동으로 만들어지는 초안을 삭제하려면 이렇게 하면 복구할 수 없는 초안이 삭제됩니다. 초안을 삭제하고 있음을 알리는 확인 메시지가 표시됩니다.

1. (선택 사항) [!UICONTROL **실행 취소**] 확인 메시지에서 작업을 되돌리고 초안을 유지합니다.

1. 다음 중 하나를 수행하십시오.

   * 클릭 **제출** 요청을 제출할 준비가 된 경우. 요청이 제출됨 섹션에 저장됩니다. 요청 큐의 라우팅 규칙에 따라 이 요청은 요청 큐로 지정된 프로젝트가 아닌 다른 프로젝트로 라우팅될 수 있습니다. 라우팅 규칙에 대한 자세한 내용은 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      또는

      클릭 **닫기** 아직 제출할 준비가 되지 않았는데 나중에 다시 와서 완료할 수 있습니다. 요청은 초안 섹션에 저장되며, 다음에 이 요청 큐에 대한 요청을 제출할 때 사용할 수 있습니다.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)
   요청을 제출하면 초안이 자동으로 삭제되고 복원할 수 없습니다.

   들어오는 요청 주소 지정에 대한 자세한 내용은 문서를 참조하십시오 [작업 및 팀 요청 관리](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   제출 또는 초안 요청 찾기에 대한 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Workfront 외부에서 요청 만들기

새 요청을 제출하고 다른 애플리케이션에 포함할 때 요청 큐에 대한 직접 링크를 공유할 수 있습니다. 웹 또는 다른 애플리케이션에서 이 링크에 액세스하는 사용자는 활성 Workfront 계정으로 로그인해야 이 큐에 액세스하여 요청을 제출할 수 있습니다. 자세한 내용은 [요청 큐에 대한 링크 공유](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Workfront으로 이메일을 보내어 요청 만들기

이메일을 통해 요청을 수신하도록 요청 큐가 활성화된 경우 요청을 요청 큐와 연결된 전자 메일에 직접 이메일로 보낼 수 있습니다.

이메일의 본문 텍스트가 요청 설명으로 추가됩니다.

>[!NOTE]
요청이 Workfront에 들어가면 HTML 형식이 제거되지만, 서명 및 기존 회신 스레드 콘텐츠는 제거되어 요청 설명에 표시되지 않습니다.

이메일을 통해 요청을 수신하도록 요청 큐를 활성화하는 방법에 대한 자세한 내용은 [사용자가 요청 큐 프로젝트에 문제를 이메일로 보낼 수 있도록 설정](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Outlook 클라이언트를 사용하여 요청 만들기

Outlook 클라이언트를 사용하여 요청을 제출할 수 있습니다. 새 요청을 만들거나 이메일을 요청으로 변환할 수 있습니다. 

Outlook 클라이언트를 사용하여 요청을 제출하는 방법은 문서를 참조하십시오 [Outlook 이메일에서 Adobe Workfront 요청 만들기](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Workfront 모바일 앱을 사용하여 요청 만들기

스마트폰에서 모바일 앱을 사용하여 요청을 제출할 수 있습니다. 새 요청을 만들고 웹 애플리케이션에서 볼 수 있는 액세스 권한이 있는 요청 큐에 제출할 수 있습니다. 

모바일 앱을 통한 요청 제출에 대한 자세한 내용은 다음을 참조하십시오. [요청](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests) 문서의 섹션:

* [Android용 Adobe Workfront](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)
* [Adobe Workfront for iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)

## 다른 응용 프로그램에서 요청 만들기

Workfront과 통합된 모든 애플리케이션을 사용하여 요청을 제출할 수 있습니다. 

* Workfront과 다른 애플리케이션 간에 사용자 지정 통합을 구축하여 다른 애플리케이션에서 Workfront에 요청을 제출할 수 있습니다.\
   사용자 지정 Workfront 통합에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront 통합](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* Salesforce용 Workfront 앱을 설치한 경우 Salesforce에서 요청을 제출할 수 있습니다.\
   Salesforce용 Workfront 앱을 사용하여 Salesforce에서 요청 제출에 대한 자세한 내용은 문서를 참조하십시오 [Salesforce 개체에서 Adobe Workfront 요청 제출](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## 제출된 요청 찾기

제출 또는 초안 요청 찾기에 대한 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
