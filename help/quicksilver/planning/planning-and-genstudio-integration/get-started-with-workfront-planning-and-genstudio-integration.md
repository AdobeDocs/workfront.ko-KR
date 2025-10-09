---
title: Workfront 계획 및 GenStudio for Performance Marketing 통합 시작
description: GenStudio for Performance Marketing 작업 영역은 회사에서 두 제품을 모두 구입한 경우 Adobe Workfront Planning에서 사용할 수 있습니다. 이 통합을 사용하여 워크플로우를 간소화하는 방법에 대한 몇 가지 기본 사항을 알아봅니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: e717e095f1995dbed0232789616d42492156d843
workflow-type: tm+mt
source-wordcount: '1906'
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

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Adobe Workfront Planning과 Adobe GenStudio for Performance Marketing을 모두 사용하는 조직은 종종 GenStudio이 기본적으로 지원하는 것보다 캠페인, 제품, 활성화 및 가상 사용자와 같은 마케팅 개념을 더 자세히 정의합니다.

GenStudio for Performance Marketing과 Workfront Planning 간에는 기본적으로 통합됩니다. 이 통합을 통해 Workfront Planning 사용자는 GenStudio에서 사용되는 캠페인, 제품, 가상 사용자, 활성화, 채널 및 지역을 관리할 수 있습니다. 또한 이를 통해 보다 연결되고 일관된 마케팅 워크플로우를 만들어 GenStudio Planning에서 기존 레코드 유형을 참조하도록 Workfront을 구성할 수 있습니다.

GenStudio for Performance Marketing 작업 영역은 회사에서 두 제품을 모두 구입한 경우 Adobe Workfront Planning에서 사용할 수 있습니다.

## 통합의 이점

Workfront Planning과 GenStudio for Performance Marketing 간의 통합을 통해 다음과 같은 작업을 수행할 수 있습니다.

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Workfront Planning에서 GenStudio 작업 영역을 봅니다.
* GenStudio for Performance Marketing에서 캠페인, 제품, 가상 사용자 및 활성화를 수정하고 Workfront Planning에서 동일한 정보를 실시간으로 업데이트합니다.
* Workfront Planning에서 캠페인, 제품, 가상 사용자 및 활성화를 수정하고 GenStudio for Performance Marketing에서 동일한 정보를 실시간으로 업데이트합니다.
* 중복 데이터 항목을 방지합니다.
* 계획 및 활성화 노력 간의 정렬을 유지합니다.

## 통합 요구 사항

Workfront Planning과 GenStudio for Performance Marketing 간의 통합을 사용하려면 조직이 다음 요구 사항을 충족해야 합니다.

* Workfront 및 GenStudio for Performance Marketing은 동일한 조직에서 활성화되어야 합니다.

  GenStudio에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Workfront 인스턴스는 Identity Management System(IMS) 사용을 포함하여 Adobe 통합 경험의 일부입니다.

  자세한 내용은 [Workfront용 Adobe 통합 환경](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)을 참조하십시오.

* Workfront Planning과 GenStudio for Performance Marketing을 모두 사용하는 사용자는 IMS 조직 내에서 하나의 Workfront 인스턴스에만 속해야 합니다.

  Workfront 사용자가 아니더라도 GenStudio for Performance Marketing 전용 사용자는 GenStudio 작업 영역을 볼 수 있습니다.

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
<p>모든 Workfront 패키지</p>
<p>모든 Planning 패키지</p>

</td> </tr>
   <tr> 
<td> 
   <p> 추가 제품</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p> 표준</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing 사용자 역할</p></td> 
   <td><p><ul><li>캠페인, 제품 및 가상 사용자에 액세스할 수 있는 모든 GenStudio 사용자 역할</li>
   <li>정품 인증에 액세스하기 위한 GenStudio System Manager <!--and Events--></li></ul>
   자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">사용자 역할 및 권한</a>을 참조하세요. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>  
   <p>Workfront Planning에서: </p>
   <ul>
   <li><p>GenStudio 작업 영역에 새 필드 또는 레코드 유형을 추가할 수 있는 GenStudio 작업 영역에 대한 권한을 관리합니다.</p></li>
   <li><p>GenStudio 작업 영역에서 레코드를 추가, 업데이트 또는 삭제할 수 있는 GenStudio 작업 영역 기여 권한</p> </li>  
   </ul>
   <p>어떤 사용자도 Workfront Planning의 GenStudio 작업 영역에서 GenStudio for Performance Marketing 레코드 유형 또는 필드를 제거할 수 없습니다</p>
   <p>Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing의 모든 권한</p></li>
   <li><p> Adobe GenStudio for Performance Marketing에서 항목을 만들 수 있는 권한 만들기</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

Adobe Workfront Planning 액세스에 대한 자세한 내용은 [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.

Adobe GenStudio for Performance Marketing에 대한 자세한 내용은 [Adobe GenStudio for Performance Marketing 사용 안내서](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)를 참조하십시오.


## Workfront Planning 및 GenStudio for Performance Marketing 통합 기능 개요

조직에 있는 Workfront 인스턴스 수에 따라 Planning의 GenStudio 작업 영역에 대해 자동으로 다음 권한을 갖습니다.

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Workfront 인스턴스 1개</p></td> 
   <td> 
<p>GenStudio 작업 영역은 Workfront Planning 인스턴스에 표시됩니다</p>
<p>Workfront 관리자를 포함한 모든 사용자는 기본적으로 Planning의 GenStudio 작업 영역에 대한 Contribute 액세스 권한이 있습니다</p>
<p>Workfront 관리자는 GenStudio 작업 영역에서 수정 및 관리 권한을 누구에게나 부여할 수 있습니다</p>
</td> </tr>
   <tr> 
<td> 
   <p> Workfront의 여러 인스턴스</p> </td> 
   <td>

<p>GenStudio 작업 영역은 모든 Workfront 인스턴스에서 볼 수 있습니다</p>
<p>GenStudio for Performance Marketing 및 Workfront Planning에 대한 액세스 권한이 있는 모든 사용자는 기본적으로 Planning의 GenStudio에 대한 기여 권한이 있습니다</p> 
<p>Workfront 관리자는 GenStudio 작업 영역에 대한 관리 권한을 누구에게도 부여할 수 없습니다</p>
</td> 
  </tr>
   </tbody> 
</table>

<!--If Iskuhi confirms, add this or a corrected version to the second row of the table above:
<p>The following are the scenarios for when your organization has more than one instance of Workfront with Workfront Planning:</p>
   <ul><li>If your company has multiple instances of Workfront at the moment when they purchase Adobe GenStudio for Performance Marketing, the GenStudio workspace is visible from all Workfront instances.</li>
   <li>If your company adds more Workfront instances after their original instance has already been integrated with Adobe GenStudio for Performance Marketing, the GenStudio workspace is visible only from the original Workfront instance. For information about connecting additional instance of Workfront to Adobe GenStudio, contact your account representative. </li></ul>  
   
   -->

Workfront Planning 권한에 대한 자세한 내용은 [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)를 참조하십시오.

아래 섹션에서는 다음을 설명합니다.

* GenStudio for Performance Marketing에서 Workfront Planning 정보를 업데이트하는 기능
* Workfront Planning에서 GenStudio for Performance Marketing 정보를 업데이트하는 기능
* Workfront Planning에서 GenStudio 작업 영역에서 관리할 수 있는 사항 및 관리할 수 없는 사항에 대한 제한 사항입니다.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront Planning의 GenStudio 작업 공간

* GenStudio 작업 공간에는 GenStudio for Performance Marketing 작업 공간을 나타내는 것으로 식별하기 위한 시각적 표시기가 Workfront Planning에 표시됩니다.

  ![Planning의 GenStudio 카드](assets/genstudio-card-with-tag-highlighted.png)

  자세한 내용은 [Adobe Workfront Planning에서 GenStudio 작업 영역 관리](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)를 참조하십시오.
* Planning에서 GenStudio 작업 영역에 대한 관리 권한이 있는 경우 다음을 수행할 수 있습니다.

   * Planning에서 GenStudio 작업 공간 업데이트(이름, 설명, 아이콘)
   * 섹션 만들기
   * 레코드 유형 추가
   * 다른 사용자와 공유

     GenStudio 계정이 없는 다른 사용자와 GenStudio 작업 영역을 공유할 수 있습니다. 조직의 IMS(Identity Management System)에서 사용할 수 있는 사용자만 공유할 수 있습니다. <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Planning에서 GenStudio 작업 영역에 대한 기여 권한이 있는 경우 Workfront Planning에서 작업 영역을 수정할 수 없습니다.

### GenStudio 작업 영역의 레코드 유형

* GenStudio for Performance Marketing 및 Planning에 모두 표시되는 레코드 유형은 Workfront Planning에 GenStudio 표시기가 있습니다.

  ![Workfront Planning의 GenStudio 레코드 유형 카드](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Planning에서 GenStudio 작업 영역에 대한 관리 권한이 있는 경우 Workfront Planning에서 다음을 수행할 수 있습니다.
   * GenStudio 레코드 유형 정보(모양, 고급 설정)를 편집합니다.
   * 다른 사용자와 GenStudio 레코드 유형을 공유합니다.
   * 레코드 유형을 만듭니다. 이러한 레코드 유형은 Workfront Planning에만 유지됩니다. GenStudio에는 표시되지 않습니다.
   * GenStudio 작업 영역의 레코드를 다른 작업 영역에서 연결할 수 있도록 합니다.
   * GenStudio 작업 영역의 레코드를 다른 작업 영역에 추가할 수 있도록 합니다.
* Planning에서 GenStudio 작업 영역에 대한 기여 권한이 있는 경우 Planning에서 GenStudio 레코드 유형을 수정할 수 없습니다.

### GenStudio 작업 영역의 레코드

* GenStudio for Performance Marketing에서 GenStudio 레코드를 편집하면 Workfront의 모든 인스턴스에 변경 사항이 GenStudio 작업 공간에 표시됩니다.
* Workfront Planning의 GenStudio 작업 영역에서 활성화 레코드를 만들거나 삭제할 수 없습니다.
* Planning에서 GenStudio 작업 영역에 대한 관리 또는 기여 권한이 있는 경우 Workfront Planning에서 다음을 수행할 수 있습니다.
   * 레코드를 추가하거나 삭제하면 GenStudio for Performance Marketing에서 표시되거나 제거됩니다.

     Workfront Planning 또는 GenStudio for Performance Marketing에서 삭제된 레코드는 30일 동안 Workfront Planning 최근에 삭제된 BIN에 배치됩니다. GenStudio for Performance Marketing에 최근에 삭제된 저장소가 없습니다.
   * 최근에 삭제된 저장소에서 레코드를 복원합니다. 삭제된 레코드를 복원하면 Workfront Planning 및 GenStudio for Performance Marketing에 다시 배치됩니다.
   * 다음과 같은 방법으로 레코드를 추가합니다.

      * 수동으로, 처음부터, 새 레코드 단추를 사용하여 모든 보기에서
      * 표 보기에서 CSV 또는 Excel 파일을 사용하여 가져오기
      * 수동으로, Workfront Planning의 모든 보기에서
      * Workfront의 레코드 유형 요청 양식에 요청을 제출하여.

  자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
* Workfront Planning에서 GenStudio 작업 공간의 모든 레코드에 대한 레코드 정보를 편집할 수 있습니다.

  자세한 내용은 [레코드 편집](/help/quicksilver/planning/records/edit-records.md)을 참조하세요.

### GenStudio 작업 영역의 레코드 유형 필드

* 레코드 유형 필드는 기본적으로 GenStudio for Performance Marketing에서 Workfront Planning으로 가져옵니다.
* GenStudio for Performance Marketing에서 레코드 유형에 필드를 추가할 수 없습니다.
<!--Iskuhi said this is not possible but I can add fields: * You cannot create or delete Activation records' fields from the GenStudio workspace in Workfront Planning. -->
* Planning에서 GenStudio 작업 영역에 대한 관리 권한이 있는 경우 Workfront Planning에서 다음을 수행할 수 있습니다.

   * GenStudio 필드 설정을 편집합니다.
   * Gen Studio 작업 영역에서 관리 액세스 권한이 있는 경우 GenStudio 레코드 유형에 대한 필드를 만듭니다.

     Planning에서 GenStudio 레코드 유형에 대한 필드를 만들면 다음 영역에서 볼 수 있습니다.

      * Workfront Planning 보기
      * Workfront Planning 레코드 세부 정보 페이지
      * GenStudio 레코드 세부 정보 페이지

     >[!TIP]
     >
     >Workfront Planning에서 생성된 필드는 GenStudio 목록 보기에 표시되지 않습니다.

   * Workfront Planning에서 GenStudio 레코드 유형의 표 보기에서 필드를 숨깁니다.
&lt;!—* Workfront Planning에서 GenStudio 레코드 유형에 대해 Workfront Planning에 생성된 필드를 삭제합니다. — 이는 Iskuhi에 따라 가능하지 않습니다. 링크가 있지만 오류가 발생합니다—>

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* Planning에서 GenStudio 작업 영역에 대한 기여 권한이 있는 경우:

   * Workfront Planning에서 GenStudio 작업 영역에서 필드 설정을 편집하거나, 필드를 삭제하거나, 추가할 수 없습니다.
   * Workfront Planning의 테이블 보기에서 필드를 숨길 수 있습니다.

#### 작성자 및 승인자 필드

* Workfront Planning에서 Workfront Planning의 GenStudio 레코드 유형에 대한 작성자 및 승인자 필드를 추가할 수 있습니다.
* 채널 및 지역 레코드 유형에 표시되는 레코드는 사용자가 만든 것으로 &quot;시스템&quot;을 표시합니다. 이러한 레코드는 Workfront Planning에서 GenStudio 작업 영역을 만들 때 자동으로 만들어집니다.
* Workfront Planning에서 작업 영역을 사용 가능하게 만든 후 GenStudio에서 만든 레코드는 GenStudio에서 레코드를 만든 사용자이고 Workfront 사용자가 아닌 경우에도 만든 사람 필드에 레코드를 만든 IMS 사용자의 이름을 표시합니다.
* 승인자 필드에는 Workfront Planning에서 GenStudio 레코드 유형의 레코드를 생성하기 위해 요청 양식을 제출할 때 승인자의 이름이 표시됩니다.
* 작성자 및 승인자 필드는 GenStudio for Performance Marketing의 레코드 세부 정보에 표시됩니다. 목록 보기에는 표시되지 않습니다.

### GenStudio 작업 공간에서 보기 기록

>[!NOTE]
>
>GenStudio 레코드 유형은 GenStudio for Performance Marketing 목록 보기에서 가져온 기본 테이블 보기에 표시됩니다.
>
>GenStudio for Performance Marketing에서 기본적으로 가져온 원본 테이블 보기는 삭제할 수 없습니다.

* GenStudio for Performance Marketing에서는 여러 보기를 만들 수 없습니다.

* Planning에서 GenStudio 작업 영역에 대한 관리 권한이 있는 경우 Workfront Planning에서 다음을 수행할 수 있습니다.

   * GenStudio 레코드 유형에 대한 보기를 만듭니다.

     자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

   * GenStudio 레코드 유형에서 사용자 지정 보기의 이름을 바꾸거나, 공유하거나, 내보내거나, 복제하거나, 삭제합니다.

* Planning에서 GenStudio 작업 영역에 대한 기여 권한이 있는 경우 Workfront Planning에서 다음을 수행할 수 있습니다.

   * GenStudio 레코드 유형에 대한 보기를 만듭니다.

     자세한 내용은 [레코드 보기 관리](/help/quicksilver/planning/views/manage-record-views.md)를 참조하십시오.

   * GenStudio 레코드 유형에서 사용자 지정 보기의 이름을 바꾸거나 내보내거나 복제하거나 삭제합니다.

     Workfront Planning에서 GenStudio 작업 공간에서 보기를 공유할 수 없습니다.

### GenStudio 작업 공간에서 연결 기록

관리 권한이 있는 GenStudio 작업 영역에서 레코드 유형 간에 연결을 만들 수 있습니다.

GenStudio 레코드 유형과 Workfront Planning의 다른 레코드 또는 개체 유형 간에 다음과 같은 연결을 만들 수 있습니다.

* 두 가지 GenStudio 레코드 유형
* 동일한 작업 영역의 GenStudio 레코드 유형과 Planning 레코드 유형
* 다른 작업 공간에서 연결하도록 레코드 유형이 구성된 경우 다른 작업 공간의 GenStudio 레코드 유형 및 Planning 레코드 유형입니다.
* GenStudio 레코드 유형 및 Workfront 개체 유형(프로젝트, 포트폴리오, 프로그램, 회사, 그룹)
* GenStudio 레코드 유형 및 AEM Assets 개체 유형입니다.

### GenStudio 레코드 유형의 요청 양식 및 자동화

* Workfront Planning에서 GenStudio 레코드 유형에 요청 양식을 추가할 수 있습니다.

  자세한 내용은 [Adobe Workfront Planning에서 요청 양식 만들기 및 관리](/help/quicksilver/planning/requests/create-request-form.md)를 참조하십시오.
* Workfront Planning에서 GenStudio 레코드 유형에 대한 자동화를 구성할 수 있습니다.

  자세한 내용은 [Adobe Workfront Planning 자동화 구성](/help/quicksilver/planning/records/configure-automations-to-create-records.md)을 참조하십시오.

## 미리보기 환경

* 프로덕션 환경에서 액세스할 수 있는 GenStudio 작업 영역도 동일한 Workfront 인스턴스의 미리보기 환경에 표시됩니다.
* 미리보기 환경에서 Workfront Planning의 GenStudio 작업 영역에 대해 이 문서에 설명된 모든 활동을 수행할 수 있지만 이러한 변경 사항은 GenStudio에서 표시되지 않습니다.

  프로덕션 환경의 항목에 대한 변경 사항만 Workfront Planning과 GenStudio 간에 동기화됩니다.

  GenStudio에는 미리보기 환경이 없습니다.

