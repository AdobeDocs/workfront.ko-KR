---
title: 종속 연결 관리
description: 작업 공간 관리자는 Adobe Workfront Planning에서 레코드 유형 간에 연결 필드를 생성할 때 종속 연결을 정의할 수 있습니다. 연결된 필드를 추가할 때 두 필드가 세 번째 레코드 유형에서 함께 나타날 때마다 연결된 레코드 유형의 값이 원본 레코드 유형(연결을 추가하는 위치)의 값에 따라 달라짐을 나타내는 설정을 켤 수 있습니다.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6f64c3e6ebb8407c38ad3a1d46b2fc63b534879e
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 1%

---


# 종속 연결 관리

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기에 릴리스된 후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 매월 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

작업 공간 관리자는 Adobe Workfront Planning에서 레코드 유형 간에 연결 필드를 생성할 때 종속 연결을 정의할 수 있습니다.

연결된 필드를 추가할 때 두 필드가 세 번째 레코드 유형에서 함께 나타날 때마다 연결된 레코드 유형의 값이 원본 레코드 유형(연결을 추가하는 위치)의 값에 따라 달라짐을 나타내는 설정을 켤 수 있습니다.

예를 들어 지역 필드에 선택한 지역에 연결된 값만 표시되도록 할 수 있습니다. 이는 연결 필드 설정에서 직접 구성됩니다. 지역 레코드 유형에서 종속 레코드 유형(예: 지역)으로 연결을 추가할 때 작업 영역 관리자가 새 설정을 통해 해당 레코드 유형 간에 이미 설정된 관계를 사용하여 지역 레코드 유형에 종속된 것으로 표시할 수 있습니다.

구성하고 나면 두 필드를 참조하는 모든 레코드 유형(예: 캠페인)에 효과가 즉시 표시됩니다. 지역 값을 선택하면 지역 선택기의 범위가 해당 지역에 실제로 연결된 지역으로만 좁혀집니다. 이렇게 하면 레코드 구조가 자동으로 적용되므로 일치하지 않는 조합이 제거되고 수동 정리가 줄어듭니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
<p>동일한 작업 영역에서 레코드 유형을 연결하려면 다음을 수행합니다. </p>
<ul> 
<li><p>모든 Planning 패키지가 있는 모든 Workfront 또는 워크플로우 패키지</p></li>
<p>또는</p>
<li><p>독립 실행형 제품으로 구입할 경우 모든 Planning 패키지</p></li>
</ul>

<p>다른 작업 공간의 레코드 유형을 연결하려면 다음을 수행합니다.</p>

<ul>

<li><p>모든 워크플로우 및 Planning Prime 또는 Ultimate 패키지</p></li>
<p>또는</p>
<li><p>독립형 제품으로 구입할 경우 모든 Planning Prime 또는 Ultimate 패키지</p></li>
</ul>
   </td> 
<tr> 
<td> 
   <p> 추가 제품</p> </td> 
   <td> 
   <p> Adobe Workfront 외에도 다음 응용 프로그램의 오브젝트와 레코드 유형을 연결하려면 다음이 있어야 합니다.</p>
   <ul><li><p>AEM 에셋을 Planning 레코드 유형과 연결하기 위한 AEM Assets 및 Workfront 간의 통합 및 Adobe Experience Manager Assets 라이선스.</p>
   <p>자세한 내용은 <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Experience Manager Assets 및 Assets Essentials용 Adobe Workfront: 기사 색인</a>을 참조하십시오. </p></li>
   <li><p> 레코드 유형을 GenStudio 개체 및 브랜드와 연결하는 Adobe GenStudio for Performance Marketing 라이선스</p>
   <p>자세한 내용은 <a href="https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/get-started">Adobe GenStudio for Performance Marketing 시작</a>을 참조하세요.</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>워크플로우 표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Planning 라이선스</p></td> 
   <td><p>계획 수립 표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가해야 합니다.</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

<!--
Sent a slack message to Norayr, Predator, Snowstorm, Armine for info for this section: 
-->

## 종속 연결된 필드에 대한 고려 사항


* 연결 필드 관계가 설정된 레코드 유형 간에만 종속 연결 필드를 설정할 수 있습니다. 관련 없는 레코드 유형 간의 종속성 논리를 정의할 수 없습니다.

* 별도의 작업 공간에 있는 레코드 유형 사이에 종속적으로 연결된 필드가 있을 수 있습니다.

* Planning 레코드 유형과 Workfront 또는 AEM 객체 유형 간에 종속적으로 연결된 필드가 있을 수 없습니다.

* 종속성 설정은 전역 규칙이 아니라 연결 필드 설정 자체 내에서 한 번에 하나의 연결로 구성됩니다.

* 연결된 두 레코드 간의 필터링 동작은 소스 필드와 종속 필드가 모두 세 번째 레코드 종류에 함께 있는 경우에만 활성화됩니다. 두 필드 중 하나만 레코드 유형에 표시되는 경우에는 종속성이 영향을 주지 않습니다.

* 종속 필드의 선택기는 레코드 수준에서 선택한 소스 값에 이미 연결된 값으로 제한됩니다. 연결되지 않은 값을 표시하거나 제안할 수 없습니다.

* 소스 필드의 값이 변경되면 종속 필드가 잘못된 상태로 남아 있지 않고 자동으로 지워져 일치하지 않는 조합이 지속되지 않습니다.

  종속 필드가 지워진 이유를 설명하는 인라인 또는 알림 메시지가 표시됩니다.

* 각 종속 필드는 최대 3개의 직접 제어 필드를 가질 수 있습니다.

* 종속성 수준은 6개의 연결로 제한됩니다. 즉, 최대 7개의 레코드 종류를 연결할 수 있습니다.

* 종속성 체인이 작동하려면 모든 종속 필드가 동일한 레코드 유형에 동시에 존재해야 합니다.

## 종속 연결 만들기

1. 작업 공간 관리자는 Workfront Planning의 레코드 유형으로 이동하여 테이블 보기에서 엽니다.
1. 테이블 보기의 오른쪽 위 모서리에 있는 **+** 아이콘을 클릭하여 새 필드를 추가합니다.
1. **새 연결**&#x200B;을 클릭한 다음 두 번째 레코드 형식에 대한 새 연결을 추가합니다.

   >[!TIP]
   >
   >두 Planning 레코드 유형 간에만 종속 연결을 생성할 수 있습니다. Workfront 또는 AEM에서 레코드 종류와 개체 간에 종속 연결을 만들 수 없습니다.
1. **연결 설정** 섹션에서 **연결을 종속적으로 설정**&#x200B;을 켭니다.

   >[!TIP]
   >
   >**이 연결을 종속적으로 만들기** 설정을 켜면 **연결된 레코드 형식에 해당하는 필드 만들기**&#x200B;가 자동으로 켜집니다. 레코드 종류당 500개의 필드로 제한됩니다.

   ![종속 연결이 활성화된 새 연결 탭](assets/dependent-connection-enabled-setting.png)

1. [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md) 문서에 설명된 대로 연결을 계속 설정합니다.
1. **저장**&#x200B;을 클릭합니다.

   다음과 같은 상황이 발생합니다.

   * 두 레코드 유형 간의 연결이 만들어지고 해당 값은 동일한 레코드 유형에서 함께 표시될 때 서로 달라집니다.
   * 제1 기록 유형을 표시하는 해당 필드가 제2 기록 유형에 대해 생성된다.
   * 두 레코드 유형이 세 번째 레코드 유형에 연결된 경우 두 번째 연결된 레코드 필드에 대한 선택 항목으로 표시되는 값은 첫 번째 레코드에 연결된 값입니다. 첫 번째 레코드 유형에 대한 선택 항목으로 표시되는 값은 두 번째 레코드 유형에 연결된 값입니다.

     자세한 내용은 이 문서에서 [종속적으로 연결된 레코드 종류의 예제](#example-of-dependent-connected-record-types) 섹션을 참조하십시오.
   * 연결된 레코드 필드의 열 헤더에 필드가 종속 연결 관계에 있음을 나타내는 표시가 있습니다.

     ![열 헤더의 종속 아이콘 도구 설명](assets/dependent-icon-tooltip-in-column-header.png)
1. (선택 사항) **레코드 필터링 규칙**&#x200B;을(를) 클릭하고 연결할 레코드 유형에서 필드를 선택하여 해당 필드 값에 대한 옵션을 제한한 다음 **완료**&#x200B;를 클릭합니다.

   두 필드가 세 번째 레코드 종류에 있으면 여기에서 선택하는 필터에 의해 연결된 필드 레코드 종류의 옵션이 제한됩니다.
1. (선택 사항 및 권장) 세 번째 레코드 유형으로 이동하고 첫 번째 및 두 번째 레코드 유형을 모두 연결된 레코드 필드로 추가합니다.

   ![세 번째 레코드 종류에 종속적으로 연결된 필드 표시기](assets/dependent-connected-field-indicator-on-a-third-record-type.png)

## 종속적으로 연결된 레코드 유형의 예

이 섹션에서는 종속 레코드 유형을 설정하는 방법과 세 번째 레코드 유형에 대해 작동하는 방법에 대한 간단한 예를 제공합니다.

1. 관리할 수 있는 작업 영역에서 다음 레코드 유형을 만듭니다.

   * 캠페인
   * 국가
   * 대륙

1. **국가** 레코드 형식에서 다음 레코드를 추가합니다.

   * 프랑스
   * 미국
   * 일본
1. **대륙** 레코드 형식에서 다음 레코드를 추가합니다.

   * 유럽
   * 아메리카
   * 아시아

1. **국가** 레코드 형식에서 **대륙**&#x200B;에 대해 연결된 종속 필드를 만드십시오.

   이렇게 하면 다음과 같은 연결된 레코드 필드가 추가됩니다.

   * **대륙** 레코드 종류에 대해 **국가**&#x200B;에 연결된 레코드 필드.
   * **국가** 레코드 종류에 대해 **대륙** 연결된 레코드 필드.

1. 다음 중 하나를 수행하십시오.

   * **국가** 레코드 형식 테이블 보기에서 대륙에 연결된 레코드 필드에 다음 값을 추가합니다.

     * 프랑스의 유럽
     * 아메리카 포 미국
     * 아시아 - 일본
   * **대륙** 레코드 형식 테이블 보기에서 연결된 **국가** 레코드 필드에 다음 값을 추가하십시오.

     * 유럽의 프랑스
     * 미국 for 아메리카
     * 일본 포 아시아
1. **국가** 및 **대륙** 연결된 필드를 **Campaign** 레코드 형식 테이블 보기에 추가합니다.
1. **Campaign** 레코드 종류의 **국가** 필드에 대해 **일본**&#x200B;을(를) 선택하십시오. 캠페인의 **대륙** 연결된 필드에 사용할 수 있는 값은 **아시아**&#x200B;뿐입니다.

   또는

   캠페인 레코드 종류의 **대륙** 필드에 대해 **유럽**&#x200B;을(를) 선택하십시오.

   캠페인의 **국가** 연결된 필드에 사용할 수 있는 값은 **프랑스**&#x200B;뿐입니다.



