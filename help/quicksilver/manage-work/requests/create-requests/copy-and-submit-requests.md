---
title: 요청 복사 및 제출
description: 요청 복사 및 제출
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# 요청 복사 및 제출

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is NWE only - hard code it in classic articles!)</p>
-->

유사한 요청을 자주 제출하는 경우 기존 제출된 요청을 복사할 수 있습니다. 이 경우 기존 요청을 복사하고, 최소 변경 작업을 수행하고, 새 요청으로 다시 제출할 수 있습니다.

## 액세스 요구 사항

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
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
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>요청 큐에 요청 추가 액세스</p> <p>기존 요청에 대한 더 높은 권한 보기</p> <p>요청 큐 설정에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

본인이나 조직의 누군가가 이전에 제출한 요청에서 해당 복사본을 복사하고 다시 제출할 수 있어야 합니다. 요청이 다른 사용자에게 속하는 경우, 보고 액세스 권한이 있어야 보고 새 요청으로 복사하고 제출할 수 있습니다.

## 요청을 새 이름으로 복사하고 제출하는 것과 관련된 고려 사항

* 제출된 요청만 복사하고 제출할 수 있습니다. 초안 요청을 복사할 수 없습니다.
* 처음에 제출한 요청을 복사 및 제출하거나, 다른 사람이 제출한 요청을 복사하고 제출할 수 있으며 적어도 보기에 액세스할 수 있습니다.
* 누군가 사용자의 권한을 제거하지 않은 한 항상 고유한 요청 사본을 복사하고 제출할 수 있는 액세스 권한이 있습니다.
* 원래 다른 사람이 제출한 복사 및 제출 요청에 대한 액세스 권한은 요청 큐의 작성자가 **동일한 회사의 사용자는 모든 요청에 대해 동일한 권한을 상속받게 됩니다** ( 대기열 세부 사항 또는 프로젝트 편집 영역) 이 설정을 비활성화하면 원래 요청자만 자신의 요청을 볼 수 있습니다.

   자세한 내용은 다음 문서를 참조하십시오.

   * [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)

* 원본 요청의 사본을 업데이트한 후 새 요청으로 다시 제출할 수 있습니다.
* 원래 요청이 제출된 후 다음 변경 사항이 발생하면 더 이상 복사하여 제출할 수 없습니다.

   * 요청 큐가 삭제되었습니다.
   * 큐 항목이 삭제되었습니다.

      >[!TIP]
      >
      >큐 주제가 요청 큐의 유일한 항목인 경우 여전히 요청을 복사하고 제출할 수 있으며 요청 큐 자체 아래에 저장됩니다.

   * 요청 큐가 더 이상 도움말 요청 큐로 게시되지 않습니다. 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * 요청 큐에 큐 항목이 없고 원래 요청이 2022년 1월 이전에 제출된 경우.

   * 요청 큐와 연결된 프로젝트의 상태 가 더 이상 최신 상태가 아닙니다.

* 전환 프로세스에서 요청이 유지된 경우 변환된 요청의 사본을 복사하고 제출할 수 있습니다. 자세한 내용은 [Adobe Workfront의 변환 문제 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

   >[!TIP]
   >
   >복사된 요청이 해결 개체에 연결되어 있지 않습니다.

## 요청 복사 및 제출

1. 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **요청**.
1. (조건부) Submitted 섹션이 기본적으로 표시되지 않으면 **제출됨** 왼쪽 패널에 표시됩니다.
1. 복사 및 제출하려는 요청을 찾아 다음 중 하나를 수행합니다.

   * 이 옵션을 선택한 다음 **새 이름으로 복사 및 제출** 아이콘 ![](assets/copy-and-submit-as-new-requests-area-nwe.png) 를 클릭합니다.
   * 을(를) 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png) 요청 이름의 오른쪽에 있는 를 클릭한 다음, **새 이름으로 복사 및 제출**

      또는

      선택한 요청을 마우스 오른쪽 단추로 클릭하고 **새 이름으로 복사 및 제출**.

      ![](assets/request-selected-more-menu-options-nwe-350x191.png)

      >[!TIP]
      >
      >문제를 만들 수 있는 액세스 권한이 없는 경우 관리자가 요청을 만들 수 없도록 제한했다는 경고를 받게 됩니다.

1. (선택 사항) 필요한 경우 다음 정보를 업데이트합니다.

   * **요청 유형**: 복사된 요청이 저장되는 요청 큐. 기본적으로 복사된 요청은 원래 요청의 요청 큐에 저장됩니다.
   * **주제 그룹** 및 **큐 항목**&#x200B;로 설정되면 eVar가 선택된 것으로 표시됩니다. 사용자 환경에 맞게 이름 또는 주제 그룹 및 큐 주제가 사용자 지정됩니다. 기본적으로 복사된 요청은 주제 그룹과 원래 요청의 큐 항목에 저장됩니다.

      >[!TIP]
      >
      >원래 요청의 경로에서 경로가 변경되면 요청 큐 작성자가 큐를 수정했습니다.

1. (선택 사항) 복사된 요청에서 정보를 업데이트합니다. 요청 큐 작성자가 **새 문제 필드** 섹션 **큐 세부 정보** 하위 탭에서 다음 필드를 찾을 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>주제</strong> </td> 
      <td>원래 요청의 이름을 표시합니다. 필요한 경우 업데이트합니다. 그렇지 않으면 Workfront에서 복사한 요청의 이름을 지정합니다 <b>의 사본 &lt;name of="" original="" request=""&gt;</b>. 필수 필드입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>설명</strong> </td> 
      <td>원래 요청의 설명을 표시합니다. 필요한 경우 업데이트합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>원래 요청의 URL을 표시합니다. 필요한 경우 업데이트합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>우선 순위</strong> </td> 
      <td> <p>요청의 우선순위를 지정합니다. 우선 순위는 이 요청이 얼마나 빨리 해결되어야 한다고 생각하는지를 정의해야 합니다. 기본 옵션은 다음과 같습니다.</p> 
       <ul> 
        <li>없음</li> 
        <li>낮음</li> 
        <li>기본</li> 
        <li>높음</li> 
        <li>긴급</li> 
       </ul> <p>Workfront 관리자는 우선순위 이름을 수정할 수 있습니다.</p> </td> 
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
       </ul> <p>Workfront 관리자는 심각도의 이름을 수정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 담당자</strong> </td> 
      <td>요청과 관련된 모든 질문을 처리할 주요 담당자이므로 요청의 기본 담당자는 기본적으로 사용자에게 표시됩니다. 그러나 다른 Workfront 사용자로 변경할 수 있습니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>할당</strong></span> </td> 
      <td> <p>요청을 지정할 활성 사용자, 작업 역할 또는 팀의 이름을 지정합니다. </p> <p> 둘 이상의 사용자, 작업 역할 또는 팀을 지정할 수 있습니다. </p> <p>요청 큐가 설정된 방법에 따라, 세 가지 리소스 대신 하나 또는 두 가지 유형의 리소스에만 요청을 할당할 수 있습니다. </p> <p>요청 대기열에 라우팅 규칙을 사용하여 해당 리소스로 자동 라우팅하는 것이 좋습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">요청 큐가 설정되는 방식에 따라, 요청(예: 사용자)에 하나의 리소스 유형만 할당할 수 있습니다. 라우팅 규칙이 요청 대기열에도 연결되어 있고 요청을 다른 리소스 유형(예: 팀)으로 자동 라우팅하는 경우, 요청(사용자)을 실행할 때 수동으로 지정하는 엔티티와 라우팅 규칙에 지정된 리소스(팀)에 모두 요청이 지정됩니다.</p> <p style="font-weight: normal;">자세한 내용은 다음 문서를 참조하십시오.</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 시간</strong> </td> 
      <td> <p>이 요청을 완료하는 데 걸리는 시간을 예측합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 시작 일자</strong> </td> 
      <td> <p>이 요청에서 작업하는 날짜입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 완료 일자</strong> </td> 
      <td>이 요청을 해결할 날짜입니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태</strong> </td> 
      <td>새 요청의 기본 상태는 "New"입니다. Workfront 관리자가 이 상태의 이름을 변경했을 수 있습니다. 이 드롭다운 메뉴에서 상태를 다른 항목으로 변경할 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>문서</strong> </td> 
      <td> <p>요청에 문서를 추가합니다. 원본 요청에 첨부된 문서는 복사된 요청으로 전송되지 않습니다.</p> <p><b>팁</b>

   요청 큐의 설정 방식에 따라 문서 섹션이 사용자 지정 필드 전이나 후에 표시될 수 있습니다.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (선택 사항) 필요한 경우 첨부된 사용자 지정 양식의 정보를 업데이트합니다.

   >[!TIP]
   >
   >* 원본 요청에 첨부된 모든 사용자 지정 양식과 사용자 지정 필드에 포함된 값이 복사된 요청으로 전송됩니다. 여기에는 논리를 포함하는 필드가 포함됩니다.
   >* 복사한 요청에서 사용자 지정 양식을 제거할 수 없습니다.


1. 클릭 **제출**.

   복사한 요청은 지정한 요청 큐에서 새 요청으로 제출됩니다.
