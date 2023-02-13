---
product-area: projects
navigation-topic: manage-issues
title: 문제 편집
description: 문제를 만든 문제 또는 다른 사용자가 사용자와 공유한 경우 만든 문제에 대한 정보를 편집할 수 있습니다.
author: Alina
feature: Work Management
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 3%

---

# 문제 편집

문제를 만든 문제 또는 다른 사용자가 사용자와 공유한 경우 만든 문제에 대한 정보를 편집할 수 있습니다.

단일 문제를 편집하거나 목록에서 문제를 편집할 수 있습니다. 목록의 문제 편집에 대한 자세한 내용은 [목록에서 문제 편집](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## 액세스 요구 사항

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
   <td> <p>요청 이상</p> <p>작업 또는 프로젝트의 문제 섹션에서 문제를 편집하는 라이선스 이상의 검토</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준*</td> 
   <td> <p>문제에 대한 액세스 편집</p> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. 액세스 수준의 문제에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">문제에 대한 액세스 권한 부여</a>. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>문제에 대한 권한을 부여하여 [문제 세부 정보] 영역에서 편집할 수 있습니다 </p> <p>문제에 대한 권한을 관리하여 문제 편집 상자에서 문제를 편집할 수 있습니다</p> <p> 문제에 대한 권한 부여에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">문제 공유 </a></p> <p>추가 권한 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 문제를 편집할 때의 제한 사항

문제를 편집하지 못하도록 하는 몇 가지 제한 사항이 있습니다.

* 승인 프로세스에 있는 문제는 편집할 수 없습니다. 승인 보류 중인 문제에 대해 시간을 기록하거나 상태를 업데이트할 수만 있습니다.
* Workfront 관리자 또는 그룹 관리자가 [프로젝트 환경 설정] 영역에서 이 기능을 활성화한 경우에만 완료, 사용 중지 또는 승인 보류 중인 프로젝트의 문제에 문서를 편집하고 추가할 수 있습니다. 프로젝트 환경 설정 설정에 대한 자세한 내용은 [시스템 전체 프로젝트 환경 설정 구성](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 단일 문제 편집

문제 편집 또는 문제 세부 정보 영역을 사용하여 문제를 편집할 수 있습니다. 다음 단계에서는 문제 편집 상자에서 문제를 편집하는 방법에 대해 설명합니다.

1. 로 이동합니다. **기본 메뉴**.
1. 클릭 **프로젝트**&#x200B;를 클릭한 다음 프로젝트 이름을 클릭하여 프로젝트를 엽니다.
1. (선택 사항) **작업** 을 클릭한 다음 작업 이름을 클릭하여 작업을 엽니다.
1. 클릭 **문제** 왼쪽 패널에 표시됩니다.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (선택 사항) 문제에 대한 제한된 정보를 편집하려면 **문제 세부 정보** 왼쪽 패널에 표시됩니다.

   ![](assets/qs-issue-details-icon-highlighted-and-expanded-on-issue-350x206.png)

   >[!NOTE]
   >
   >Workfront 관리자 또는 그룹 관리자가 레이아웃 템플릿을 수정한 방법에 따라 문제 세부 정보 영역의 필드가 재배열되거나 표시되지 않을 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   세부 정보 섹션에서 정보를 편집하려면 다음을 수행합니다.

   1. (선택 사항) **모두 축소** 오른쪽 위 모서리의 아이콘을 클릭하여 모든 영역을 축소합니다.
   1. (선택 사항 및 조건부) 영역이 축소되면 **오른쪽 화살표** ![](assets/right-pointing-arrow.png) 각 영역 옆에 있으면 편집할 영역을 확장합니다.
   1. (선택 사항) 사용자 지정 양식을 첨부하려면 **사용자 지정 양식 추가** 필드를 선택한 다음 목록에 표시될 때 선택한 다음 **변경 내용 저장**.
   1. (선택 사항) **내보내기** 아이콘 ![](assets/export.png) 개요 및 사용자 지정 양식 정보를 PDF 파일로 내보내려면 **내보내기**. 다음 중에서 선택합니다.

      * 모두 선택(하나 이상의 사용자 지정 양식이 첨부된 경우에만 표시)
      * 개요
      * 하나 이상의 사용자 지정 양식의 이름

      PDF 파일이 컴퓨터에 다운로드됩니다.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      자세한 내용은 [사용자 지정 양식 및 개체 세부 정보 내보내기](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   문제 세부 정보 섹션에 표시되는 필드에 대한 자세한 내용은 아래 설명된 대로 문제 편집 상자에서 문제를 계속 편집합니다.

1. 문제에 대한 모든 정보를 편집하려면 목록에서 문제를 선택한 다음 **편집** 목록의 맨 위에서

   또는

   목록에서 문제 이름을 클릭한 다음 **자세히** 문제 이름 옆에 있는 메뉴를 클릭한 다음 **편집.**

   다음 **문제 편집** 대화 상자가 표시됩니다.

   >[!IMPORTANT]
   >
   >편집 링크를 보려면 문제에 대한 관리 권한이 있어야 합니다.

   모든 문제 필드는 [문제 편집] 상자에서 사용할 수 있으며 왼쪽 패널에 나열된 영역으로 그룹화됩니다.

1. 다음 섹션에서 정보를 지정하는 것이 좋습니다.

   * [문제 이름](#issue-name)
   * [개요](#overview)
   * [할당](#assignments)
   * [사용자 정의 양식](#Custom%C2%A0F)
   * [설정](#settings)

   >[!NOTE]
   >
   >Workfront 관리자가 레이아웃 템플릿을 설정하는 방법에 따라 문제 편집 상자의 필드가 사용자 환경에서 다를 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 세부 사항 보기 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### 문제 이름 {#issue-name}

1. 위에 설명된 대로 문제 편집을 시작합니다.
1. 클릭 **문제 이름**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. 업데이트 **문제 이름** 필드.
1. 클릭 **저장** 또는 다음 섹션을 계속 편집합니다.

### 개요 {#overview}

1. 위에 설명된 대로 문제 편집을 시작합니다.
1. 클릭 **개요**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. 다음 테이블의 필드를 업데이트하거나 검토합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td> <p>문제에 대한 추가 정보를 추가합니다.</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">기본 정보 섹션</td> 
     </tr> 
     <tr> 
      <td role="rowheader">상태</td> 
      <td> <p>문제의 상태를 선택합니다. 문제 상태에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">시스템 문제 상태 목록에 액세스합니다</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">우선 순위</td> 
      <td> <p>문제의 우선 순위를 지정할 수 있는 시각적 플래그입니다.</p> <p>다음 옵션 중에서 선택합니다.</p> 
       <ul> 
        <li> <p><strong>없음</strong> </p> </li> 
        <li> <p><strong>낮음</strong> </p> </li> 
        <li> <p><strong>기본</strong> </p> </li> 
        <li> <p><strong>높음</strong> </p> </li> 
        <li> <p><strong>긴급</strong> </p> </li> 
       </ul> <p>Workfront 관리자가 선택한 프로젝트 환경 설정에 따라 우선순위 이름이 다를 수 있습니다. 우선순위 편집에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">우선순위 만들기 및 사용자 지정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">심각도</td> 
      <td> <p>문제에 설명된 문제가 얼마나 심각한지를 나타내는 시각적 플래그입니다. 몇 가지는 문제에만 적용됩니다. 다음 옵션 중에서 선택합니다.</p> 
       <ul> 
        <li> <p style="font-weight: bold;">표시용</p> </li> 
        <li> <p style="font-weight: bold;">혼란 야기</p> </li> 
        <li> <p style="font-weight: bold;">해결 방법이 있는 버그</p> </li> 
        <li> <p style="font-weight: bold;">해결 방법이 없는 버그</p> </li> 
        <li> <p style="font-weight: bold;">치명적인 오류</p> </li> 
       </ul> <p>Workfront 관리자가 선택한 프로젝트 환경 설정에 따라 여러 가지 기능 이름이 다를 수 있습니다. 심각도 편집에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">문제 심각도 만들기 또는 사용자 지정</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>문제에 대한 정보와 관련된 웹 링크를 입력합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">유형</td> 
      <td> <p>프로젝트의 큐 세부 정보 영역에서 프로젝트 관리자가 선택한 큐 속성에 따라 문제 유형을 지정할 수 있습니다. 의 다음 옵션 중에서 선택합니다 <b>유형</b> 드롭다운 메뉴: </p> 
       <ul> 
        <li> <p><strong>버그 신고</strong> </p> </li> 
        <li> <p><strong>순서 변경</strong> </p> </li> 
        <li> <p><strong>문제</strong> </p> </li> 
        <li> <p><strong>요청</strong> </p> </li> 
       </ul> <p>Workfront 관리자가 선택한 프로젝트 환경 설정에 따라 문제 유형의 이름이 달라질 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">기본 담당자</td> 
      <td>기본적으로 기본 연락처는 문제의 작성자입니다. 이를 수정하려면 Workfront에서 활성 사용자의 이름을 입력한 다음 목록에서 해당 이름을 선택합니다. 문제에 기본 연락처는 하나만 있을 수 있습니다.<br> 기본 연락처를 변경하면 원래 기본 연락처는 여전히 문제에 대한 관리 액세스 권한을 갖습니다. 문제를 공유할 때 문제 액세스 상자에서 이 액세스를 수동으로 제거해야 합니다.

   <b>팁</b>

   기본 연락처 사용자를 추가할 때 아바타, 사용자의 기본 역할 및 이메일 주소를 확인하여 동일한 이름을 사용하는 사용자를 구별하십시오. 사용자를 추가할 때 해당 역할을 보려면 사용자를 하나 이상의 작업 역할과 연결해야 합니다.


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">커밋 날짜 및 시간</td> 
      <td> <p>문제 할당자가 문제가 완료될 것으로 예상되는 날짜입니다. 할당된 사람만 이 필드를 편집할 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획 시작 날짜</td> 
      <td>기본적으로 계획 시작 일자는 문제가 생성된 날짜 및 시간입니다. 을(를) 업데이트할 수 있습니다 <strong>계획 시작 날짜</strong> 문제. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계획 완료 날짜 및 시간</td> 
      <td> 기본적으로 계획 완료 일자는 기본 계획 시작 일자부터 24시간입니다. 기본적으로 문제는 1일입니다. 을(를) 업데이트할 수 있습니다 <strong>계획 완료 일자</strong> 문제.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 시작 날짜 및 시간</td> 
      <td>문제의 상태를 로 변경하면 실제 시작 날짜가 자동으로 채워집니다 <strong>진행 중</strong>. 을(를) 업데이트할 수 있습니다 <strong>실제 시작 날짜</strong> 문제. 필요한 경우 날짜를 수동으로 업데이트할 수 있습니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">실제 완료 날짜 및 시간</td> 
      <td>문제의 상태를 로 변경하면 실제 완료 날짜가 자동으로 채워집니다 <strong>닫힘</strong> 또는<strong>해결됨</strong>. 을(를) 업데이트할 수 있습니다 <strong>실제 완료 날짜</strong> 참조하십시오. 필요한 경우 날짜를 수동으로 업데이트할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">해결한 사람</td> 
      <td> <p>다른 개체에서 문제가 해결되었는지 여부를 보여줍니다. 드롭다운 메뉴에서 이 문제가 작업, 프로젝트 또는 다른 문제로 해결되는지 여부를 선택한 다음 문제를 해결할 작업, 프로젝트 또는 문제의 이름을 입력할 수 있습니다. 목록에 있으면 선택합니다.</p>

   <b>메모</b>

   문제를 해결할 개체를 선택하면 문제 상태가 해결 개체의 상태에 연결되므로 문제 시 변경할 수 없습니다. 개체 해결에 대한 자세한 내용은 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">해결 가능한 객체 해결 및 해결 방법 개요 </a>.

   <b>팁</b>

   시스템 또는 그룹 관리자가 문제 사용자 지정 헤더에 &quot;해결된 사람&quot; 필드를 추가하면 문제와 연관된 해결 개체가 있으면 필드가 &quot;문제 해결&quot;, &quot;작업 해결&quot; 또는 &quot;프로젝트 해결&quot;으로 변경됩니다.

   이 필드가 문제 헤더에 표시되면 편집할 수 없습니다. 문제 헤더 사용자 지정에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정 </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">문제 해결, 작업 해결 또는 프로젝트 해결</td> 
      <td>문제를 해결하는 문제, 작업 또는 문제의 연결된 이름입니다.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">해결됩니다</td> 
      <td>액세스 중인 문제가 해결되면 완료되는 문제에 대한 연결된 이름입니다.  </td> 
     </tr>


   </tbody> 
   </table>





1. 클릭 **저장** 또는 다음 섹션을 계속 편집합니다.

#### 할당 {#assignments}

1. 위에 설명된 대로 문제 편집을 시작합니다.
1. 클릭 **지정** 왼쪽 패널에 표시됩니다.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. 클릭 **사람, 역할 및 팀 검색** 작업을 지정할 사용자, 역할 또는 팀의 이름을 입력하고 작업을 클릭하거나 목록에 표시되면 Enter 키를 누릅니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >사용자 이름에 특수 문자가 포함되어 있으면 검색 필드에 특수 문자를 포함해야 합니다.

   >[!TIP]
   >
   >여러 사용자, 작업 역할 또는 팀을 할당할 수 있습니다. 활성 사용자, 작업 역할 및 팀만 할당할 수 있습니다.
   >
   >
   >사용자, 작업 역할 또는 팀이 비활성화되기 전에 지정된 경우 작업 항목에 지정된 상태로 유지됩니다. 이 경우 다음을 권장합니다.
   >
   >* 작업 항목을 활성 자원에 재지정합니다.
   >* 비활성화된 팀의 사용자를 활성 팀과 연결하고 작업 항목을 활성 팀에 재할당합니다.


1. (선택 사항) 할당자의 이름을 마우스로 가리키고 를 클릭하여 할당자가 문제의 기본 할당자인지 여부를 나타냅니다 **기본 구성**. 팀은 문제의 주요 할당자가 될 수 없습니다.
1. 다음 필드를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">계획된 시간</td> 
      <td> <p>이 시간은 문제를 완료하는 데 걸린 실제 시간입니다. 문제에 대한 계획된 시간 수를 입력합니다.<br></p> <p>참고: 문제의 계획 시간 변경은 계획 완료 일자를 변경하지 않습니다. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">할당자의 역할</td> 
      <td> <p>에서 역할 선택 <strong>할당자의 역할</strong> 담당자를 할당자로 선택한 경우 드롭다운 메뉴. 이는 할당자가 이 문제에 대해 수행할 수 있는 역할입니다. </p> <p><b>팁</b>

   프로필의 각 할당자와 연관된 작업 역할만 드롭다운 메뉴에 나타납니다.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. 클릭 **저장** 또는 다음 섹션을 계속 편집합니다.

### 사용자 지정 Forms

1. 위에 설명된 대로 문제 편집을 시작합니다.
1. 클릭 **사용자 지정 Forms**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. 에서 **사용자 지정 양식 추가** 필드에서 문제와 연결할 사용자 지정 양식이나 양식을 선택합니다. 이 필드에서 사용자 지정 양식을 선택하려면 먼저 사용자 지정 양식을 작성해야 합니다. 활성 사용자 지정 양식만 목록에 표시됩니다. 사용자 지정 양식 작성에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 문제에 최대 10개의 사용자 지정 양식을 추가할 수 있습니다.

1. (조건부) 문제에 사용자 지정 양식을 첨부한 경우 양식의 필드를 편집합니다. 문제를 저장하려면 먼저 모든 필수 필드를 지정해야 합니다.

   >[!NOTE]
   >
   >Workfront 관리자가 사용자 지정 양식의 섹션에 대한 권한을 설정하는 방법에 따라 모든 사람이 주어진 사용자 지정 양식에서 동일한 필드를 보거나 편집할 수 있는 것은 아닙니다. 사용자 지정 양식의 섹션 내에서 필드를 편집할 수 있는 권한은 문제 자체에 대한 사용 권한에 따라 다릅니다. 사용자 지정 양식의 섹션에 대한 권한 설정에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 문제 권한 설정에 대한 자세한 내용은 [문제 공유](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. 클릭 **저장** 또는 다음 섹션을 계속 편집합니다.

### 설정 {#settings}

1. 위에 설명된 대로 문제 편집을 시작합니다.
1. 클릭 **설정**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   다음 정보를 업데이트합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">승인 진행</td> 
      <td> 
       <div> 
       <p>문제와 연결할 승인 프로세스를 선택합니다. 문제와 연결하려면 먼저 Workfront 관리자가 시스템 수준 승인 프로세스를 정의해야 합니다. 승인 프로세스에 대한 관리자 액세스 권한이 있는 사용자 <span> 그룹별 승인 프로세스를 만들 수도 있습니다.</span>승인 프로세스 생성에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">작업 항목에 대한 승인 프로세스 생성</a>. </p> 
       <p>승인 프로세스를 추가할 때 다음 사항을 고려하십시오. </p> 
       <ul> 
       <li>활성 승인 프로세스만 목록에 표시됩니다. </li> 
       <li> <p>시스템 전체 및 그룹별 승인 프로세스가 목록에 표시됩니다. 프로젝트 이외의 그룹과 연관된 승인 프로세스가 목록에 표시되지 않습니다.</p> <p>중요 사항: 프로젝트 그룹이 변경되면 그룹별 승인 프로세스는 단일 사용 승인 프로세스가 됩니다. 프로젝트 그룹의 변경 사항이나 승인 프로세스의 변경 사항이 승인 설정에 미치는 영향에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">그룹 및 승인 프로세스 변경이 지정된 승인 프로세스에 미치는 영향</a>. </p> </li> 
       <li> <p>요청 큐 또는 큐 항목을 만들 때 문제에 자동으로 첨부할 기본 승인 프로세스를 정의할 수 있습니다. 큐 세부 정보 업데이트에 대한 자세한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">요청 큐 만들기</a>. 큐 항목 만들기에 대한 내용은 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">큐 항목 만들기</a>. </p> </li> 
       <li>벌크 편집 문제가 발생하면 다음 시나리오가 있습니다. 
       <ul> 
       <li><p>동일한 그룹에서 여러 문제를 선택하면 시스템 레벨과 그룹별 승인 프로세스가 모두 이 필드에 표시됩니다.</p></li> 
       <li><p>여러 그룹에서 여러 문제를 선택하면 시스템 수준 승인 프로세스만 이 필드에 표시됩니다.</p></li> 
       <li><p>문제에 단일 사용 승인 프로세스가 첨부된 경우 선택한 시스템 수준 또는 그룹 수준 승인 프로세스로 대체됩니다. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">미리 알림</td> 
      <td> <p>이 문제에 첨부할 알림 확인란을 선택합니다. 문제에 대한 모든 미리 알림 알림이 표시됩니다. 문제에 대해 알림 을 선택하려면 Workfront 관리자가 미리 알림 알림을 구성해야 합니다. 미리 알림 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">미리 알림 설정</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 클릭 **저장.**

## 문제 헤더에서 문제 편집(제한)

문제 헤더에서 제한된 양의 정보를 편집할 수 있습니다.

시스템 또는 그룹 관리자는 문제 헤더에 표시되는 필드를 사용자 지정할 수 있습니다. 자세한 내용은 [레이아웃 템플릿을 사용하여 개체 머리글 사용자 지정](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

기본적으로 다음 필드가 문제 헤더에 포함되어 있습니다.

* 문제 이름
* 완료율
* 할당
* 계획 완료 날짜 및 시간
* 상태
* 현재 승인 프로세스에서 승인자로 설정된 경우 승인 결정을 수행합니다
