---
product-area: requests
navigation-topic: create-requests
title: Adobe Workfront 요청 만들기 및 제출
description: 계획된 작업은 Adobe Workfront에서 프로젝트 및 작업으로 표시됩니다. 그러나 무작위 요청의 형태로 계획되지 않은 작업이 언제든지 들어올 수 있는 환경에서 작업할 수 있습니다. Workfront은 요청 대기열 을 사용하여 이러한 유형의 환경을 수용하는 워크플로를 제공합니다.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 1%

---

# Adobe Workfront 요청 만들기 및 제출

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

계획된 작업은 Adobe Workfront에서 프로젝트 및 작업으로 표시됩니다. 그러나 요청 형태로 계획되지 않은 작업이 언제든지 들어올 수 있는 환경에서 작업할 수 있습니다. Workfront은 요청 대기열 을 사용하여 이러한 유형의 환경을 수용하는 워크플로를 제공합니다.

요청 대기열에서 요청을 만든 후 완료할 요청을 할당하거나 작업 또는 프로젝트로 전환할 수 있습니다.\
문제를 작업 또는 프로젝트로 전환하는 방법에 대한 자세한 내용은 문서 를 참조하십시오 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

다음과 같은 방법으로 요청을 만들 수 있습니다.

* 이 문서에 설명된 대로 처음부터.
* 초안에서. 자세한 내용은 [초안에서 요청 만들기](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* 기존 요청에서 복사본을 복사하고 제출합니다. 자세한 내용은 [요청 복사 및 제출](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

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
   <td> <p>새로운 기능: 기여자 이상</p>
   또는
   <p>현재: 요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p>  </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 요청 대기열 사용을 위한 사전 요구 사항

Workfront 관리자는 이 기능을 사용하려면 먼저 요청 대기열을 만들어 사용자가 사용할 수 있도록 해야 합니다. 플래너 라이선스를 가지고 있고 프로젝트에 대한 편집 액세스 권한 및 특정 프로젝트에 대한 관리 권한을 가진 사용자는 요청 대기열을 만들 수도 있습니다.

요청 대기열을 만드는 방법에 대한 자세한 내용은 문서를 참조하십시오 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Workfront 관리자는 요청 대기열의 다음 구성 요소를 만들어야 합니다.

* 도움말 요청 대기열로 게시된 현재 상태의 프로젝트.
* 대기열 주제.\
  자세한 내용은 이 문서 를 참조하십시오. [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* 라우팅 규칙.\
  자세한 내용은 이 문서 를 참조하십시오. [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (선택 사항) 주제 그룹.\
  자세한 내용은 이 문서 를 참조하십시오. [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (선택 사항) 사용자 정의 양식을 요청합니다.\
  자세한 내용은 이 문서 를 참조하십시오. [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (선택 사항) 승인 프로세스를 요청합니다.\
  자세한 내용은 이 문서 를 참조하십시오. [작업 항목에 대한 승인 프로세스 만들기](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Workfront 웹 앱에서 요청 만들기 및 초안 생성

Workfront 웹 앱에서 요청을 만들면 Workfront은 요청을 제출하기 전에 초안으로 저장합니다. Workfront은 요청 대기열을 선택하고 해당 정보를 입력하는 즉시 초안을 만듭니다.

요청을 계속 제출하거나, 가능한 한 많은 정보를 작성하고 다른 곳으로 이동하여 나중에 완료할 수 있습니다. Workfront은 초안 폴더에서 시작한 초안 요청을 저장합니다.

>[!IMPORTANT]
>
>초안으로 작업할 때 다음 사항을 고려하십시오.
>
>* Workfront은 서드파티 애플리케이션에서 요청을 제출할 때 초안 요청을 생성하지 않습니다(예: Workfront으로 이메일 전송 또는 다른 애플리케이션을 사용하여 요청 생성). Workfront 웹 앱 외부에서 요청을 제출하면 요청이 제출됨 섹션에 저장됩니다.
>* 요청 대기열의 구조가 변경되면 더 이상 기존 초안에 액세스할 수 없습니다. 예를 들어 대기열 주제를 제거하거나 주제 그룹을 추가하는 경우 저장된 초안에 더 이상 액세스할 수 없습니다.
>

기존 초안에서 요청을 만드는 방법에 대한 자세한 내용은 [초안에서 요청 만들기](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). 요청 초안 삭제에 대한 자세한 내용은 [요청 초안 삭제](../../../manage-work/requests/create-requests/delete-request-draft.md).

Workfront 웹 앱에서 요청을 만들려면 다음 작업을 수행하십시오.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리입니다.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. 클릭  **요청**&#x200B;을 클릭한 다음 을 클릭합니다 **새 요청** 페이지의 오른쪽 상단 모서리에서 을 참조하십시오.

   >[!TIP]
   >
   >* 요청 영역의 섹션에서 새 요청 옵션에 액세스할 수 있습니다.
   >* 문제를 만들 수 있는 액세스 권한이 없는 경우 새 요청 옵션이 흐리게 표시됩니다.

1. (조건부) **요청 유형** 필드를 작성하고 다음 중 하나를 수행합니다.

   * 다음에서 **최근 경로** 섹션에서 요청 대기열을 여는 데 최근에 사용한 경로를 선택합니다. 경로에는 요청 대기열, 주제 그룹 및 최근에 제출한 대기열 주제가 포함됩니다. 기본적으로 마지막 세 개의 경로가 표시됩니다.

     >[!NOTE]
     >
     >Workfront은 사용자가 실제로 요청을 제출한 경우에만 경로를 저장합니다. 초안 요청에 대한 경로는 생성되지 않습니다.

     ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * 다음에서 **요청 대기열** 섹션에서 요청 대기열을 선택합니다.
   * 이전에 액세스한 경로에 속하는 키워드를 입력하여 요청 대기열을 검색합니다.

     예를 들어 &quot;Location&quot;이라는 주제 그룹과 &quot;Remote&quot;라는 대기열 주제가 있는 &quot;Help Desk&quot;라는 요청 대기열이 있는 경우 &quot;remote&quot;를 입력하면 경로의 모든 요소에 &quot;remote&quot;가 포함된 모든 요청 대기열이 표시됩니다.

     >[!TIP]
     >
     >특수 문자가 포함된 이름을 입력하면 문자를 입력하지 않아도 요청 대기열, 대기열 주제 또는 주제 그룹이 표시됩니다.

     ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     사용 가능한 요청 대기열 및 최근 경로 목록은 결과에 강조 표시된 키워드가 포함된 경로만 포함하도록 동적으로 업데이트됩니다.

     검색 결과가 다음 영역 아래에 표시됩니다.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">요청 대기열</td> 
        <td>이름에 키워드가 포함된 요청 큐</td> 
       </tr> 
       <tr> 
        <td role="rowheader">경로 요청</td> 
        <td> <p>요소 이름에 키워드가 포함된 경로(요청 대기열, 주제 그룹, 대기열 주제 포함)</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* 처음 200개의 요청 대기열은 기본적으로 알파벳 순서로 표시됩니다.
   >* 요청 대기열의 이름은 도움말 요청 대기열로 게시된 프로젝트의 이름입니다.
   >* 선택한 요청 대기열로 구성된 프로젝트에 대한 설명이 요청 대기열 이름의 오른쪽에 표시됩니다.
   >   
   >프로젝트를 도움말 요청 대기열로 게시하는 방법에 대한 자세한 내용은 문서 를 참조하십시오 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 다음에서 **새 요청** 양식에서 다음 중 하나를 수행합니다.

   * (조건부) 요청 유형 필드 아래에 표시되는 통지 메시지에서 사용 가능한 초안을 선택합니다.

     이 영역은 초안을 제출하지 않고 이전에 저장한 경우에만 표시됩니다.

     기본적으로 세 개의 다른 대기열 주제의 최신 초안이 표시됩니다.

     ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * 선택한 큐에 새 요청 입력을 시작합니다.

     새 요청에 대한 정보를 입력하고 요청 이름을 제목 필드에 지정한 후 새 초안이 자동으로 초안 섹션에 저장됩니다.

1. (선택 사항) 요청 대기열에 주제 그룹이 포함된 경우 첫 번째 드롭다운 필드에서 주제 그룹의 이름을 선택합니다. 그렇지 않으면 대기열 주제를 선택합니다.

   >[!TIP]
   >
   >주제 그룹 또는 대기열 주제 위로 마우스를 가져가면 오른쪽에 설명 필드가 표시됩니다. 여기에는 주제 그룹 또는 대기열 주제에 대한 추가 정보가 포함되어 있습니다.
   >
   >
   >![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >
   >

   요청 대기열에 최대 10개의 주제 그룹 계층을 구축할 수 있습니다.\
   주제 그룹을 만드는 방법에 대한 자세한 내용은 문서를 참조하십시오 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 대기열 주제 생성에 대한 자세한 내용은 문서를 참조하십시오 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   >
   >초안 또는 이전 경로를 선택한 경우 주제 그룹 및 대기열 주제가 이미 선택되어 있습니다. 필요한 경우 다른 항목을 선택할 수 있습니다.

1. Workfront 관리자가 에서 활성화한 필드에 따라 **새 문제 필드** 의 섹션 **대기열 세부 정보** 프로젝트의 하위 탭에서 새 요청을 실행할 때 다음 필드 중 하나를 찾을 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>제목</strong> </td> 
      <td>요청의 이름을 지정합니다. 필수 필드입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>설명</strong> </td> 
      <td>요청에 대한 설명을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>요청과 관련될 수 있는 URL을 지정하십시오.</p> </td> 
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
      <td> <p>요청에 대한 심각도를 지정하십시오. 심각도는 이 요청이 제시간에 해결되지 않을 경우 작업에 미치는 영향을 정의해야 합니다. 기본 옵션은 다음과 같습니다.</p> 
       <ul> 
        <li>표시용</li> 
        <li>혼란 야기</li> 
        <li>해결 방법이 있는 버그</li> 
        <li>해결 방법이 없는 버그</li> 
        <li>치명적인 오류</li> 
       </ul> <p>시스템 관리자는 심각도 이름을 수정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 담당자</strong> </td> 
      <td>사용자가 요청과 관련된 모든 질문을 처리할 수 있으므로 요청의 기본 연락처는 기본적으로 귀하에게 제공됩니다. 그러나 다른 Workfront 사용자로 변경할 수 있습니다.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>할당</strong> </td> 
      <td> <p><span>요청을 할당해야 하는 활성 사용자, 작업 역할 또는 팀의 이름을 지정합니다.</span> </p> <p>한 팀만 지정할 수 있습니다.</p>

   <p> 요청 대기열이 설정된 방법에 따라 세 가지 리소스 모두 대신 하나 또는 두 가지 유형의 리소스만 요청에 할당할 수 있습니다(예: 사용자에게 요청을 할당할 수 있을 수도 있음).</p>

   <p>라우팅 규칙도 요청 대기열에 연결되어 있으며 자동으로 요청을 다른 유형의 리소스(예: 팀)로 라우팅하는 경우 요청을 제출할 때 수동으로 지정하는 엔티티(사용자)와 라우팅 규칙에 지정된 리소스(팀) 모두에 요청이 할당됩니다. </p>

   <p> 자세한 내용은 다음 문서를 참조하십시오.</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a> <br> </p> </li> 
      </ul> </p>

   <p><span>요청 대기열을 적절한 리소스로 자동으로 라우팅할 수 있도록 라우팅 규칙을 사용하는 것이 좋습니다.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>계획된 시간</strong> </td> 
      <td> <p>이 요청을 완료하는 데 걸리는 시간을 예상합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 시작 일자</strong> </td> 
      <td> <p>이 요청에 대한 작업을 시작해야 하는 날짜를 지정합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 완료 일자</strong> </td> 
      <td>이 요청을 해결할 날짜를 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태</strong> </td> 
      <td>새 요청의 기본 상태는 "신규"입니다. 시스템 관리자가 이 상태의 이름을 변경했을 수 있습니다. 이 드롭다운 메뉴에서 상태를 다른 것으로 변경할 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>문서</strong> </td> 
      <td> <p>요청에 문서를 추가합니다. </p> <p> 요청 대기열을 설정한 방법에 따라 문서 섹션이 사용자 정의 필드의 앞 또는 뒤에 표시될 수 있습니다. </p> <p>Workfront에 업로드하는 문서는 초안 요청에서 24시간 동안 저장됩니다. 그 후에는 초안을 편집하고 제출하기 위해 돌아갈 때 다시 첨부해야 합니다. 다른 드라이브에서 연결된 문서는 초안에 영구적으로 저장됩니다. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) Workfront 관리자가 사용자 정의 양식을 요청 대기열 또는 대기열 주제와 연결한 경우 사용자 정의 양식 내에 필드를 지정합니다.\
   사용자 정의 양식은 모든 Workfront 인스턴스에 대해 다릅니다.
1. (선택 사항 및 조건부) 요청을 입력하는 동안 언제든지 을 클릭합니다. [!UICONTROL **초안 삭제**] 자동으로 생성된 초안을 삭제하려면 이렇게 하면 복구할 수 없는 초안이 삭제됩니다. 초안을 삭제하고 있음을 확인하는 확인 메시지가 표시됩니다.

1. (선택 사항) [!UICONTROL **실행 취소**] 작업을 되돌리고 초안을 유지하려면 확인 메시지에서 을(를) 클릭합니다.

1. 다음 중 하나를 수행하십시오.

   * 클릭 **제출** 요청을 제출할 준비가 되면 요청은 제출됨 섹션에 저장됩니다. 요청 대기열의 라우팅 규칙에 따라 이 요청은 요청 대기열로 지정된 프로젝트가 아닌 다른 프로젝트로 라우팅될 수 있습니다. 라우팅 규칙에 대한 자세한 내용은 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     또는

     클릭 **닫기** 제출할 준비가 되지 않았다면 나중에 다시 와서 완료할 수 있습니다. 요청이 초안 섹션에 저장되었으며, 다음에 이 요청 대기열에 대한 요청을 제출할 때 사용할 수 있습니다.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   요청을 제출하면 초안이 자동으로 삭제되고 복원할 수 없습니다.

   수신 요청 주소 지정에 대한 자세한 내용은 문서 를 참조하십시오. [작업 및 팀 요청 관리](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   제출된 요청 또는 초안 요청 찾기에 대한 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Workfront 외부에서 요청 만들기

새 요청을 제출할 때 요청 대기열에 대한 직접 링크를 공유하고 다른 애플리케이션에 포함할 수 있습니다. 웹 또는 다른 애플리케이션에서 이 링크에 액세스하는 사용자는 활성 Workfront 계정으로 로그인하여 이 큐에 액세스하고 요청을 제출해야 합니다. 자세한 내용은 [요청 대기열에 대한 링크 공유](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Workfront으로 이메일로 요청 만들기

요청 대기열이 이메일을 통해 요청을 수신하도록 설정된 경우 요청을 요청 대기열과 연관된 이메일 주소로 직접 이메일로 보낼 수 있습니다.

이메일의 본문이 요청 설명으로 추가됩니다.

>[!NOTE]
>
>HTML이 Workfront을 입력하면 요청 서식이 제거되지만 서명 및 기존 회신 스레드 컨텐츠는 제거되지 않고 요청 설명에 표시됩니다.

요청 대기열이 이메일을 통해 요청을 수신하도록 하는 방법에 대한 자세한 내용은 을 참조하십시오. [사용자가 문제를 요청 대기열 프로젝트에 이메일로 보낼 수 있도록 설정](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Outlook 클라이언트를 사용하여 요청 만들기

Outlook 클라이언트를 사용하여 요청을 제출할 수 있습니다. 새 요청을 만들거나 이메일을 요청으로 변환할 수 있습니다.

Outlook 클라이언트를 사용하여 요청을 제출하는 방법에 대한 자세한 내용은 문서 를 참조하십시오 [Outlook 이메일에서 Adobe Workfront 요청 만들기](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Workfront 모바일 앱을 사용하여 요청 만들기

스마트폰에서 모바일 앱을 이용하여 요청을 제출할 수 있습니다. 새 요청을 만들어 웹 애플리케이션에서 볼 수 있는 액세스 권한이 있는 요청 대기열로 제출할 수 있습니다.

모바일 앱을 통해 요청을 제출하는 방법에 대한 자세한 내용은 다음 문서의 요청 섹션을 참조하십시오.

* [Android용 Adobe Workfront](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests)
* [iOS용 Adobe Workfront](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## 다른 응용 프로그램에서 요청 만들기

Workfront과 통합된 애플리케이션을 사용하여 요청을 제출할 수 있습니다.

* Workfront과 다른 애플리케이션 간에 사용자 정의 통합을 구축하여 다른 애플리케이션에서 Workfront에 요청을 제출할 수 있습니다.\
  사용자 지정 Workfront 통합에 대한 자세한 내용은 문서 를 참조하십시오 [Adobe Workfront 통합](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* Salesforce용 Workfront 앱을 설치한 경우 Salesforce에서 요청을 제출할 수 있습니다.\
  Salesforce용 Workfront 앱을 사용하여 Salesforce에서 요청을 제출하는 방법에 대한 자세한 내용은 문서를 참조하십시오. [Salesforce 오브젝트에서 Adobe Workfront 요청 제출](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## 제출된 요청 찾기

제출된 요청 또는 초안 요청 찾기에 대한 자세한 내용은 [제출된 요청 찾기](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
