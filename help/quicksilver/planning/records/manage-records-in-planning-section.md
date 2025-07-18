---
title: Adobe Workfront 개체의 계획 섹션에서 레코드 관리
description: 왼쪽 패널의 Workfront 오브젝트의 계획 섹션에서 Adobe Workfront 오브젝트에 연결된 Workfront Planning 레코드를 표시할 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Workfront 개체에서 레코드 연결 관리

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

연결된 오브젝트의 다음 영역에 Workfront에서 Workfront Planning 레코드를 표시할 수 있습니다.

* Workfront 객체의 계획 섹션: 객체에 연결된 모든 레코드 유형과 해당 연결된 레코드를 표시합니다.
* Planning 연결 사용자 정의 필드: 하나의 레코드 유형, 각 연결된 레코드 및 연결된 레코드의 최대 7개의 조회 필드를 표시합니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
<p>임의</p>
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td>
   <td>
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p>
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>프로젝트, 프로그램 및 포트폴리오 보기 또는 상위 액세스</p>  
   <p>Workfront Planning에 대한 액세스 수준 구성이 없습니다. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <p>Workfront에서 프로젝트, 포트폴리오 또는 프로그램에 대한 권한 보기 이상</a> </p> 
   <p>Workfront Planning에서:
   <ul><li>
   작업 공간 및 레코드 유형에 대한 권한을 보고 연결된 레코드를 볼 수 있습니다 </li>
   또는
   <li> 작업 공간 및 레코드 유형에 참여하거나 더 높은 권한을 부여하여 레코드 연결 또는 연결 해제</a></li></ul> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 Workfront Planning 작업 영역에 대한 권한을 가집니다</p> 
  </td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 계획 섹션의 레코드 관리

Workfront 객체의 Planning 섹션을 사용하여 Workfront 객체에 연결된 모든 레코드 유형과 해당 레코드를 볼 수 있습니다.
계획 섹션은 다음 Workfront 객체에 사용할 수 있습니다.

* 프로젝트
* 포트폴리오
* 프로그램
<!--* Group
* Company-->

### Workfront 객체의 계획 섹션에 대한 고려 사항

Workfront 객체의 계획 섹션에서 Workfront Planning 레코드를 볼 때는 다음 사항을 고려하십시오.

* Workfront Planning 레코드 유형은 먼저 Workfront 객체 유형에 연결되어야 합니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [레코드 유형 연결](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [기록 연결](/help/quicksilver/planning/records/connect-records.md)
* Workfront 객체와 연관된 레코드가 없는 경우에도 Workfront 객체에서 계획 섹션을 볼 수 있습니다.

### 계획 섹션에서 레코드 연결 관리

{{step1-to-planning}}

1. 작업 영역의 카드를 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. Workfront 프로젝트, 포트폴리오 또는 프로그램에 연결된 레코드 유형의 카드를 클릭합니다.
1. 테이블 보기 또는 레코드의 세부 사항 페이지에서 Workfront 개체와 연결된 연결된 레코드 필드로 이동합니다. 자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.
1. 연결된 레코드 필드에서 Workfront 개체의 이름을 클릭합니다.
개체의 페이지가 Workfront에서 열립니다.

   >[!NOTE]
   >
   >  Planning 레코드에 이미 연결된 Workfront 객체를 알고 있는 경우 Workfront 객체에서 Planning 섹션으로 이동할 수 있습니다.

1. 왼쪽 패널에서 **계획**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >   Workfront 또는 그룹 관리자는 Workfront 프로젝트, 포트폴리오 또는 프로그램에 대해 표시되기 전에 레이아웃 템플릿에 계획 섹션을 추가해야 합니다.

   계획 섹션에는 다음 정보가 표시됩니다.

   * 연결된 레코드는 다음 정보가 포함된 개별 카드에 표시됩니다.
      * 레코드 이름
      * 레코드 썸네일
      * Workfront Planning에 표시되는 연결된 레코드 필드의 이름.
   * 레코드는 해당 작업 공간 및 레코드 유형 아래에 표시됩니다.

   ![프로젝트의 계획 섹션](assets/planning-section-on-project.png)

1. (선택 사항) 연결된 레코드가 없는 레코드 종류를 포함하여 연결된 모든 레코드 종류를 표시하려면 **모든 연결 표시**&#x200B;를 클릭합니다. 기본적으로 연결된 레코드가 없는 레코드 유형은 표시되지 않습니다.
1. 레코드에 대한 자세한 내용을 표시하려면 레코드 카드를 클릭합니다. 레코드 미리 보기 상자가 표시됩니다.
1. (선택 사항) 레코드의 미리 보기 상자에서 필드 수정을 시작합니다. 변경 사항은 자동으로 저장됩니다.
1. (선택 사항) 미리 보기 상자의 오른쪽 상단에 있는 **새 탭에서 열기** 아이콘 ![새 탭에서 세부 정보 열기](assets/open-details-in-a-new-tab-icon.png)을 클릭하여 레코드의 세부 정보 페이지를 엽니다. 레코드의 세부 사항 페이지가 Workfront Planning에 열립니다.
1. (선택 사항) 레코드 카드 위로 마우스를 가져간 다음 레코드 연결 끊기 아이콘 **-**&#x200B;을 클릭한 다음 **연결 끊기**를 클릭합니다.
다음과 같은 상황이 발생합니다.
   * 레코드가 더 이상 Workfront 개체에 연결되어 있지 않습니다.
   * Workfront 개체는 Workfront Planning에서 레코드의 연결된 필드에서도 제거됩니다.
   * 계획 레코드에 연결된 Workfront 조회 필드의 값도 삭제됩니다.
1. 연결된 레코드 형식에 대한 레코드를 더 연결하려면 **연결**&#x200B;을(를) 클릭하십시오.

   자세한 내용은 [레코드 연결](/help/quicksilver/planning/records/connect-records.md)을 참조하세요.
1. (선택 사항) 연결할 레코드를 찾을 수 없는 경우 해당 레코드를 추가하려면 **+ 추가**&#x200B;를 클릭하여 새 레코드를 추가합니다. 자세한 내용은 문서 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)의 &quot;다른 레코드와 연결할 때 레코드 만들기&quot; 섹션을 참조하십시오.

   다음과 같은 상황이 발생합니다.

   * 레코드는 즉시 Workfront 개체에 연결되고 계획 섹션에 표시됩니다.
   * Workfront 개체가 Workfront Planning 레코드의 연결된 필드에 추가됩니다.
   * 계획 레코드에 연결된 Workfront 조회 필드의 값은 Workfront Planning에서 채워집니다.

## Planning 연결 필드 유형의 레코드 관리

Workfront 객체에서 Planning 연결 사용자 정의 필드를 사용하여 Workfront 객체에 연결된 하나의 레코드 유형과 해당 레코드를 볼 수 있습니다.

Planning 연결 사용자 정의 필드를 생성할 때 Workfront 객체에 대해 표시되는 Planning 레코드 유형을 제어할 수 있습니다.

* Planning 연결 필드는 연결이 설정된 후 필드가 다음 Workfront 객체의 양식에 첨부된 경우 Planning 레코드를 표시합니다.

   * 프로젝트
   * 포트폴리오
   * 프로그램
   * 그룹
   * 회사

자세한 내용은 [양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

### Planning 연결 필드 유형에 대한 고려 사항

Workfront 객체의 Planning 연결 필드에서 Workfront Planning 레코드를 볼 때 다음 사항을 고려하십시오.

* Planning 레코드가 Workfront 객체에 연결된 후 Planning 연결 필드가 Workfront 객체의 사용자 정의 양식에 다음과 같이 표시됩니다.

   * 연결된 레코드의 기본 필드만 선택한 경우, 연결에 의해 여러 레코드가 연결될 수 있는 경우 Planning 연결 필드는 여러 값이 있는 필드로 표시됩니다. 자세한 내용은 [레코드 종류 연결 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)를 참조하십시오.
   * Workfront 또는 그룹 관리자가 사용자 정의 양식에 연결된 레코드에서 추가 조회 필드를 추가한 경우 Planning 연결 필드가 표로 표시됩니다. Planning 연결 필드에 대해 최대 7개의 필드를 선택할 수 있습니다. 테이블 보기는 읽기 전용입니다.

* 하나의 레코드 유형만 하나의 Planning 연결 필드에 연결할 수 있습니다. 양식에 있는 Planning 연결 필드 수에는 제한이 없습니다.
* Planning 연결 사용자 정의 필드가 있는 사용자 정의 양식을 Workfront 객체에 첨부하려면 객체, 레코드 및 Workfront Planning에 대한 올바른 액세스 및 권한이 있어야 합니다.
* Workfront 개체의 Planning 연결 필드에서 레코드를 연결하거나 연결을 끊으려면 Workfront Planning의 작업 영역에 대한 Contribute 권한이 있어야 합니다.
* Workfront Planning 레코드 유형은 먼저 Workfront 객체 유형에 연결되어야 합니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하십시오.이렇게 하면 Workfront에서 Workfront Planning 레코드에 액세스할 수 있습니다.
* Workfront Planning 연결이 가능한 객체에 대해서만 Workfront 객체의 Planning 연결 필드에서 레코드를 연결하거나 연결을 해제할 수 있습니다.

  예를 들어 Planning 연결 필드가 있는 사용자 정의 양식을 작업에 첨부할 수 있지만 Workfront Planning 객체를 작업에 연결할 수는 없습니다.
* Workfront 오브젝트를 일괄적으로 편집할 때는 Planning 연결 필드를 편집할 수 없습니다.

### Planning 연결 필드 유형에서 레코드 연결 관리

1. Workfront Planning 레코드 유형과 연결된 다음 객체 유형 중 하나로 이동합니다.

   * 프로젝트
   * 포트폴리오
   * 프로그램
   * 회사
   * 그룹

1. 왼쪽 패널에서 **&lt; 개체 > 세부 정보**&#x200B;를 클릭합니다.
1. (조건부) 선택한 객체에 대해 하나 이상의 Planning 연결 필드가 있는 사용자 정의 양식을 추가합니다(없는 경우).

   >[!NOTE]
   >
   >먼저 Workfront 또는 그룹 관리자가 양식을 만들고 Planning 연결 필드를 추가한 후에 객체에 추가해야 합니다.


1. 연결된 레코드를 추가하려면 필드 내부를 클릭하고 목록에서 레코드를 선택하려면 필드 내부의 아래쪽 화살표를 클릭합니다.

   ![레코드 목록이 열려 있는 프로젝트의 Planning 연결 필드](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >필드를 구성할 때 선택한 개체가 아닌 Workfront 개체와 연결된 Planning 연결 필드에는 레코드를 추가할 수 없습니다.
   >
   >예를 들어 프로젝트의 사용자 정의 양식에서 Portfolio 연결을 위해 만들어진 Planning 연결 필드에 레코드를 추가할 수 없습니다.
   >
   >필드의 개체와 선택한 개체가 일치하지 않음을 나타냅니다.
   >
   >![양식의 지원되지 않는 개체 계획 연결 필드 경고](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. 목록 외부를 클릭하여 닫습니다.

   다음과 같은 상황이 발생합니다.

   * 레코드는 즉시 Workfront 개체에 연결되고 Workfront 개체의 Planning 섹션과 Planning 연결 필드에 표시됩니다.
   * Workfront 개체가 Workfront Planning 레코드의 연결된 필드에 추가됩니다.
   * 계획 레코드에 연결된 Workfront 조회 필드의 값은 Workfront Planning에서 채워집니다.
   * Workfront 또는 그룹 관리자가 사용자 정의 양식을 만들 때 레코드 조회 필드를 추가한 경우 레코드의 조회 필드가 표 보기에 자동으로 채워집니다. Planning 연결 필드의 테이블 보기는 읽기 전용입니다.

     ![프로젝트 세부 정보 사용자 정의 양식의 테이블이 있는 연결 필드 계획](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

     >[!NOTE]
     >
     >조회 필드가 사용자 정의 양식의 Planning 연결 필드에 추가된 경우에만 테이블 보기가 표시됩니다.


1. (선택 사항) 레코드 이름을 클릭하거나 테이블의 레코드 이름을 마우스로 가리킨 다음, Planning 연결 필드에서 **레코드 열기** 아이콘 ![Planning 연결 사용자 정의 양식의 레코드 열기 아이콘](assets/open-record-icon-on-planning-connection-custom-form.png)을 클릭하여 Workfront Planning에서 엽니다.
Workfront Planning 레코드 세부 정보 미리 보기 상자가 열립니다.
1. 레코드에 대한 정보를 검토하거나 편집하거나 **새 탭에서 열기** 아이콘 ![새 탭에서 레코드 열기](assets/open-details-in-a-new-tab-icon.png)를 클릭하여 레코드 세부 정보 페이지를 엽니다.

1. (선택 사항) Workfront의 사용자 정의 양식에서 레코드의 **제거** 아이콘 ![제거 아이콘](assets/remove-icon.png)을 클릭하여 Planning 연결 필드에서 제거하고 Workfront 개체에서 연결을 해제합니다.
Planning 레코드에서 Workfront 개체의 연결이 끊기고 Workfront의 모든 조회 정보가 레코드에서 제거됩니다.

1. **변경 내용 저장**&#x200B;을 클릭하여 사용자 정의 양식과 Workfront 개체에 적용한 다른 변경 내용을 저장합니다.
