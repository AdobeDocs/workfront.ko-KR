---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 요청 대기열 만들기
description: 사용자가 프로젝트에서 계획된 작업이 아닌 간혹 요청을 입력할 수 있는 요청 대기열을 설정할 수 있습니다. 예를 들어 IT 부서에 접수되는 모든 사용자 요청을 캡처하도록 헬프 데스크 요청 대기열을 설정할 수 있습니다.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '2653'
ht-degree: 2%

---


# 요청 대기열 만들기

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

사용자가 프로젝트에서 계획된 작업이 아닌 간혹 요청을 입력할 수 있는 요청 대기열을 설정할 수 있습니다. 예를 들어 IT 부서에 접수되는 모든 사용자 요청을 캡처하도록 헬프 데스크 요청 대기열을 설정할 수 있습니다.

이 문서에서는 사용자가 요청을 제출할 수 있는 요청 대기열을 만드는 방법에 대해 설명합니다. 요청 대기열에 새 요청을 제출하는 방법에 대한 자세한 내용은 [요청 복사 및 제출](../create-requests/copy-and-submit-requests.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> 
   <p>새 라이선스: Standard </p>
   또는
   <p>현재 라이선스: 플랜 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>프로젝트에 대한 액세스 편집</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p> 프로젝트에 대한 권한 관리</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


<!--old access levels: 
You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b></p> 
   
   <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator
-->

## 요청 대기열 개요

요청 대기열을 프로젝트로 설정합니다. 프로젝트를 요청 대기열로 지정하면 Adobe Workfront의 요청 영역에서 대기열에 액세스할 수 있습니다. 요청 대기열을 사용자 정의하는 경우 사용자가 요청을 제출할 때 작성하는 양식을 사용자 정의하는 경우도 있습니다.

이 문서에서는 기존 프로젝트에서 요청 대기열을 만드는 방법에 대해 설명합니다. 그러나 요청 접수 프로세스에 대한 일관성을 구축하거나 보고 목적 및 개선된 관리를 위해 요청 접수 프로세스에 여러 계층을 추가하려면 다음 표에 설명된 요청 대기열의 추가 구성 요소를 구성할 수도 있습니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">대기열 세부 정보</td> 
   <td> <p>대기열 세부 정보 영역에서 프로젝트를 요청 대기열로 설정해야 합니다. 이 단계는 필수입니다. </p> <p>자세한 내용은 이 문서의 <a href="#create-a-request-queue" class="MCXref xref">요청 큐 만들기</a> 섹션을 참조하십시오.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">주제 그룹</td> 
   <td> <p>일반적인 기능에 따라 요청을 분류하는 추가 메뉴입니다. 예를 들어 IT 요청 대기열의 경우 "온사이트" 및 "원격" 주제 그룹이 있을 수 있습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">주제 그룹 만들기</a>를 참조하십시오. </p> <p>선택 사항입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">대기열 주제</td> 
   <td> <p>공통 기능을 기반으로 동일한 주제 그룹에 속하는 요청을 분류하는 추가 메뉴입니다. 주제 그룹에는 여러 개의 대기열 주제가 포함될 수 있습니다. </p> <p>예를 들어 IT 요청 대기열에 대한 "온사이트" 항목 그룹에는 "하드웨어", "소프트웨어" 및 "네트워크" 대기열 항목이 포함될 수 있습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">대기열 주제 만들기</a>를 참조하십시오. </p> <p>선택 사항입니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">라우팅 규칙</td> 
   <td> <p>이를 통해 각 요청을 사용자, 작업 역할, 팀 또는 프로젝트에 라우팅할 수 있습니다. </p> <p>자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a>를 참조하세요. </p> <p>선택 사항입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 요청 대기열 만들기

프로젝트를 요청 대기열로 설정할 때 Workfront의 요청 영역에 표시하려면 프로젝트 상태가 현재여야 합니다.

>[!TIP]
>
>Workfront 또는 그룹 관리자가 다음 단계에 설명된 섹션 중 일부를 포함하지 않을 수 있는 사용자 지정 레이아웃 템플릿에 귀하를 할당할 수 있습니다.


요청 대기열을 만들려면 다음 작업을 수행하십시오.

1. 요청 대기열로 설정할 프로젝트로 이동합니다.
1. (선택 사항) 왼쪽 패널의 **프로젝트 세부 정보**&#x200B;를 클릭하고 **개요** 영역의 프로젝트에 **설명**&#x200B;을(를) 추가합니다. 이 정보는 모든 새 요청에 표시됩니다.
1. 왼쪽 패널에서 **큐 세부 정보**&#x200B;를 클릭합니다. **자세히 표시**&#x200B;를 클릭한 다음 **큐 세부 정보**&#x200B;를 클릭해야 할 수 있습니다.

   그러면 대기열 세부 정보 섹션이 열립니다.

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. 다음 정보를 지정합니다.

   * **도움말 요청 대기열로 Publish:** 이 프로젝트를 요청 대기열로 식별하려면 이 옵션을 선택하십시오. 모든 수신 문제는 요청으로 간주됩니다.\
     이 옵션을 선택하지 않으면 프로젝트가 Workfront의 표준 프로젝트처럼 작동하고 들어오는 모든 문제가 문제입니다.

   * **이 대기열에 요청을 추가할 수 있는 사용자:** 이 대기열에 요청을 추가할 수 있는 액세스 권한을 가진 사용자를 선택하십시오. 새 요청을 추가할 때 다음 그룹의 사용자가 전역 탐색 막대의 요청 영역에서 요청 대기열을 볼 수 있도록 허용할 수 있습니다.

     | 요청을 입력할 수 있는 사람 | 설명 |
     |---|---|
     | 모든 사용자 | 활성 계정이 있는 모든 Workfront 사용자는 이 요청 대기열을 보고 요청을 추가할 수 있습니다 |
     | 이 프로젝트에 대한 보기 액세스 권한이 있는 직원 | 프로젝트에 대한 보기 권한이 있는 사용자는 요청을 보고 이 큐에 추가할 수 있습니다. |
     | 이 프로젝트 회사의 사람 | 이 프로젝트와 연계된 회사에 속하는 사용자는 요청을 보고 이 큐에 추가할 수 있습니다. 프로젝트와 연결된 회사가 있는 경우 이 설정 뒤에 회사 이름이 괄호 안에 나열됩니다. |
     | 이 프로젝트의 그룹에 있는 직원들 | 이 프로젝트와 연계된 그룹에 속하는 사용자는 요청을 보고 이 큐에 추가할 수 있습니다. 프로젝트와 연결된 그룹이 있는 경우 이 설정 뒤에 그룹 이름이 괄호 안에 회색 글꼴로 나열됩니다. |

     {style="table-layout:auto"}

   * **다음 링크와 공유:** 다음 옵션을 사용하면 Workfront 외부의 사용자 또는 외부 페이지를 사용하는 Workfront 사용자에게 요청 큐 및 이와 관련된 양식에 직접 액세스할 수 있습니다. 대시보드에 외부 페이지로 요청 큐를 포함하는 방법에 대한 자세한 내용은 [대시보드에 요청 큐 포함](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md)을 참조하십시오.

     직접 액세스 권한을 얻으려면 사용자에게 요청 대기열에 대한 액세스 권한이 있어야 합니다. 여기에 설명된 두 옵션 중 하나를 사용하면 사용자에게 자동으로 액세스 권한이 부여되지 않습니다.

     >[!TIP]
     >
     >사용자는 다른 애플리케이션에서 [요청 대기열] 페이지에 액세스할 때 요청 대기열에 액세스하려면 먼저 Workfront에 로그인해야 합니다.

      * **직접 액세스 URL:** 사용자가 브라우저에서 이 URL에 액세스하면 사용자가 요청 영역의 새 요청 섹션으로 바로 이동하며 이 요청이 기본적으로 선택됩니다.

        ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >대시보드에 요청 대기열을 외부 페이지로 표시할 수 있습니다. 이 경우 요청 대기열이 미리 선택되지만 요청 유형 필드에서 다른 요청 대기열을 선택할 수 있습니다. 사용자는 요청 유형을 변경할 수 있습니다. 요청의 탐색 구성 요소도 표시됩니다.

      * **포함 코드:** 이 HTML 코드를 사용하여 요청 큐 양식을 HTML 페이지 내에 iframe으로 포함합니다.\
        코드가 포함된 페이지를 볼 때 Workfront에 대해 사용자가 아직 인증되지 않은 경우 Workfront 로그인 대화 상자가 표시됩니다. 사용자가 로그인하면 요청 대기열 양식이 표시됩니다.

        >[!NOTE]
        >
        >iframe에 요청 대기열 을 표시할 때 요청 양식만 표시되고, 요청 이름이 미리 선택되고 흐리게 표시됩니다. 사용자가 요청 유형을 변경할 수 없습니다. 요청 영역의 탐색 구성 요소가 표시되지 않습니다.

        이 포함 코드를 사용할 때 요청 대기열 양식을 표시하려면 시스템 설정에서 &quot;iframe에 Workfront 포함 허용&quot; 설정을 활성화해야 합니다. iframe에서 Workfront 포함을 활성화하는 방법에 대한 자세한 내용은 [시스템 보안 환경 설정 구성](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오. 이 설정을 활성화하지 않으면 iframe이 공백으로 표시됩니다.

        임베드된 양식 표시 방식의 다양한 측면을 다음과 같이 조정할 수 있습니다.

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
           <td> <p>"width" 및 "height" 속성을 수정합니다.</p> <p>기본적으로 너비는 "500"이고 높이는 "600"입니다.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>특정 대기열 주제 또는 주제 그룹으로 사용자 전달</p> </td> 
           <td> <p>src URL에 "path" 매개 변수를 추가합니다. 경로 매개 변수는 포함되지 않은 양식의 원하는 대기열 주제 또는 주제 그룹으로 이동하여 URL을 검사하여 찾을 수 있습니다.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>미리 구성된 주제 그룹 드롭다운 목록을 표시하고 사용자가 변경할 수 있도록 허용</p> </td> 
           <td> <p><code>src URL</code>에 <code>showPreSelectedOptions=true</code> 매개 변수를 추가하여 "path" 매개 변수를 사용하십시오.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>양식 제출 시기 감지</p> </td> 
           <td> <p>웹 페이지의 창에 "메시지" 이벤트 수신기를 추가하고 <code>event.data.type</code>이(가) <code>requestSubmitted</code>인지 확인합니다. <code>event.data.newIssueID</code>이(가) 생성된 문제의 ID로 설정됩니다.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **요청 유형:** 아래 기본 옵션에서 선택하십시오.

     Workfront 관리자는 기본 요청 유형의 이름을 변경할 수 있습니다. 요청 유형 이름을 바꾸는 방법에 대한 자세한 내용은 [기본 문제 유형 사용자 지정](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md)을 참조하십시오.

      * 버그 신고
      * 순서 변경
      * 문제
      * 요청

        필수 필드이므로 최소 하나 이상의 옵션을 선택해야 합니다.

     >[!NOTE]
     >
     >요청 유형은 대기열 세부 정보 및 대기열 주제 페이지에서 모두 요청 유형을 선택한 경우에만 요청 영역에 선택 항목으로 표시됩니다. 프로젝트의 대기열 세부 정보 영역 설정에 대한 자세한 내용은 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)를 참조하십시오.

     여기에서 선택한 각 유형은 양식에서 사용할 수 있습니다(두 개 이상을 선택할 수 있음). 두 개 이상의 유형을 선택하면 들어오는 여러 요청을 구성하는 데 도움이 될 수 있습니다.\
     예를 들어 IT 프로젝트에 대한 요청 대기열에서 양식을 사용하는 경우 하드웨어, 소프트웨어, 버그 수정 및 문제와 같은 요청 유형이 대기열에 들어올 수 있습니다.

   * **기본 기간:** 기본 기간은 일반적으로 문제를 완료하는 데 걸리는 시간입니다. 모든 수신 문제에 대한 기본값이 되며 수동으로 수정할 수 있습니다. 기간은 일반적으로 시간, 일 또는 주 단위로 설정됩니다. 문제의 기본 기간은 문제에 대한 계획된 시간과 동일합니다. 문제의 계획된 완료 일자 는 이 필드를 기반으로 계산됩니다.\
     문제 지속 시간의 기본값은 1일 또는 8시간입니다. Workfront 관리자가 근무일당 일반 시간을 8시간 미만으로 설정한 경우 문제에 대한 기본 기간은 여전히 8시간입니다. 예를 들어, 일반 근무일당 시간을 7시간으로 설정하면 문제에 대한 기본 기간은 1.14일 또는 8시간입니다. 시스템을 설정하는 방법에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)의 &quot;타임라인 계산&quot; 섹션을 참조하십시오.

   * **같은 회사의 직원들이 모든 요청에 대해 동일한 권한을 상속합니다.:** 이 옵션을 선택하면 큐에 제출된 모든 요청이 동일한 회사의 사용자에 대해 표시됩니다. 사용자는 요청 영역 내에 있는 모든 요청 섹션에서 이러한 요청을 볼 수 있습니다. 이 설정을 활성화하거나 비활성화할 때 이후의 모든 요청에 영향을 주며 정보에 소급하여 영향을 주지는 않습니다.
   * **다른 사람이 요청을 할 때 자동으로 다음 권한을 부여합니다.** 사용자가 요청 대기열에 요청을 하면 해당 요청에 대해 선택한 권한 수준이 사용자에게 자동으로 부여됩니다. 다음 권한 수준 중에서 선택합니다.

      * **액세스 보기**
      * **Contribute 액세스**. 이것이 기본 선택입니다.
      * **액세스 관리**

     Workfront 권한 모델에 대한 자세한 내용은 [개체에 대한 공유 권한 개요](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.\
     여기서 권한을 설정하면 들어오는 각 요청에 대해 권한을 부여할 필요 없이 시간이 절약됩니다. 이 옵션을 선택하면 향후 모든 요청에 영향을 주지만 기존 요청에는 소급하여 영향을 주지 않습니다.

   * **기본 승인**: 승인 프로세스를 이 요청 대기열과 연결합니다. 문제 승인 프로세스만 이 드롭다운 메뉴에 표시됩니다. 이 대기열에 제출된 모든 문제는 이 승인 프로세스와 연결됩니다. 요청 대기열과 연결하려면 Workfront 관리자가 시스템 수준 승인 프로세스를 정의해야 합니다. 승인 프로세스에 대한 관리 액세스 권한이 있는 사용자는 그룹별 승인 프로세스를 만들 수도 있습니다.

     >[!IMPORTANT]
     >
     >프로젝트의 그룹이 변경되면 기존 문제에 첨부된 그룹별 승인 프로세스가 일회성 승인 프로세스가 됩니다. 프로젝트 그룹 변경 또는 승인 프로세스 변경 내용이 승인 설정에 미치는 영향에 대한 자세한 내용은 [그룹 및 승인 프로세스 변경 내용이 할당된 승인 프로세스에 미치는 영향](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md)을 참조하십시오.

     요청 대기열과 관련된 대기열 주제가 여러 개 있는 경우 대신 승인 프로세스를 대기열 주제와 연결하는 것이 좋습니다. 대기열 주제 만들기에 대한 자세한 내용은 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)를 참조하십시오.

     요청 대기열에 승인 프로세스를 추가할 때는 다음 사항을 고려하십시오.

      * 활성 승인 프로세스만 목록에 표시됩니다.
      * 시스템 전체 및 그룹별 승인 프로세스가 목록에 표시됩니다. 프로젝트 그룹 이외의 그룹과 연결된 승인 프로세스가 목록에 표시되지 않습니다.

   * **기본 경로**: 라우팅 규칙을 이 요청 대기열과 연결합니다. 라우팅 규칙을 사용하여 요청 대기열에 제출된 새 문제를 올바른 리소스(사용자, 작업 역할 또는 팀) 및 올바른 프로젝트에 자동으로 할당합니다. 이 큐에 제출된 모든 문제는 이 라우팅 규칙과 연결됩니다. 라우팅 규칙이 [대기열 세부 정보] 섹션에 표시되고 요청 대기열에 연결되기 전에 먼저 라우팅 규칙을 구성해야 합니다.\
     요청 대기열과 관련된 대기열 주제가 여러 개 있는 경우 라우팅 규칙을 대기열 주제와 대신 연결하는 것이 좋습니다. 라우팅 규칙 만들기에 대한 자세한 내용은 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)를 참조하십시오.

   * **새 문제 필드:** **선택한 다음 필드를 모든 사용자에게 표시** 섹션에서 프로젝트에 요청을 제출하거나 프로젝트 또는 작업에 문제를 추가하는 모든 사용자에게 표시할 필드를 선택합니다.

     >[!TIP]
     >
     >[대기열 세부 정보] 섹션에서 선택한 새 문제 필드는 <!--this is confusing: or to the tasks in the Issues section--> 프로젝트에 추가된 새 문제와도 연결되어 있습니다.

     할당 대상, 작업 역할 또는 팀 필드를 활성화하면 항상 요청 양식에서 할당으로 이름이 변경되지만 여기에서 선택한 할당 유형만 지정할 수 있습니다.

     >[!NOTE]
     >
     >대기열 세부 정보 영역에서 할당 대상을 선택한 경우 요청 양식의 할당 필드에 사용자만 입력할 수 있습니다. 이 경우 작업 역할이나 팀을 입력할 수 없습니다.

   * **문서**: 새 요청 양식에 문서 섹션을 표시하도록 선택한 경우 문서 업로드 섹션의 위치를 선택하십시오. 다음 중에서 선택합니다.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">사용자 정의 양식 후</td> 
        <td><span>문서 섹션이 요청 양식 하단에 표시됩니다.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">사용자 정의 양식 전</td> 
        <td> <p><span>문서 섹션은 Workfront 필드와 요청 양식의 사용자 지정 필드 사이에 표시됩니다.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **선택한 필드와 선택 해제된 필드 모두 표시 대상:** 새 요청 양식에 모든 필드를 표시할 사용자를 선택합니다. 다음 옵션은 양식의 필드에 대한 액세스를 제어합니다.

     | 요청 양식에서 모든 필드를 볼 수 있는 사용자 | 설명 |
     |---|---| 
     | 모든 사용자(플랜 라이선스) | 플랜 라이선스가 있는 모든 사용자는 선택한 필드와 선택하지 않은 필드를 볼 수 있습니다. |
     | 이 프로젝트에 대한 보기 액세스 권한이 있는 직원(플랜 라이선스) | 이 프로젝트에 대한 보기 권한도 있는 플랜 라이선스가 있는 사용자는 선택한 필드와 선택하지 않은 필드를 볼 수 있습니다. 이 프로젝트에 요청을 제출할 수 있는 나머지 사용자에게는 선택한 필드만 표시됩니다. |
     | 사용자 없음 | 선택되지 않은 필드는 사용자가 볼 수 없습니다. 이 프로젝트에 요청을 제출할 수 있는 모든 사용자는 선택한 필드만 볼 수 있습니다. |

   * **사용자 지정 Forms**: 요청 대기열과 연결할 사용자 지정 양식을 선택하십시오. 문제 사용자 지정 Forms 만 이 드롭다운 메뉴에서 선택할 수 있습니다. 요청 대기열에 제출된 모든 문제는 선택한 양식과 연결됩니다. 대기열 세부 정보 섹션에 표시되기 전에 문제 사용자 정의 양식을 만들어야 합니다.
요청 대기열과 관련된 대기열 주제가 여러 개 있는 경우 사용자 정의 양식을 대기열 주제와 대신 연결하는 것이 좋습니다. 요청 대기열의 하위 섹션을 만드는 방법에 대한 자세한 내용은 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)를 참조하십시오.

     ![](assets/custom-forms-on-queue-details.png)

     요청 대기열과 연결된 사용자 정의 양식이 여러 개 있는 경우 양식을 끌어다 놓아 **Forms 순서 바꾸기** 섹션에서 원하는 순서로 정렬하십시오.

     >[!TIP]
     >
     >큐 세부 정보 섹션에 추가된 사용자 정의 양식도 <!--this is confusiong: or the tasks in the Issues  section--> 프로젝트에 추가된 새 문제와 연결되어 있습니다.

1. 사용자가 요청 대기열 프로젝트에 대한 요청을 이메일로 보낼 수 있도록 **이메일 대기열 설정** 영역의 설정에 대한 정보를 계속 선택합니다.

   자세한 내용은 [사용자가 요청 대기열 프로젝트에 문제를 이메일로 보낼 수 있도록 설정](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md)을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.\
   이제 프로젝트가 요청 대기열로 구성되었으며 사용자는 여기에 요청을 추가할 수 있습니다.

1. (선택 사항) 요청 대기열 기능을 향상시키려면 대기열에 대한 추가 하위 섹션과 수신 요청을 올바른 팀, 할당자 또는 프로젝트로 라우팅하는 규칙을 빌드합니다.

   * 요청 대기열의 하위 섹션 만들기에 대한 자세한 내용은 문서 [대기열 주제 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) 및 [주제 그룹 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)를 참조하십시오.
   * 요청을 적절한 담당자, 팀 및 적절한 프로젝트로 라우팅하는 방법에 대한 자세한 내용은 [라우팅 규칙 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)를 참조하십시오.
