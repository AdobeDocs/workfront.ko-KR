---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 요청 큐 만들기
description: 프로젝트에서 작업하지 않을 경우에 따라 요청을 입력할 수 있는 요청 큐를 설정할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '2551'
ht-degree: 2%

---

# 요청 큐 만들기

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

프로젝트에서 작업하지 않을 경우에 따라 요청을 입력할 수 있는 요청 큐를 설정할 수 있습니다. 예를 들어, IT 부서의 모든 사용자 요청을 캡처하도록 헬프데스크 요청 큐를 설정할 수 있습니다.

## 액세스 요구 사항

<!--drafted for P&P: replace the table below with this:

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
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
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
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 플랜, 라이선스 유형 또는 액세스를 알아보려면 Workfront 관리자에게 문의하십시오

## 요청 큐 개요

요청 큐를 프로젝트로 설정합니다. 프로젝트를 요청 큐로 지정하면 Adobe Workfront의 요청 영역에서 큐에 액세스할 수 있습니다. 요청 큐를 사용자 지정할 때 사용자가 요청을 제출할 때 작성하는 양식을 사용자 지정할 수도 있습니다.

이 문서에서는 기존 프로젝트에서 요청 큐를 만드는 방법을 설명합니다. 하지만 보고 및 관리를 위해 요청 수집 프로세스에 대한 일관성을 작성하거나 여러 레이어를 요청 대기열에 추가하려면 다음 표에 설명된 요청 큐의 추가 구성 블록을 구성할 수도 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">대기열 세부 정보</td> 
   <td> <p>큐 세부 정보 영역에서 프로젝트를 요청 큐로 설정해야 합니다. 이 단계는 필수입니다. </p> <p>자세한 내용은 <a href="#create-a-request-queue" class="MCXref xref">요청 큐 만들기</a> 섹션에 자세히 설명되어 있습니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">주제 그룹</td> 
   <td> <p>일반적인 기능을 기반으로 요청을 분류하는 추가 메뉴입니다. 예를 들어 IT 요청 큐의 경우 "On-site" 및 "Remote" 주제 그룹이 있을 수 있습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">주제 그룹 만들기</a>. </p> <p>선택 사항입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">대기열 주제</td> 
   <td> <p>일반 기능을 기반으로 동일한 주제 그룹에 속하는 요청을 분류하는 추가 메뉴입니다. 항목 그룹에는 여러 큐 주제가 포함될 수 있습니다. </p> <p>예를 들어 IT 요청 큐의 "사이트 내" 항목 그룹에는 "하드웨어", "소프트웨어" 및 "네트워크" 큐 항목이 포함될 수 있습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">큐 항목 만들기</a>. </p> <p>선택 사항입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">라우팅 규칙</td> 
   <td> <p>이를 통해 각 요청을 사용자, 작업 역할, 팀 또는 프로젝트에 라우팅할 수 있습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a>. </p> <p>선택 사항입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 요청 큐 만들기

프로젝트를 요청 큐로 설정할 때 Workfront의 요청 영역에 표시하려면 프로젝트 상태가 현재여야 합니다.

요청 큐를 만들려면:

1. 요청 큐로 설정할 프로젝트로 이동합니다.
1. (선택 사항) **프로젝트 세부 사항** 왼쪽 패널에서 **설명** 에서 프로젝트에 **개요** 영역. 이 정보는 모든 새 요청에 표시됩니다.
1. 클릭 **큐 세부 정보** 왼쪽 패널에 표시됩니다. 을(를) 클릭하여 **자세히 표시**, 그런 다음 **큐 세부 정보**.

   큐 세부 사항 섹션이 열립니다.

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. 다음 정보를 지정합니다.

   * **도움말 요청 큐로 게시:** 이 프로젝트를 요청 큐로 식별하려면 이 옵션을 선택합니다. 들어오는 모든 문제는 요청으로 간주됩니다.\
      이 옵션을 선택하지 않으면 프로젝트는 Workfront에서 표준 프로젝트처럼 동작하며 수신되는 모든 문제가 문제입니다.

   * **이 큐에 요청을 추가할 수 있는 사람:** 이 큐에 요청을 추가할 수 있는 액세스 권한을 가진 사용자를 선택합니다. 다음 사용자 그룹이 전역 탐색 막대의 요청 영역에서 요청 큐를 볼 수 있도록 허용할 수 있습니다.

      | 모든 사용자 | 활성 계정이 있는 모든 Workfront 사용자는 이 요청 큐를 보고 해당 요청에 요청을 추가할 수 있습니다 |
      |---|---|
      | 이 프로젝트에 대한 보기 액세스 권한이 있는 직원 | 프로젝트에 대한 보기 권한이 있는 사용자는 이 큐에 요청을 보고 추가할 수 있습니다 |
      | 이 프로젝트 회사의 사람 | 이 프로젝트와 연결된 회사에 속하는 사용자는 이 큐에 요청을 보고 추가할 수 있습니다. 프로젝트와 연결된 회사가 있는 경우 이 설정 후에는 회사 이름이 괄호로 묶입니다. |
      | 이 프로젝트의 그룹에 있는 직원들 | 이 프로젝트와 연결된 그룹에 속하는 사용자는 이 큐에 요청을 보고 추가할 수 있습니다. 프로젝트와 연결된 그룹이 있는 경우 이 설정 후에는 그룹 이름이 괄호로 묶입니다. |

      {style=&quot;table-layout:auto&quot;}

   * **다음 링크와 공유:** 다음 옵션을 사용하면 요청 큐 및 이와 연관된 양식에 직접 액세스할 수 있고, 외부 페이지를 사용하여 Workfront 외부의 사용자 또는 Workfront 사용자에게 직접 액세스할 수 있습니다. 대시보드에 외부 페이지로 요청 큐 포함에 대한 자세한 내용은 [대시보드에 요청 큐 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

      직접 액세스하려면 사용자가 요청 큐에 대한 액세스 권한을 이미 가지고 있어야 합니다. 여기에 설명된 두 옵션 중 하나를 사용하면 사용자에게 액세스를 자동으로 부여하지 않습니다.

      >[!TIP]
      >
      >사용자는 다른 애플리케이션에서 요청 큐 페이지에 액세스할 때 요청 큐에 액세스하려면 먼저 Workfront에 로그인해야 합니다.

      * **직접 액세스 URL:** 사용자가 브라우저에서 이 URL에 액세스하면 사용자가 요청 영역의 새 요청 섹션으로 직접 이동하며 이 요청은 기본적으로 선택됩니다.

         ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

         >[!NOTE]
         >
         >대시보드에 요청 큐를 외부 페이지로 표시할 수 있습니다. 이 경우 요청 큐가 미리 선택되지만 요청 유형 필드에서 다른 요청 큐를 선택할 수 있습니다. 사용자는 요청 유형을 변경할 수 있습니다. 요청의 탐색 구성 요소도 표시됩니다.

      * **포함 코드:** 이 HTML 코드를 사용하여 요청 큐 양식을 HTML 페이지 내에 iframe으로 포함합니다.\
         사용자가 코드가 포함된 페이지를 볼 때 Workfront에 대해 아직 인증되지 않은 경우 Workfront 로그인 대화 상자가 표시됩니다. 사용자가 로그인하면 요청 큐 양식이 표시됩니다.

         ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

         >[!NOTE]
         iframe에 요청 큐를 표시할 때 요청 양식만 표시되고 요청 이름이 미리 선택되어 흐리게 표시됩니다. 사용자가 요청 유형을 변경할 수 없습니다. 요청 영역의 탐색 구성 요소는 표시되지 않습니다.

         이 포함 코드를 사용할 때 요청 큐 양식이 표시되도록 하려면 시스템 설정에서 &quot;Workfront을 iframe에 포함 허용&quot; 설정을 활성화해야 합니다. iframe에 Workfront 포함을 활성화하는 방법에 대한 자세한 내용은 [시스템 보안 환경 설정 구성](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). 이 설정이 활성화되어 있지 않으면 iframe이 공백으로 표시됩니다.

         다음과 같이 포함된 양식이 표시되는 방식의 다양한 측면을 조정할 수 있습니다.

         <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>기능</strong> </p> </th> 
           <th> <p><strong>솔루션</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>프레임 크기 조정</p> </td> 
           <td> <p>"width" 및 "height" 속성을 수정합니다.</p> <p>기본적으로 너비는 "500"이고 높이는 "600"입니다</p> </td> 
          </tr> 
          <tr> 
           <td> <p>특정 큐 주제 또는 주제 그룹으로 사용자를 표시합니다</p> </td> 
           <td> <p>src URL에 "path" 매개 변수를 추가합니다. 포함되지 않은 양식에서 원하는 큐 주제 또는 주제 그룹으로 이동하여 URL을 검사하면 경로 매개 변수를 찾을 수 있습니다.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>사전 구성된 주제 그룹 드롭다운 목록을 표시하고 사용자가 변경할 수 있도록 허용</p> </td> 
           <td> <p>를 추가하여 "path" 매개 변수를 사용합니다 <code>showPreSelectedOptions=true</code> 매개 변수 <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>양식 전송 시기 검색</p> </td> 
           <td> <p>웹 페이지의 창에 "메시지" 이벤트 리스너를 추가하고 확인 <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> 이 작성된 문제의 ID로 설정됩니다.</p> </td> 
          </tr> 
         </tbody> 
        </table>
   * **요청 유형:** 아래의 기본 옵션 중에서 선택합니다.

      Workfront 관리자는 기본 요청 유형의 이름을 바꿀 수 있습니다. 요청 유형 이름 바꾸기에 대한 자세한 내용은 [기본 문제 유형 사용자 지정](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * 순서 변경
      * 문제
      * 요청
      * 위험

         필수 필드이므로 하나 이상의 옵션을 선택해야 합니다.
      >[!NOTE]
      요청 유형은 대기열 세부 사항 및 대기열 항목 페이지 모두에서 요청 유형을 선택한 경우에만 요청 영역에 선택 항목으로 표시됩니다. 프로젝트의 큐 세부 정보 영역 설정에 대한 자세한 내용은 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      여기에서 선택한 각 유형은 양식에서 사용할 수 있습니다(두 개 이상 선택할 수 있음). 두 개 이상의 유형을 선택하면 여러 요청이 수신되는 것을 구성할 수 있습니다.\
      예를 들어 IT 프로젝트에 대한 요청 큐에서 양식을 사용하는 경우 다음 요청 유형이 큐에 들어올 수 있습니다. 하드웨어, 소프트웨어, 버그 수정 및 문제

   * **기본 기간:** 기본 기간은 일반적으로 문제를 완료하는 데 걸리는 시간입니다. 이 값은 모든 수신 문제에 대한 기본값이 되며 수동으로 수정할 수 있습니다. 기간은 일반적으로 시간, 일 또는 주 단위로 설정됩니다. 문제의 기본 기간은 문제에 대한 계획 시간과 같습니다. 문제의 계획 완료 일자는 이 필드를 기반으로 계산됩니다.\
      문제 기간 의 기본값은 1일 또는 8시간입니다. Workfront 관리자가 하루 평균 시간 을 8시간 미만으로 설정한 경우 문제에 대한 기본 기간은 여전히 8시간입니다. 예를 들어, 일일 평균 시간 이 7시간으로 설정되면 문제에 대한 기본 기간은 1.14일 또는 8시간입니다. 시스템을 설정하는 방법에 대한 자세한 내용은(일반 근무 시간) 문서에서 &quot;타임라인 계산&quot; 섹션을 참조하십시오 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **같은 회사의 직원들은 모든 요청에 대해 동일한 권한을 상속합니다.:** 이 옵션을 선택하면 동일한 회사의 사용자가 큐에 제출한 모든 요청을 볼 수 있습니다. 사용자는 요청 영역 내에 있는 모든 요청 섹션에서 이러한 요청을 볼 수 있습니다. 이 설정이 활성화되거나 비활성화될 때 이후의 모든 요청에 영향을 줍니다. 정보는 소급하여 영향을 받지 않습니다.
   * **누군가가 요청을 하면 자동으로 다음 권한을 부여합니다.** 사용자가 요청 큐에 요청을 하면 해당 요청에 대해 선택한 권한 수준이 자동으로 사용자에게 부여됩니다. 다음 권한 수준 중에서 선택합니다.\
      **- 보기**

      **- 참여**
      **- 관리**

      Workfront 권한 모델에 대한 자세한 내용은 [개체에 대한 권한 공유 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
      여기에서 권한을 설정하면 들어오는 각 요청에 대한 권한을 부여하지 않고 시간이 절약됩니다. 이 옵션을 선택하면 향후 모든 요청에 영향을 주지만 기존 요청에 소급하여 영향을 주지는 않습니다.

   * **기본 승인**: 승인 프로세스를 이 요청 큐와 연결합니다. 이 드롭다운 메뉴에는 문제 승인 프로세스만 표시됩니다. 이 큐에 제출된 모든 문제가 이 승인 프로세스와 연결됩니다. 요청 큐와 연결하려면 먼저 Workfront 관리자가 시스템 수준 승인 프로세스를 정의해야 합니다. 승인 프로세스에 대한 관리자 액세스 권한이 있는 사용자는 그룹별 승인 프로세스를 만들 수도 있습니다.

      >[!IMPORTANT]
      프로젝트 그룹이 변경되면 기존 문제에 첨부된 그룹별 승인 프로세스가 단일 사용 승인 프로세스가 됩니다. 프로젝트 그룹의 변경 사항이나 승인 프로세스의 변경 사항이 승인 설정에 미치는 영향에 대한 자세한 내용은 [그룹 및 승인 프로세스 변경이 지정된 승인 프로세스에 미치는 영향](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

      요청 큐와 연결된 대기열 항목이 여러 개 있는 경우 승인 프로세스를 대기열 항목과 대신 연결하는 것이 좋습니다. 큐 항목 만들기에 대한 자세한 내용은 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      요청 큐에 승인 프로세스를 추가할 때 다음 사항을 고려하십시오.

      * 활성 승인 프로세스만 목록에 표시됩니다.
      * 시스템 전체 및 그룹별 승인 프로세스가 목록에 표시됩니다. 프로젝트 이외의 그룹과 연관된 승인 프로세스가 목록에 표시되지 않습니다.
   * **기본 경로**: 라우팅 규칙을 이 요청 대기열에 연결합니다. 라우팅 규칙을 사용하여 요청 큐에 제출된 새 문제를 올바른 리소스(사용자, 작업 역할 또는 팀)와 올바른 프로젝트에 자동으로 지정합니다. 이 큐에 제출된 모든 문제는 이 라우팅 규칙과 연결됩니다. 라우팅 규칙을 요청 대기열에 연결하려면 먼저 이를 구성해야 합니다.\
      요청 대기열과 연관된 대기열 항목이 여러 개 있는 경우 라우팅 규칙을 대기열 항목과 연결하는 것이 좋습니다. 라우팅 규칙 만들기에 대한 자세한 내용은 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **새 문제 필드:** 모든 사용자에게 다음 선택한 필드 표시 섹션에서 프로젝트에 요청을 제출하거나 프로젝트 또는 작업에 문제를 추가하는 모든 사용자에게 표시할 필드를 선택합니다.

      >[!TIP]
      큐 세부 정보 섹션에서 선택한 새 문제 필드는 프로젝트나 문제 섹션의 작업에 추가된 새 문제와 연결됩니다.

      지정 대상, 작업 역할 또는 팀 필드를 활성화할 때 항상 요청 양식에서 지정 이름으로 변경되지만 여기에서 선택한 할당 유형만 지정할 수 있습니다.

      **예:** 대기열 상세내역 영역에서 지정 대상 을 선택한 경우 요청 양식의 지정 필드에 사용자만 입력할 수 있습니다. 이 경우 작업 역할이나 팀을 입력할 수 없습니다.

   * **문서**: 새 요청 양식에 문서 섹션을 표시하려면 문서 업로드 섹션을 배치할 위치를 선택합니다. 다음 중에서 선택합니다.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">사용자 정의 양식 후</td> 
        <td><span>문서 섹션은 요청 양식 하단에 표시됩니다.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">사용자 정의 양식 전</td> 
        <td> <p><span>문서 섹션은 Workfront 필드와 요청 양식의 사용자 지정 필드 사이에 표시됩니다.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

      ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **선택한 필드와 선택되지 않은 필드를 모두 표시할 대상:** 양식의 모든 필드를 표시할 사용자를 선택합니다. 다음 옵션은 양식의 필드에 대한 액세스를 제어합니다.

      | 모든 사용자(계획 라이센스) | 계획 라이센스가 있는 모든 사용자는 선택한 필드와 선택되지 않은 필드를 볼 수 있습니다. |
      |---|---|
      | 이 프로젝트에 대한 보기 액세스 권한이 있는 직원(플랜 라이선스) | 이 프로젝트에 대한 보기 권한도 있는 계획 라이센스가 있는 사용자는 선택한 필드와 선택되지 않은 필드를 볼 수 있습니다. 이 프로젝트에 요청을 제출할 수 있는 나머지 사용자는 선택한 필드만 볼 수 있습니다. |
      | 사용자 없음 | 선택되지 않은 필드를 볼 수 있는 사용자가 없습니다. 이 프로젝트에 요청을 제출할 수 있는 모든 사용자는 선택한 필드만 볼 수 있습니다. |

      {style=&quot;table-layout:auto&quot;}

   * **사용자 지정 Forms**: 요청 큐와 연결할 사용자 지정 양식을 선택합니다. 이 드롭다운 메뉴에서 문제 사용자 지정 Forms만 선택할 수 있습니다. 요청 큐에 제출된 모든 문제에 선택한 양식이 연결됩니다.\
      요청 큐에 여러 개의 큐 항목이 연결된 경우 사용자 지정 양식을 큐 항목과 대신 연결하는 것이 좋습니다. 요청 큐의 하위 섹션 만들기에 대한 자세한 내용은 다음을 참조하십시오 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      요청 대기열과 연결된 사용자 지정 양식이 여러 개 있는 경우 양식을 드래그하여 놓아 원하는 순서대로 정렬합니다. **Forms 재정렬** 섹션을 참조하십시오.

      >[!TIP]
      큐 세부 정보 섹션에 추가된 사용자 지정 양식은 프로젝트에 추가된 새 문제 또는 문제 섹션의 작업과 연결됩니다.

   * **이메일을 통해 문제를 추가할 수 있습니다.** 이메일을 통해 요청을 제출할 수 있도록 하려면 이 옵션을 선택합니다.\
      자세한 내용은 [사용자가 요청 큐 프로젝트에 문제를 이메일로 보낼 수 있도록 설정](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).




1. **저장**&#x200B;을 클릭합니다.\
   이제 프로젝트가 요청 큐로 구성되었으며 사용자는 이제 요청에 요청을 추가할 수 있습니다.

1. (선택 사항) 요청 큐 기능을 향상시키기 위해 큐에 대한 추가 하위 섹션을 작성하고 들어오는 요청을 올바른 팀, 할당자 또는 프로젝트로 라우팅하는 규칙을 만듭니다.

   요청 큐의 하위 섹션 만들기에 대한 내용은 문서를 참조하십시오 [큐 항목 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) 및 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).\
   적절한 담당자, 팀 및 적절한 프로젝트에 요청을 라우팅하는 방법에 대한 자세한 내용은 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
