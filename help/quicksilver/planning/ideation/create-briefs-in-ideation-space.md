---
title: 관념화 공간에 브리프 만들기
description: 이 문서에서는 Ideation 공간에서 브레인스토밍하고 전략하여 브리프를 만드는 방법에 대해 설명합니다. 완료된 Ideation Brief를 파일이나 Workfront Planning으로 내보내 레코드를 만들거나 업데이트할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: e209f8e5ada29b1c488fcfe42c13c6c9523a26bd
workflow-type: tm+mt
source-wordcount: '1621'
ht-degree: 1%
---

# Ideation 공간에 브리프 만들기

<!--add to TOC and miniTOC-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. **관념화 공간 Beta** 프로그램의 일부로서만 사용할 수 있습니다. </span>

<span class="preview">자세한 내용은 [Adobe Workfront Planning의 Ideation 공간 시작](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)을 참조하십시오.</span>

{{planning-important-intro}}

Adobe Workfront Planning의 새로운 기능인 Ideation Space를 사용하여 브리핑을 Planning 레코드로 변환하거나 외부 파일로 저장할 수 있습니다. 내보낸 브리프는 새 레코드를 만들거나 기존 레코드를 업데이트합니다.

이 문서에서는 Ideation 공간에서 브레인스토밍하고 전략하여 브리프를 만드는 방법에 대해 설명합니다.

다음을 수행할 수 있습니다.

* 레코드를 만들거나 업데이트하려면 완료된 관념화 브리핑을 Workfront Planning으로 내보냅니다.

* 다른 응용 프로그램에서 개요 정보를 사용하려면 다음 파일 형식 중 하나로 내보냅니다.

  * PDF
  * 단어
  * PowerPoint
  * PowerPoint 템플릿

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul> 
<li><p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p></li>
<!--
Add this at GA - not available in beta:
Or
<li><p>Any Planning package when purchased as a standalone product</p></li>
-->
</ul>
   </td> 
<!--
<tr> 
<td role="rowheader"><p>Additional products</p></td> 
<td><ul>
<li><p>Adobe GenStudio for Performance Marketing</p></li>
<li><p>Adobe Customer Journey Analytics</p></li>
</ul>
</td> 
</tr> 
-->
  <tr> 
   <td role="rowheader"><p>Adobe Workflow 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr>  
<tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> 
   <ul>
   <li><p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가해야 합니다.</p>   </li>
   <li><p>액세스 수준의 관념화 공간 사용 안 함 설정을 선택 해제해야 합니다.</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td> <p>레코드를 추가할 작업 영역 및 레코드 유형에 대한 또는 그 이상의 사용 권한을 부여합니다. </p>
      <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
      <!--
      not available right now:
      <p>View permissions to Workfront objects to add them to briefs </p>
      -->
      <p>브리프를 만들 수 있는 편집 공간 권한</p>
   </td> 
  </tr>  
    <!--
    <tr> 
    <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
    <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
    <li>GenStudio System Manager to access Activations and Events</li></ul>
    For information, see <a href="https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
    </p>
    </td> 
    </tr> 
    -->
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++  

## 관념화 공간 개요 만들기

브리프를 생성하여 Planning 레코드를 생성 또는 편집하거나 다른 응용 프로그램으로 내보낼 수 있는 파일을 생성할 수 있습니다.

1. Coworker가 설정된 Planning으로 Workfront에 로그인하고 다음 중 하나를 수행합니다.

   * **주 메뉴** > **관념화 공간**(으)로 이동
   * **기본 메뉴로 이동** > **계획** > 작업 공간 클릭 > 레코드 유형 클릭 > **새 레코드** > **관념화 공간 시작**

     Ideation Space를 사용하여 레코드를 만드는 방법에 대한 자세한 내용은 [Ideation Space Brief에서 계획 레코드 만들기](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)를 참조하십시오.
   * **기본 메뉴로 이동** > **계획** > 작업 공간 클릭 > 레코드 유형 클릭 > 기존 레코드 클릭 > **관념에서 열기**

   관념화 공간이 열리고 새 관념화의 제목이 기본적으로 다음 형식으로 지정됩니다.

   `catalyze-canvas-< number > - Month date, year at time` <!--submitted bug to change the default name to "Untitled ideation"-->

   기존 레코드에서 관념화를 열면 관념화 이름이 레코드 이름과 일치합니다.

1. (권장) 이름을 변경하려면 관념의 이름을 클릭합니다.

1. (조건부 및 선택 사항) 다른 기존 관념화 공간을 열려면 관념화 이름 오른쪽에 있는 드롭다운 메뉴를 클릭하고 이름별로 관념화를 검색한 다음 목록에 표시될 때 관념을 클릭합니다.

1. **관념화 공간**&#x200B;이 열리면 오른쪽에 CX Coworker이 열립니다. Coworker 프롬프트를 사용하여 만들려는 개요 종류를 설명하십시오.

   예를 들어, &quot;미국의 부모와 교사를 위해 K-12 학생들이 8월 한 달 동안 진행할 등교 캠페인을 만들기&quot;를 입력합니다.  개요를 최대한 작성하려면 어떤 유형의 캠페인, 타임라인, 관련자, 승인 체크포인트 및 기타 세부 정보에 사용 가능한 한 많은 정보를 표시하십시오.

1. Enter를 클릭합니다.

1. Coworker의 질문에 답변하여 아이디어를 계속한 다음 **제출**&#x200B;을 클릭합니다

   또는

   추가 질문을 건너뛰려면 **질문서 건너뛰기**&#x200B;를 클릭하십시오.

1. (조건부) Coworker가 관념에 대한 카드 만들기를 제안하면 **예**&#x200B;라고 답합니다.

   카드가 이미지 공간에 추가되며 각 카드의 소스를 확인하고 브리프에 추가할 항목을 결정할 수 있습니다.

1. **검색** 아이콘 ![검색 아이콘](assets/search-icon.png)을 클릭하여 관념화 공간에서 항목을 검색한 다음 목록에 표시될 때 클릭하여 탐색합니다.

1. (선택 사항) 모든 카드의 맨 아래에 있는 **소스**&#x200B;를 클릭하여 정보가 수집된 위치를 이해합니다.

   Workfront Planning 또는 웹에서 정보를 가져올 수 있습니다.

   또한 스페이스의 오른쪽 상단에 있는 **소스** 아이콘 ![소스 아이콘](assets/sources-icon.png)을 클릭하여 스페이스의 모든 카드에 대한 소스 목록을 표시할 수도 있습니다.
1. (선택 사항) 스페이스의 오른쪽 상단에 있는 **댓글** ![댓글 아이콘](assets/comments-icon.png)을 클릭하고 **@**&#x200B;을(를) 태깅하여 스페이스 내에서 브레인스토밍을 시작합니다.

   사용자는 태그에 대한 이메일 알림을 받게 됩니다.
1. (선택 사항) 댓글 카드 내의 **필터** 아이콘 ![](assets/filter-comments-icon.png)을(를) 클릭하여 다음 기준으로 댓글을 필터링합니다.

   * 검토자
   * 댓글이 추가된 시간
   * 상태(댓글이 해결되었거나 해결되지 않은 경우)
   * 읽지 않음(읽지 않은 의견만 표시)
1. (선택 사항) 카드에 있는 **엄지 위쪽** 또는 **엄지 아래쪽** 아이콘 ![엄지 위쪽 또는 아래쪽 아이콘](assets/thumbs-up-and-down-icons.png)을 사용하여 카드에 있는 정보의 정확성에 대한 피드백을 제공합니다.
1. 카드를 클릭하거나 모든 카드가 들어 있는 프레임을 클릭한 다음 **브리핑에 추가**&#x200B;를 클릭하여 해당 정보를 설명에 추가합니다.

   Workfront은 각 정보를 저장할 가능성이 가장 높은 필드와 일치시킵니다.

   예를 들어 타임라인은 날짜 유형 필드에 추가되고 설명은 단락 유형 필드에 추가됩니다.

1. (조건부) 카드를 클릭한 다음 **AI에게 묻기...**&#x200B;를 클릭하여 다음 단계에 대한 아이디어를 얻은 후 정보를 개요에 추가합니다. 답변은 각 카드의 정보 컨텍스트에 있습니다.
1. Ideation 스페이스의 왼쪽 위 모서리에 있는 **문서 추가** 아이콘 ![문서 추가 아이콘](assets/add-documents-in-ideation-space.png)을 클릭하여 스페이스에 문서를 업로드하십시오. 새 문서나 이전에 이미 추가한 문서를 스페이스에 추가할 수 있습니다.

   >[!TIP]
   >
   >문서에 액세스하여 이를 스페이스에 업로드하려면 문서 설정을 켜야 합니다.
   >자세한 내용은 이 문서의 [관념화 공간 구성](#configure-the-ideation-space) 섹션을 참조하십시오.
   > 
1. **WF 분류 카드 추가** 아이콘 ![Workfront Planning에서 추가](assets/add-from-wf-planning-on-ideations-space.png) <!--asked to change this tooltip-->를 클릭하고 연결된 레코드 유형을 선택한 다음 각 유형의 레코드를 선택하여 해당 레코드의 정보를 선택한 레코드 유형에 추가합니다.

   스페이스에 추가하기 위해 선택한 레코드에 대한 카드가 만들어집니다. 레코드 유형은 레코드 카드의 왼쪽 상단 모서리에 표시됩니다.

   >[!TIP]
   >
   >**WF 분류 카드 추가** 아이콘 <!--check UI name-->은(는) 기본 메뉴에서 관념화 공간에 액세스할 때 사용할 수 없으며 개요가 Planning 레코드에 연결되어 있지 않습니다.

1. (선택 사항) 연결된 레코드 카드에서 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭하고 **Workfront에서 보기**&#x200B;를 클릭합니다.

   레코드의 세부 사항 페이지가 Workfront Planning의 다른 브라우저 탭에서 열립니다.
1. (선택 사항) 이미지 프레임 또는 카드를 선택하고 **삭제** 아이콘을 클릭한 다음, **삭제**&#x200B;를 클릭하여 확인합니다. 카드가 관념화 공간에서 제거됩니다.

   저장된 문서나 레코드에 해당하는 카드를 삭제하면 해당 항목이 Ideation 공간에서 제거되지만 해당 응용 프로그램에는 남아 있습니다.

1. (선택 사항) 언제든지 오른쪽 아래 모서리에 있는 **Ask Coworker anything** 상자를 사용하여 아이디어를 구체화합니다.

   예를 들어 업데이트된 컨텍스트를 사용하여 특정 카드를 AI가 다시 실행하도록 하려면 `regenerate`을(를) 입력합니다. 관념화 공간은 추론 단계(검색, 합성, 인용)를 재실행하고 영향을 받는 카드를 업데이트합니다.

1. (선택 사항) IDEATION 카드 세트에서 자주색 커넥터 중 하나를 클릭한 다음, **전체 프롬프트 복사** 아이콘을 클릭하여 카드를 생성한 프롬프트를 클립보드에 복사한 다음 Coworker 프롬프트 상자에 붙여넣습니다.

   ![프롬프트 표시줄 아이콘에 복사](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (선택 사항) 작업을 취소하거나 취소하려면 관념화 공간 상단의 **실행 취소** 또는 **다시 실행** 아이콘 ![실행 취소 및 다시 실행 아이콘](assets/undo-redo-icons.png)을 클릭합니다.
1. 축소하여 전체 그림을 보십시오. 원래 캠페인 목표, 인용이 있는 모든 AI 생성 개념 카드, 추가 문서, 가져온 실제 Workfront Planning 레코드(제품, 가상 사용자 등). 왼쪽 아래 모서리에 있는 **Brief** 요약 카드는 모두 가져옵니다.

1. 왼쪽 하단의 간략한 미리 보기 이미지를 클릭하고 간략한 내용을 검토한 후 다음 옵션 중 하나를 클릭합니다.

   * **파일로 내보내기**. 개요를 다음 파일 형식으로 내보낼 수 있습니다.

     * PDF
     * 단어
     * PowerPoint(템플릿 포함 또는 제외)
   * **Workfront 계획으로 내보내기**. 내보내기는 해당 관념에 해당하는 Planning 레코드의 모든 기존 필드 데이터를 덮어씁니다.

   >[!TIP]
   >
   >기본 메뉴에서 Ideation 공간에 액세스할 때 **Workfront Planning으로 내보내기**&#x200B;가 흐리게 표시되고 개요가 Planning 레코드에 연결되어 있지 않습니다.

   그러면 추가 정보가 있는 레코드 또는 파일 작성이 완료됩니다. 기존 레코드에서 시작한 경우 브리프의 정보가 레코드에 추가됩니다. 새 레코드로 시작한 경우 개요에 나와 있는 정보로 레코드가 만들어집니다.

   Brief를 사용하여 Planning 레코드를 업데이트하는 방법에 대한 자세한 내용은 [Ideation Space Brief에서 Planning 레코드 만들기](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md) 문서의 &quot;ConsiderationsConsiderations: Ideation Space를 사용하여 레코드를 만드는 방법에 대한 고려 사항&quot; 섹션을 참조하십시오.


## 관념화 공간 구성

Ideation 공간에는 공간을 탐색하는 데 도움이 될 뿐만 아니라 화면에 표시되는 내용을 구성하는 컨트롤이 있습니다.

1. AI가 정보를 가져오는 위치를 제어하려면 **설정** 아이콘 ![설정](assets/setting-icon.png)을 클릭하고 다음 **Source 유형** 중에서 선택하십시오.

   * **문서** — 선택한 스페이스에 업로드된 문서
   * **웹 검색** — 외부 웹 조사
   <!--
     **CJA** — Adobe Customer Journey Analytics
    -->
1. **저장**&#x200B;을 클릭합니다.

1. **도움말** 아이콘 왼쪽에 있는 **확대/축소 수준** 드롭다운 아이콘이나 **도움말** 아이콘 ![도움말 아이콘](assets/more-information-icon.png)을 클릭하여 옵션을 선택하거나, 편집 공간을 탐색하거나 다른 확대/축소 값을 선택하는 데 사용할 수 있는 키보드 단축키를 검토합니다.

   다음 확대/축소 수준 중에서 선택합니다.

   * 100%로 확대/축소
   * 200%로 확대/축소
   * 크기에 맞게 확대/축소

   또는 다음 단축키 중 하나를 사용하여 페이지를 탐색합니다.

   | 작업 | 단축키 |
   | --- | --- |
   | 확대/축소 | Ctrl/⌘ + / − |
   | 선택 영역에 맞게 확대/축소 | — |
   | 커서로 확대/축소 | Ctrl/⌘ + 스크롤 |
   | 캔버스 패닝 | 스페이스바를 누른 채 드래그 |
   | 점 격자 표시/숨기기 | G |



<!--

    Once opened, the Ideation space agent goes through the following steps:

    1. **Data ingestion and synthesis**:  Pulls relevant information from connected sources. For example: 
    
        * Existing record types or the existing record type that you started from. 
        * Recent documents you might have uploaded in the ideation space. 
        * Web information that matches your prompt criteria.

            >[!TIP]
            >
            >The Web search setting must be turned on for AI to be able to look for information on the web.  
            >For information, see the section [Configure the Ideation space](#configure-the-ideation-space)in this article.
            >
    1. **Audience definition**: Identifies or recommends target audience parameters based on historical patterns
    1. **Strategy framing**: Structures the strategic narrative for the campaign
    1. **Messaging and concept ideation**: Generates initial message options and creative concept directions
    1. **Brief generation and planning handoff**: Produces a structured brief that feeds back into the Workfront Planning workspace

        When the Ideation agent finishes the process of collecting all the information, the following things occur: 
    
        * Five cards are created and are organized by relevant and like-information. 

            The cards are titled using various steps in the creation of the requested record, for easy recognition. 
    
            For example, they could be named:

            * Plan
            * Timeline
            * Segments
            * Mechanics  
            * Messaging 

        The cards titles are custom to each card in the ideation. 

        * The cards are placed inside the same frame indicating this is the result of one ideation. 

        * A brief is created and displays in a preview image in the lower-left corner of the Ideation space. <!
    
        The brief contains suggested fields that the system considers pertinent to the ideas you are exploring. 
-->






