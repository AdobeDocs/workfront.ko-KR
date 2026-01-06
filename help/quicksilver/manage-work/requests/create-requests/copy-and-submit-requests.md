---
title: 요청 복사 및 제출
description: 유사한 요청을 자주 제출하는 경우 제출된 기존 요청을 복사할 수 있습니다. 이 경우 기존 요청을 복사하고 최소 변경 내용을 적용한 다음 새 요청으로 다시 제출할 수 있습니다.
author: Becky
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 3%

---

# 요청 복사 및 제출


<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있습니다.</span>

유사한 요청을 자주 제출하는 경우 제출된 기존 요청을 복사할 수 있습니다. 이 경우 기존 요청을 복사하고 최소 변경 내용을 적용한 다음 새 요청으로 다시 제출할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>기여자 이상</p>
   <p>요청 이상</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문제에 대한 액세스 편집</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader">개체 권한</td> 
   <td><p>요청 대기열에 요청을 추가하는 액세스 권한</p> <p>기존 요청에 대한 이상의 권한 보기</p> <p>요청 대기열 설정에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 대기열 만들기</a>를 참조하십시오. </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader"> 제품</td> 
   <td> <ul><li>Adobe Workfront</li><li>Planning 요청 또는 요청 양식을 보려면 Adobe Workfront Planning이 있어야 합니다.</td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

귀하 또는 귀하 조직의 누군가가 이전에 제출한 요청을 복사하여 다시 제출할 수 있어야 합니다. 요청이 다른 사용자에게 속한 경우 새 요청으로 복사하고 제출하려면 보기 액세스 권한이 있어야 합니다.

## 요청을 새 요청으로 복사 및 제출하는 것에 대한 고려 사항

* 제출된 요청만 복사하고 제출할 수 있습니다. 초안 요청은 복사할 수 없습니다.
* 처음에 제출한 요청이나 다른 사람이 제출한 요청을 복사하여 제출할 수 있으며 최소한 [보기]에 액세스할 수 있습니다.
* 다른 사용자가 자신의 요청에 대한 권한을 제거하지 않은 한 해당 요청을 복사하여 제출할 수 있는 액세스 권한이 항상 있습니다.
* 요청 대기열의 작성자가 **같은 회사의 직원들이 대기열 세부 정보 또는 프로젝트 편집 영역에서 모든 요청에 대해 동일한 권한을 상속**&#x200B;할 경우 다른 사람이 원래 제출한 요청을 복사하고 제출하는 액세스 권한이 같은 회사의 직원들에게 자동으로 부여될 수 있습니다. 이 설정을 비활성화하면 원래 요청자만 자신의 요청을 볼 수 있습니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [프로젝트 편집](../../../manage-work/projects/manage-projects/edit-projects.md)

* 새 요청으로 다시 제출하기 전에 원래 요청의 사본을 업데이트할 수 있습니다.
* 원래 요청이 제출된 후에 다음 변경 사항이 발생하면 더 이상 복사하여 다시 제출할 수 없습니다.

   * 요청 대기열이 삭제되었습니다.
   * 대기열 주제가 삭제되었습니다.

     >[!TIP]
     >
     >대기열 주제가 요청 대기열에 있는 유일한 항목인 경우에도 요청을 복사하고 제출할 수 있으며 요청 대기열 자체 아래에 저장됩니다.

   * 요청 대기열이 더 이상 도움말 요청 대기열로 게시되지 않습니다. 자세한 내용은 [요청 큐 만들기](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)를 참조하세요.
   * 요청 대기열에 대기열 주제가 없고 원래 요청이 2022년 1월 이전에 제출된 경우.

   * 요청 대기열과 연결된 프로젝트의 상태가 더 이상 현재가 아닙니다.

* 요청이 변환 프로세스에서 유지된 경우 변환된 요청의 사본을 복사하여 제출할 수 있습니다. 자세한 내용은 [Adobe Workfront의 문제 전환 개요](../../../manage-work/issues/convert-issues/convert-issues.md)를 참조하십시오.

  >[!TIP]
  >
  >복사된 요청이 해결 중 오브젝트에 연결되어 있지 않습니다.

## 기존 요청 경험에서 요청 복사 및 제출

{{step1-to-requests}}

1. (조건부) 제출 섹션이 기본적으로 표시되지 않으면 왼쪽 패널에서 **제출됨**&#x200B;을(를) 클릭합니다.

   >[!TIP]
   >
   >   Workfront 또는 그룹 관리자는 레이아웃 템플릿을 사용자 정의하고 주 메뉴 또는 사용자 환경의 왼쪽 패널에서 영역을 제거할 수 있습니다. 이 경우 사용하지 못할 수 있습니다.

1. 새로 복사하여 제출할 요청을 찾은 후 다음 중 하나를 수행합니다.

   * 선택한 다음 제출된 요청 목록의 왼쪽 상단 모서리에서 **복사** ![](assets/copy-and-submit-as-new-requests-area-nwe.png)를 클릭합니다.

   >[!TIP]
   >
   > 요청을 먼저 선택하지 않은 경우 복사 아이콘이 흐리게 표시됩니다.

   * 요청 이름 오른쪽의 **자세히** 메뉴 ![](assets/more-icon.png)을(를) 클릭한 다음 **새 이름으로 복사 및 제출**&#x200B;을 클릭합니다

     또는

     선택한 요청을 마우스 오른쪽 단추로 클릭한 다음 **새 요청으로 복사 및 제출**&#x200B;을 클릭합니다.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >문제를 만들 수 있는 액세스 권한이 없는 경우 관리자가 요청 만들기를 제한했다는 경고가 표시됩니다.

1. (선택 사항) 필요한 경우 다음 정보를 갱신합니다.

   * **요청 유형**: 복사된 요청이 저장되는 요청 큐입니다. 기본적으로 복사된 요청은 원래 요청의 요청 대기열에 저장됩니다.
   * **주제 그룹** 및 **주제 대기열**(선택한 경우). 사용자 환경에 맞게 이름 또는 주제 그룹 및 대기열 주제를 사용자 정의합니다. 기본적으로 복사된 요청은 원래 요청의 주제 그룹 및 대기열 주제에 저장됩니다.

     >[!TIP]
     >
     >원래 요청의 경로에서 경로가 변경되면 요청 대기열 생성자가 대기열을 수정했습니다.

1. (선택 사항) 복사된 요청에서 모든 정보를 업데이트합니다. 요청 대기열 생성자가 프로젝트의 **대기열 세부 정보** 하위 탭의 **새 문제 필드** 섹션에서 활성화한 필드에 따라 다음 필드를 찾을 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>제목</strong> </td> 
      <td>원래 요청의 이름을 표시합니다. 필요한 경우 업데이트합니다. 그렇지 않으면 Workfront에서 복사된 요청의 이름을 <b>복사본 &lt;원본 요청 이름&gt;</b>으로 지정합니다. 필수 필드입니다.</td> 
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
        <li>일반</li> 
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
      <td role="rowheader"><strong>기본 연락처</strong> </td> 
      <td>사용자가 요청과 관련된 모든 질문을 처리할 수 있으므로 요청의 기본 연락처는 기본적으로 귀하에게 제공됩니다. 그러나 다른 Workfront 사용자로 변경할 수 있습니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>할당</strong></span> </td> 
      <td> <p>요청을 할당해야 하는 활성 사용자, 작업 역할 또는 팀의 이름을 나타냅니다. </p> <p> 두 명 이상의 사용자, 작업 역할 또는 팀을 지정할 수 있습니다. </p> <p>요청 대기열이 설정된 방법에 따라 세 가지 리소스 유형 모두 대신 하나 또는 두 가지 유형의 리소스에만 요청을 할당할 수 있습니다. </p> <p>요청 대기열을 적절한 리소스로 자동으로 라우팅할 수 있도록 라우팅 규칙을 사용하는 것이 좋습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">요청 대기열이 설정된 방법에 따라 한 가지 유형의 리소스만 요청에 할당할 수 있습니다(예: 사용자). 라우팅 규칙도 요청 대기열에 연결되어 있으며 자동으로 요청을 다른 유형의 리소스(예: 팀)로 라우팅하는 경우 요청을 제출할 때 수동으로 지정하는 엔티티(사용자)와 라우팅 규칙에 지정된 리소스(팀) 모두에 요청이 할당됩니다.</p> <p style="font-weight: normal;">자세한 내용은 다음 문서를 참조하십시오.</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a> </p> </li> 
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

1. **제출을 클릭합니다**.

   복사된 요청이 지정한 요청 대기열에 새 요청으로 제출됩니다.

<div class="preview">

## 새 요청 경험에서 요청 복사 및 제출

Workfront의 요청 영역이나 홈의 내 요청 위젯에서 요청을 복사하고 제출할 수 있습니다.

{{step1-to-requests}}

1. 홈에서 내 요청 위젯에 액세스하려면 다음을 수행하십시오.

   {{step1-to-home}}

   1. 내 요청 위젯을 찾습니다.

      내 요청 위젯에 대한 자세한 내용은 [내 요청 위젯 사용](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)을 참조하십시오.

1. 요청 목록 또는 내 요청 위젯에서 복사할 요청 위로 마우스를 가져갑니다.

   3점 추가 메뉴가 나타납니다.
   ![](assets/more-menu.png)

1. 요청 이름 오른쪽의 **자세히** 메뉴를 클릭한 다음 **복사**&#x200B;를 클릭합니다.

   또는

   선택한 요청을 마우스 오른쪽 단추로 클릭한 다음 **복사**&#x200B;를 클릭합니다.

   >[!TIP]
   >
   >문제를 만들 수 있는 액세스 권한이 없는 경우 관리자가 요청 만들기를 제한했다는 경고가 표시됩니다.

1. (선택 사항) 복사된 요청에서 모든 정보를 업데이트합니다. 사용 가능한 필드는 요청에 사용된 요청 대기열 또는 요청 양식에 따라 다릅니다.

   복사된 요청에서 필드 값을 입력하거나 변경하면 초안으로 저장됩니다.

1. **제출을 클릭합니다**.

   복사된 요청이 새 요청으로 제출됩니다.

</div>

