---
title: Adobe Workfront Planning CX Coworker 개요
description: Workfront Planning의 CX Coworker을 사용하여 일반적으로 인터페이스에서 수행하는 Planning의 레코드 및 기타 객체와 유사한 작업을 수행할 수 있습니다. 사용자의 명령과 AI의 해당 명령 실행은 함께 작동하여 AI가 수행한 변경 사항이 환경에 정확하게 반영되도록 합니다.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3934b1b333f86c8c700617871bfaac23d2b19213
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%
---

# Adobe Workfront Planning CX Coworker 개요

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기에 릴리스된 후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 매월 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>


{{planning-important-intro}}

CX Coworker은 목표를 일반 언어로 설명한 다음 Workfront Planning 및 기타 연결된 Adobe 시스템에서 작업을 계획, 실행 및 검증한 후 승인을 위해 다시 가져오는 대화 인터페이스입니다.

CX Coworker은 새로운 전체 화면 경험과 Workfront 오른쪽 레일 모두에서 강력한 엔드 투 엔드 기능을 추가하면서 현재 AI Assistant가 수행하는 모든 작업을 유지합니다.

조직의 기존 제품 수준 액세스 제어 내에서 작동하므로 사용자는 기본적으로 읽기 전용 액세스 권한과 Workfront 관리자가 제어하는 쓰기 액세스 권한으로 Workfront에서 이미 허용된 작업만 수행할 수 있습니다.

>[!IMPORTANT]
>
>CX Coworker 는 현재 의료 서비스, 금융 기관 또는 중요한 데이터가 있는 기타 업계 조직에서 사용할 수 없습니다. 이러한 조직에서는 AI Assistant를 사용할 수 있습니다.
>
>자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.


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
<p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p>
또는
<p>독립 실행형 제품으로 구입할 경우 모든 Planning 패키지</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning 라이선스</p></td> 
   <td><p>표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td>  
   <p>관리자는 Planning에서 CX Coworker에 대한 액세스를 허용하려면 다음을 수행해야 합니다.</p>
   <ul>
   <li><p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가합니다.</p></li>
   <li><p>액세스 수준에서 Workfront의 CX Coworker 패널 비활성화 설정을 선택 취소합니다. 기본적으로 선택되어 있습니다.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>시스템 설정</p></td> 
   <td>   <p>Workfront 관리자는 [설정]의 [시스템 환경 설정] 영역에서 [읽기 전용] 및 [쓰기 전용] MCP 도구를 선택해야 합니다. 읽기 전용 MCP 도구는 기본적으로 선택됩니다.</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## CX Coworker에 대한 고려 사항

* 조직의 사용자가 CX Coworker을 사용하려면 먼저 귀사에서 활성화해야 합니다.

  자세한 내용은 [CX Coworker 개요](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)를 참조하십시오.

* Workfront이 Workfront 인스턴스에 대해 에이전트를 활성화하면 기본 Workfront 관리자가 이를 사용할 수 있으며 조직에서 활성화할 수 있습니다. 자세한 내용은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

* Workfront 관리자는 또한 액세스 수준에서 CX Coworker을 활성화해야 합니다. 자세한 내용은 [액세스 수준 만들기 및 수정](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)을 참조하세요.

* CX Coworker은 Workfront 또는 Workfront Planning에 있고 사용자가 액세스할 수 있는 권한이 있는 정보 및 오브젝트와 함께 작동합니다. [계획] 오른쪽 레일에서 [동료] 패널은 사용자가 연 작업 공간, 레코드 유형 또는 레코드 페이지의 컨텍스트에서 작동합니다.

* 계획 영역에서 CX Coworker이 수행하는 작업은 Workfront Planning 권한 및 Workfront 액세스 수준의 컨텍스트에 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

  * [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)

* 사용자를 대신하여 CX Coworker에서 수행한 변경 사항은 레코드의 내역 패널에서 추적됩니다.

* CX Coworker에서 수행한 작업은 영구적이며 취소가 불가능합니다. 예를 들어 필드를 삭제하면 되돌릴 수 없습니다. CX Coworker에서 제안한 모든 작업을 수락하기 전에 검토하십시오.

* CX Coworker을 통해 오브젝트를 만들거나, 업데이트하거나, 삭제할 때, CX Coworker은 의도한 작업을 표시하고 확인을 요청합니다. 그런 다음 작업을 확인하거나 취소할 수 있습니다.

## 현재 CX Coworker에서 사용할 수 있는 기능

현재 CX Coworker은 Workfront의 계획 영역에서 사용할 수 있으며 일련의 기술을 사용하여 Planning 객체의 정보에 액세스하고 정보를 조작합니다. 자세한 내용은 [CX Coworker 기술](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md)을 참조하세요.

CX Coworker을 사용하여 다음 작업을 수행할 수 있습니다.

* 레코드를 검색합니다. 레코드 필드에 포함된 정보별로 검색할 수 있습니다.
* 레코드를 만듭니다. 새 레코드에 대한 링크가 있는 ID는 레코드가 생성된 후에 표시됩니다. 생성 프로세스 중에 업데이트할 날짜 또는 설명 등의 필드를 지정할 수 있습니다.
* 업로드한 문서를 기반으로 레코드를 만듭니다. Workfront은 CX Coworker에 대해 다음 문서 형식을 지원합니다.

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT 및 대부분의 이미지 형식
* 화면에 표시되는 레코드의 필드를 업데이트합니다.
* 레코드 삭제, 복제 또는 복원
* 다른 레코드에 레코드 연결
* 레코드의 변경 내역 보기


## Workfront Planning에서 CX Coworker 찾기

Workfront Planning의 다음 영역에서 CX Coworker을 찾을 수 있습니다.

* 화면 오른쪽 상단의 기본 탐색 모음
* 새 탭에서 레코드를 열 때 레코드의 세부 정보 영역 내부에 있습니다.

## 계획 영역에서 CX Coworker 액세스

1. Workfront에 로그인한 다음 왼쪽 상단의 **주 메뉴** 아이콘 ![줄 주 메뉴](assets/lines-main-menu.png)를 클릭한 다음 **계획**&#x200B;을 클릭합니다.

   계획 영역이 열립니다.

   페이지의 오른쪽 상단에 있는 **Coworker** 아이콘 ![Coworker 아이콘](assets/coworker-icon.png)을 찾거나 아래 단계를 계속 진행합니다.

1. **작업 영역 카드**&#x200B;를 클릭합니다.

1. **레코드 종류 카드**&#x200B;를 클릭합니다.

1. **레코드**&#x200B;을(를) 클릭하여 레코드의 **세부 정보** 페이지를 연 다음 **새 탭에서 열기** 아이콘 ![새 탭에서 열기](assets/open-workspace-on-new-tab-icon.png)을(를) 클릭합니다.

1. 화면 오른쪽 상단의 **CX Coworker 아이콘** ![Coworker 아이콘](assets/coworker-icon.png)을 클릭합니다.

1. 제공된 공백에서 CX Coworker에 대한 명령을 입력한 다음 완료되면 Enter 키를 누릅니다.

   ![빈 명령 상자가 있는 CX Coworker 패널](assets/cx-coworker-right-rail.png)

   예를 들어 다음 중 하나를 입력할 수 있습니다.

   * Summer Sale 2026이라는 새로운 캠페인 레코드 만들기
   * 여름 캠페인 레코드의 예산 필드를 $75,000로 업데이트
   * 이전 프로모션이라는 캠페인 레코드 삭제
   * 내가 실수로 삭제한 캠페인 복원

   >[!TIP]
   >
   >Workfront 관리자에게 개체에 대한 편집 작업을 수행하도록 요청하기 전에 시스템 환경 설정에서 CX Coworker 관리자가 쓰기 전용 MCP 도구를 활성화했는지 확인하십시오.

   CX Coworker이 명령을 처리하는 동안 시각적 표시기가 표시되어 응답 시간에 대한 기대를 설정합니다.

   성공적인 응답을 받은 후 제공된 링크를 따르거나 왼쪽에 변경 사항을 확인합니다.


1. (선택 사항) **전체 화면 확장** 아이콘 ![전체 화면 확장](assets/expand-full-screen-icon.png)을 클릭하여 전체 브라우저 탭에서 동료 대화 상자를 엽니다.


