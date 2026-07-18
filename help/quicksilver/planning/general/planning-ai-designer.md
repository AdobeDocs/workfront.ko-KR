---
title: Adobe Workfront Planning Designer 시작
description: AI에서 제공하는 Adobe Planning Designer을 사용하여 작업 공간 및 데이터 구조를 쉽게 구성할 수 있습니다. Planning Designer은 작업 공간 생성 및 구성에서 필드 및 공식 정의, 레코드 관리, 변경 내용 검토 및 사용자 정의 보기 작성에 이르기까지 모든 작업을 지원합니다. Planning Designer은 직접 사용하든 AI Assistant를 통해 사용하든 상관없이 구조화되고 연결된 정보를 구축하고 유지할 수 있는 유연하고 강력한 환경을 제공합니다.
recommendations: noDisplay, noCatalog
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
exl-id: ba7a4b04-5faa-41b6-86d0-4d0ce946ad1e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YZRzcl8ymUo85jplCgKOx-qI83Gqa4CUI6saxfijtec
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 184cff4f2ebf8a1343d784936f10c902e350c134
workflow-type: tm+mt
source-wordcount: 1386
ht-degree: 1%

---

# Adobe Workfront Planning Designer 시작

<!--remove the Beta tags in the screen shots on this page when this is released to GA - maybe March 2, 2026-->

>[!IMPORTANT]
>
>Planning Designer은 현재 Beta 상태의 모든 고객이 사용할 수 있습니다.
>
>이 문서의 정보는 Adobe Workfront의 추가 기능인 Adobe Workfront Planning을 참조합니다.
>
>Workfront Planning에 액세스하기 위한 요구 사항 목록은 [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.
> 
>Workfront Planning에 대한 일반적인 정보는 [Adobe Workfront Planning 시작](/help/quicksilver/planning/general/planning-overview.md)을 참조하십시오.

AI에서 제공하는 Adobe Planning Designer을 사용하여 작업 공간 및 데이터 구조를 쉽게 구성할 수 있습니다. Planning Designer은 작업 공간 생성 및 구성에서 필드 및 공식 정의, 레코드 관리, 변경 내용 검토 및 사용자 정의 보기 작성에 이르기까지 모든 작업을 지원합니다.

Planning Designer은 직접 사용하든 AI Assistant를 통해 사용하든 상관없이 구조화되고 연결된 정보를 구축하고 유지할 수 있는 유연하고 강력한 환경을 제공합니다.

Workfront Planning에 대한 자세한 내용은 다음 문서를 참조하십시오.

* [Adobe Workfront Planning에 대한 일반 정보 및 문서 색인](/help/quicksilver/planning/planning-information.md)
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
   <p>시스템 관리자가 조직에 대해 Planning Designer을 활성화해야 합니다.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  
   </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 조직에 대해 Planning Designer 활성화

시스템 관리자는 조직에 대해 Planning Beta을 켤 수 있습니다. 이 설정이 켜지면 Workfront 인스턴스의 모든 사용자가 계획 영역에서 계획 Designer의 기능을 볼 수 있습니다.

1. Workfront에서 Workfront 관리자로 로그인합니다.
1. **주 메뉴** ![주 메뉴 아이콘](assets/main-menu-shell.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.
1. **시스템** > **환경 설정** > **AI 환경 설정**(으)로 이동합니다.
1. **AI 활성화**<!--and ensure you have a signed Gen AI Agreement with Adobe-->를 켭니다.
   <!--1. Turn on the **Opt in to AI Beta** setting.-->
1. **계획 Designer** 설정을 켭니다.
   <!-- add new screenshot-->
   ![시스템 환경 설정에서 Planning Designer 설정](assets/planning-designer-toggle-in-system-preferences.png)

1. **저장**&#x200B;을 클릭합니다.

   이제 Planning에 액세스할 수 있는 조직의 모든 사용자가 작업 공간을 만들거나 편집할 수 있는 Planning Designer 기능을 사용할 수 있습니다.

<!--

## Turn off the Planing Designer for your organization

After your Workfront administrator accepts the AI Assistant agreement, the Planning Designer is turned on for everyone in your organization, by default. 

To turn it off: 

1. Log in to Workfront as a System Administrator. 
1. Click **Main Menu** ![Main menu icon](assets/main-menu-shell.png) in the upper-left corner of the screen, then click **Setup**.
1. Click **System** >  in the left panel, then go to the **AI preferences** area.
1. Turn off the **Planning Onboarding** setting.
1. Click **Save**.

    This removes the Planning Designer for all users in the system.

-->

<!--

## Enroll in the Closed Beta program for the Planning Designer

Currently, you can request to participate in the Closed Beta program for the Planning Designer by sending us an email to sargism@adobe.com.

After we receive the email, our Engineering team will turn on the Planning Designer in your Workfront instance. 

>[!IMPORTANT]
>
>Your company must first accept the AI Assistant agreement before the Planning Designer is available in your system. 

-->

## Planning Designer에 대한 피드백 제출

Beta 프로그램 중에 Planning Designer에 대한 피드백을 제출할 수 있습니다.

1. Workfront에 로그인한 다음 왼쪽 상단의 **주 메뉴** 아이콘 ![줄 주 메뉴](assets/lines-main-menu.png)를 클릭한 다음 **계획**&#x200B;을 클릭합니다.

   **계획** 영역이 열립니다.

1. **AI로 만들기**&#x200B;를 클릭합니다. <!--update this tag name when they change it-->

   **계획 Designer** 창이 열립니다.

1. 페이지 하단의 **여기에 피드백 제출**&#x200B;을 클릭합니다.
1. 제공된 스페이스에 피드백을 추가한 다음 **제출**&#x200B;을 클릭합니다.
귀하의 피드백은 엔지니어링 및 제품 팀에 제출됩니다.

## Planning Designer에 대한 고려 사항

* Planning Designer에 액세스하려면 AI 계약을 활성화할 필요가 없습니다.

<!--* You must sign the Beta agreement to access the Planning Designer.-->

<!--
Sargis and Ashot  said these are not required: 

* To use the Planning Designer, you first need to enable AI for your organization. The following must be in place for the AI features to be available to everyone in your organization:

    * Workfront must make the AI features available for your organization.

        For details, see [Prerequisites to AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
    * After Workfront makes the AI features available for your organization, the main Workfront administrator can access it. 

        For information, see [Configure basic information for your system](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md). 
    * The Workfront administrator must accept the Gen AI agreement, and then turn on AI and the Planning Designer for your organization. 

        For more information, see [Enable or disable AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md). 

-->

* Workfront 관리자는 조직에 대해 Planning Designer을 켜야 합니다. 이 이후에는 기본적으로 Planning Designer을 모든 사용자가 사용할 수 있습니다.
* 조직에서 AI 계약에 서명한 경우 Planning Designer에서 수행하는 작업도 Planning 영역에서 사용할 때 AI Assistant에서 수행할 수 있습니다.
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

<!--On March 2: * Edit workspaces-->

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
  >.XLSX 파일 형식은 지원되지만 Planning Designer을 통해 대규모 레코드 가져오기에는 사용할 수 없습니다.
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

1. **AI로 만들기**&#x200B;를 클릭하거나 **작업 영역 만들기**&#x200B;를 클릭한 다음 맨 위에 있는 프롬프트 창을 사용하여 만들 작업 영역을 나타냅니다. <!--update this when they change it to Generate with AI-->

   **계획 Designer** 창이 열립니다. <!--remove the Beta tag here when this removes from Beta-->

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
1. (선택 사항) 작업 영역을 편집하려면 다음 중 하나를 수행합니다.

   * 작업 영역을 열고 수동으로 변경합니다. 자세한 내용은 [작업 영역 편집](/help/quicksilver/planning/architecture/edit-workspaces.md)을 참조하십시오.
   * **AI로 편집**&#x200B;을 클릭합니다. 그러면 Planning Designer이 열립니다. 위의 단계를 반복하여 AI를 사용하고 작업 영역을 추가로 변경합니다.


