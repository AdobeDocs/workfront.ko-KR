---
title: GenStudio for Performance Marketing에 Workfront Planning Workspace 활성화
description: Adobe Workfront Planning에 이미 작업 영역이 있는 경우 데이터를 다시 만드는 대신 GenStudio for Performance Marketing에 대해 활성화할 수 있습니다.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 0bcb6ef2abbf3789339af27119422ef413cd6eef
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%
---
# GenStudio for Performance Marketing에 Workfront Planning 작업 영역 활성화

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
Workfront Planning 외에 귀사에서 Adobe GenStudio for Performance Marketing도 구입한 경우 Workfront 인스턴스가 귀사의 GenStudio 인스턴스와 통합되면 Adobe Workfront Planning에서 GenStudio 작업 영역을 사용할 수 있습니다.

Workfront Planning에 이미 작업 영역이 있는 경우 데이터를 다시 만드는 대신 GenStudio에 대해 활성화할 수 있습니다.

작업 영역을 활성화하면 해당 작업 영역이 Adobe 스토리지 프로젝트에 연결되고 레코드 유형 및 필드가 GenStudio 작업 영역 스키마에 매핑됩니다. 구성을 완료한 후 GenStudio에서 작업 공간의 레코드를 열 수 있습니다.

다음 사항을 고려하십시오.

* Workfront Planning 및 GenStudio for Performance Marketing 모두에 대한 액세스 권한이 있어야 합니다.
* 작업 영역에 연결하려면 Adobe 클라우드 스토리지 프로젝트가 있어야 합니다. 조직 관리자는 Adobe Admin Console에서 만들 수 있습니다.

  자세한 내용은 [Adobe 저장소 관리](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)를 참조하십시오. <!--ensure this site still works-->


## GenStudio에 Workfront Planning 작업 영역 활성화

1. Workfront Planning에서 활성화할 작업 영역을 엽니다.
1. 작업 영역 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **GenStudio 사용**&#x200B;을 클릭합니다.

   **Make workspace GenStudio** enabled 상자가 다음 단계와 함께 열립니다.

   1. **ACPC 프로젝트**: 이 작업 영역과 동기화할 **ACPC 프로젝트**(Adobe 클라우드 저장소 프로젝트)를 선택한 후 **다음**&#x200B;을(를) 클릭합니다. 사용자는 이 프로젝트를 통해 GenStudio의 작업 영역에 액세스합니다.

      ![작업 영역 GenStudio을 사용하도록 설정 - ACPC 프로젝트 단계](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **레코드 종류**: 작업 영역의 레코드 종류를 GenStudio에 필요한 6개의 레코드 종류에 매핑합니다.

      * 캠페인
      * 제품
      * 페르소나
      * 채널
      * 지역
      * 활성화

      각 테이블에 대해 목록을 열고 일치하는 Planning 레코드 유형을 선택하거나 **새로 추가**&#x200B;를 선택하여 만든 후 **다음**&#x200B;을 클릭합니다.

      ![작업 영역 GenStudio을 사용하도록 설정 - 레코드 종류 단계](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **필드**: 각 레코드 종류의 필드를 매핑합니다. 레코드 유형 간에 이동하려면 대화 상자 맨 위에 있는 탭을 사용합니다. 각 필드에 대해 일치하는 Planning 필드를 선택하거나 **새로 추가**&#x200B;를 선택하여 만듭니다.

      모든 레코드 유형에 대해 필드 설정을 반복합니다.

      ![작업 영역 GenStudio을 사용하도록 설정 - 필드 단계](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. 경고를 검토하고 해결하십시오.

      예를 들어 새 필드가 레코드 유형의 기본 필드가 되거나 이미 사용 중인 필드 별칭의 이름이 변경됩니다(이름이 &quot;지역&quot;인 필드가 이미 있는 경우 가져온 필드가 &quot;지역 2&quot;가 될 수 있음).

      **상태** 필드를 매핑하면 필수 옵션이 추가됩니다.

   1. **게시**&#x200B;를 클릭합니다.

      작업 영역이 활성화되면 확인 메시지가 나타납니다. 매핑된 레코드 유형은 작업 영역에 표시됩니다.

      GenStudio에서 액세스할 수 있도록 매핑된 레코드 형식의 카드에 새 **Adobe** 아이콘이 있습니다.

      ![Adobe 아이콘이 있는 캠페인 레코드 유형](assets/campaigns-record-type-card-with-adobe-icon.png)

1. GenStudio을 열고 **캠페인**&#x200B;을 선택한 다음 화면 왼쪽 하단에서 이 설정에 대해 원래 구성한 **ACPC 프로젝트**&#x200B;를 클릭합니다. 가져온 레코드 종류 및 필드를 검토합니다.

   >[!TIP]
   >
   >ACPC 프로젝트 구성원이 허용하는 레코드만 표시됩니다.
