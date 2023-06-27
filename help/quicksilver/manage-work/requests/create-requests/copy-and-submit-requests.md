---
title: 요청 복사 및 제출
description: 유사한 요청을 자주 제출하는 경우 제출된 기존 요청을 복사할 수 있습니다. 이 경우 기존 요청을 복사하고 최소 변경 내용을 적용한 다음 새 요청으로 다시 제출할 수 있습니다.
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 742565b06395e5092152b1d04262344dc1020d74
workflow-type: tm+mt
source-wordcount: '1339'
ht-degree: 2%

---

# 요청 복사 및 제출

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

유사한 요청을 자주 제출하는 경우 제출된 기존 요청을 복사할 수 있습니다. 이 경우 기존 요청을 복사하고 최소 변경 내용을 적용한 다음 새 요청으로 다시 제출할 수 있습니다.

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
이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>요청 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>요청 대기열에 요청을 추가하는 액세스 권한</p> <p>기존 요청에 대한 이상의 권한 보기</p> <p>요청 대기열 설정에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

## 전제 조건

귀하 또는 귀하 조직의 누군가가 이전에 제출한 요청을 복사하여 다시 제출할 수 있어야 합니다. 요청이 다른 사용자에게 속한 경우 새 요청으로 복사하고 제출하려면 보기 액세스 권한이 있어야 합니다.

## 요청을 새 요청으로 복사 및 제출하는 것에 대한 고려 사항

* 제출된 요청만 복사하고 제출할 수 있습니다. 초안 요청은 복사할 수 없습니다.
* 처음에 제출한 요청이나 다른 사람이 제출한 요청을 복사하여 제출할 수 있으며 최소한 [보기]에 액세스할 수 있습니다.
* 다른 사용자가 자신의 요청에 대한 권한을 제거하지 않은 한 해당 요청을 복사하여 제출할 수 있는 액세스 권한이 항상 있습니다.
* 원래 다른 사람이 제출한 요청을 복사하고 제출하는 액세스 권한은 요청 대기열의 작성자가 **같은 회사의 직원들은 모든 요청에 대해 동일한 권한을 상속합니다.** 대기열 세부 정보 또는 프로젝트 편집 영역. 이 설정을 비활성화하면 원래 요청자만 자신의 요청을 볼 수 있습니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)

* 새 요청으로 다시 제출하기 전에 원래 요청의 사본을 업데이트할 수 있습니다.
* 원래 요청이 제출된 후에 다음 변경 사항이 발생하면 더 이상 복사하여 다시 제출할 수 없습니다.

   * 요청 대기열이 삭제되었습니다.
   * 대기열 주제가 삭제되었습니다.

     >[!TIP]
     >
     >대기열 주제가 요청 대기열에 있는 유일한 항목인 경우에도 요청을 복사하고 제출할 수 있으며 요청 대기열 자체 아래에 저장됩니다.

   * 요청 대기열이 더 이상 도움말 요청 대기열로 게시되지 않습니다. 자세한 내용은 [요청 대기열 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * 요청 대기열에 대기열 주제가 없고 원래 요청이 2022년 1월 이전에 제출된 경우.

   * 요청 대기열과 연결된 프로젝트의 상태가 더 이상 현재가 아닙니다.

* 요청이 변환 프로세스에서 유지된 경우 변환된 요청의 사본을 복사하여 제출할 수 있습니다. 자세한 내용은 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >복사된 요청이 해결 중 오브젝트에 연결되어 있지 않습니다.

## 요청 복사 및 제출

1. 다음을 클릭합니다. **메인 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 상단에서 을(를) 클릭한 다음 **요청**.
1. (조건부) 제출됨 섹션이 기본적으로 표시되지 않으면 **제출됨** 왼쪽 패널에서
1. 새로 복사하여 제출할 요청을 찾은 후 다음 중 하나를 수행합니다.

   * 선택한 다음 **새 항목으로 복사 및 제출** 아이콘 ![](assets/copy-and-submit-as-new-requests-area-nwe.png) 을 클릭합니다. <!--update this icon the 23.3 preview release, or shortly after: replace this step with this: Select it, then click the **Copy** icon ![](assets/copy-and-submit-as-new-requests-area-nwe.png) in the upper-left corner of the Submitted requests list.-->

   <!-- reveal this tip for 23.3 preview release:
   >[!TIP]
   >
   > <span class="preview">If you did not select a request first, the Copy icon is dimmed.</span> 
   -->

   * 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-icon.png) 요청 이름 오른쪽에 있는 을 클릭합니다. **새 항목으로 복사 및 제출** <!--ensure this does not change with the Copy icon improvements with 23.3 preview-->

     또는

     선택한 요청을 마우스 오른쪽 단추로 클릭한 다음 **새 항목으로 복사 및 제출**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >문제를 만들 수 있는 액세스 권한이 없는 경우 관리자가 요청 만들기를 제한했다는 경고가 표시됩니다.

1. (선택 사항) 필요한 경우 다음 정보를 갱신합니다.

   * **요청 유형**: 복사된 요청이 저장되는 요청 대기열입니다. 기본적으로 복사된 요청은 원래 요청의 요청 대기열에 저장됩니다.
   * **주제 그룹** 및 **대기열 주제**&#x200B;을 선택합니다. 사용자 환경에 맞게 이름 또는 주제 그룹 및 대기열 주제를 사용자 정의합니다. 기본적으로 복사된 요청은 원래 요청의 주제 그룹 및 대기열 주제에 저장됩니다.

     >[!TIP]
     >
     >원래 요청의 경로에서 경로가 변경되면 요청 대기열 생성자가 대기열을 수정했습니다.

1. (선택 사항) 복사된 요청에서 모든 정보를 업데이트합니다. 에서 요청 대기열 생성자가 활성화한 필드에 따라 **새 문제 필드** 의 섹션 **대기열 세부 정보** 프로젝트의 하위 탭에서 다음 필드 중 하나를 찾을 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>주제</strong> </td> 
      <td>원래 요청의 이름을 표시합니다. 필요한 경우 업데이트합니다. 그렇지 않으면 Workfront에서 복사된 요청의 이름을 지정합니다 <b>다음의 사본 &lt;name of="" original="" request=""&gt;</b>. 필수 필드입니다.</td> 
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
      <td> <p>요청의 우선 순위를 지정하십시오. 우선 순위는 이 요청이 얼마나 빨리 해결되어야 한다고 생각하는지를 정의해야 합니다. 기본 옵션은 다음과 같습니다.</p> 
       <ul> 
        <li>없음</li> 
        <li>낮음</li> 
        <li>기본</li> 
        <li>높음</li> 
        <li>긴급</li> 
       </ul> <p>Workfront 관리자는 우선 순위 이름을 수정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>심각도</strong> </td> 
      <td> <p>요청의 심각도를 지정하십시오. 심각도는 이 요청이 제시간에 해결되지 않을 경우 작업에 미치는 영향을 정의해야 합니다. 기본 옵션은 다음과 같습니다.</p> 
       <ul> 
        <li>표시용</li> 
        <li>혼란 야기</li> 
        <li>해결 방법이 있는 버그</li> 
        <li>해결 방법이 없는 버그</li> 
        <li>치명적인 오류</li> 
       </ul> <p>Workfront 관리자는 심각도 이름을 수정할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>기본 담당자</strong> </td> 
      <td>사용자가 요청과 관련된 모든 질문을 처리할 수 있으므로 요청의 기본 연락처는 기본적으로 귀하에게 제공됩니다. 그러나 다른 Workfront 사용자로 변경할 수 있습니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>할당</strong></span> </td> 
      <td> <p>요청을 할당해야 하는 활성 사용자, 작업 역할 또는 팀의 이름을 나타냅니다. </p> <p> 두 명 이상의 사용자, 작업 역할 또는 팀을 지정할 수 있습니다. </p> <p>요청 대기열이 설정된 방법에 따라 세 가지 리소스 유형 모두 대신 하나 또는 두 가지 유형의 리소스에만 요청을 할당할 수 있습니다. </p> <p>요청 대기열을 적절한 리소스로 자동으로 라우팅할 수 있도록 라우팅 규칙을 사용하는 것이 좋습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">요청 대기열이 설정된 방법에 따라 한 가지 유형의 리소스만 요청에 할당할 수 있습니다(예: 사용자). 라우팅 규칙도 요청 대기열에 연결되어 있으며 자동으로 요청을 다른 유형의 리소스(예: 팀)로 라우팅하는 경우 요청을 제출할 때 수동으로 지정하는 엔티티(사용자)와 라우팅 규칙에 지정된 리소스(팀) 모두에 요청이 할당됩니다.</p> <p style="font-weight: normal;">자세한 내용은 다음 문서를 참조하십시오.</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">라우팅 규칙 만들기</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 시간</strong> </td> 
      <td> <p>이 요청을 완료하는 데 걸리는 시간을 예상합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 시작 일자</strong> </td> 
      <td> <p>이 요청에 대한 작업이 시작되어야 하는 날짜입니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>계획된 완료 일자</strong> </td> 
      <td>이 요청을 해결하고자 하는 날짜.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태</strong> </td> 
      <td>새 요청의 기본 상태는 "신규"입니다. Workfront 관리자가 이 상태의 이름을 변경했을 수 있습니다. 이 드롭다운 메뉴에서 상태를 다른 것으로 변경할 수도 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>문서</strong> </td> 
      <td> <p>요청에 문서를 추가합니다. 원래 요청에 첨부된 문서는 복사된 요청으로 전송되지 않습니다.</p> <p><b>팁</b>

   요청 대기열을 설정한 방법에 따라 문서 섹션이 사용자 정의 필드의 앞 또는 뒤에 표시될 수 있습니다.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (선택 사항) 필요한 경우 첨부된 사용자 정의 양식의 모든 정보를 업데이트합니다.

   >[!TIP]
   >
   >* 원래 요청에 첨부된 모든 사용자 정의 양식과 사용자 정의 필드에 포함된 값은 복사된 요청으로 전송됩니다. 여기에는 논리가 포함된 필드가 포함됩니다.
   >* 복사된 요청에서 사용자 정의 양식을 제거할 수 없습니다.

1. 클릭 **제출**.

   복사된 요청이 지정한 요청 대기열에 새 요청으로 제출됩니다.
