---
title: Adobe Workfront Planning Designer 시작
description: AI에서 제공하는 Adobe Planning Designer을 사용하여 작업 공간 및 데이터 구조를 쉽게 구성할 수 있습니다. Planning Designer은 작업 공간 생성 및 구성에서 필드 및 공식 정의, 레코드 관리, 변경 내용 검토 및 사용자 정의 보기 작성에 이르기까지 모든 작업을 지원합니다. Planning Designer은 직접 사용하든 AI Assistant를 통해 사용하든 상관없이 구조화되고 연결된 정보를 구축하고 유지할 수 있는 유연하고 강력한 환경을 제공합니다.
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
source-git-commit: b52c188d767ee37699ead71ed90642458d9889fa
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---


# Adobe Workfront Planning Designer 시작

>[!IMPORTANT]
>
>Planning Designer은 현재 Closed Beta 프로그램에 참여하는 사용자만 사용할 수 있습니다.
>
>이 문서의 정보는 Adobe Workfront의 추가 기능인 Adobe Workfront Planning을 참조합니다.
>
>Workfront Planning에 액세스하기 위한 요구 사항 목록은 [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.
> 
>Workfront Planning에 대한 일반적인 정보는 [Adobe Workfront Planning 시작](/help/quicksilver/planning/general/planning-overview.md)을 참조하십시오.

AI에서 제공하는 Adobe Planning Designer을 사용하여 작업 공간 및 데이터 구조를 쉽게 구성할 수 있습니다. Planning Designer은 작업 공간 생성 및 구성에서 필드 및 공식 정의, 레코드 관리, 변경 내용 검토 및 사용자 정의 보기 작성에 이르기까지 모든 작업을 지원합니다.

Planning Designer은 직접 사용하든 AI Assistant를 통해 사용하든 상관없이 구조화되고 연결된 정보를 구축하고 유지할 수 있는 유연하고 강력한 환경을 제공합니다.

Workfront Planning에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront Planning에 대한 일반 정보](/help/quicksilver/planning/planning-information.md)
* [Adobe Workfront Planning 시작](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)


## 액세스 요구 사항 <!--edit theses??-->

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
<p>모든 Workfront 및 Planning 패키지</p>
<p>모든 워크플로우 및 계획 패키지</p>
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

## Planning Designer에 대해 마감된 Beta 프로그램에 등록

현재, sargism@adobe.com으로 이메일을 보내 Planning Designer에 대한 Closed Beta 프로그램에 참여를 요청할 수 있습니다.

이메일을 수신하면 엔지니어링 팀이 Workfront 인스턴스에서 계획 Designer을 켭니다.

>[!IMPORTANT]
>
>시스템에서 Planning Designer을 사용하려면 먼저 귀사에서 AI Assistant 계약에 동의해야 합니다.

## Planning Designer에 대한 피드백 제출

Beta 프로그램 중에 Planning Designer에 대한 피드백을 제출할 수 있습니다.

1. Workfront에 로그인한 다음 왼쪽 상단의 **주 메뉴** 아이콘 ![줄 주 메뉴](assets/lines-main-menu.png)를 클릭한 다음 **계획**&#x200B;을 클릭합니다.

   **계획** 영역이 열립니다.

1. **AI로 만들기**&#x200B;를 클릭합니다. <!--update this tag name when they change it-->

   **Workspace 계획 중** 창의 **Designer 설정** 영역이 열립니다. <!--replace shot below when they rename the area to Planning Designer-->

1. 페이지 하단의 **여기에 피드백 제출**&#x200B;을 클릭합니다.
1. 제공된 스페이스에 피드백을 추가한 다음 **제출**을 클릭합니다.
귀하의 피드백은 엔지니어링 및 제품 팀에 제출됩니다.

## Planning Designer에 대한 고려 사항

* Planning Designer을 사용하려면 먼저 조직에 대한 AI Assistant를 켜야 합니다. 조직의 모든 사용자가 AI Assistant를 사용할 수 있으려면 다음 조건을 충족해야 합니다.

   * Workfront은 귀사에서 AI Assistant를 사용할 수 있도록 해야 합니다.

     자세한 내용은 [AI Assistant의 필수 구성 요소](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)를 참조하십시오.
   * Workfront에서 조직에서 AI Assistant를 사용할 수 있도록 하면 주 Workfront 관리자가 액세스할 수 있습니다.

     자세한 내용은 [시스템에 대한 기본 정보 구성](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.
   * Workfront 관리자는 AI Assistant 계약에 동의한 다음 다른 모든 사용자에 대해 AI Assistant를 켜야 합니다.

     자세한 내용은 [AI Assistant 사용 또는 사용 안 함](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)을 참조하십시오.
* 시스템 관리자가 조직에 대해 AI 비서를 켜면 기본적으로 모든 사용자가 Planning Designer을 사용할 수 있습니다(조직에서 사용할 수 있게 된 경우).
* Planning Designer에서 수행하는 작업은 계획 영역에서 AI 도우미를 사용할 때도 수행할 수 있습니다.
* 계획 영역에서 AI 어시스턴트에 의해 수행되는 작업이나 Planning Designer에 의해 수행되는 작업은 Workfront Planning 권한 및 Workfront 액세스 수준의 컨텍스트에 있습니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)

* 사용자를 대신하여 AI Assistant 또는 Planning Designer에서 수행한 변경 사항은 레코드의 내역 패널에서 추적됩니다.

* Planning Designer에서 수행한 작업은 영구적이며 취소가 불가능합니다. 예를 들어 필드를 삭제하면 되돌릴 수 없습니다. Designer에서 제안한 모든 작업을 수락하기 전에 검토하십시오.

  >[!IMPORTANT]
  >
  >Planning Designer을 통해 객체를 생성, 업데이트 또는 삭제할 때 프롬프트는 취소할 수 없는 작업에 대해서만 확인을 요청합니다. 예를 들어 레코드 유형이나 작업 영역을 삭제하면 되돌릴 수 없습니다. 레코드 삭제는 허용되지 않습니다. Planning Designer은 레코드 유형 또는 작업 영역을 삭제하려고 할 때만 확인을 요청합니다.

* Planning Designer을 사용하여 작업 공간 및 레코드 유형을 만들면 뷰 및 필드도 자동으로 생성됩니다.

## 현재 Planning Designer에서 사용할 수 있는 기능

Planning Designer 또는 AI Assistant를 사용하여 다음 작업 중 하나를 수행할 수 있습니다.

* 작업 공간 만들기 및 구성

* 작업 공간에 글로벌 레코드 유형 정의 및 추가를 포함한 레코드 유형 만들기

* 디자인 필드 또는 공식 필드

* 레코드 생성, 삭제, 복제 및 복원

* 레코드의 필드 편집, 업데이트 및 첨부

* 다른 레코드에 레코드 연결

* 레코드 변경 내역 액세스

* 사용자 정의 보기 작성

* 문서를 가져와서 레코드 만들기

  예를 들어 회사의 조직도 사진을 업로드할 수 있으며 Planning Designer에서 이를 기반으로 작업 공간을 생성할 수 있습니다.

  가져온 문서에서 개체를 만드는 방법은 Planning Designer에서만 사용할 수 있으며 AI Assistant에서는 사용할 수 없습니다.

  >[!IMPORTANT]
  >
  >.XLSX 및 .CSV 파일 유형은 지원되지만 Planning Designer을 통한 대규모 레코드 가져오기에는 사용할 수 없습니다.
  >지금 많은 레코드를 가져와야 하는 경우 Planning에서 사용할 수 있는 수동 기능을 사용하여 가져오는 것이 좋습니다.
  >
  >자세한 내용은 [CSV 또는 Excel 파일에서 정보를 가져와서 레코드 만들기](/help/quicksilver/planning/records/import-file-to-create-records.md)를 참조하십시오.
  >파일 형식 제한 사항에 대해서는 [AI에서 제공하는 양식 채우기를 사용하여 프롬프트 또는 문서를 사용하여 요청을 채우는 방법](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md)의 &quot;업로드한 문서에 따라 제안 받기&quot; 섹션을 참조하십시오.


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Planning Designer을 사용하여 객체 생성 또는 갱신

별도로 지정하지 않는 한 Planning Designer 또는 AI Assistant를 사용하여 Workfront Planning에서 객체를 생성하거나 갱신할 수 있습니다.

1. Workfront에 로그인한 다음 왼쪽 상단의 **주 메뉴** 아이콘 ![줄 주 메뉴](assets/lines-main-menu.png)를 클릭한 다음 **계획**&#x200B;을 클릭합니다.

   **계획** 영역이 열립니다. <!--update screen shot when they change the name of the button-->

   ![작업 영역 페이지에서 AI로 디자인 단추](assets/design-with-ai-button-on-workspaces-page.png)

1. **AI로 만들기**&#x200B;를 클릭합니다. <!--update this when they change it-->

   **Workspace 계획 중** 창의 **Designer 설정** 영역이 열립니다. <!--replace shot below when they rename the area to Planning Designer-->

   ![계획 Designer 창](assets/planning-designer-window.png)

1. 제공된 스페이스에서 AI Assistant에 대한 프롬프트를 입력한 다음 완료되면 Enter 키를 누릅니다.

   <!--add screen shot-->

   예를 들어 아래 프롬프트와 유사한 프롬프트를 입력할 수 있습니다.

   * 캠페인을 관리할 다섯 가지 레코드 유형으로 작업 영역 만들기 및 구성

   * 올해 월별 마케팅 캠페인 만들기

   * 마케팅 디자인 작업 영역의 상태에 대한 캠페인 필드 추가

   * 부실 상태의 모든 레코드 삭제

   * 모든 Planning 캠페인을 활성 상태로 업데이트

   * Marketing Design Workspace에서 캠페인을 가상 사용자에 연결

   * &quot;발렌타인 데이&quot; 캠페인에 대한 변경 내역 표시

   * 마케팅 디자인 작업 영역에서 캠페인에 대한 타임라인 보기 작성

   * 문서를 가져와서 레코드를 만듭니다. 가져온 문서에서 레코드를 만드는 방법은 Planning Designer에서만 사용할 수 있으며 AI Assistant에서는 사용할 수 없습니다.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. 성공적인 응답을 받은 후 프롬프트 영역에 제공된 링크에 따라 요청 개체를 생성, 업데이트 또는 검토하십시오.

   개체를 만드는 데 동의하면 변경 내용이 프롬프트 영역의 오른쪽에 표시됩니다.

   프롬프트 오른쪽에 있는 미리보기 영역에서 작업 공간, 레코드 유형, 필드, 보기 및 레코드를 볼 수 있습니다.

   >[!TIP]
   >
   >일부 객체는 확인이 필요 없이 즉시 생성됩니다.

1. (선택 사항) 객체를 추가로 편집하려면 추가 프롬프트를 입력합니다.
1. (선택 사항) **미리 보기 화면 표시 또는 숨기기** 아이콘 ![미리 보기 화면 표시 또는 숨기기 아이콘](assets/hide-show-preview-screen-in-planning-designer.png)을 클릭하여 오른쪽의 미리 보기 화면을 열거나 닫습니다.
1. **새 탭에서 작업 영역 열기** ![새 탭에서 작업 영역 열기](assets/open-workspace-on-new-tab-icon.png)를 클릭하여 업데이트하려는 작업 영역을 새 탭에서 엽니다.
1. **닫기** 아이콘 **X**&#x200B;을(를) 클릭하여 Planning Designer을 닫고 작업 영역 영역을 엽니다.
1. Planning Designer을 사용하여 편집한 작업공간을 열고 해당 객체를 추가로 변경합니다.

## 조직에 대한 Designer 계획 해제

Workfront 관리자가 AI Assistant 계약을 수락하면 기본적으로 조직의 모든 사람에 대해 Planning Designer이 켜집니다.

해제하려면:

1. Workfront에 시스템 관리자로 로그인합니다.
1. 화면 왼쪽 상단에서 **주 메뉴** ![주 메뉴 아이콘](assets/main-menu-shell.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.
1. 왼쪽 패널에서 **시스템** > 을 클릭한 다음 **AI 환경 설정** 영역으로 이동합니다.
1. **온보딩 계획** 설정을 끕니다. <!--add new screen shot with info icon and new name of the toggle; ensure you don't show the AI Reviewer if it is not in Prod yet-->

   ![시스템 환경 설정에서 Planning Designer 설정](assets/planning-designer-toggle-in-system-preferences.png)
1. **저장**&#x200B;을 클릭합니다.

   이렇게 하면 시스템의 모든 사용자에 대한 Planning Designer이 제거됩니다.






