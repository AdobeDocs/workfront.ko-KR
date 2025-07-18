---
title: Workfront Planning에서 Workfront 객체를 레코드에 연결할 때 만들기
description: Workfront Planning의 다른 레코드에서 연결할 때 Workfront 개체 유형을 생성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront Planning에서 Workfront 객체를 레코드에 연결할 때 만들기

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

다음과 같은 방법으로 Workfront Planning에서 Adobe Systems Workfront 객체를 만들 수 있습니다.

* Planning 레코드에서 Workfront 객체를 연결할 때

  이 문서에서는 Planning 레코드에서 Workfront 개체를 연결할 때 Workfront Planning에서 Workfront 개체를 만드는 방법을 설명합니다.
* 레코드의 페이지 에서 자동화를 사용하는 경우.

  자동화를 사용하여 Workfront 개체를 만드는 방법에 대한 자세한 내용은 Adobe Systems Workfront Planning 레코드 자동화를 사용하여 개체 만들기 단원 [을 참조하십시오](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Workfront Planning 레코드를 다음 Workfront 객체 유형과 연결할 때 Workfront Planning에서 다음 유형의 Workfront 객체를 생성할 수 있습니다.

* 프로젝트
* 포트폴리오
* 프로그램

>[!IMPORTANT]
>
>* 레코드에서 연결할 때 Workfront에서 프로젝트, 포트폴리오 및 프로그램만 만들 수 있습니다.
>
>* Workfront Planning의 레코드에서 연결할 때 그룹 또는 회사를 만들 수 없습니다.
>

Workfront Planning의 다음 영역에 있는 연결 필드에서 프로젝트, 포트폴리오 및 프로그램을 연결할 수 있습니다.

* 레코드 종류의 테이블 보기
* 레코드의 세부 정보 페이지 또는 미리 보기 상자
* 레코드의 연결 탭

Planning 레코드를 Workfront 개체와 연결하는 방법에 대한 자세한 내용은 레코드[ 연결을 참조하세요](/help/quicksilver/planning/records/connect-records.md).

## 액세스 요구 사항

+++ 액세스 요구 사항을 보려면 확장합니다.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 제품</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 계획 패키지*</p></td> 
   <td> 
<p>어떤 </p> 
<p>각 Workfront Planning 플랜에 포함된 항목에 대한 자세한 내용은 Workfront 계정 관리자 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe Systems 통합 환경에 온보딩되어 있어야 합니다.</p> 
<p>자세한 내용은 Adobe Systems Unified Experience for Workfront<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">를 참조하십시오</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Systems Workfront 라이선스*</p></td> 
   <td> 표준
   <p>Workfront Planning은 기존 Workfront 라이선스에 사용할 수 없습니다</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Systems Workfront Planning에 대한 액세스 수준 컨트롤은 없습니다</p> 
   <p>생성하려는 개체 유형(프로젝트, 포트폴리오, 프로그램)에 대한 Workfront에서 개체 만들기 액세스 권한이 있는 편집 권한. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 사용 권한</p></td> 
   <td> <p>레코드를 추가하려는 작업 영역 및 레코드 종류에 대한 사용 권한을 관리합니다. </p>  
   <p>시스템 관리자는 자신이 생성하지 않은 작업 영역을 포함하여 모든 작업 공간에 대한 권한을 갖습니다</p>
   <p>Workfront 개체(포트폴리오)에 대한 권한을 관리하여 하위 개체(프로젝트)를 추가합니다.</p>
   </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서[의 액세스 요구 사항을 참조하십시오](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Workfront Planning의 레코드와 연결할 때 Workfront 개체를 생성하기 위한 전제 조건

기존 레코드에서 연결하여 새 프로젝트나 포트폴리오를 추가하려면 다음 사항이 있어야 합니다.

* Workfront 프로젝트, 포트폴리오 또는 프로그램에 연결된 레코드 유형입니다. 자세한 내용은 레코드 종류[ 연결을 참조하세요](/help/quicksilver/planning/architecture/connect-record-types.md).
* 레코드. 자세한 내용은 레코드[ 만들기 섹션을 참조하세요](/help/quicksilver/planning/records/create-records.md).
* Workfront Planning 및 Workfront의 올바른 액세스 및 권한은 이 문서의 액세스 요구 사항[ 섹션에 ](#access-requirements)설명되어 있습니다.

## Workfront Planning의 레코드와 연결하여 프로젝트를 만들기

다른 레코드에서 연결할 때 프로젝트를 만들려면:

1. 레코드 연결 문서에 [설명된 대로 레코드의 세부 정보 페이지 또는 레코드 유형의 테이블로 이동하여 Workfront](/help/quicksilver/planning/records/connect-records.md) Planning 레코드를 Workfront 프로젝트와 연결하기 시작합니다.

1. (조건부) 프로젝트&#x200B;**추가를 클릭합니다**
또는
프로젝트 이름을 시작 입력한 다음, 프로젝트 이름을 찾을 수 없으면 프로젝트**추가를 클릭합니다**. [추가 버튼] 버튼 뒤에 입력한 프로젝트 이름이 옵니다.

   ![연결 필드에서 연결할 때 프로젝트 추가](assets/add-project-when-connecting-it-from-connection-field.png)

   **프로젝트** 만들기 상자가 열립니다.

1. (선택 사항) 프로젝트 이름을 업데이트합니다&#x200B;****. 기본적으로 프로젝트 이름은 레코드에서 연결할 때 검색 항목으로 추가한 항목의 이름을 따서 지정됩니다.
1. (선택 사항) 프로젝트 템플릿&#x200B;**선택.** 템플릿 을 선택하지 않으면 Workfront에서 작업 없이 빈 프로젝트를 만듭니다.
1. Click **Create**.
1. (조건부) 템플릿에서 프로젝트를 만들도록 선택한 경우 템플릿[ 문서를 사용하여 프로젝트 만들기 문서의 ](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)단계를 팔로우 수행하여 프로젝트 추가를 완료합니다.

   새 프로젝트가 만들어지고 선택한 레코드의 연결된 필드에 추가됩니다.

1. (선택 사항) Workfront Planning에서 새 프로젝트의 이름을 클릭하여 Workfront에서 프로젝트의 페이지 를 열고 프로젝트를 추가로 업데이트합니다.

## Workfront Planning의 레코드와 연결하여 포트폴리오를 만들기

Planning 레코드에서 포트폴리오를 연결할 때 포트폴리오를 생성하려면 다음을 수행하십시오.

1. 레코드의 세부 정보 페이지 또는 레코드 유형의 테이블로 이동하여 레코드[ 연결 문서에 ](/help/quicksilver/planning/records/connect-records.md)설명된 대로 Workfront Planning 레코드를 Workfront 포트폴리오와 연결하기 시작합니다.

1. (조건부) Add Portfolio(포트폴리오 추가)를 클릭합니다 **.**

   또는

   포트폴리오 이름을 입력한 시작 찾을 수 없는 경우 포트폴리오&#x200B;**추가를 클릭합니다**. 추가 버튼 다음에는 입력한 포트폴리오 이름이 옵니다.

   ![연결 필드에서 연결할 때 포트폴리오 추가](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   포트폴리오 생성이 완료되고 선택한 레코드의 연결 필드에 추가됩니다.

1. (선택 사항) Workfront Planning에서 새 포트폴리오의 이름을 클릭하여 Workfront에서 포트폴리오의 페이지를 열고 포트폴리오를 추가로 업데이트합니다.

## Workfront Planning의 레코드와 연결하여 프로그램 만들기

Planning 레코드에서 연결하는 프로그램을 작성하려면 다음을 수행하십시오.

1. 레코드의 세부 정보 페이지 또는 레코드 유형의 테이블로 이동하여 레코드[ 연결 문서에 ](/help/quicksilver/planning/records/connect-records.md)설명된 대로 Workfront Planning 레코드를 Workfront 포트폴리오와 연결하기 시작합니다.

1. 프로그램 추가를 클릭합니다.****

   또는

   프로그램 이름을 시작 입력한 다음 찾을 수 없는 경우 프로그램&#x200B;**추가를 클릭합니다**. 추가 버튼 뒤에 입력한 프로그램 이름이 옵니다.

   ![연결 필드에서 연결할 때 Workfront 프로그램 추가](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   **프로그램** 만들기 상자가 열립니다.

1. 프로그램 이름을 업데이트합니다&#x200B;****. 필수 필드입니다.
1. **드롭다운에서 Portfolio** 선택하거나 포트폴리오 이름을 입력하기 시작한 다음 목록에 표시되면 선택합니다. 필수 필드입니다.
1. Click **Create**.

   프로그램이 만들어지고 선택한 레코드의 연결 필드에 추가됩니다.

1. (선택 사항) Workfront Planning에서 새 프로그램의 이름을 클릭하여 Workfront에서 프로그램의 페이지 를 열고 추가로 업데이트합니다.

