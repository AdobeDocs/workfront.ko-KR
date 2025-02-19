---
title: Adobe Workfront Planning 레코드 자동화를 사용하여 Workfront 객체 생성
description: 활성화된 경우 Adobe Workfront Planning에서 개체 또는 Workfront Planning의 레코드를 만들도록 Workfront Planning에서 자동화를 구성할 수 있습니다. 생성된 객체와 레코드는 자동으로 기존 Planning 레코드에 연결됩니다. 이 문서에서는 개체와 레코드를 만들도록 편집, 비활성화, 삭제 및 트리거하는 방법을 포함하여 자동화를 관리하는 방법에 대해 설명합니다.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 966c2a2b0159c89a41d4502fb0eb0e318f3e5ba9
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 2%

---

# Adobe Workfront Planning 레코드 자동화를 사용하여 객체 생성

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

활성화된 경우 Planning 레코드에서 트리거될 때 Adobe Workfront Planning의 객체 또는 Workfront Planning의 레코드를 생성하도록 Workfront Planning에서 자동화를 구성할 수 있습니다. 생성된 개체 또는 레코드는 자동화를 트리거하는 레코드에 자동으로 연결됩니다.

Workfront Planning의 레코드 유형 페이지에서 자동화를 구성하고 활성화할 수 있습니다. 생성된 연결된 개체는 자동화를 실행하는 레코드 유형의 연결된 필드에 배치됩니다.

예를 들어, Workfront Planning 캠페인을 가져와 Workfront에서 프로젝트를 생성하여 해당 캠페인의 진행 상황을 추적하는 자동화를 만들 수 있습니다. 프로젝트는 캠페인의 연결된 프로젝트 필드에서 Workfront 계획 캠페인에 연결됩니다.

연결된 레코드에 대한 자세한 내용은 [연결된 레코드 개요](/help/quicksilver/planning/records/connected-records-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 Workfront Planning에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
<p>임의 </p> 
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront 플랫폼</p></td> 
   <td> 
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td> 표준
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p> 
   <p>만들려는 객체 유형(프로젝트, 포트폴리오, 프로그램)에 대한 Workfront의 액세스 권한을 편집합니다. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td> <p>레코드를 추가할 작업 영역에 대한 권한을 관리합니다. </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
   <p>하위 개체(프로젝트)를 추가하기 위해 Workfront 개체(포트폴리오)에 대한 권한을 관리합니다.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## 자동화를 사용하여 오브젝트 및 레코드 만들기에 대한 고려 사항

* 새 개체 또는 레코드 이름은 해당 개체를 만든 레코드 이름과 같습니다.
* 새 개체 또는 레코드는 동일한 필드의 기존 개체보다 우선하지 않습니다. 동일한 레코드에 대해 동일한 자동화를 여러 번 트리거하면 이전에 만든 레코드 외에 원본 레코드의 연결된 동일한 필드에 새 개체나 레코드가 추가됩니다.
* 자동화는 다대다 또는 일대다 연결 유형 필드에만 추가 개체를 추가합니다. 다른 모든 경우에는 자동화가 개체를 만들지만 자동화가 트리거되는 원본 레코드에 연결하지는 않습니다.

## Workfront Planning에서 자동화 구성

개체를 만드는 데 사용하려면 먼저 Workfront Planning에서 레코드 유형에 대한 자동화를 구성해야 합니다.

{{step1-to-planning}}

1. 레코드 유형 카드를 클릭한 다음 레코드 이름을 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. 레코드 종류 이름의 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **자동화 관리**&#x200B;를 클릭합니다.

   선택한 레코드 유형에 사용할 수 있는 자동화 목록이 열립니다.

1. 화면 오른쪽 상단의 **새 자동화**&#x200B;를 클릭합니다. **새 자동화** 상자가 열립니다.
1. 다음 필드를 업데이트합니다.

   * **제목 없는 자동화**&#x200B;를 자동화 단추에 표시할 텍스트로 바꿉니다. 자동화를 사용하여 Workfront 개체 또는 Planning 레코드를 만들 때 이 단추를 클릭합니다.
   * **설명**: 자동화의 목적을 식별하려면 설명을 추가하십시오.
1. **저장**을 클릭합니다.
자동화 세부 정보 페이지가 열립니다.

1. 자동화의 세부 정보 페이지에서 **트리거** 섹션의 다음 필드를 업데이트하십시오.

   * **트리거**: 자동화를 트리거할 작업을 선택하십시오. 예를 들어 **단추 클릭**&#x200B;을 선택합니다. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. **작업** 섹션에서 다음 필드를 업데이트합니다. <!--submitted bugs for these fields - see if they need changing here-->
   * **개체 유형**: 자동화를 만들 개체를 선택하십시오. 필수 필드입니다.

     Workfront Planning 레코드에서 다음 객체를 생성할 수 있습니다.

      * 프로젝트
      * 포트폴리오
      * 프로그램
      * 그룹
      * 레코드

     >[!TIP]
     >
     >자동화를 저장한 후에는 더 이상 이 필드의 객체 유형을 변경할 수 없습니다.

1. (조건부) 만들려는 개체 유형에 따라 다음 필드를 업데이트합니다.


   * **프로젝트**:
      * **개체가 만들어지는 연결된 필드**: 새 프로젝트가 표시될 연결된 필드입니다. 필수 필드입니다.
      * **프로젝트를 만들 템플릿**: Workfront에서 프로젝트를 만드는 데 사용할 프로젝트 템플릿을 선택하십시오.
   * **Portfolio**:
      * **개체가 만들어지는 연결된 필드**: 새 포트폴리오가 표시될 연결된 필드입니다. 필수 필드입니다.
      * **새 포트폴리오에 첨부할 사용자 정의 양식**: 새 포트폴리오에 첨부할 사용자 정의 양식을 선택하십시오. 포트폴리오 사용자 정의 양식을 선택하려면 먼저 만들어야 합니다.
   * **프로그램**:
      * **개체가 만들어지는 연결된 필드**: 새 프로그램이 표시될 연결된 필드입니다. 필수 필드입니다.
      * **프로그램 포트폴리오**: 새 프로그램을 추가할 포트폴리오를 선택하십시오. 필수 필드입니다.
      * **새 프로그램에 첨부할 사용자 정의 양식**: 새 프로그램에 첨부할 사용자 정의 양식을 선택합니다. 프로그램 사용자 정의 양식을 선택하려면 먼저 만들어야 합니다.
   * **그룹**:
      * **개체가 만들어지는 연결된 필드**: 새 그룹이 표시될 연결된 필드입니다. 필수 필드입니다.
      * **새 그룹에 첨부할 사용자 정의 양식**: 새 프로그램에 첨부할 사용자 정의 양식을 선택합니다. 프로그램 사용자 정의 양식을 선택하려면 먼저 만들어야 합니다.
   * **레코드**:
      * **연결된 레코드 종류**: 만들 레코드 종류를 선택하십시오.
      * **레코드가 만들어지는 연결된 필드**: 새 레코드가 표시되는 연결된 필드입니다. 필수 필드입니다. <!--this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label-->
      * **필드 매핑**
         * **전송 원본**: 연결된 레코드 형식의 필드에 매핑하려면 자동화를 만드는 레코드 형식에서 필드를 선택하십시오.
      * **전송 대상**: 새로 만든 레코드에서 자동화를 실행 중인 레코드의 정보로 채울 필드를 선택합니다.
1. (선택 사항 및 조건부) 레코드를 만들도록 선택한 경우 **필드 추가**&#x200B;를 클릭하여 한 레코드에서 다른 레코드로 추가 조회 필드를 매핑합니다.
1. (선택 사항 및 조건부) Workfront 개체 유형에 대한 연결 필드가 없는 경우 **연결 필드 만들기** 아이콘 ![연결 필드 만들기 아이콘](assets/create-a-connection-field-icon.png)을 클릭하여 필드를 추가합니다.

   새 필드가 자동으로 만들어지고 이름이 **연결됨 &lt; Workfront 개체 이름 >**&#x200B;으로 지정됩니다. 예를 들어 레코드에 대해 포트폴리오 연결 필드를 만들 경우 해당 필드를 &quot;연결된 포트폴리오&quot;라고 합니다.

1. 자동화 세부 정보 페이지의 오른쪽 상단에서 **저장**&#x200B;을 클릭합니다.

   자동화는 자동화 목록에 표시되며 레코드에서 사용할 수 있습니다.
1. (선택 사항) 자동화를 편집, 비활성화 또는 삭제하려면 다음을 수행합니다.

   1. 자동화 목록에서 저장된 자동화의 이름을 마우스로 가리킨 다음 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭합니다.

   1. 자동화에 대한 정보를 업데이트하고 필드를 구성하려면 **편집**&#x200B;을(를) 클릭하십시오.
   1. 테이블 보기에서 자동화를 제거하고 사용자가 이를 사용하여 레코드나 개체를 만들지 못하도록 하려면 **사용 안 함**&#x200B;을 클릭합니다. 다시 사용하려면 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 다시 클릭한 다음 **활성화**&#x200B;를 클릭하십시오.
   1. 자동화를 삭제하려면 **삭제**&#x200B;를 클릭하십시오. 삭제된 자동화는 복구할 수 없습니다. 자동화를 사용하여 생성된 레코드는 원래 선택한 레코드에 연결된 상태로 유지됩니다.

## Workfront Planning 자동화를 사용하여 객체 또는 레코드 생성

1. Workfront Planning에서 Workfront 객체 또는 Planning 레코드를 생성하는 데 사용할 레코드가 포함된 레코드 유형 페이지를 엽니다.
1. 테이블 뷰를 엽니다.
1. 하나 이상의 레코드를 선택합니다.

   테이블 하단에 자동화 버튼을 비롯한 추가 버튼과 함께 파란색 막대가 표시됩니다.
1. 화면 오른쪽 아래 모서리에 있는 자동화 버튼을 클릭합니다.

   ![자동화 단추](assets/automation-custom-button.png)

   자동화가 개체 또는 레코드를 성공적으로 만든 경우 화면 하단에 확인 메시지가 표시됩니다.

   새 객체는 자동화 버튼 설정에 지정한 연결된 필드에 표시됩니다. 새 개체를 보기 전에 페이지를 새로 고쳐야 할 수도 있습니다.

   >[!NOTE]
   >
   >개체가 예상대로 만들어지고 연결되었는지 확인하는 것이 좋습니다.

1. (선택 사항) 연결된 필드에서 새 개체를 클릭합니다. 객체 페이지가 열리고 새 객체를 추가로 변경할 수 있습니다.

<!--you might need to add something about notifications and emails?!-->


<!--****************************************FUTURE ARTICLE AFTER THE RELEASE TO PREVIEW ON FEBRUARY 20:*****************************************************  

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same record adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 

(************hide this for now: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. ***************)

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. *************update this step with a list of all possible triggers; right now only Button click is available*********

1. Update the following fields in the **Actions** section: **********submitted bugs for these fields - see if they need changing here***********
   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Select one of the following actions: 

      * Create group
      * Create program
      * Create portfolio
      * Create project
      * Create record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the action selected in this field.

1. (Conditional) Depending on what action you selected, update the following fields:

   * **Create project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Project template**: Select a project template that Workfront will use to create the project.  
   * **Create portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Create program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create record**: 
      * **Record type**: Select the record type you want to create. 

      The **Settings** sub-section displays. Update the following fields in the **Settings** sub-section: 

      * **Field on the connected record type where the current record will show**: This is the connected field on the record type selected for the action where the current record will display. 
      
      For example, if you are creating an automation for campaigns to connect Product records from, this is the connected field on the Product record type where the campaigns will display, after the products are created using the automation. 
      
      This is a required field. 
      
      ******submitted a change in functionality and UI text for this - revise?? *******
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 

      >[!TIP]
      >
      >The field types from the original record type must match the field types from the newly created record type.

1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Conditional) If you selected to create a record and there are no connection fields between the original record type and the record type selected in the **Actions** area, click the question mark icon to the right of the **Field on the connected record type where the current record will show** field, then click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   The new field is automatically created for the record type you selected in the **Actions** area, and named **Connected Record**. 
   
   A connected field for the selected record type is also created on the original record type from where you are configuring the automation. 
1. (Optional and conditional) If you selected to create a Workfront object and don't have a connection field for the selected Workfront object type, click the question mark icon to the right of the **Connected field where the < Workfront object type name > is created** field, and click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.

## Manage existing automations

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. (Optional) To edit, disable, or delete an automation, do one of the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.

      >[!TIP]
      >
      >   You cannot change the action you originally selected for an automation. 
   

   1. Click **Disable** to remove the automation from the record's table view and prevent users from using it to create records or objects. 

   Records that have been created using a disabled automation remain connected to the record originally selected.
   
   To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. 
   
   Records that have been created using a deleted automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the automation you want to use to automatically create and connect records or objects. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   The following things occur: 

   * A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   * The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   * The record you are triggering the automation from is added to the connected field of the new record.

   >[!NOTE]
   >
   >We recommend checking that the objects or records were created and the connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

***********you might need to add something about notifications and emails?!*************

-->