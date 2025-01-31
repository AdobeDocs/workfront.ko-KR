---
title: Adobe Workfront Planning 레코드 자동화를 사용하여 Workfront 객체 생성
description: 활성화된 경우 Adobe Workfront Planning에서 개체 또는 Workfront Planning의 레코드를 만들도록 Workfront Planning에서 자동화를 구성할 수 있습니다. 생성된 객체와 레코드는 자동으로 기존 Planning 레코드에 연결됩니다.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 3%

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

활성화된 경우 Adobe Workfront Planning에서 개체를 만들거나 Workfront Planning을 기록하는 Workfront Planning에서 자동화를 구성할 수 있습니다. 생성된 개체 또는 레코드는 자동화를 트리거하는 레코드에 자동으로 연결됩니다.

Workfront Planning의 레코드 페이지에서 자동화를 구성하고 활성화할 수 있습니다. 생성된 연결된 개체는 자동화를 실행하는 레코드 유형의 연결된 필드에 배치됩니다.

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
<p>Workfront Planning의 모든 기능에 액세스할 수 있으려면 조직의 Workfront 인스턴스가 통합 경험 Adobe에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>를 참조하십시오. </p> 
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

* 새 개체 또는 레코드 이름은 해당 개체를 만든 레코드 이름과 같습니다. <!--take this out when they add the field mapping - no longer just the name of the original record-->
* 새 오브젝트는 동일한 필드의 기존 오브젝트를 재정의하지 않습니다.
* 자동화는 다대다 또는 일대다 연결 유형 필드에서만 추가 개체를 만듭니다.

## Workfront Planning에서 자동화 구성

개체를 만드는 데 사용하려면 먼저 Workfront Planning에서 레코드 유형에 대한 자동화를 구성해야 합니다.

{{step1-to-planning}}

1. 레코드 유형 카드를 클릭한 다음 레코드 이름을 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. 레코드 형식 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **자동화 관리**&#x200B;를 클릭합니다.

   사용 가능한 자동화 목록이 열립니다.

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
1. (조건부) 만들려는 개체 유형에 따라 다음 필드를 업데이트합니다.

   * **프로젝트**:
      * **개체가 만들어지는 연결된 필드**: 새 프로젝트가 표시될 연결된 필드입니다. 필수 필드입니다
      * **프로젝트를 만들 템플릿**: Workfront에서 프로젝트를 만드는 데 사용할 프로젝트 템플릿을 선택하십시오.
   * **Portfolio**:
      * **개체가 만들어지는 연결된 필드**: 새 포트폴리오가 표시될 연결된 필드입니다. 필수 필드입니다.
      * **새 포트폴리오에 첨부할 사용자 정의 양식**: 새 포트폴리오에 첨부할 사용자 정의 양식을 선택하십시오. 포트폴리오 사용자 정의 양식을 선택하려면 먼저 만들어야 합니다.
   * **프로그램**:
      * **개체가 만들어지는 연결된 필드**: 새 프로그램이 표시될 연결된 필드입니다. 필수 필드입니다.
      * **프로그램 포트폴리오**: 새 프로그램을 추가할 포트폴리오를 선택하십시오. 필수 필드입니다.
      * 
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
1. (선택 사항 및 조건부) Workfront 개체 유형에 대한 연결 필드가 없는 경우 **연결 필드 만들기** 아이콘 ![](assets/create-a-connection-field-icon.png)을 클릭하여 필드를 추가합니다.
1. 자동화 세부 정보 페이지의 오른쪽 상단에서 **저장**&#x200B;을 클릭합니다.

   자동화는 자동화 목록에 표시되며 레코드에서 사용할 수 있습니다.
1. (선택 사항) 자동화를 편집, 비활성화 또는 삭제하려면 다음을 수행합니다.

   1. 자동화 목록에서 저장된 자동화의 이름을 마우스로 가리킨 다음 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭합니다.

   1. 자동화에 대한 정보를 업데이트하고 필드를 구성하려면 **편집**&#x200B;을(를) 클릭하십시오.
   1. 테이블 보기에서 자동화를 제거하고 사용자가 이를 사용하여 레코드나 개체를 만들지 못하도록 하려면 **사용 안 함**&#x200B;을 클릭합니다. 다시 사용하려면 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 다시 클릭한 다음 **활성화**&#x200B;를 클릭하십시오.
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
