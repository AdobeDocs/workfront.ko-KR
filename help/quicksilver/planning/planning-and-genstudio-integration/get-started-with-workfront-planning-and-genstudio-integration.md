---
title: Workfront 계획 및 GenStudio for Performance Marketing 통합 시작
description: GenStudio for Performance Marketing 작업 영역은 회사에서 두 제품을 모두 구입한 경우 Adobe Workfront Planning에서 사용할 수 있습니다. 이 통합을 사용하여 워크플로우를 간소화하는 방법에 대한 몇 가지 기본 사항을 알아봅니다.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1475'
ht-degree: 0%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Adobe Workfront Planning 및 Adobe GenStudio for Performance Marketing 통합 시작

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

Adobe Workfront Planning과 Adobe GenStudio for Performance Marketing을 모두 사용하는 조직은 종종 GenStudio이 기본적으로 지원하는 것보다 캠페인, 제품 및 가상 사용자와 같은 마케팅 개념을 더 자세히 정의합니다.

GenStudio for Performance Marketing과 Workfront Planning 간에는 기본적으로 통합됩니다. 이 통합을 통해 Workfront Planning 사용자는 GenStudio에서 사용되는 캠페인, 제품, 가상 사용자, 활성화, 채널 및 지역을 관리할 수 있습니다. 또한 이를 통해 보다 연결되고 일관된 마케팅 워크플로우를 만들어 GenStudio Planning에서 기존 레코드 유형을 참조하도록 Workfront을 구성할 수 있습니다.

GenStudio for Performance Marketing 작업 영역은 회사에서 두 제품을 모두 구입한 경우 Adobe Workfront Planning에서 사용할 수 있습니다.

## 통합의 이점

Workfront Planning과 GenStudio for Performance Marketing 간의 통합을 통해 다음과 같은 작업을 수행할 수 있습니다.

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Workfront Planning에서 GenStudio 작업 영역을 봅니다.
* GenStudio에서 캠페인을 수정하고 Workfront Planning에서 동일한 정보를 실시간으로 업데이트합니다.
* Workfront Planning에서 캠페인을 수정하고 GenStudio에서 동일한 정보를 실시간으로 업데이트합니다.
* 중복 데이터 항목을 방지합니다.
* 계획 및 활성화 노력 간의 정렬을 유지합니다.

## 통합 요구 사항

* Workfront 및 GenStudio for Performance Marketing은 동일한 조직에서 활성화되어야 합니다.

  GenStudio에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.

* 회사에 여러 Workfront 인스턴스가 있으면 Workfront Planning에서 GenStudio을 사용할 수 없습니다. <!--this will change-->

* Workfront 인스턴스는 Identity Management System(IMS) 사용을 포함하여 Adobe 통합 경험의 일부입니다.

  자세한 내용은 [Workfront용 Adobe 통합 환경](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하십시오.

* Planning과 GenStudio을 모두 사용하는 사용자는 IMS 조직 내에서 하나의 Workfront 인스턴스에만 속할 수 있습니다.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## 액세스 요구 사항

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>모든 Adobe Workfront 워크플로 패키지</p>
<p>모든 Adobe Workfront Planning 패키지</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio 패키지</p></td> 
   <td> 
<p>??? GEN STUDIO에 이를 지원하는 패키지가 있습니까???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p> 표준</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio 라이선스</p></td> 
   <td><p> ??? GEN STUDIO에는 이를 지원하는 특정 라이센스가 필요합니까???</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> 추가 제품</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
   <p>GenStudio 구성: ???GEN에 필요한 액세스 수준은 무엇입니까???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한*</p></td> 
   <td>  
   <p>Workfront Planning에서: </p>
   <ul>
   <li><p>작업 공간 및 레코드 유형에 대한 또는 그 이상의 권한 기여  </p> </li> 
   <li><p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p></li>
   </ul>
   <p>Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing의 모든 권한</p></li>
   <li><p> Adobe GenStudio for Performance Marketing에서 항목을 만들 수 있는 권한 만들기</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.
*Adobe GenStudio for Performance Marketing에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.


## Workfront Planning 및 GenStudio 통합 개요

다음 절에서는 다음을 설명합니다.

* GenStudio에서 Workfront Planning 정보를 업데이트하는 기능
* Workfront Planning에서 GenStudio 정보를 업데이트하는 기능
* Workfront Planning에서 GenStudio 작업 영역에서 관리할 수 있는 사항 및 관리할 수 없는 사항에 대한 제한 사항입니다.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront Planning의 GenStudio 작업 공간

* 조직에 여러 Workfront 인스턴스가 있는 경우 Workfront 인스턴스에서 GenStudio 작업 영역을 볼 수 없습니다. <!-- this might change-->
* GenStudio 작업 공간에는 GenStudio에서 가져왔음을 분명히 하는 시각적 표시기가 표시됩니다. 자세한 내용은 [Adobe Workfront Planning에서 GenStudio 작업 영역 관리](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)를 참조하십시오.
* GenStudio 및 Workfront Planning 모두에 액세스할 수 있는 모든 사용자는 Workfront Planning에서 GenStudio 작업 영역을 볼 수도 있습니다.
* Workfront Planning 사용자가 Workfront에서 GenStudio 작업 영역을 보고 사용할 수 있으려면 Adobe Identity Management 시스템(IMS)을 통해 관리되어야 합니다.

  Workfront 전용 사용자는 GenStudio 작업 영역을 Workfront에서 사용할 수 있는 경우에도 볼 수 없습니다.

  자세한 내용은 [Workfront용 Adobe 통합 환경](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하십시오.


### 레코드 유형

* Workfront Planning에서 GenStudio 레코드 유형 정보(예: 모양)를 편집할 수 있습니다.
* GenStudio 레코드 유형을 Planning의 다른 사용자와 공유할 수 있습니다.
* GenStudio 작업 영역의 Planning에서 레코드 유형을 만들 수 있습니다. 이러한 레코드 유형은 Planning에만 유지됩니다. GenStudio에는 표시되지 않습니다.
* GenStudio과 동기화된 레코드 유형은 GenStudio에서 레코드 유형을 가져왔음을 분명히 하는 시각적 표시기를 Workfront Planning에 표시합니다.

### 레코드

다음은 GenStudio 및 Workfront Planning에 모두 표시되는 GenStudio 레코드 유형에 속하는 레코드에 대해 가능합니다.

* GenStudio에서 레코드를 추가하거나 삭제할 수 있으며 Workfront Planning에서 표시되거나 제거됩니다.
* Workfront Planning에서 레코드를 추가하거나 삭제할 수 있으며 GenStudio에서 표시되거나 제거됩니다.
* Workfront Planning 또는 GenStudio에서 레코드를 삭제하면 30일 동안 Workfront Planning 최근 삭제 BIN에 배치됩니다. GenStudio에 최근에 삭제된 저장소가 없습니다.
* 최근에 삭제된 bin에서 레코드를 복원하면 Workfront Planning 및 GenStudio에 다시 배치됩니다.
* 다음과 같은 방법으로 Workfront Planning에서 레코드를 추가할 수 있습니다.

   * 수동으로, 처음부터, 새 레코드 단추를 사용하여 모든 보기에서
   * CSV 또는 Excel 파일을 사용하여 가져옴
   * 수동, 인라인, 테이블 보기
   * 수동으로, 타임라인 또는 달력 보기 <!--ensure the calendar is released when this releases-->에서 직접

  자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
* Workfront Planning에서 활성화 레코드를 만들거나 삭제할 수 없습니다.
* Workfront Planning의 표시되는 필드 중 하나에서 GenStudio Workspace Planning의 모든 레코드에 대한 레코드 정보를 편집할 수 있습니다.

  자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### 필드

* 레코드 필드는 GenStudio에서 가져옵니다. Workfront Planning에서 GenStudio 필드 설정을 편집할 수 있습니다.
* Gen Studio에 관리 액세스 권한이 있는 경우 Workfront Planning에서 GenStudio 레코드 유형에 대한 필드를 만들 수 있습니다.
* Planning에서 GenStudio 레코드 유형에 대한 필드를 만들면 다음 영역에서 볼 수 있습니다.
   * 계획 보기
   * 계획 레코드 세부 정보 페이지
   * GenStudio 레코드 세부 정보 페이지

  >[!TIP]
  >
  >Workfront Planning에서 생성된 필드는 GenStudio 목록 보기에 표시되지 않습니다.

* Planning에서 GenStudio 레코드 유형의 표 보기에서 필드를 숨길 수 있습니다.
* Workfront Planning에서 GenStudio에서 가져온 필드는 삭제할 수 없습니다.
* Workfront Planning에서 GenStudio 레코드 유형에 대해 Workfront Planning에서 생성된 필드를 삭제할 수 있습니다.

### 작성자 및 승인자 필드

* Workfront Planning에서 Workfront Planning의 GenStudio 레코드 유형에 대한 작성자 및 승인자 필드를 추가할 수 있습니다.
* 채널 및 지역 레코드 유형에 표시되는 레코드는 사용자가 만든 것으로 &quot;시스템&quot;을 표시합니다. 이러한 레코드는 Workfront Planning에서 GenStudio 작업 영역을 만들 때 자동으로 만들어집니다.
* Workfront Planning에서 작업 영역을 사용 가능하게 만든 후 GenStudio에서 만든 레코드는 GenStudio에서 레코드를 만든 사용자이고 Workfront 사용자가 아닌 경우에도 만든 사람 필드에 레코드를 만든 IMS 사용자의 이름을 표시합니다.
* 승인자 필드에는 Workfront Planning에서 GenStudio 레코드 유형의 레코드를 생성하기 위해 요청 양식을 제출할 때 승인자의 이름이 표시됩니다.

### 보기 횟수

* GenStudio 레코드 유형에 대한 보기를 만들 수 있습니다.

  자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

* GenStudio 레코드 유형의 보기를 공유하는 것은 Planning 레코드 유형의 보기를 공유하는 것과 동일합니다.
* GenStudio에서는 여러 보기를 만들 수 없습니다.

### 연결

* GenStudio 레코드 유형과 Workfront Planning의 다른 레코드 또는 개체 유형 간에 다음과 같은 연결을 만들 수 있습니다.

   * 두 가지 GenStudio 레코드 유형
   * 동일한 작업 영역의 GenStudio 레코드 유형과 Planning 레코드 유형
   * 다른 작업 공간에서 연결하도록 레코드 유형이 구성된 경우 다른 작업 공간의 GenStudio 레코드 유형 및 Planning 레코드 유형입니다.
   * GenStudio 레코드 유형 및 Workfront 개체 유형(프로젝트, 포트폴리오, 프로그램, 회사, 그룹)
   * GenStudio 레코드 유형 및 AEM Assets 개체 유형입니다.

### 요청 양식 및 자동화

* Workfront Planning에서 GenStudio 레코드 유형에 요청 양식을 추가할 수 있습니다.
* Workfront Planning에서 GenStudio 레코드 유형에 대한 자동화를 구성할 수 있습니다.

### 미리보기 환경

* 프로덕션 환경에서 액세스할 수 있는 GenStudio 작업 영역도 미리보기 환경에 표시됩니다.
* 미리보기 환경에서 Workfront Planning의 GenStudio 작업 영역에 대해 이 문서에 설명된 모든 활동을 수행할 수 있지만 이러한 변경 사항은 GenStudio으로 전송되지 않습니다.
프로덕션 환경의 항목에 대한 변경 사항만 Workfront Planning과 GenStudio 간에 동기화됩니다.
GenStudio에는 미리보기 환경이 없습니다.

