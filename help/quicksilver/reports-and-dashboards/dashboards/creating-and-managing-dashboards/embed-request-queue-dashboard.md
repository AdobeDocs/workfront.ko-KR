---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 대시보드에 요청 큐 포함
description: 요청 영역으로 이동할 필요 없이 대시보드에 새 요청 큐를 포함하여 요청 큐에 직접 액세스할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# 대시보드에 요청 큐 포함

요청 영역으로 이동할 필요 없이 대시보드에 새 요청 큐를 포함하여 요청 큐에 직접 액세스할 수 있습니다. 

예를 들어, 도움말 데스크 대기열과 같이 전체 조직에 열려 있거나 모든 사람이 정기적으로 액세스해야 하는 PTO 요청 대기열이 있는 경우, 요청 대기열을 해당 대시보드 중 하나에 직접 삽입하여 빠르고 쉽게 액세스할 수 있습니다. 이를 설정하는 프로세스는 대시보드에서 외부 페이지를 만드는 프로세스와 유사합니다.

먼저 요청 큐의 URL을 가져와야 합니다. 둘째, 외부 페이지를 추가하여 URL을 대시보드에 포함할 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이선스*</strong></td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>보고서, 대시보드, 달력에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>대시보드에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

요청 큐를 대시보드에 포함하려면 먼저 다음 두 항목을 모두 만들어야 합니다.

* **대시보드**: 대시보드 만들기에 대한 자세한 내용은 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **요청 큐**: 요청 큐 만들기에 대한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## 요청 큐의 URL 가져오기 {#obtain-the-url-of-the-request-queue}

요청 큐의 URL은 대시보드에서 액세스할 때 사용자에게 노출하려는 요청 큐의 부분에 따라 여러 가지 방법으로 가져올 수 있습니다.

* [요청 유형을 변경할 수 있는 기능을 사용하여 특정 큐 항목에 대한 링크를 가져옵니다](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [요청 큐에 대한 링크 및 요청 유형을 변경하는 기능 가져오기](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [요청 유형을 변경할 수 없는 요청 큐에 대한 링크 가져오기](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### 요청 유형을 변경할 수 있는 기능을 사용하여 특정 큐 항목에 대한 링크를 가져옵니다 {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

특정 큐 항목에 대한 링크를 다른 사용자와 공유하면 요청 양식이 요청을 제출하는 데 필요한 정확한 큐 항목에서 열립니다. 이 기능은 특정 요청 큐에 대한 요청을 로깅할 때 선택할 큐 항목을 사용자가 모를 때 유용합니다.

사용자는 필요한 경우 요청 유형을 변경하거나 다른 항목을 선택할 수 있습니다. 요청 영역의 탐색도 표시됩니다.

1. 을(를) 클릭합니다. **기본 메뉴** > **요청** > **새 요청**.
1. 특정 큐를 공유하려는 경우 대시보드에서 공유할 큐에 도달할 때까지 주제 그룹 및 큐 항목을 계속 선택합니다. 요청 제출에 대한 자세한 내용은 [Adobe Workfront 요청 만들기 및 제출](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >항목 그룹 및 큐 항목을 선택하는 것은 선택 사항입니다.

1. 클릭 **공유 경로** 를 클릭합니다.

   그러면 화면에 표시할 때 요청 큐 또는 큐 항목에 대한 링크가 복사됩니다. 사용자는 요청 유형이나 사용 가능한 항목 그룹 및 대기열 항목을 업데이트할 수 있습니다.

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### 요청 큐에 대한 링크 및 요청 유형을 변경하는 기능 가져오기 {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

요청 유형에 대한 링크를 공유하면 사용자에 대해 요청 유형이 선택됩니다. 이 기능은 사용자가 동일한 요청 유형에 대해 여러 주제 그룹 또는 큐 항목 중에서 선택해야 할 때 유용합니다. 사용자는 요청 유형을 변경하고 다른 유형을 선택할 수 있습니다. 요청 영역의 탐색도 표시됩니다.

1. 요청 큐로 지정된 프로젝트로 이동합니다.

   프로젝트에서 요청 큐 만들기에 대한 자세한 내용을 보려면 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 이동 **큐 세부 정보**.
1. 에서 찾을 코드를 복사합니다. **직접 액세스 URL** 필드.

   코드는 다음과 유사해야 합니다.

   ```
   <samp>https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=</samp>
   ```

   선택한 프로젝트와 연결된 요청 큐에 대한 링크입니다.요청 유형 이 미리 선택됩니다.

   사용자는 필요한 주제 그룹 또는 큐 항목을 선택하거나 다른 요청 유형을 선택할 수 있습니다.

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### 요청 유형을 변경할 수 없는 요청 큐에 대한 링크 가져오기 {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

미리 선택된 요청 유형에 대한 링크를 공유하면 사용자에 대해 요청 유형이 선택되며, 변경할 수 없습니다(흐리게 표시됨). 사용자는 필요한 주제 그룹이나 큐 주제를 선택할 수 있습니다. 이 기능은 사용자가 다른 요청 유형을 보고 선택하지 않도록 할 때 유용합니다. 요청 영역의 탐색이 표시되지 않습니다.

1. 요청 큐로 지정된 프로젝트로 이동합니다.

   프로젝트에서 요청 큐 만들기에 대한 자세한 내용을 보려면 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 이동 **큐 세부 정보**.
1. 에서 찾을 코드를 복사합니다. **포함된 코드** 필드.

   코드는 다음과 유사해야 합니다.

   ```
   <samp><iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe></samp>
   ```

1. 아래 정보만 보존하려면 코드를 편집합니다.

   ```
   <samp>https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71</samp>
   ```

   >[!TIP]
   >
   >을 보존할 수 있습니다 `<samp>iframe </samp>` 태깅 합니다.

   선택한 프로젝트와 연결된 요청 큐에 대한 링크입니다. 요청 유형이 미리 선택되어 있으므로 변경할 수 없습니다.

   사용자는 선택한 요청 유형에 필요한 주제 그룹 또는 큐 항목을 선택할 수 있습니다. 사용자는 다른 요청 유형을 선택할 수 없습니다.

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## 대시보드에 요청 큐 포함

요청 큐 또는 요청 큐 아래에 중첩된 큐 항목에 대한 링크를 대시보드에 포함하여 사용자가 요청 입력에 직접 액세스할 수 있도록 할 수 있습니다.

1. 에 설명된 방법 중 하나를 사용하여 요청 큐 URL을 얻습니다. [요청 큐의 URL 가져오기](#obtain-the-url-of-the-request-queue) 섹션 을 참조하십시오.
1. 을(를) 클릭합니다. **기본 메뉴** > **대시보드** > **새 대시보드**.
1. 입력 **이름** 참조하십시오. 필수 필드입니다.
1. 클릭 **외부 페이지 추가**.

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. 에서 **외부 페이지 추가** 상자에서 다음 필드를 편집합니다.

   * **이름**: 대시보드에 표시할 요청 큐의 이름을 입력합니다. 필수 필드입니다.

   * **설명**: 이 외부 페이지에 표시되는 설명을 입력합니다. 이 필드는 필수 필드가 아니며 보고 목적으로만 중요합니다. 대시보드에 표시되지 않습니다.
   * **URL**: 1단계에서 설명한 방법 중 하나를 사용하여 가져온 URL을 붙여넣습니다.

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **높이**: 외부 페이지의 높이를 입력합니다. 요청 큐가 포함된 외부 페이지가 대시보드에서 차지하는 공간을 정의합니다. 필수 필드이며 기본값은 500입니다.

1. **저장**&#x200B;을 클릭합니다.
1. 클릭 **저장 + 닫기**. 

   요청 큐는 대시보드에 별도의 대시보드 구성 요소로 표시됩니다.

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. (선택 사항) **대시보드 작업**, 그런 다음 **편집** 보고서, 달력 또는 추가 외부 페이지를 동일한 대시보드에 추가하려면\
   대시보드에 구성 요소 추가에 대한 자세한 내용은 [대시보드 만들기](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

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
