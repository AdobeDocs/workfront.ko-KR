---
title: Ideation Space Brief에서 계획 레코드 생성
description: Adobe Workfront Planning의 새로운 기능인 Ideation Space를 사용하여 브리핑을 Planning 레코드로 변환할 수 있습니다. 내보낸 브리프는 새 레코드를 만들거나 기존 레코드를 업데이트합니다. 이 문서에서는 관념화 공간을 사용하여 기존 Planning 레코드를 생성하거나 편집하는 방법에 대해 설명합니다.
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---


# Ideation Space Brief에서 계획 레코드 생성

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. **관념화 공간 Beta** 프로그램의 일부로서만 사용할 수 있습니다. </span>

<span class="preview">자세한 내용은 [Adobe Workfront Planning의 Ideation 공간 시작](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)을 참조하십시오.</span>

{{planning-important-intro}}

Adobe Workfront Planning의 새로운 기능인 Ideation Space를 사용하여 브리핑을 Planning 레코드로 변환할 수 있습니다. 내보낸 브리프는 새 레코드를 만들거나 기존 레코드를 업데이트합니다.

이 문서에서는 관념화 공간을 사용하여 기존 Planning 레코드를 생성하거나 편집하는 방법에 대해 설명합니다.

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
또는
<li><p>독립 실행형 제품으로 구입할 경우 모든 Planning 패키지</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>추가 제품</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
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
      <p>Workfront 개체에 대한 권한을 보고 Brief에 추가 <!--not sure if this is available--></p>
      <p>브리프를 만들 수 있는 편집 공간 권한</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing 사용자 역할</p></td> 
   <td><p><ul><li>캠페인, 제품 및 가상 사용자에 액세스할 수 있는 모든 GenStudio 사용자 역할</li>
   <li>GenStudio System Manager를 사용하여 활성화 액세스 <!--and Events--></li></ul>
   자세한 내용은 <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">사용자 역할 및 권한</a>을 참조하세요. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++  

## 관념화 공간을 사용하여 레코드 만들기에 대한 고려 사항

* 레코드를 만들거나 편집할 때 Workfront Planning에서만 관념화 공간을 실행할 수 있습니다. 관념화 공간이 Workfront Planning 외부에 없습니다.
* 관념화 공간에 액세스하려면 Workfront Planning에 작업 공간 및 레코드 유형이 있어야 합니다.
* 새 레코드는 만드는 방법에 관계없이 항상 자리 표시자 콘텐츠로 시작합니다.
* 관념화 요약에 연결된 계획 레코드를 삭제하면 요약이 관념화 공간에 남아 있으며 관념화 공간의 연결된 캔버스는 삭제되지 않습니다.
* 정보 동기화는 관념화 공간에서 Workfront Planning으로만 수행됩니다. Planning 레코드에서 Ideation Space Brief로의 역방향 또는 자동 동기화는 없습니다.
* Workfront Planning에서 필드를 생성, 편집 또는 제거할 때 다음과 같은 시나리오가 발생합니다.

  * 관념화 요약에 연결된 레코드에서 생성된 새 필드는 요약에 매일 추가됩니다. 관념화 개요에 새 필드가 비어 있습니다.
  * 제거된 필드는 개요에 남아 있으며 이전 값을 유지합니다.
  * 이름이 변경된 필드는 개요에서 해당 이름을 업데이트합니다.
* 관념화 공간에 문서를 카드로 추가할 수 있습니다. 이미지도 포함됩니다.

  지원되는 파일 유형은 PDF, Excel, CSV, PNG(및 기타 이미지 형식), Word, PowerPoint입니다. 비디오는 지원되지 않습니다.

  업로드된 모든 문서는 처리를 위해 백엔드의 PDF으로 변환됩니다.
* 레코드를 Workfront Planning에서 스페이스로 직접 끌어다 놓을 수 있으며, 수동으로 업로드한 파일과 같은 방식으로 표시됩니다.

## 관념화 공간을 사용하여 레코드 만들기

1. Workfront Planning 랜딩 페이지에서 관리할 수 있는 작업 영역에 대한 카드를 클릭합니다.
1. 레코드를 추가할 수 있는 레코드 종류의 카드를 클릭합니다.
1. 다음 중 하나를 수행하여 레코드를 만듭니다.

   * 레코드 종류 페이지의 모든 보기에서 페이지의 오른쪽 상단에 있는 **새 레코드**&#x200B;을 클릭하고 **레코드를 추가할 방법을 선택** 상자에서 **관념화 공간 열기**&#x200B;를 클릭한 다음 **계속**&#x200B;을 클릭합니다.
   * 레코드 테이블의 맨 아래로 스크롤하여 **새 행**&#x200B;을 클릭한 다음 **관념화 공간 열기**&#x200B;를 클릭합니다.

     >[!TIP]
     >
     >**표시 안 함**&#x200B;을 선택하면 이후 메시지가 영구적으로 사라집니다. 닫기 아이콘 **X**&#x200B;을(를) 클릭하면 이 상자가 닫히지만 다음에 레코드 인라인을 추가할 때 다시 나타납니다.

   ![새 레코드 상자와 [편집 공간 열기] 단추](assets/new-record-creation-picker-with-ideation.png)

   새 탭에서 관념화 공간이 열리고 프롬프트가 비어 있습니다.

   레코드는 자리 표시자 텍스트로 즉시 만들어집니다.

1. (선택 사항) 프롬프트 상자에서 **기존 개요 사용**&#x200B;을 클릭하여 Ideation 공간에서 개요 및 향후 레코드를 만드는 데 사용할 기존 문서를 검색하고 추가합니다.

   ![빈 관념에 대한 프롬프트](assets/empty-ideation-prompt.png)

1. (선택 사항) 프롬프트 상자의 오른쪽 상단에 있는 **이전 캔버스 열기** <!--accurate??--> 아이콘 ![기존 브리프 열기 아이콘](assets/open-existing-briefs-icon.png)을 클릭하여 기존 브리프를 엽니다

1. **무엇을 진행 중입니까?** 프롬프트 상자에서 만들려는 레코드 종류를 설명합니다.

   세부 정보를 공유하면 할수록 관념화 공간에서 제공하는 정보가 더 유용할 것이다. 예를 들어 계획하고 있는 캠페인에 대한 설명을 입력합니다. &quot;마케팅 에이전시의 Back to school campaign&quot;.

1. **식별 시작**&#x200B;을 클릭합니다.

   아이디어 공간은 아이디어를 빌드하는 동안 다음 단계를 통해 작동합니다. <!--check some of these in the UI - there might have been UI text changes-->

   1. 목표 및 컨텍스트 이해
   2. 스페이스 및 선택한 자료 검토
   3. 문서, 웹 및 데이터에서 증거 수집
   4. 결과를 연구 요약으로 종합하기
   5. 인용이 있는 카드 만들기 및 세분화

   이 프로세스 중에 접속된 Workfront Planning 데이터 또는 웹에서 사용할 수 있는 정보를 검색하는 데 사용되는 관념화 공간을 볼 수 있습니다.

   예를 들어 기존 프로그램, 제품, 가상 사용자 또는 지역은 물론 온라인에서 사용 가능한 유사한 개념도 검색할 수 있습니다. <!--check on this with Et-->

   관념이 완료되면 관념 공간에 다음과 같은 것들이 추가됩니다.

   * 고려해야 할 사항에 대한 자세한 정보가 포함된 여러 카드와 연결된 AI 결과 요약 세부 사항 카드가 새 섹션에 표시됩니다. 커넥터는 어떤 카드 섹션이 어떤 요약에 속하는지를 나타냅니다.

   * 관념화 공간의 왼쪽 아래에 있는 **Brief** 파일입니다. 개요는 향후 레코드의 초안이며 레코드의 세부 정보 페이지로 표시됩니다.

   ![분기가 있는 관념화 카드](assets/ideation-card-with-branched-off-additional-cards.png)

1. 아이디어 공간에 정보를 계속 추가하여 개요 작성을 완료합니다.

1. (조건부) 개요가 완료되면 왼쪽 하단의 미리 보기 이미지를 클릭한 후 다음 중 하나를 클릭합니다.

   * 파일을 만들려면 **파일로 내보내기**
   * 계획 레코드를 만들려면 **Workfront Planning으로 내보내기**

   항목을 브리프에 추가하고 내보내는 방법에 대한 자세한 내용은 [Ideation Space에서 브리프 만들기](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)를 참조하십시오.

   이렇게 하면 추가 정보가 포함된 레코드 생성이 완료되고 원래 선택한 레코드 유형에 추가됩니다.

## 관념화 공간에서 기존 레코드 편집

기존 레코드에서 관념화 공간을 열어 업데이트할 수 있습니다.

관념화 공간에서는 레코드를 벌크 편집할 수 없습니다.

1. Workfront Planning의 기존 레코드로 이동하여 세부 정보 페이지를 엽니다.

1. **Ideation 공간에서 열기**&#x200B;를 클릭합니다. 새 탭에서 관념화 공간이 열립니다.

   레코드에 대한 관념이 이미 있으면 해당 공간을 엽니다.

   관념이 존재하지 않는 경우 관념화 공간과 약식을 만든다.

   >[!TIP]
   >
   >관념화 공간을 사용하여 레코드를 벌크 편집할 수 없습니다.

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. 이 문서의 [이상 공간을 사용하여 레코드 만들기](#create-records-using-the-ideation-space) 섹션에 설명된 대로 간단한 편집을 계속합니다.






<!-- this is from Claude, but rephrased and included most of this above: 

## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.


![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.



![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


