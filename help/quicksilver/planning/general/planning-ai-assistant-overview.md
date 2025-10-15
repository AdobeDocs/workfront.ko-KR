---
title: Adobe Workfront Planning AI Assistant 개요
description: AI 비서를 사용하여 현재 페이지 컨텍스트 및 레코드 구조를 기반으로 레코드를 생성, 업데이트 또는 제거할 수 있습니다. 사용자의 명령과 AI의 해당 명령 실행은 함께 작동하여 AI가 수행한 변경 사항이 환경에 정확하게 반영되도록 합니다.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: a24180f95c89c76605eaa735467a791102254645
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---


# Adobe Workfront Planning AI Assistant 개요

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

AI Assistant를 사용하여 현재 페이지 컨텍스트 및 레코드 구조를 기반으로 레코드를 생성, 업데이트 또는 제거할 수 있습니다.

사용자의 명령과 AI의 해당 명령 실행은 함께 작동하여 AI가 수행한 변경 사항이 환경에 정확하게 반영되도록 합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul><li><p>모든 Workfront 패키지</p></li>
And
<li><p>모든 Planning 패키지</p></li></ul>
또는
<ul><li><p>모든 워크플로우 패키지</p></li>
And
<li><p>모든 Planning 패키지</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## AI Assistant에 대한 고려 사항

* 귀사의 사용자가 AI Assistant를 사용할 수 있으려면 먼저 귀사에서 AI Assistant를 활성화해야 합니다. 자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.
* Workfront이 조직에 대해 AI Assistant를 활성화하면 기본 Workfront 관리자가 사용할 수 있습니다. 자세한 내용은 [시스템에 대한 기본 정보 구성](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.

* Workfront 관리자는 다른 모든 사용자에 대해 AI Assistant를 활성화해야 합니다. 자세한 내용은 [AI Assistant 사용 또는 사용 안 함](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)을 참조하십시오.

* AI 도우미는 각 페이지의 컨텍스트에서 작동합니다. AI Assistant에 대해 제출 중인 요청은 열려 있는 페이지에서 사용할 수 있는 기능을 참조해야 합니다.

* 계획 영역에서 AI 어시스턴트가 수행하는 작업은 Workfront 계획 권한 및 Workfront 액세스 수준의 컨텍스트에 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)

* 사용자를 대신하여 AI 어시스턴트가 변경한 내용은 레코드 기록 패널에서 추적됩니다.

* 명령을 사용하여 작업을 취소할 수 있습니다. 예를 들어 &quot;마지막 변경 내용 실행 취소&quot;를 입력하여 변경 내용을 되돌릴 수 있습니다.

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

Workfront Planning의 다음 영역에서 AI Assistant를 찾을 수 있습니다.

* 화면 오른쪽 상단의 기본 탐색 모음
* 미리 보기에서 레코드를 연 후 또는 레코드의 페이지를 연 후 레코드의 세부 사항 영역 내에서.

## 계획 영역에서 AI 지원에 액세스

1. Workfront에 로그인한 다음 화면 오른쪽 상단의 **주 메뉴** 아이콘 ![점 주 메뉴](assets/dots-main-menu.png) 또는 사용 가능한 경우 왼쪽 상단의 **주 메뉴** 아이콘 ![선 주 메뉴](assets/lines-main-menu.png)을 클릭합니다.

. **계획**&#x200B;을 클릭합니다. 계획 영역이 열립니다.

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



