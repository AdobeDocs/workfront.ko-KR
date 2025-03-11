---
title: Workfront Planning에서 Workfront 개체 만들기
description: Workfront Planning의 다른 레코드에서 연결할 때 Workfront 객체 유형을 만들 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 2%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 레코드에 연결할 때 Workfront Planning에서 Workfront 개체 만들기

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

Workfront Planning에서 다음과 같은 방법으로 Adobe Workfront 객체를 생성할 수 있습니다.

* Planning 레코드에서 Workfront 객체를 연결할 때

  이 문서에서는 Planning 레코드에서 연결할 때 Workfront Planning에서 Workfront 객체를 만드는 방법에 대해 설명합니다.
* <span class="preview">레코드 페이지에서 자동화를 사용하는 경우.</span>

  <span class="preview">자동화를 사용하여 Workfront 개체를 만드는 방법에 대한 자세한 내용은 [Adobe Workfront Planning 레코드 자동화를 사용하여 개체 만들기](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)를 참조하십시오. </span>

Workfront Planning 레코드를 다음 Workfront 객체 유형과 연결할 때 Workfront Planning에서 다음 유형의 Workfront 객체를 생성할 수 있습니다.

* 프로젝트
* 포트폴리오
* <span class="preview">프로그램</span>

>[!IMPORTANT]
>
>* 레코드에서 연결할 때 Workfront에서 프로젝트, 포트폴리오 및 <span class="preview">프로그램</span>만 만들 수 있습니다.
>
>* Workfront Planning의 레코드에서 그룹 또는 회사를 연결할 때 그룹 또는 회사를 만들 수 없습니다.
>

Workfront Planning의 다음 영역에 있는 연결 필드에서 프로젝트, 포트폴리오, <span class="preview"> 및 프로그램 </span>을(를) 연결할 수 있습니다.

* 레코드 유형의 표 보기
* 레코드의 세부 정보 페이지 또는 미리보기 상자
* 레코드의 연결 탭

Planning 레코드를 Workfront 개체와 연결하는 방법에 대한 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항 보기..

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <li><p> Adobe Workfront 계획<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 플랜*</p></td> 
   <td> 
<p>다음 Workfront 플랜 중 하나:</p> 
<ul><li>선택</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning은 기존 Workfront 플랜에 사용할 수 없습니다.</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 계획 패키지*</p></td> 
   <td> 
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td> 표준
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p> 
   <p>레코드를 연결할 때 만들려는 개체 유형(프로젝트, 프로그램 및 포트폴리오)에 대한 Workfront의 액세스 권한을 편집합니다. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td> <p>레코드를 추가할 작업 영역 <!--<span class="preview">and record type</span>-->에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
   <p>하위 개체(프로젝트)를 추가하기 위해 Workfront 개체(포트폴리오)에 대한 권한을 관리합니다.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## Workfront Planning의 레코드와 연결할 때 Workfront 개체를 만들기 위한 사전 요구 사항

기존 레코드에서 새 프로젝트 또는 포트폴리오를 연결하여 추가하려면 먼저 다음 사항이 있어야 합니다.

* Workfront 프로젝트, 포트폴리오 또는 <span class="preview">프로그램</span>에 연결된 레코드 유형입니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
* 레코드. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
* 이 문서의 [액세스 요구 사항](#access-requirements) 섹션에 설명된 대로 Workfront Planning 및 Workfront의 올바른 액세스 및 권한.

## 프로젝트를 Workfront Planning의 레코드와 연결할 때 생성

다른 레코드에서 프로젝트를 연결할 때 프로젝트를 만들려면 다음 작업을 수행하십시오.

1. [레코드 연결](/help/quicksilver/planning/records/connect-records.md) 문서에 설명된 대로 레코드의 세부 정보 페이지 또는 레코드 유형의 테이블로 이동하여 Workfront Planning 레코드와 Workfront 프로젝트 연결을 시작합니다.

1. (조건부) <span class="preview">**프로젝트 추가**</span> 클릭
또는
프로젝트 이름을 입력한 다음 찾을 수 없는 경우 **프로젝트 추가**&#x200B;를 클릭합니다.

   다른 레코드의 연결된 레코드 필드에서 프로젝트를 추가할 때 프로젝트를 찾을 수 없으면 이름을 추가한 다음 **프로젝트 추가**&#x200B;를 클릭합니다. [추가] 단추 다음에 입력한 프로젝트 이름이 옵니다.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![연결 필드에서 연결할 때 프로젝트 추가](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">프로젝트 만들기&#x200B;**상자가 열립니다.</span>**

1. <span class="preview">(선택 사항) **프로젝트 이름**&#x200B;을(를) 업데이트합니다. 레코드에서 연결할 때 검색 항목으로 추가한 항목의 이름을 따라 기본적으로 프로젝트 이름이 지정됩니다. </span>
1. <span class="preview">(선택 사항) **프로젝트 템플릿**&#x200B;을(를) 선택하십시오. 템플릿을 선택하지 않으면 Workfront에서 작업이 없는 빈 프로젝트를 만듭니다. </span>
1. <span class="preview">**만들기**&#x200B;를 클릭합니다. </span>
1. <span class="preview">(조건부) 템플릿에서 프로젝트를 만들도록 선택한 경우 문서 [템플릿을 사용하여 프로젝트 만들기](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) 문서의 단계에 따라 프로젝트 추가를 완료합니다.</span>

   새 프로젝트가 만들어지고 선택한 레코드의 연결된 필드에 추가됩니다.

1. (선택 사항) Workfront Planning에서 새 프로젝트의 이름을 클릭하여 Workfront에서 프로젝트 페이지를 열고 프로젝트를 추가로 업데이트합니다.

## Workfront Planning의 레코드와 연결할 때 포트폴리오 만들기

Planning 레코드에서 포트폴리오를 연결할 때 포트폴리오를 생성하려면 다음을 수행합니다.

1. [레코드 연결](/help/quicksilver/planning/records/connect-records.md) 문서에 설명된 대로 레코드의 세부 정보 페이지 또는 레코드 유형의 테이블로 이동하여 Workfront Planning 레코드와 Workfront 포트폴리오의 연결을 시작합니다.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. (조건부) <span class="preview">**포트폴리오 추가**</span> 클릭

   또는

   포트폴리오의 이름을 입력한 다음 찾을 수 없는 경우 **포트폴리오 추가**&#x200B;를 클릭합니다.—> 다른 레코드의 연결된 레코드 필드에서 포트폴리오를 추가할 때 해당 포트폴리오를 찾을 수 없으면 이름을 추가한 다음 **포트폴리오 추가**&#x200B;를 클릭합니다. 추가 단추 뒤에는 입력한 포트폴리오 이름도 표시됩니다.

   ![연결 필드에서 연결할 때 포트폴리오 추가](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   포트폴리오가 만들어지고 선택한 레코드의 연결 필드에 추가됩니다.

1. (선택 사항) Workfront Planning에서 새 포트폴리오의 이름을 클릭하여 Workfront에서 포트폴리오의 페이지를 열고 포트폴리오를 추가로 업데이트합니다.

<div class="preview">

## Workfront Planning의 레코드와 연결하여 프로그램을 만듭니다.

Planning 레코드에서 프로그램을 연결할 때 프로그램을 생성하려면 다음을 수행합니다.

1. [레코드 연결](/help/quicksilver/planning/records/connect-records.md) 문서에 설명된 대로 레코드의 세부 정보 페이지 또는 레코드 유형의 테이블로 이동하여 Workfront Planning 레코드와 Workfront 포트폴리오의 연결을 시작합니다.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."-->

1. **프로그램 추가** 클릭

   또는

   프로그램 이름을 입력한 다음 찾을 수 없는 경우 **프로그램 추가**&#x200B;를 클릭합니다. [추가] 단추 다음에 프로그램 이름을 입력합니다.

   ![연결 필드에서 연결할 때 Workfront 프로그램 추가](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   **프로그램 만들기** 상자가 열립니다.

1. **프로그램 이름**&#x200B;을(를) 업데이트합니다. 필수 필드입니다.
1. 드롭다운에서 **Portfolio**&#x200B;을(를) 선택하거나 포트폴리오의 이름을 입력한 다음 목록에 표시될 때 선택하십시오. 필수 필드입니다.
1. Click **Create**.

   선택한 레코드의 연결 필드에 프로그램이 만들어지고 추가됩니다.

1. (선택 사항) Workfront Planning에서 새 프로그램 이름을 클릭하여 Workfront에서 프로그램 페이지를 열고 추가로 업데이트합니다.

</div>

