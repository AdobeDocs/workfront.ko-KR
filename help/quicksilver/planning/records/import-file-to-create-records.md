---
title: CSV 또는 Excel 파일에서 정보를 가져와 레코드 만들기
description: 레코드는 Adobe Workfront Planning의 객체 유형인 레코드 유형의 개별 인스턴스입니다. Workfront Planning에서 CSV 또는 Excel 파일에서 정보를 가져와서 레코드를 만들 수 있습니다.
hide: true
hidefromtoc: true
source-git-commit: 9f17fcab210768923e866d2f1596f40ddf8a558e
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---


<!-- add the following in the metadata when live:

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog-->

# CSV 또는 Excel 파일에서 정보를 가져와서 레코드 만들기

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

레코드는 Adobe Workfront Planning의 객체 유형인 레코드 유형의 개별 인스턴스입니다. Workfront Planning에서 CSV 또는 Excel 파일에서 정보를 가져와서 레코드를 만들 수 있습니다.

레코드 만들기에 대한 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

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
   <p>레코드를 연결할 때 만들려는 개체 유형(프로젝트 및 포트폴리오)에 대한 Workfront의 액세스 권한을 편집합니다. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td> <p>레코드를 추가할 작업 영역에 대한 권한을 관리합니다. </p>  
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

## Excel 또는 CSV 파일을 사용하여 레코드 유형 가져오기에 대한 고려 사항

* 각 시트의 열 머리글은 레코드와 연결된 필드가 됩니다.
* 각 시트의 각 행은 연결된 고유한 레코드가 됩니다.
* Excel 파일에 둘 이상의 시트가 포함되어 있는 경우 가져오는 과정에서 선택한 한 시트의 정보만 가져옵니다.
* 파일은 다음을 초과할 수 없습니다.
   * 10,000행
   * 500열
* 파일은 5MB보다 크지 않아야 합니다.
* 빈 시트는 지원되지 않습니다.
* 다음 유형의 필드는 지원되지 않으며 가져오기 시트의 필드에 매핑할 수 없습니다.
   * 연결된 레코드 또는 연결된 Workfront 개체의 조회 필드
   * 공식 필드
   * 만든 날짜, 만든 사람
   * 마지막 수정 날짜, 마지막 수정자
   * 사용자
* 다중 또는 단일 선택 필드를 가져오고 Planning의 유사한 필드보다 더 많은 선택 사항이 있는 경우 가져오는 동안 추가 옵션이 생성됩니다.

## CSV 또는 Excel 파일을 가져와서 레코드 만들기

{{step1-to-planning}}

1. 레코드 유형을 만들 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.
1. 레코드를 가져올 레코드 유형의 카드를 클릭합니다.
1. 화면 오른쪽 상단에서 **새 레코드**&#x200B;을(를) 클릭합니다.
1. **파일에서 업로드**&#x200B;를 클릭한 다음 **계속**&#x200B;을 클릭합니다.
1. 이전에 컴퓨터에 저장한 Excel 또는 CSV 파일을 끌어서 놓거나 **CSV 또는 Excel 파일 선택**&#x200B;을 클릭하여 찾습니다.
1. **미리 보기 및 편집**&#x200B;을 클릭합니다.
1. (조건부) 가져온 파일에 시트가 두 개 이상 있으면 **가져올 시트 선택** 상자에서 가져올 시트의 라디오 단추를 선택한 후 **다음**&#x200B;을 클릭합니다. 그렇지 않으면 다음 단계를 계속 진행하십시오.

   ![레코드를 가져올 시트 선택](assets/select-a-sheet-to-import-box.png)
1. **Planning 필드를 열 헤더에 매핑**&#x200B;에서 각 시트의 열에 있는 정보와 가장 일치하는 **Planning 필드**&#x200B;을(를) 선택합니다.

   ![레코드를 가져올 때 Planning 필드를 열에 매핑](assets/map-planning-fields-to-columns-when-importing-records.png)

   각 행은 새 레코드를 나타냅니다. 처음 10개의 레코드만 [미리 보기 및 편집] 상자에 표시됩니다.

1. (선택 사항) 화면 왼쪽 아래에서 **누락된 옵션 만들기**&#x200B;를 선택합니다. 활성화되면 단일 및 다중 선택 필드의 누락된 선택 사항이 추가됩니다.

   예를 들어 선택한 레코드 유형에 새로 만들기, 진행 중 및 닫힘 선택 사항이 있는 단일 선택 상태 필드가 있고 파일에서 가져온 상태 필드에 보류 중 상태 선택 사항이 있는 경우 보류 중 상태 선택 사항도 추가됩니다

   <!--when we add connected records and the info icon in the tool changes, also add those items to this step-->

1. **가져오기**&#x200B;를 클릭합니다.

   다음 정보는에서 Workfront Planning으로 가져옵니다.

   * 선택한 레코드 종류의 표 보기 아래쪽에 표시되는 새 레코드입니다.
   * 각 레코드와 연결된 기존 필드의 새 필드 값.
   * Planning에 존재하지 않았던 다중 선택 필드 또는 단일 선택 필드의 새 선택 사항입니다.

   레코드 유형 페이지에서 필드 및 레코드 관리를 시작할 수 있습니다.

   이제 Workfront Planning 및 작업 영역에 대한 액세스 권한이 있는 모든 사람이 가져온 레코드 및 해당 정보를 보고 편집할 수 있습니다.