---
product-area: reporting
navigation-topic: reporting-elements
title: Adobe Workfront에서 보기 만들기 또는 편집
description: 보기를 사용하여 화면에 표시할 정보 유형을 사용자 정의할 수 있습니다. Adobe Workfront에서 여러 유형의 보기를 사용할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 1%

---

# Adobe Workfront에서 보기 만들기 또는 편집

<!-- Audited: 11/2024 -->

보기를 사용하여 화면에 표시할 정보 유형을 사용자 정의할 수 있습니다. Adobe Workfront에서 여러 유형의 보기를 사용할 수 있습니다.

이 문서에서는 목록 및 보고서에 대한 표준 보기를 만들고 편집하는 방법과 애자일 보기를 만드는 방법을 설명합니다. 자세한 내용은 [Adobe Workfront의 보기 개요](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 플랜</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront 라이센스*</strong></td> 
   <td> 
      <p>신규:</p>
         <ul>
         <li><p>기여자 이상</p></li>
         </ul>
      <p>현재:</p>
         <ul>
         <li><p>요청 이상</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>필터, 보기, 그룹화에 대한 액세스 편집</p> <p>보고서, 대시보드, 캘린더에 대한 액세스 권한을 편집하여 보고서에서 보기 만들기</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한*</strong></td> 
   <td> <p>보고서에서 보기를 만들거나 편집하려면 보고서에 대한 권한 관리</p> <p>보기에 대한 편집 권한 관리</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 보기 만들기 또는 사용자 지정

표준 보기를 작성하는지 또는 애자일 보기를 작성하는지 여부에 따라 보기를 작성하거나 사용자 정의하는 프로세스가 다릅니다.

* [표준 보기 만들기 또는 사용자 지정](#create-or-customize-a-standard-view)
* [애자일 보기 만들기 또는 사용자 지정](#create-or-customize-an-agile-view)

### 표준 보기 만들기 또는 사용자 지정 {#create-or-customize-a-standard-view}

새 표준 뷰를 생성하거나 이전에 생성한 기존 표준 뷰를 사용자 정의할 수 있습니다.

1. 보기를 만들거나 사용자 지정할 목록에서 **보기** 드롭다운 메뉴를 클릭합니다.

1. 새 보기를 만들려면 **+ 새 보기** 단추를 클릭하십시오.
또는
편집할 기존 보기의 오른쪽 마우스에 표시되는 **편집** 아이콘 ![편집 아이콘](assets/edit-icon.png)을 클릭합니다.
**보기 사용자 지정** 대화 상자가 표시됩니다.

1. **열 미리 보기** 섹션에서 다음 중 하나를 수행합니다.

   * 열 제목을 클릭한 다음 새 필드를 선택하여 열의 값을 수정합니다.
   * **열 추가**&#x200B;를 클릭하여 열을 추가하고 추가할 열의 이름을 입력한 다음 드롭다운 목록에 나타나면 해당 열을 클릭합니다.
   * 열 제목을 새 위치로 끌어 열 표시 순서를 조정합니다.

      * (선택 사항) **열 설정** 영역에서 **이 열을 다음 기준으로 요약** 드롭다운 목록을 클릭한 다음, 정보를 요약하는 데 사용할 수 있는 옵션 중 하나를 선택하십시오. 이 옵션을 선택하면 열의 정보가 보고서 그룹화로 집계됩니다.\
        날짜 필드의 경우 다음 옵션으로 값을 요약할 수 있습니다.

         * 최대
         * 최소

        숫자 및 통화 필드의 경우 다음 옵션으로 값을 요약할 수 있습니다.

         * 개수
         * 합계
         * 평균
         * 최대
         * 최소

        >[!NOTE]
        >
        >그룹화에서 다음 필드의 값을 합산하는 경우 상위 객체(예: 상위 작업)에 다음 예외가 적용됩니다.
        >   
        >   * 실제 시간을 제외한 모든 숫자 및 통화 필드(예: 계획된/실제 인건비, 계획된/실제 경비, 계획된/실제 원가, 계획된 시간)는 하위 태스크 및 독립형 태스크에 대한 값만 집계합니다. 상위 작업 또는 상위 작업의 값을 집계하지 않습니다.
        >   * 실제 시간은 기본 상위 작업과 독립형 작업에 대한 값을 집계합니다. 상위 작업 또는 하위 작업의 상위 작업에 대한 값은 집계하지 않습니다.
        >   * 숫자 및 통화 값에 대한 사용자 정의 데이터 필드는 상위, 1차 하위 구성요소, 1차 상위 구성요소 및 독립 실행형 작업과 같은 모든 작업을 집계합니다.
        >   
        >

        보고서에서 그룹화를 사용하는 방법에 대한 자세한 내용은 문서 [Adobe Workfront의 그룹화 개요](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)를 참조하십시오.

      * (선택 사항) 열에 대해 다음 정보를 지정하려면 **고급 옵션**&#x200B;을 클릭합니다.

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
           <td><p>보고서가 다른 보고서와 나란히 표시되는 경우 대시보드에 이 열을 표시하려면 이 옵션을 선택합니다. 이 옵션을 선택하지 않으면 보고서가 나란히 표시되는 대시보드에서 보고서를 볼 때 이 열이 표시되지 않습니다.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>열 규칙</strong></td> 
           <td><p><strong>+ 이 열에 대한 규칙 추가</strong>를 클릭하여 열에 대한 규칙을 정의합니다. 규칙을 추가한 후 해당 규칙과 일치하는 필드가 표시되는 방식에 대한 필드 및 텍스트 스타일을 정의할 수 있습니다. 규칙 정의를 마치면 <strong>규칙 추가</strong>를 클릭합니다.</p></td> 
          </tr> 
         </tbody> 
        </table>

        보고서의 조건부 서식 보기에 대한 자세한 내용은 문서 [텍스트 모드에서 조건부 서식 사용](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)을 참조하십시오.

1. (조건부) **고급 옵션**&#x200B;을 클릭한 경우 **완료**&#x200B;를 클릭합니다.

1. 새 보기를 만들거나 현재 보기를 변경 내용으로 바꾸려면 **보기 저장**&#x200B;을 클릭하세요.\
   또는\
   **새 보기로 저장**&#x200B;을 클릭하여 변경 내용을 새 보기로 저장합니다.

   >[!TIP]
   >
   >기본 제공 Workfront 보기를 사용자 지정할 때 사용할 수 있는 옵션은 **새 보기로 저장**&#x200B;뿐입니다.

   액세스 권한에 따라 보기가 저장되는 방법이 결정됩니다. 원래 뷰를 생성한 경우 변경 사항을 저장할 수 있습니다. 그렇지 않으면 버전을 저장하라는 메시지가 표시됩니다. 보기에 대한 변경 내용은 보기가 공유된 사용자에게 영향을 줍니다.

### 애자일 보기 만들기 또는 사용자 지정 {#create-or-customize-an-agile-view}

애자일 보기를 만들거나 이전에 만든 기존 애자일 보기를 사용자 정의할 수 있습니다.

>[!IMPORTANT]
>
>애자일 보기는 프로젝트를 볼 때만 사용할 수 있습니다.

애자일 보기에 대한 자세한 내용은 문서 [애자일 보기에서 프로젝트 관리](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)를 참조하십시오.

>[!NOTE]
>
>이 절차는 프로젝트의 보드 보기가 아닌 레거시 애자일 보기에만 적용됩니다.

애자일 보기를 생성하거나 사용자 정의하려면

1. 프로젝트의 작업 목록으로 이동합니다.
1. **게시판** 아이콘 ![게시판 아이콘](assets/board-icon-for-agile-view.png)을 클릭한 다음 게시판 보기에서 **기존 애자일 사용**&#x200B;을 클릭합니다.

1. (조건부) 기존 애자일 보기를 사용자 정의하려면 다음을 수행합니다.

   1. **보기** 드롭다운 메뉴를 클릭한 다음 사용자 지정할 애자일 보기를 선택합니다.\
      기본 애자일 보기는 사용자 정의할 수 없습니다.

   1. **보기** 드롭다운 메뉴를 다시 클릭한 다음 **보기 사용자 지정**&#x200B;을 클릭합니다.\
      ![](assets/view-agile-customize.png)

1. (조건부) 새 애자일 보기를 만들려면 **새 보기**&#x200B;를 클릭합니다.\
   **애자일 보기 사용자 지정** 대화 상자가 표시됩니다.

1. **애자일 보기 사용자 지정** 대화 상자에서 애자일 보기의 이름을 지정합니다.\
   사용자가 이것이 애자일 보기임을 알 수 있도록 보기 이름에 &quot;애자일&quot;이라는 단어를 포함하는 것이 좋습니다.\
   보기를 선택하면 **보기** 드롭다운 메뉴에 이 이름이 표시됩니다.

1. 애자일 보기의 스토리 보드에 표시할 상태 열을 정의합니다. [상태 만들기 또는 편집](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)에 설명된 대로 Workfront 관리자가 정의한 작업 상태입니다.

   애자일 스토리 보드에서는 시스템 상태만 사용할 수 있습니다. 구성원인 개별 그룹에 대해서만 상태를 사용할 수 있는 경우 애자일 스토리 보드에서 상태를 사용할 수 없습니다. 또한 사용자 정의 그룹에만 사용할 수 있는 상태의 작업은 애자일 보기에서 프로젝트를 볼 때 표시되지 않습니다.

   사용자는 애자일 스토리 보드에서 이러한 상태 열 간에 스토리를 이동할 수 있습니다.\
   상태 열을 정의할 때 다음을 수행할 수 있습니다.

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>상태 열 순서 바꾸기:</strong> </td> 
      <td> 상태 열을 표시하려는 순서로 드래그합니다.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태 열 제거:</strong> </td> 
      <td>제거할 열의 (x) 아이콘을 클릭합니다.<br>사용자 지정 상태가 보기에 추가되어 있고 해당 사용자 지정 상태가 "새로 만들기"와 같지 않으면 "새로 만들기" 상태를 제거할 수 없습니다.<br>사용자 지정 상태 만들기에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">상태 만들기 또는 편집</a>을 참조하세요.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>상태 열 추가:</strong> </td> 
      <td> <p><strong>더하기</strong> 아이콘을 클릭한 다음 추가할 상태를 선택합니다.<br>모든 기본 시스템 상태와 사용자와 공유된 사용자 지정 상태가 표시됩니다.<br>표시할 상태를 최대 10개까지 구성할 수 있습니다.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. **카드 색상을**&#x200B;과(와) 연결 영역에서 다음 옵션 중 하나를 선택하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>스토리:</strong> </td> 
      <td>모든 하위 작업은 상위 작업의 색상과 일치하므로 주어진 수영장에 있는 모든 스토리의 색상은 동일합니다.<br>작업에 하위 작업이 없거나 상위 작업이 없는 경우 작업이 만들어지면 작업에 색상이 임의로 할당됩니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>자유 형식:</strong> </td> 
      <td> 사용자가 색상을 수동으로 변경할 때까지 문서 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">스크럼 보드에서 색상별로 스토리 분류</a>에 설명된 대로 모든 카드는 기본적으로 파란색으로 표시됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>우선 순위:</strong> </td> 
      <td> <p> 색상은 다음과 같이 스토리 우선 순위와 연결됩니다.</p> 
       <ul> 
        <li>높음 = 빨간색</li> 
        <li>Medium = 노란색</li> 
        <li>낮음 = 녹색<br>Workfront 관리자가 Workfront 시스템에 대해 사용자 지정 우선 순위를 구성한 경우, 가장 높은 우선 순위는 빨간색이고 두 번째 높은 우선 순위는 노란색이며 나머지 우선 순위는 녹색입니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>작업 소유자:</strong> </td> 
      <td> 기본 할당자가 동일한 모든 스토리의 색은 동일합니다.<br>기본 피할당자는 작업에 처음 할당된 사용자입니다. </td> 
     </tr> 
    </tbody> 
   </table>

1. **추가 필드** 영역에서 **필드 추가**&#x200B;를 클릭한 다음 스토리 카드에 추가할 필드를 선택합니다. (이는 보기를 사용자 정의하거나 보고서에 대한 열을 만들 때 추가할 수 있는 필드와 동일합니다.)\
   이 프로세스를 반복하여 스토리 카드에 최대 3개의 추가 필드를 추가합니다.\
   스토리 카드에 필드를 추가할 때 필드는 보기 전용이며 필드가 채워질 때만 표시됩니다.

   기본적으로 스토리 카드에는 다음 유형의 데이터가 표시됩니다.

   * 작업에 직접 연결된 링크가 있는 스토리 이름
   * 프로젝트에 직접 연결되는 링크가 있는 프로젝트 이름\
     이 링크는 반복에서 애자일 보기를 사용할 때만 표시되고, 프로젝트에서 애자일 보기를 사용할 때는 표시되지 않습니다.
   * 작업 설명
   * 현재 약정
   * 완료율 자체를 조정하거나 완료된 점수 또는 시간을 조정하여 완료율을 조회 및 편집합니다.
   * 할당된 사용자

   스토리 카드에 추가 데이터(사용자 정의 데이터 포함)를 표시할 수 있습니다. 여러 가지 이유로 스토리 카드에 추가 필드를 표시할 수 있습니다. 예를 들어, 프로젝트 내에서 여러 고객에 대한 스토리를 작업하는 경우 고객 ID를 표시하거나 작업 시작 날짜를 표시할 수 있습니다.

1. **저장**&#x200B;을 클릭합니다.\
   액세스 권한에 따라 보기가 저장되는 방법이 결정됩니다. 원래 뷰를 생성한 경우 변경 사항을 저장할 수 있습니다. 그렇지 않으면 버전을 저장하라는 메시지가 표시됩니다. 보기에 대한 변경 내용은 보기가 공유된 사용자에게 영향을 줍니다.

1. (선택 사항) 작업 목록으로 돌아가려면 **목록** 아이콘을 클릭합니다.
