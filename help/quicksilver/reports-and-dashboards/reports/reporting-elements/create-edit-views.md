---
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront에서 보기 만들기 또는 편집
description: 뷰를 사용하여 화면에 표시하는 정보의 유형을 사용자 정의할 수 있습니다. Adobe Workfront에서는 여러 유형의 보기를 사용할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# Adobe Workfront에서 보기 만들기 또는 편집

뷰를 사용하여 화면에 표시하는 정보의 유형을 사용자 정의할 수 있습니다. Adobe Workfront에서는 여러 유형의 보기를 사용할 수 있습니다.

이 문서에서는 목록 및 보고서에 대한 표준 보기를 만들고 편집하는 방법, 애자일 보기를 만드는 방법에 대해 설명합니다. 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 달력에 대한 액세스를 편집하여 보고서에서 보기를 만듭니다</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>보고서에 대한 권한을 관리하여 보고서에서 보기를 만들거나 편집합니다</p> <p>보기에 대한 권한을 관리하여 편집합니다</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 보기 만들기 또는 사용자 지정

보기를 만들거나 사용자 지정하는 프로세스는 표준 보기를 만들거나 사용자 정의하는지 또는 애자일 보기를 만드는지에 따라 다릅니다.

* [표준 보기 만들기 또는 사용자 지정](#create-or-customize-a-standard-view)
* [애자일 뷰 만들기 또는 사용자 정의](#create-or-customize-an-agile-view)

### 표준 보기 만들기 또는 사용자 지정 {#create-or-customize-a-standard-view}

새 표준 보기를 만들거나 이전에 만든 기존 표준 보기를 사용자 지정할 수 있습니다.

1. 을(를) 클릭합니다. **보기** 보기를 만들거나 사용자 지정할 목록의 드롭다운 메뉴.
1. (선택 사항) 기존 보기를 사용자 지정하려면 사용자 지정할 표준 보기를 선택합니다.\
   표준 보기는 보고서, 프로젝트 목록 또는 작업 목록과 같은 Workfront의 모든 유형의 목록에서 사용할 수 있습니다.
1. 을(를) 클릭합니다. **보기** 드롭다운 메뉴를 클릭한 다음 **보기 사용자 지정** 또는 **새 보기**.\
   다음 **보기 사용자 지정** 대화 상자가 표시됩니다.

1. 에서 **열 미리 보기** 섹션에서 다음 중 하나를 수행합니다.

   * 열 제목을 클릭한 다음 새 필드를 선택하여 열의 값을 수정합니다.
   * 다음을 클릭하여 열 추가 **열 추가**&#x200B;추가할 열의 이름을 입력하고 드롭다운 목록에 있으면 클릭합니다.
   * 열 제목을 새 위치로 드래그하여 열이 표시되는 순서를 조정합니다.

      * (선택 사항)에서 **열 설정** 영역에서 **다음 방법으로 이 열 요약** 드롭다운 목록에서 정보를 요약하는 데 사용할 수 있는 옵션 중 하나를 선택합니다. 이 옵션을 선택하면 열의 정보가 보고서 그룹으로 집계됩니다.\
         날짜 필드의 경우 다음 선택 사항으로 값을 요약할 수 있습니다.

         * 최대
         * 최소

         숫자 및 통화 필드의 경우 다음 선택 사항으로 값을 요약할 수 있습니다.

         * 수
         * Sum
         * 평균
         * 최대
         * 최소

         >[!NOTE]
         >
         >다음 필드에 대한 값을 그룹화하면 상위 객체(예: 상위 작업)에 다음 예외가 적용됩니다.
         >   
         >   * 실제 시간(예: 계획/실제 노무비, 계획/실제 비용, 계획/실제 비용, 계획/실제 비용, 계획 시간)을 제외한 모든 숫자 및 통화 필드는 하위 태스크 및 독립형 태스크에 대한 값만 집계합니다. 상위 작업 또는 상위 항목에 대한 값을 집계하지 않습니다.
         >   * 실제 시간은 주 상위 및 독립형 작업의 값을 집계합니다. 상위 작업 또는 하위 작업의 상위 항목에 대한 숫자를 집계하지 않습니다.
         >   * 숫자 및 통화 값에 대한 사용자 지정 데이터 필드는 모든 작업을 집계합니다. 부모, 자녀, 부모의 부모 및 독립형 작업


         보고서에서 그룹화를 사용하는 방법에 대한 자세한 내용은 문서를 참조하십시오 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (선택 사항) **고급 옵션** 열에 대해 다음 정보를 지정하려면

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>사용자 정의 열 레이블</strong></td> 
           <td><p>열에 대한 사용자 지정 레이블을 지정합니다. 이 레이블은 기본 레이블을 대체합니다.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>필드 형식</strong></td> 
           <td>열의 필드에 값을 표시할 형식을 선택합니다.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>대시보드에 있을 때 이 열 표시</strong></td> 
           <td><p>보고서가 다른 보고서와 나란히 표시될 때 대시보드에 이 열을 표시하려면 이 옵션을 선택합니다. 이 옵션을 선택하지 않으면 보고서가 나란히 표시되는 대시보드에서 보고서를 볼 때에는 이 열이 표시되지 않습니다.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>열 규칙</strong></td> 
           <td><p>클릭 <strong>이 열에 대한 규칙 추가</strong> 를 눌러 열에 대한 규칙을 정의합니다. 규칙을 추가한 후 해당 규칙과 일치하는 필드가 표시되는 방식에 대한 필드 및 텍스트 스타일을 정의할 수 있습니다. 클릭 <strong>규칙 추가</strong> 규칙 정의를 완료하면 됩니다.</p></td> 
          </tr> 
         </tbody> 
        </table>

         보고서에서 조건부 보기 서식에 대한 자세한 내용은 문서를 참조하십시오 [텍스트 모드에서 조건부 서식 사용](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).



1. (조건부) **고급 옵션**&#x200B;를 클릭합니다. **완료**.

1. 클릭 **보기 저장** 새 뷰를 만들거나 현재 뷰를 변경 사항으로 바꿉니다.\
   또는\
   클릭 **새 보기로 저장** 변경 사항을 새 보기로 저장

   >[!TIP]
   >
   >다음 **새 보기로 저장** 기본 제공 Workfront 보기를 사용자 지정할 때 사용할 수 있는 유일한 선택 사항입니다.

   액세스가 뷰가 저장되는 방식을 지시합니다. 원래 뷰를 생성한 경우에는 변경 사항을 저장할 수 있습니다. 그렇지 않으면 버전을 저장하라는 메시지가 표시됩니다. 보기에 대한 변경 사항은 보기가 공유된 사용자에게 영향을 줍니다.

### 애자일 뷰 만들기 또는 사용자 정의 {#create-or-customize-an-agile-view}

새로운 애자일 뷰를 생성하거나 이전에 생성한 기존 애자일 뷰를 사용자 정의할 수 있습니다.

>[!IMPORTANT]
>
>애자일 보기는 프로젝트를 볼 때만 사용할 수 있습니다.

애자일 보기에 대한 자세한 내용은 문서를 참조하십시오 [Agile 보기에서 프로젝트 관리](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

애자일 뷰를 생성하거나 사용자 정의하려면

1. 프로젝트의 작업 목록으로 이동합니다.
1. 을(를) 클릭합니다. **애자일 스토리보드** 아이콘 ![](assets/agile-storyboard-nwe.png).

1. (조건부) 기존 Agile 보기를 사용자 정의하려면

   1. 을(를) 클릭합니다. **보기** 드롭다운 메뉴를 선택한 다음 사용자 지정할 Agile 보기를 선택합니다.\
      기본 Agile 보기를 사용자 지정할 수 없습니다.

   1. 을(를) 클릭합니다. **보기** 드롭다운 메뉴를 다시 클릭한 다음 **보기 사용자 지정**.\
      ![](assets/view-agile-customize.png)

1. (조건부) 새 애자일 보기를 만들려면 **새 보기**.\
   다음 **Agile 보기 사용자 정의** 대화 상자가 표시됩니다.

1. 에서 **Agile 보기 사용자 정의** 대화 상자에서 애자일 뷰의 이름을 지정합니다.\
   보기 이름에 &quot;Agile&quot;이라는 단어를 포함하는 것이 좋습니다. 따라서 사용자는 이것이 Agile 보기임을 알 수 있습니다.\
   이 이름은 **보기** 보기를 선택할 때 드롭다운 메뉴

1. 애자일 보기에서 스토리 보드에 표시할 상태 열을 정의합니다. 다음은 Workfront 관리자가 정의한 작업 상태입니다. [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   애자일 스토리 보드에서 시스템 상태만 사용할 수 있습니다. 사용자가 속한 개별 그룹에만 상태를 사용할 수 있는 경우, 애자일 스토리 보드에서 상태를 사용할 수 없습니다. 또한 사용자 지정 그룹에서만 사용할 수 있는 상태인 작업은 Agile 보기에서 프로젝트를 볼 때 표시되지 않습니다.

   사용자는 애자일 스토리 보드의 이러한 상태 열 간에 스토리를 이동할 수 있습니다.\
   상태 열을 정의할 때 다음을 수행할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>상태 열 재정렬:</strong> </td> 
      <td> 상태 열을 표시할 순서로 드래그합니다.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태 열 제거:</strong> </td> 
      <td>제거할 열에서 (x) 아이콘을 클릭합니다.<br>사용자 지정 상태가 보기에 추가되고 해당 사용자 지정 상태가 "새로 만들기"와 같지 않으면 "새로 만들기" 상태를 제거할 수 없습니다.<br>사용자 지정 상태 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태 열 추가:</strong> </td> 
      <td> <p>을(를) 클릭합니다. <strong>플러스</strong> 아이콘을 클릭한 다음 추가할 상태를 선택합니다.<br>모든 기본 시스템 상태와 사용자와 공유된 사용자 정의 상태가 표시됩니다.<br>표시할 상태를 최대 10개까지 구성할 수 있습니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. 에서 **카드 색상 연결** 영역에서 다음 선택 사항 중에서 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>스토리:</strong> </td> 
      <td>모든 하위 작업은 상위 작업의 색상과 일치하므로 지정된 모든 수영장에 있는 모든 스토리의 색상이 동일합니다.<br>작업에 하위 작업이 없거나 상위 작업이 없는 경우 색상이 작업을 만들 때 작업에 임의로 할당됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>자유 양식:</strong> </td> 
      <td> 문서에 설명된 대로 사용자가 수동으로 색상을 변경할 때까지 기본적으로 모든 카드가 파란색으로 표시됩니다 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">스크럼 보드의 색상별로 이야기를 분류합니다</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>우선 순위:</strong> </td> 
      <td> <p> 색상은 다음과 같이 스토리 우선 순위와 연결됩니다.</p> 
       <ul> 
        <li>높음 = 빨강</li> 
        <li>보통 = 노란색</li> 
        <li>낮음 = 녹색<br>Workfront 관리자가 Workfront 시스템에 대해 사용자 지정 우선 순위를 구성한 경우 가장 높은 우선 순위는 빨간색이고 두 번째 우선 순위는 노란색이며 나머지 부분은 녹색입니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>작업 소유자:</strong> </td> 
      <td> 기본 할당자가 같은 모든 스토리는 동일한 색입니다.<br>기본 할당자는 작업에 처음 할당된 사용자입니다. </td> 
     </tr> 
    </tbody> 
   </table>

1. 에서 **애자일** 섹션, **추가 필드** 영역을 클릭합니다. **필드 추가**&#x200B;그런 다음 스토리 카드에 추가할 필드를 선택합니다. (이 필드는 보기를 사용자 지정하거나 보고서에 대한 열을 만들 때 추가할 수 있는 필드와 동일합니다.)\
   이 프로세스를 반복하여 스토리 카드에 최대 3개의 필드를 추가합니다.\
   스토리 카드에 필드를 추가할 때 필드는 보기 전용이며 필드가 채워지는 경우에만 표시됩니다.

   기본적으로 스토리 카드에 다음과 같은 유형의 데이터가 표시됩니다.

   * 작업에 직접 연결되는 링크가 있는 스토리 이름
   * 프로젝트에 직접 연결되는 링크가 있는 프로젝트 이름\
      이 링크는 반복에서 애자일 보기를 사용할 때만 표시됩니다. 프로젝트에서 Agile 보기를 사용할 때는 표시되지 않습니다.
   * 작업 설명
   * 현재 약정
   * 완료 퍼센트를 직접 조정하거나 완료된 포인트 또는 시간 수를 조정하여 완료 비율을 보고 편집합니다
   * 할당된 사용자

   스토리 카드에 추가 데이터(사용자 지정 데이터 포함)를 표시할 수 있습니다. 여러 가지 이유로 스토리 카드에 추가 필드를 표시할 수 있습니다. 예를 들어, 프로젝트 내에서 여러 고객을 위한 스토리에 작업하거나 작업 시작 날짜를 표시하려는 경우 고객 ID를 표시할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.\
   액세스가 뷰가 저장되는 방식을 지시합니다. 원래 뷰를 생성한 경우에는 변경 사항을 저장할 수 있습니다. 그렇지 않으면 버전을 저장하라는 메시지가 표시됩니다. 보기에 대한 변경 사항은 보기가 공유된 사용자에게 영향을 줍니다.

1. (선택 사항) **목록 보기** 아이콘 ![](assets/list-view-in-agile-view-for-tasks.png) 작업 목록으로 돌아갑니다.
