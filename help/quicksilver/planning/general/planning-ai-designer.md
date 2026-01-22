---
title: Adobe Workfront Planning Designer 시작
description: Adobe Planning Designer을 사용하여 Workfront Planning의 레코드 유형 및 필드로 완료된 새 작업 공간을 생성하거나 작업 공간에 객체를 추가하거나 레코드의 변경 내역을 볼 수 있습니다.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---


# Adobe Workfront Planning Designer 시작

{{planning-important-intro}}

Adobe Planning Designer을 사용하여 Workfront Planning의 레코드 유형 및 필드로 완료된 새 작업 공간을 생성하거나 작업 공간에 객체를 추가하거나 레코드의 변경 내역을 볼 수 있습니다.

>[!IMPORTANT]
>
>Planning Designer은 현재 비공개 베타 단계에 참여하는 사용자만 사용할 수 있습니다.

## 액세스 요구 사항 <!--edit theses-->

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

<!--these are from the AI Assistant - edit these-->

* Planning Designer을 사용하려면 먼저 조직에 대해 AI Assistant를 활성화해야 합니다. 조직의 모든 사용자가 AI Assistant를 사용할 수 있도록 하려면 다음을 활성화해야 합니다.

   * 귀사의 사용자가 AI Assistant를 사용할 수 있으려면 먼저 귀사에서 AI Assistant를 활성화해야 합니다. 자세한 내용은 [AI Assistant 개요](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)를 참조하십시오.
   * Workfront이 조직에 대해 AI Assistant를 활성화하면 기본 Workfront 관리자가 사용할 수 있습니다. 자세한 내용은 [시스템에 대한 기본 정보 구성](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)을 참조하십시오.

   * Workfront 관리자는 다른 모든 사용자에 대해 AI Assistant를 활성화해야 합니다. 자세한 내용은 [AI Assistant 사용 또는 사용 안 함](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)을 참조하십시오.

   * AI 도우미는 각 페이지의 컨텍스트에서 작동합니다. AI Assistant에 대해 제출 중인 요청은 열려 있는 페이지에서 사용할 수 있는 기능을 참조해야 합니다.

* Planning Designer을 사용하려면 시스템 관리자가 설정의 시스템 환경설정 영역에서 활성화해야 합니다.

* 계획 영역에서 AI 어시스턴트가 수행하는 작업은 Workfront 계획 권한 및 Workfront 액세스 수준의 컨텍스트에 있습니다. 자세한 내용은 다음 문서를 참조하십시오.

   * [Adobe Workfront Planning의 공유 권한 개요](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Adobe Workfront Planning 사용 시 라이선스 유형 개요](/help/quicksilver/planning/access/license-type-overview.md)

* 사용자를 대신하여 AI 어시스턴트가 변경한 내용은 레코드 기록 패널에서 추적됩니다.

* 명령을 사용하여 작업을 취소할 수 있습니다. 예를 들어 &quot;마지막 변경 내용 실행 취소&quot;를 입력하여 변경 내용을 되돌릴 수 있습니다.

* AI 어시스턴트를 통해 오브젝트를 생성, 업데이트, 삭제할 경우 AI 어시스턴트가 의도한 동작을 표시하고 확인을 요청한다. 그런 다음 작업을 확인하거나 취소할 수 있습니다.

—>

## 현재 Planning Designer에서 사용할 수 있는 기능

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

Planning Designer 또는 AI Assistant를 사용하여 다음 작업 중 하나를 수행할 수 있습니다.

* 작업 공간 만들기 및 구성

* 레코드 유형 만들기

* 디자인 필드 또는 공식 필드

* 레코드 생성, 삭제, 복제 및 복원

* 레코드의 필드 편집, 업데이트 및 첨부

* 다른 레코드에 레코드 연결

* 레코드 변경 내역 액세스

* 사용자 정의 보기 작성

* 문서를 가져와서 레코드를 만듭니다. 가져온 문서에서 레코드를 만드는 방법은 Planning Designer에서만 사용할 수 있으며 AI Assistant에서는 사용할 수 없습니다. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Workfront Planning에서 Planning Designer 찾기

Workfront Planning의 메인 페이지에서 Planning Designer에 액세스할 수 있습니다.

<!--add screen shot-->

AI Assistant를 사용하여 Planning Designer이 제공하는 것과 동일한 기능을 사용할 수도 있습니다.

## 조직에 대한 Designer 계획 활성화

Workfront 관리자는 먼저 조직에 대해 Planning Designer을 활성화해야 합니다.

<!--add steps here-->

## Planning Designer을 사용하여 객체 생성 또는 갱신

별도로 지정하지 않는 한 Planning Designer 또는 AI Assistant를 사용하여 Workfront Planning에서 객체를 생성하거나 갱신할 수 있습니다.

1. Workfront에 로그인한 다음 화면 오른쪽 상단의 **주 메뉴** 아이콘 ![점 주 메뉴](assets/dots-main-menu.png) 또는 사용 가능한 경우 왼쪽 상단의 **주 메뉴** 아이콘 ![선 주 메뉴](assets/lines-main-menu.png)을 클릭합니다.

1. **계획**&#x200B;을 클릭합니다. 계획 영역이 열립니다.

1. **AI로 디자인**&#x200B;을 클릭합니다.

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

   시각적 미리 보기에는 도우미가 빌드할 수 있는 샘플 이 표시됩니다.

1. 성공적인 응답을 받은 후 명령줄에 제공된 링크에 따라 요청 개체를 만들거나 업데이트하거나 검토하십시오.




