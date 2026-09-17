---
title: Adobe Workfront Planning AI Assistant 개요
description: AI 비서를 사용하여 현재 페이지 컨텍스트 및 레코드 구조를 기반으로 레코드를 생성, 업데이트 또는 제거할 수 있습니다. 사용자의 명령과 AI의 해당 명령 실행은 함께 작동하여 AI가 수행한 변경 사항이 환경에 정확하게 반영되도록 합니다.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3I5y7eTZml-nkAiAYnBFuaw72DyXgNG12D-EVYVourA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 1%
---
# Adobe Workfront Planning AI Assistant 개요



<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 미리보기에 릴리스된 후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 매월 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>



{{planning-important-intro}}

AI Assistant를 사용하여 현재 페이지 컨텍스트를 기반으로 Adobe Workfront Planning에서 레코드 및 기타 객체를 변경하거나 갱신할 수 있습니다.

사용자의 명령과 AI의 해당 명령 실행은 함께 작동하여 AI가 수행한 변경 사항이 환경에 정확하게 반영되도록 합니다.

>[!IMPORTANT]
>
><span class="preview">일부 조직에서는 AI 도우미가 CX Coworker으로 대체되었습니다. 자세한 내용은 [Adobe Workfront Planning CX Coworker 개요](/help/quicksilver/planning/general/planning-cx-coworker-overview.md).</span>를 참조하십시오.

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
     <p>관리자는 AI Assistant에 대한 액세스를 허용하려면 다음을 수행해야 합니다.</p>
   <ul>
   <li><p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가합니다.</p></li>
   <li><p>액세스 수준에서 Workfront AI Assistant 설정 비활성화를 선택 취소합니다</p></li></ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>시스템 설정</p></td> 
   <td>   <p>Workfront 관리자가 설정의 시스템 환경 설정 영역에서 AI 활성화 설정을 선택하고 AI에 서명하여 AI Assistant에 액세스해야 합니다</p>  
    </td> 
  </tr> 
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## AI Assistant에 대한 고려 사항

* 귀사의 사용자가 AI Assistant를 사용할 수 있으려면 먼저 귀사에서 AI Assistant를 활성화해야 합니다.

  자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.

* Workfront이 조직에 대해 에이전트를 활성화하면 기본 Workfront 관리자가 사용할 수 있습니다. 자세한 내용은 [시스템 환경 설정 구성](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

* Workfront 관리자는 다른 모든 사용자에 대해 AI Assistant를 활성화해야 합니다. 자세한 내용은 [AI Assistant 사용 또는 사용 안 함](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)을 참조하십시오.

* AI 도우미는 각 페이지의 컨텍스트에서 작동합니다. AI Assistant에 대해 제출 중인 요청은 열려 있는 페이지에서 사용할 수 있는 기능을 참조해야 합니다.

* 계획 영역에서 AI 어시스턴트가 수행하는 작업은 Workfront 계획 권한 및 Workfront 액세스 수준의 컨텍스트에 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

  * [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)

* 사용자를 대신하여 AI 어시스턴트가 변경한 내용은 레코드 기록 패널에서 추적됩니다.

* AI 관리자가 수행하는 작업은 영구적이며 취소될 수 있습니다. 예를 들어 필드를 삭제하면 되돌릴 수 없습니다. AI 도우미가 제안한 모든 작업을 수락하기 전에 검토하십시오.

* AI 어시스턴트를 통해 오브젝트를 생성, 업데이트, 삭제할 경우 AI 어시스턴트가 의도한 동작을 표시하고 확인을 요청한다. 그런 다음 작업을 확인하거나 취소할 수 있습니다.

## 현재 AI Assistant에서 사용할 수 있는 기능

현재 Workfront의 계획 영역에서 다음 페이지에 AI Assistant를 사용할 수 있습니다.

* Workspace 페이지
* 레코드 유형 페이지
* 레코드 페이지

현재 AI Assistant를 사용하여 다음 작업을 수행할 수 있습니다.

* 레코드를 검색합니다. 레코드 필드에 포함된 정보별로 검색할 수 있습니다.
* 레코드를 만듭니다. 새 레코드에 대한 링크가 있는 ID는 레코드가 생성된 후에 표시됩니다. 생성 프로세스 중에 업데이트할 날짜 또는 설명 등의 필드를 지정할 수 있습니다.
* 업로드한 문서를 기반으로 레코드를 만듭니다. Workfront은 AI Assistant에 대해 다음 문서 형식을 지원합니다.

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT 및 대부분의 이미지 형식
* 화면에 표시되는 레코드의 필드를 업데이트합니다.
* 레코드 삭제
* 방금 삭제한 레코드 복원


## Workfront Planning에서 AI Assistant 찾기

>[!NOTE]
>
><span class="preview">조직에서 CX Coworker에 대한 액세스 권한을 받은 경우 CX Coworker을 찾는 것은 AI Assistant를 찾는 것과 비슷합니다. 자세한 내용은 [Adobe Workfront Planning CX Coworker 개요](/help/quicksilver/planning/general/planning-cx-coworker-overview.md).</span>를 참조하십시오.


Workfront Planning의 다음 영역에서 AI Assistant를 찾을 수 있습니다.

* 화면 오른쪽 상단의 기본 탐색 모음
* 미리 보기에서 레코드를 연 후 또는 레코드의 페이지를 연 후 레코드의 세부 사항 영역 내에서.

### 계획 영역에서 AI 지원에 액세스

1. Workfront에 로그인한 다음 왼쪽 상단의 **주 메뉴** 아이콘 ![줄 주 메뉴](assets/lines-main-menu.png)를 클릭한 다음 **계획**&#x200B;을 클릭합니다.

   계획 영역이 열립니다.

1. **작업 영역 카드**&#x200B;를 클릭합니다.

1. (선택 사항) **레코드 종류 카드**&#x200B;를 클릭합니다.

1. (선택 사항) **레코드**&#x200B;을(를) 클릭하여 레코드의 **세부 정보** 페이지를 엽니다.

1. 전역 탐색 막대에서 화면 오른쪽 위 모서리나 레코드 미리 보기 또는 페이지의 오른쪽 위 모서리에 있는 **AI Assistant 아이콘**&#x200B;을 클릭합니다.

   ![AI 길잡이 아이콘](assets/ai-assistant-icon-highlighted.png)

1. 제공된 공간에서 AI Assistant에 대한 명령을 입력한 다음 완료되면 Enter 를 클릭합니다.

   ![빈 명령 상자가 있는 AI 도우미 패널](assets/ai-assistant-panel-with-empty-command-box.png)

   예를 들어 다음 중 하나를 입력할 수 있습니다.

   * 시작일이 7월 4일이고 종료일이 7월 30일인 캠페인 만들기
   * 결정해야 하는 날짜로 여름 캠페인 레코드의 설명 필드를 업데이트합니다.
   * 마지막 레코드 삭제
   * 레코드 복원

   AI 어시스턴트가 명령을 처리하는 동안 시각적 표시기가 표시돼 응답 시간에 대한 기대치를 설정할 수 있다.

   성공적인 응답을 받은 후 제공된 링크를 따르거나 왼쪽에 변경 사항을 확인합니다.



