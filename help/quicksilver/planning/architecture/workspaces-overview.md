---
title: 작업 공간 개요
description: 작업 영역은 팀에서 사용하는 레코드 유형의 컬렉션으로, 팀의 작업 라이프사이클을 나타냅니다. 조직 단위의 워크플로와 일치하도록 Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 9053a824ecec4feb35a612b26aebb91904ef2546
workflow-type: tm+mt
source-wordcount: 516
ht-degree: 0%

---

# 작업 공간 개요

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

작업 영역은 조직 단위에서 사용하는 레코드 유형의 컬렉션이며 해당 단위의 작업 주기 및 프로세스를 나타냅니다. Adobe Workfront Planning에서 작업 공간을 완전히 사용자 정의할 수 있습니다.

<!--update screenshot with production, it was broken at Preview-->

![작업 영역 랜딩 페이지 관리자 계정](assets/workspaces-landing-page-admin-account.png)

## 작업 공간에 대한 고려 사항

* 조직 내의 특정 조직 단위에 대한 작업 공간을 만들어 각 단위의 고유한 작업 방식을 일치시킬 수 있습니다.
* Workfront Planning에는 사전 구성된 작업 영역이 없습니다. 조직의 필요에 따라 만들어야 합니다.
* 다음과 같은 방법으로 작업 공간을 만들 수 있습니다.

   * 처음부터
   * 템플릿 사용. 템플릿에는 미리 구성된 레코드 종류 수와 해당 필드가 포함되어 있습니다.
   * AI 기반 Planning Designer 사용. 이 기능은 현재 Beta에 있습니다.
   * 다중 작업 영역 템플릿 번들 사용.

  자세한 내용은 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)를 참조하십시오.

* 작업 공간은 조직 단위(팀, 그룹, 부서 또는 부서)가 작동하는 프레임워크입니다. 필드와 연결할 수 없습니다. 작업 영역 내의 레코드 유형만 필드와 연결할 수 있습니다.

  자세한 내용은 [레코드 종류 개요](/help/quicksilver/planning/architecture/overview-of-record-types.md)를 참조하세요.
* 작업 공간은 계획 영역의 다음 탭에 표시됩니다.

   * **내가 있는 작업 영역**: 사용자가 만든 작업 영역 또는 사용자와 공유된 작업 영역을 표시합니다.
   * **다른 작업 영역**: 시스템의 다른 작업 영역을 모두 표시합니다. 이 기능은 시스템 관리자만 사용할 수 있습니다.
   * <span class="preview">**샘플 작업 영역**: 모범 사례 작업 영역의 기본 제공 예제를 표시합니다. 작업 공간, 레코드 종류를 편집하거나 레코드 또는 필드를 추가할 수 없지만 다른 사용자와 추가, 편집 및 공유할 수 있습니다.</span>

  >[!NOTE]
  >
  ><span class="preview">샘플 작업 영역을 편집하지 않고 대신 참조로 사용하여 직접 만드는 것이 좋습니다. 다중 작업 영역 템플릿 번들을 사용하여 샘플 작업 영역 탭에 나열된 작업 영역과 동일한 작업 영역을 생성합니다. 자세한 내용은 문서 [작업 영역 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)의 &quot;모범 사례 다중 작업 영역 템플릿 번들을 사용하여 여러 작업 영역 만들기&quot; 섹션을 참조하십시오. </span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* 작업 영역에 포함된 레코드 유형은 조직 단위의 작업 수명 주기와 개념을 반영해야 합니다.

  예를 들어, 장치의 작업 객체가 캠페인, 제품 및 지역인 경우 해당 장치의 작업공간에는 캠페인, 제품 및 지역의 레코드 유형이 포함되어야 합니다.
* 작업 공간을 만들 때 사용자만 작업 공간에 액세스하고 관리할 수 있습니다. 다른 사용자가 동일한 공간에서 나와 공동 작업하려면 이 세그먼트를 다른 사용자와 공유해야 합니다.

  자세한 내용은 [작업 영역 공유](/help/quicksilver/planning/access/share-workspaces.md)를 참조하십시오.

  시스템 관리자는 작성하지 않은 작업 영역까지 모든 작업 영역을 관리할 수 있습니다.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Workfront Planning 인스턴스에 만들 수 있는 작업 영역 객체의 수에 제한이 있습니다. 자세한 내용은 [Adobe Workfront Planning 개체 제한 사항 개요](/help/quicksilver/planning/general/limitations-overview.md)를 참조하십시오.
