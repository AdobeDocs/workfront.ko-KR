---
title: Adobe Workfront Planning에 환경 프로모션 사용
description: 환경 홍보 기능을 사용하여 한 Workfront 환경에서 다른 Workfront 환경으로 Planning 작업 공간, 레코드 유형, 필드 및 보기를 복사할 수 있습니다. 모든 항목을 직접 재구축하는 대신 구성을 소스 환경의 패키지로 취합하고 타겟 환경에 설치합니다.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1eaa497ba7e446f7fdf978f369205f309bbe231f
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 2%
---

# Adobe Workfront Planning에 환경 프로모션 사용

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>이 문서의 정보는 Adobe Workfront Planning을 참조합니다. Workfront Planning에 액세스하려면 회사에서 추가 Planning 패키지를 구매해야 합니다.
>
>여기에 설명된 기능은 조직이 Workfront Planning을 독립형 제품으로 구입한 경우에는 사용할 수 없습니다.
>
>Workfront Planning에 대한 일반적인 정보는 [Adobe Workfront Planning 시작](/help/quicksilver/planning/general/planning-overview.md)을 참조하십시오.
> 
>

<!--
Future - when they make it available in Planning: replace the above with this OR ... insert the snippet:

>[!IMPORTANT]
>
>The information in this article refers to Adobe Workfront Planning which your organization can purchase either as an Adobe Workfront package or a standalone product. 
>
>Not all capabilities included in the Planning package are available to Workfront Planning when it is purchased as a standalone product. 
>
>For general information about Workfront Planning, see [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
> 
>For information about Workfront Planning as a standalone product, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md). 
>
-->

환경 홍보 기능을 사용하여 한 Workfront 환경에서 다른 Workfront 환경으로 Planning 작업 공간, 레코드 유형, 필드 및 보기를 복사할 수 있습니다.

모든 항목을 직접 재구축하는 대신 구성을 소스 환경의 패키지로 취합하고 타겟 환경에 설치합니다.

Planning과 함께 환경 프로모션을 사용하는 것은 Workfront에 사용하는 것과 비슷합니다. 자세한 내용은 문서 [Adobe Workfront 테스트 환경](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md)의 &quot;환경 홍보&quot; 섹션을 참조하십시오.

## Planning과 함께 환경 프로모션 사용에 대한 고려 사항

* 환경 프로모션을 사용하려면 Workfront 관리자여야 합니다.
* 다음은 환경 프로모션을 통해 가져옵니다.

  * 작업 영역
  * Workspace 섹션
  * 레코드 유형
  * 필드
  * 보기 횟수
  * 계층
  * 모든 개체에 대한 공유 설정
  * 자동화 <!--this might not be part of it; Lilit is checking-->
  * 요청 양식
  * 비즈니스 규칙
  * 연결된 오브젝트
  * 작업공간이 종속되거나 다른 객체가 공유되는 객체(예: 그룹, 팀, 작업 역할 등) 다음과 같은 시나리오가 있습니다.

    * 대상 환경에 이름이 같은 개체가 이미 있으면 Workfront에서 충돌에 플래그를 지정하고 이를 처리하는 방법을 결정합니다.
    * 객체가 공유된 팀이나 그룹이 대상 환경에 존재하지 않으면 프로모션을 통해 생성됩니다.
* 각 객체에 대해 다음 작업을 수행할 수 있습니다.

  * 새 개체로 만들기
  * 기존 개체를 사용하되 새 이름으로 만듭니다.
  * 기존 개체를 덮어씁니다. 덮어쓰기는 타겟에서 구성을 대체합니다.

* 설치하는 데 몇 분 정도 걸릴 수 있습니다. 필요한 경우 결과 페이지에서 설치를 롤백할 수 있습니다.
* 가능하면 진행하기 전에 프로세스를 테스트하는 것이 좋습니다. 프로덕션 환경으로 승격하기 전에 샌드박스 또는 미리보기 환경에 설치할 수 있습니다.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<p>Prime 또는 Ultimate Planning 패키지가 있는 Prime 또는 Ultimate Workflow 패키지</p>
<!--This might come later: <p>Prime or Ultimate Planning package when purchased as a standalone product</p>-->
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>워크플로우 표준</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Planning 라이선스</p></td> 
   <td><p>계획 수립 표준</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가해야 합니다.</p>  
   <p>시스템 관리자여야 합니다.</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 환경 프로모션을 사용하여 Planning 구성 가져오기

다음은 Planning 구성을 다른 환경으로 승격하는 주요 단계입니다.

* [원본 환경에서 패키지를 만듭니다](#create-a-package-in-the-source-environment)
* [패키지 설치 준비 완료](#make-the-package-ready-to-install)
* [대상 환경에 패키지 설치](#install-the-package-in-the-target-environment)
* [결과 확인](#verify-the-results)

다음 섹션의 지침에 따라 두 Workfront 환경 간에 Planning 구성을 복사합니다.

### 소스 환경에서 패키지 만들기

1. 원하는 구성이 있는 소스 환경이 있어야 합니다.
1. 소스 환경에서 **주 메뉴** ![주 메뉴](assets/main-menu-shell.png)를 클릭한 다음 **설정** > **시스템** > **환경 홍보**&#x200B;로 이동합니다.
**구성 패키지** 목록에는 상태, 원본 환경 및 배포된 위치가 있는 기존 패키지가 표시됩니다.
1. **패키지 만들기**&#x200B;를 클릭합니다.

   >[!TIP]
   >
   >패키지를 조립하고 설치하려면 하나 이상의 개체가 필요합니다.
1. **패키지 세부 정보** 탭에서 패키지의 **이름** 및 **설명**&#x200B;을(를) 입력하십시오. 소스 환경이 이미 현재(소스) 환경으로 채워져 있습니다.
1. 왼쪽의 개체 형식 목록에서 **Planning 작업 영역**&#x200B;을 선택합니다.
1. 승격할 작업 영역을 검색하고 해당 확인란을 선택한 다음 **계획 작업 영역 추가**&#x200B;를 클릭합니다. 작업 영역은 **패키지 내용** 아래에 나타납니다.

   ![환경 프로모션을 위해 Workspace이 선택됨](assets/workspace-selected-for-environment-promotion.png)
1. **저장 및 결합**&#x200B;을 클릭합니다.

   Workfront이 패키지를 조합하고 패키지의 **업데이트** 탭에 항목을 추가합니다. 콘텐츠 탭에서 패키지에 포함된 내용을 검토할 수 있습니다.
1. (조건부 및 선택 사항) 나중에 마치려면 대신 **저장 후 닫기**&#x200B;를 클릭합니다.
1. (선택 사항) 패키지의 내용을 검토하려면 **내용**&#x200B;을 클릭하고 이 패키지가 여러 번 배포되었는지 확인하려면 **배포**&#x200B;를 클릭하십시오.

   패키지를 설치할 준비가 되도록 계속 만듭니다.

### 패키지 설치 준비 완료

대상 환경에 패키지를 설치하기 전에 테스트 환경에서 테스트하는 것이 좋습니다.

1. 이전 섹션에 설명된 대로 패키지 빌드가 완료되면 **패키지 세부 정보**&#x200B;를 클릭하고 **편집**&#x200B;을 클릭한 다음 **상태**&#x200B;를 **테스트**&#x200B;로 설정한 다음 **저장 및 닫기**&#x200B;를 클릭하십시오.

   >[!TIP]
   >
   >패키지를 빌드하면 상태가 **초안**(으)로 설정됩니다. 먼저 패키지를 테스트할 때까지 **Active** 상태를 사용할 수 없습니다.
1. (권장) **설치**&#x200B;를 클릭하고 사용 가능한 테스트 환경 중 하나를 선택하여 배포하고 구성을 테스트합니다.

   >[!TIP]
   >
   >상태가 **테스트**(으)로 설정된 경우 프로덕션 환경을 옵션 중 하나로 사용할 수 없습니다.

1. 테스트 환경에 설치한 후 **편집**&#x200B;을 다시 클릭하고 **상태**&#x200B;를 **활성**(으)로 설정한 다음 **저장 및 닫기**&#x200B;를 클릭합니다.

   >[!TIP]
   >
   >테스트 환경에 패키지를 설치하는 것은 다음 섹션에 설명된 대로 프로덕션에 설치하는 것과 비슷합니다.

   다음 섹션을 계속 진행하여 대상 환경에 패키지를 설치합니다.


### 대상 환경에 패키지 설치

1. 패키지 페이지에서 확인한 후 **설치**&#x200B;를 클릭합니다.
1. **대상 환경** 목록에서 배포할 환경(예: 프로덕션 환경)을 선택하고 **계속**&#x200B;을 클릭합니다. 기본 대상은 현재 환경입니다.
1. **패키지 정보** 페이지에서 배포 중인 원본 환경과 환경을 확인합니다.
1. **개체 매핑** 섹션에서 **그룹** 및 **계획 작업 영역**&#x200B;과 같은 각 개체 그룹화를 확장하여 개체를 검토하십시오.
1. 각 개체에 대해 **충돌** 및 **상태** 열을 검토한 다음 목록에서 **배포 작업**&#x200B;을 선택하십시오. 다음 선택 사항 중 하나를 선택합니다.

   * **새로 만들기**: 개체를 대상에 추가합니다. 충돌이 감지되지 않을 때 이 옵션을 사용합니다.
   * **기존 사용**: 개체를 같은 이름의 그룹과 같이 대상에 이미 있는 개체에 매핑합니다.
   * **새 이름으로 만들기**: 지정한 이름으로 개체를 추가합니다.
   * **덮어쓰기**: 대상의 기존 개체를 패키지의 개체로 바꿉니다.
1. (선택 사항) 여러 객체를 한 번에 변경하려면 해당 확인란을 선택하고 그룹 상단의 배포 작업 목록에서 작업을 선택한 다음 선택한 항목에 적용을 누릅니다. 오류만 표시 와 같은 목록 위의 필터를 사용하여 특정 객체에 초점을 맞춥니다.
1. 모든 오류 표시기를 해결합니다. 개체에 대해 **기존 개체 사용**&#x200B;을 선택한 경우 매핑되는 개체도 선택해야 합니다.  그렇지 않으면 상태가 오류가 표시되고 **배포**&#x200B;를 사용할 수 없습니다.
1. **배포**&#x200B;를 클릭한 다음 **배포**&#x200B;를 클릭하여 확인합니다.

   Workfront에 **이 패키지가 설치 중입니다** 메시지가 표시된 설치 페이지가 표시됩니다. 몇 분 정도 걸릴 수 있습니다.

   설치가 완료되면 페이지에 성공 메시지, 패키지가 설치된 환경 및 각 개체에 대한 상태와 함께 설치된 개체 목록이 표시됩니다(예: **기존 항목 사용됨** 또는 **설치됨(새로 만들기)**).
1. (선택 사항) 설치를 되돌리고 대상 환경에서 구성을 제거하려면 필요한 경우 **설치 되돌리기**&#x200B;를 클릭합니다.

   설치 결과를 계속 확인합니다.

### 결과 확인

1. 대상 환경 > **기본 메뉴** > **계획**(으)로 이동하여 가져온 작업 영역을 찾습니다.
1. 레코드 종류 및 보기를 열어 필드 및 레이아웃이 원본과 일치하는지 확인합니다. 레코드가 포함되지 않아 테이블이 비어 있습니다.


