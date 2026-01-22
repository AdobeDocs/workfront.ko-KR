---
title: Adobe Workfront Planning Designer 시작
description: Adobe Planning Designer을 사용하면 Workfront Planning의 레코드 유형 및 필드로 완료된 새 작업 공간을 생성하거나 작업 공간에 객체를 추가하거나 레코드에 대한 변경 내역을 볼 수 있습니다.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 1%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Adobe Workfront Planning Designer 시작

{{planning-important-intro}}

AI에서 제공하는 Adobe Planning Designer을 사용하여 새 작업 영역을 생성하거나, 작업 영역에 객체(레코드 유형, 레코드, 보기 또는 필드)를 추가하거나, 레코드에 대한 변경 내용을 볼 수 있습니다.

>[!IMPORTANT]
>
>Planning Designer은 현재 Closed Beta 프로그램에 참여하는 사용자만 사용할 수 있습니다.

Workfront Planning에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront Planning에 대한 일반 정보](/help/quicksilver/planning/planning-information.md)
* [Adobe Workfront Planning 시작](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)


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

## Planning Designer에 대해 Closed Beta 프로그램에 등록

<!--edit this Or create a new article under Beta programs?? -->

현재, Planning Designer에 대해 Closed Beta 프로그램 참여를 요청할 수 있습니다.

## Planning Designer에 대한 고려 사항

* Planning Designer을 사용하려면 조직에서 Workfront AI Assistant를 사용하기 위한 요구 사항을 충족해야 합니다.

  자세한 내용은 [AI Assistant의 필수 구성 요소](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)를 참조하십시오.

* Planning Designer을 사용하려면 시스템 관리자가 설정의 시스템 환경설정 영역에서 활성화해야 합니다.

* Planning 영역에서 Workfront AI Assistant를 사용하거나 Planning Designer을 사용하여 Planning 객체를 작성하는 프롬프트를 사용할 수 있습니다.

* 계획 영역에서 AI 어시스턴트에 의해 수행되는 작업이나 Planning Designer에 의해 수행되는 작업은 Workfront Planning 권한 및 Workfront 액세스 수준의 컨텍스트에 있습니다.

  자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)

* 사용자를 대신하여 Planning Designer에서 수행한 변경 사항은 레코드의 기록 패널에서 추적됩니다.

* 명령을 사용하여 작업을 취소할 수 있습니다. 예를 들어 &quot;마지막 변경 내용 실행 취소&quot;를 입력하여 변경 내용을 되돌릴 수 있습니다.

* Planning Designer을 통해 객체를 생성, 업데이트 또는 삭제할 때 의도한 작업을 표시하고 확인을 요청합니다. 그런 다음 작업을 확인하거나 취소할 수 있습니다.

* Planning Designer을 사용하여 작업 공간 및 레코드 유형을 만들면 뷰 및 필드도 자동으로 생성됩니다.

## 현재 Planning Designer에서 사용할 수 있는 기능

Planning Designer 또는 AI Assistant를 사용하여 다음 작업 중 하나를 수행할 수 있습니다.

* 작업 공간 만들기 및 구성

* 레코드 유형 만들기

* 디자인 필드 또는 공식 필드

* 레코드 생성, 삭제, 복제 및 복원

* 레코드의 필드 편집, 업데이트 및 첨부

* 다른 레코드에 레코드 연결

* 레코드 변경 내역 액세스

* 사용자 정의 보기 작성

* 문서를 가져와서 레코드를 만듭니다.

  가져온 문서에서 레코드를 만드는 방법은 Planning Designer에서만 사용할 수 있으며 AI Assistant에서는 사용할 수 없습니다.

  허용되는 파일 형식 및 크기에 대한 자세한 내용은 문서 [AI에서 제공하는 양식 채우기를 사용하여 프롬프트 또는 문서를 사용하여 요청을 채우는 방법](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md)의 &quot;문서 보호&quot; 섹션을 참조하십시오.

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## 조직에 대한 Designer 계획 활성화

Workfront 관리자는 먼저 조직에 대해 Planning Designer을 활성화해야 합니다.

<!--add steps here-->

1. Workfront에 시스템 관리자로 로그인합니다.
1. 화면 왼쪽 상단에서 **주 메뉴** ![주 메뉴 아이콘](assets/main-menu-shell.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.
1. 왼쪽 패널에서 **시스템** > 을 클릭한 다음 **AI 환경 설정** 영역으로 이동합니다.
1. 다음 설정을 켭니다.
   * **AI 사용**
   * **AI 베타 옵트인**
   * **Designer 계획**

   ![시스템 환경 설정에서 Planning Designer 설정](assets/planning-designer-toggle-in-system-preferences.png)
1. **저장**&#x200B;을 클릭합니다.

   이제 표준 라이선스가 있는 시스템의 모든 사용자가 계획 영역의 작업 영역 기본 페이지에서 **AI로 디자인** 단추를 볼 수 있습니다. <!--check screen shot-->

   ![작업 영역 페이지의 AI 단추로 디자인](assets/design-with-ai-button-on-workspaces-page.png)

   이제 모든 사용자는 Planning Designer을 시작하고 사용하여 Workfront Planning 객체를 생성하고 업데이트할 수 있습니다.

## Planning Designer을 사용하여 객체 생성 또는 갱신

별도로 지정하지 않는 한 Planning Designer 또는 AI Assistant를 사용하여 Workfront Planning에서 객체를 생성하거나 갱신할 수 있습니다.

1. Workfront에 로그인한 다음 왼쪽 상단의 **주 메뉴** 아이콘 ![줄 주 메뉴](assets/lines-main-menu.png)를 클릭합니다.

1. **계획**&#x200B;을 클릭합니다. 계획 영역이 열립니다.

1. **AI로 디자인**&#x200B;을 클릭합니다.

   **계획 Designer** 창이 열립니다.

   ![계획 Designer 창](assets/planning-designer-window.png)

1. 제공된 공간에서 AI Assistant에 대한 명령을 입력한 다음 완료되면 Enter 를 클릭합니다.

   <!--add screen shot-->

   예를 들어 아래 요청과 유사한 요청을 입력할 수 있습니다.

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

   프롬프트 오른쪽에 있는 미리보기 영역에서 작업 공간, 레코드 유형, 필드, 보기 및 레코드를 검토할 수 있습니다.
1. (선택 사항) 객체를 추가로 편집하려면 추가 프롬프트를 입력합니다.
1. (선택 사항) **AI 작업 영역 미리 보기 화면 전환** 아이콘 ![미리 보기 화면 숨기기 또는 표시 아이콘](assets/hide-show-preview-screen-in-planning-designer.png)을 클릭하여 오른쪽의 미리 보기 화면을 열거나 닫습니다.
1. **새 탭에서 작업 영역 열기** ![새 탭에서 작업 영역 열기](assets/open-workspace-on-new-tab-icon.png)를 클릭하여 업데이트하려는 작업 영역을 새 탭에서 엽니다.
1. **닫기** 아이콘 **X**&#x200B;을(를) 클릭하여 Planning Designer을 닫고 작업 영역 영역을 엽니다.
1. Planning Designer을 사용하여 편집한 작업공간을 열고 해당 객체를 추가로 변경합니다.




