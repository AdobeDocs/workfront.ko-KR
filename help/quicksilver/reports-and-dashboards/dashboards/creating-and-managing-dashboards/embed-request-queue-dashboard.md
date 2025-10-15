---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드에 요청 대기열 포함
description: 요청 영역으로 이동할 필요 없이 새 요청 대기열을 대시보드에 포함하여 사용자에게 요청 대기열에 직접 액세스할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 1%

---

# 대시보드에 요청 대기열 포함

<!-- Audited: 1/2025 -->

요청 영역으로 이동할 필요 없이 새 요청 대기열을 대시보드에 포함하여 사용자에게 요청 대기열에 직접 액세스할 수 있습니다.

예를 들어, 헬프 데스크 대기열과 같이 전체 조직에 열려 있는 요청 대기열이나 모든 사용자가 정기적으로 액세스해야 하는 PTO 요청 대기열이 있는 경우, 빠르고 쉽게 액세스할 수 있도록 요청 대기열을 대시보드 중 하나에 직접 삽입하는 것이 편리할 수 있습니다. 이를 설정하는 프로세스는 대시보드에 외부 페이지를 생성하는 프로세스와 유사합니다.

먼저 요청 대기열에 대한 URL을 얻어야 합니다. 두 번째로 외부 페이지를 추가하여 URL을 대시보드에 포함할 수 있습니다.

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
      <p>표준</p>
      <p>플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>대시보드에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.


+++

## 전제 조건

요청 대기열을 대시보드에 포함하려면 먼저 다음 두 가지를 모두 생성해야 합니다.

* **대시보드**: 대시보드를 만드는 방법에 대한 자세한 내용은 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)를 참조하세요.

* **요청 큐**: 요청 큐 만들기에 대한 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하세요.

## 요청 대기열의 URL 가져오기 {#obtain-the-url-of-the-request-queue}

사용자가 대시보드에서 액세스할 때 표시할 요청 대기열의 부분에 따라 여러 가지 방법으로 요청 대기열의 URL을 가져올 수 있습니다.

* [요청 유형을 변경할 수 있는 특정 대기열 주제에 대한 링크를 가져옵니다](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)

* [요청 대기열에 대한 링크 및 요청 유형을 변경할 수 있는 기능을 가져옵니다](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)

* [요청 유형을 변경할 수 없는 요청 대기열에 대한 링크 가져오기](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### 요청 유형을 변경할 수 있는 기능을 가진 특정 대기열 주제에 대한 링크 얻기 {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

특정 대기열 주제에 대한 링크를 다른 사용자와 공유하면 요청을 제출하는 데 사용해야 하는 정확한 대기열 주제에서 요청 양식이 열립니다. 이 기능은 사용자가 특정 요청 대기열에 대한 요청을 기록할 때 선택할 대기열 주제를 모를 수 있는 경우에 유용합니다.

사용자는 요청 유형을 변경하거나 필요한 경우 다른 주제를 선택할 수 있습니다. 요청 영역의 탐색도 표시됩니다.

1. **기본 메뉴** > **요청** > **새 요청**&#x200B;을 클릭합니다.
1. 특정 대기열을 공유하려는 경우 대시보드에서 공유할 대기열에 도달할 때까지 주제 그룹 및 대기열 주제를 계속 선택합니다. 요청 제출에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md)을 참조하십시오.

   >[!TIP]
   >
   >주제 그룹 및 대기열 주제를 선택하는 것은 선택 사항입니다.

1. 새 요청 영역의 오른쪽 상단 모서리에서 **경로 공유**&#x200B;를 클릭합니다.

   화면에 표시할 때 요청 대기열 또는 대기열 주제에 링크가 복사됩니다. 사용자는 요청 유형 또는 사용 가능한 모든 주제 그룹 및 대기열 주제를 업데이트할 수 있습니다.

   ![공유 경로가 있는 요청 큐](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### 요청 대기열에 대한 링크 및 요청 유형 변경 기능 얻기 {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

요청 유형에 대한 링크를 공유할 때 사용자에 대해 요청 유형이 선택됩니다. 이 기능은 사용자가 동일한 요청 유형에 대해 여러 주제 그룹 또는 대기열 주제를 선택해야 할 때 유용합니다. 사용자는 요청 유형을 변경하고 다른 유형을 선택할 수 있습니다. 요청 영역의 탐색도 표시됩니다.

1. 요청 대기열로 지정된 프로젝트로 이동합니다.

   프로젝트에서 요청 대기열을 만드는 방법에 대한 자세한 내용을 보려면 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)(으)로 이동하십시오.

1. **대기열 세부 정보**(으)로 이동합니다.
1. **직접 액세스 URL** 필드에 있는 코드를 복사합니다.

   코드는 다음과 유사해야 합니다.

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   선택한 프로젝트와 연결된 요청 대기열에 대한 링크입니다. 요청 유형이 미리 선택됩니다.

   사용자는 필요한 주제 그룹 또는 대기열 주제를 선택하거나 다른 요청 유형을 선택할 수 있습니다.

   ![요청 큐 URL](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### 요청 유형을 변경할 수 없는 요청 대기열에 대한 링크 가져오기 {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

미리 선택된 요청 유형에 대한 링크를 공유하는 경우 해당 사용자에 대해 요청 유형이 선택되고 변경될 수 없습니다(흐리게 표시됨). 사용자는 필요한 주제 그룹 또는 대기열 주제를 선택할 수 있습니다. 사용자가 다른 요청 유형을 보고 선택하지 않으려는 경우에 유용합니다. 요청 영역의 탐색이 표시되지 않습니다.

1. 요청 대기열로 지정된 프로젝트로 이동합니다.

   프로젝트에서 요청 대기열을 만드는 방법에 대한 자세한 내용을 보려면 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)(으)로 이동하십시오.

1. **대기열 세부 정보**(으)로 이동합니다.
1. **포함된 코드** 필드에 있는 코드를 복사합니다.

   코드는 다음과 유사해야 합니다.

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. 코드를 편집하여 아래 정보만 보존합니다.

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >Workfront 이외의 응용 프로그램에 코드를 포함할 때 `<samp>iframe </samp>` 태그를 추가할 수 있습니다.

   선택한 프로젝트와 연결된 요청 대기열에 대한 링크입니다. 요청 유형은 미리 선택되었으며 변경할 수 없습니다.

   사용자는 선택한 요청 유형에 필요한 주제 그룹 또는 대기열 주제를 선택할 수 있습니다. 사용자가 다른 요청 유형을 선택할 수 없습니다.

   ![요청 큐 코드](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## 대시보드에 요청 대기열 포함

요청 대기열 또는 요청 대기열 아래에 중첩된 대기열 주제에 대한 링크를 대시보드에 포함하여 사용자가 요청 입력에 직접 액세스할 수 있도록 합니다.

1. 이 문서의 [요청 큐의 URL 가져오기](#obtain-the-url-of-the-request-queue) 섹션에 설명된 방법 중 하나를 사용하여 요청 큐 URL을 가져옵니다.

1. **기본 메뉴** > **대시보드** > **새 대시보드**&#x200B;를 클릭합니다.

1. 대시보드에 대한 **이름**&#x200B;을(를) 입력하십시오. 필수 필드입니다.

1. **외부 페이지 추가**&#x200B;를 클릭합니다.

   ![외부 페이지](assets/add-external-page-highlighted---nwe-350x214.png)

1. **외부 페이지 추가** 상자에서 다음 필드를 편집합니다.

   * **이름**: 대시보드에 표시할 요청 대기열의 이름을 입력하십시오. 필수 필드입니다.

   * **설명**: 이 외부 페이지에 표시할 설명을 입력하십시오. 이 필드는 필수 필드가 아니며 보고용으로만 중요합니다. 대시보드에 표시되지 않습니다.

   * **URL**: 1단계에서 설명한 방법 중 하나를 사용하여 얻은 URL을 붙여 넣습니다.

   * **높이**: 외부 페이지의 높이를 입력하십시오. 요청 대기열이 포함된 외부 페이지가 대시보드에서 차지하는 공간을 정의합니다. 필수 필드이며 기본값은 500입니다.

1. **저장**&#x200B;을 클릭합니다.

1. **저장 및 닫기**&#x200B;를 클릭합니다.

   요청 대기열은 대시보드에 별도의 대시보드 구성 요소로 표시됩니다.

1. (선택 사항) **대시보드 작업**&#x200B;을 클릭한 다음 **편집**&#x200B;을 클릭하여 보고서, 캘린더 또는 추가 외부 페이지를 동일한 대시보드에 추가합니다.

   대시보드에 구성 요소를 추가하는 방법에 대한 자세한 내용은 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)를 참조하십시오.

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
