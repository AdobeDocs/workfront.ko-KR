---
title: Adobe Workfront Planning에서 요청 양식 생성 및 관리
description: Adobe Workfront Planning 영역에서 레코드 유형을 선택한 후 요청 양식을 만들어 해당 레코드 유형과 연결할 수 있습니다. 그런 다음 다른 내부 또는 외부 사용자와 링크를 공유할 수 있습니다. 양식에 대한 링크가 있는 사용자는 해당 양식의 필드 값을 채울 수 있으며, 양식 제출을 통해 관련 레코드 유형에 대한 새 레코드를 추가할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 99e26d4249162e46da1a73301e68bdf30436a81d
workflow-type: tm+mt
source-wordcount: '2678'
ht-degree: 1%

---

# Adobe Workfront Planning에서 요청 양식 만들기 및 관리

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

요청 양식을 만들어 Adobe Workfront Planning에서 레코드 유형과 연결할 수 있습니다. 그런 다음 다른 사용자와 양식을 공유하고 해당 유형의 레코드를 만들도록 요청을 제출할 수 있습니다.

이 문서에서는 작업 영역 관리자가 레코드 유형과 연결된 요청 양식을 만드는 방법에 대해 설명합니다.

레코드를 만들기 위해 레코드 형식에 요청을 제출하는 방법에 대한 자세한 내용은 [레코드를 만들기 위한 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

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
<p>모든 Workfront 패키지 및 모든 Planning 패키지</p>
또는
<p>모든 워크플로우 패키지 및 모든 Planning 패키지</p>
<p>각 Workfront Planning 패키지에 포함된 내용에 대한 자세한 내용은 Workfront 계정 담당자에게 문의하십시오.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>표준</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 영역 또는 레코드 형식에 대한 권한 관리</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 요청 양식의 필드 및 값 표시 제한

요청을 제출한 후 특정 필드가 요청 양식에 표시되는 방식과 해당 값이 나중에 레코드 또는 요청 세부 정보 페이지에 표시되는 방식에는 제한이 있습니다.

Workfront Planning 요청 제출에 대한 자세한 내용은 [레코드를 만들도록 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

* 다음은 특정 필드가 요청 양식, 요청 양식에서 만든 레코드 또는 요청 세부 정보 페이지에 표시되는 방식에 대한 제한 사항입니다.

   * 다음 유형의 필드를 요청 양식에 추가할 수 없습니다.

      * 작성자, 마지막 수정자, 승인자
      * 생성 날짜, 마지막 수정 날짜, 승인 날짜
      * Workfront 개체의 조회 필드
      * Workfront Planning 연결된 레코드의 조회 필드

* 다음은 요청 양식 빌더에 필드 형식이 표시되는 방식과 레코드 또는 요청 세부 정보 페이지에서 필드 값의 형식이 지정되는 방식의 차이점입니다.

   * 통화, 숫자 및 백분율 필드는 양식 빌더에 한 줄 텍스트 필드 유형으로 표시됩니다.

     그러나 필드 형식은 유지되고 요청이 제출된 후 레코드 유형 및 요청 세부 정보 페이지에서 통화, 숫자 및 백분율로 필드 값이 표시됩니다.

* 다음은 요청 양식 및 요청 세부 정보 페이지에 일부 필드 값이 표시되는 방식을 설명합니다.

   * 통화, 숫자 및 백분율 필드에 대한 특수 서식은 유지되지 않습니다. 예를 들어, 이러한 영역의 이러한 필드 값에 대한 소수점 이하 자리수는 유지되지 않습니다.
   * 사람 필드 값은 ID로 표시됩니다.
   * 다른 필드 또는 계산을 참조하지 않는 수식 필드에는 값이 표시되지 않습니다. 예를 들어 `STRING` 수식이 있는 필드는 &quot;N/A&quot; 값을 표시합니다.
   * 통화 필드를 참조하는 공식 필드에는 환율을 계산하지 않고 값이 표시됩니다.
   * 단락 필드의 값은 요청 양식에 &quot;N/A&quot; 값을 표시하며, 요청 세부 정보 페이지의 서식 있는 텍스트 대신 html 태그를 표시합니다.

## 요청 양식 만들기

요청 양식을 만들려면 양식 만들기를 시작하고 양식 세부 정보를 설정한 다음 양식을 게시하고 공유하여 완료해야 합니다.

### 요청 양식 만들기 시작

<!--span class="preview">, or from the Requests area of Workfront.</span>--> 양식과 연결된 레코드 형식에서 요청 양식을 만들 수 있습니다.

#### 레코드 유형에서 요청 양식 만들기

{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.

1. 이미 양식이 있고 추가 양식을 만들려면 페이지 헤더의 레코드 종류 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **요청 양식 만들기** 또는 **요청 양식 관리**&#x200B;를 클릭합니다.
1. (조건부) 다른 양식을 추가하려면 **새 요청 양식**&#x200B;을 클릭하세요.

   요청 양식 만들기 상자가 열립니다.

1. 요청 양식 만들기 상자에서 요청 양식의 이름을 업데이트합니다. 기본적으로 양식 이름은 **제목 없는 양식**&#x200B;입니다. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (선택 사항) 요청 양식에 대해 **설명**&#x200B;을(를) 추가합니다.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Click **Create**.

   선택한 레코드 유형에 대한 요청 양식이 양식 탭에서 열립니다.
1. [양식을 구성](#configure-the-form)합니다.

<!--

<div class="preview">

#### Create a request form from the Requests area of Workfront

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Requests**.
1. In the upper-right corner of the screen, click **Request forms**.
1. (Conditional) If you are editing an existing request form, select it from the list, then continue to [Configure the form](#confgure-the-form).
1. If you are creating a new request form, in the upper-right corner of the screen, click **New request form**.

   The Create request form box opens

1. In the Create request form box, update the name of the request form. By default, the name of the form is **Untitled form**. 
1. In the Object types field, select the record type that the request form will be associated with. Record types are grouped into the workspace that they exist within.
1. (Optional) Add a **Description** for the request form. 

1. Click **Create**. 

   The request form for the selected record type opens in the Form tab.
1. Continue to [Set up details for the request form](#set-up-details-for-the-request-form).



</div>

-->

### 요청 양식에 대한 세부 정보 설정

양식 세부 사항은 탭으로 나뉩니다.

* **양식** 탭에서 필드 및 콘텐츠 요소를 양식에 추가할 수 있습니다.
* **구성** 탭에서 양식의 승인 프로세스를 설정하고 요청 완료 옵션을 설정할 수 있습니다.&lt;
  <!--* <span class="preview">The **Automations** tab allows you to automate what will occur based on features of the request made with the form.</span>-->

#### 양식 세부 정보 설정

1. [요청 양식 만들기 시작](#begin-creating-a-request-form) 섹션에 설명된 대로 요청 양식을 만들거나 편집하십시오.

   또는

   요청 양식 목록에서 요청 양식을 찾아 양식 이름 옆에 있는 상자를 클릭한 다음 화면 하단의 파란색 막대에서 **양식 편집**&#x200B;을 클릭합니다.

   선택한 레코드 유형에 대한 요청 양식이 양식 탭에서 열립니다.

   ![캠페인 요청 양식 편집 모드](assets/campaigns-request-form-edit-mode.png)

   요청 양식에는 기본적으로 다음 정보가 포함되어 있습니다.

   * 선택한 레코드 유형의 표 보기에서 사용할 수 있는 레코드 필드입니다. <!--they are working on removing the limitation below-->

   * **기본 섹션**: Workfront이 요청 양식에 적용하는 기본 섹션 구분입니다. 모든 레코드 필드가 **기본 섹션** 영역에 표시됩니다.
   * **제목** 필드: Workfront에서 요청을 식별하는 필드입니다. 제목 필드의 구성 및 값을 편집할 수 없습니다.

     >[!NOTE]
     >
     >* **제목** 필드는 요청 양식에 표시되면 값이 필요합니다. 그러나 필요한 경우 **제목** 필드를 제거할 수 있으며 요청자가 요청을 제출할 때 양식에 표시되지 않습니다.
     >* 요청 양식에서 제목 필드가 누락되었지만 이후 레코드의 이름에 대한 이름 필드가 있는 경우 요청 이름은 생성된 레코드와 동일한 이름으로 자동 할당됩니다.
     >* 요청 양식에 제목 필드와 이름 필드가 모두 없으면 `< Record name > request form < Entry date of the request >` 패턴을 사용하여 요청의 이름이 지정됩니다. 레코드의 이름은 **제목 없음**&#x200B;입니다.

   * 레코드 유형과 연결된 모든 필드.

     요청 양식에 포함된 필드는 이 레코드 유형에 요청을 제출하는 모든 사람에게 표시됩니다.

1. (선택 사항) 제거할 양식의 필드 위에 마우스를 놓은 다음 **x** 아이콘을 클릭하여 제거합니다. 양식 왼쪽의 **필드** 탭에 추가됩니다.

1. (선택 사항) 양식에서 **기본 섹션**&#x200B;을(를) 제거하려면 다음을 수행하십시오.

   1. 기본 섹션에서 모든 필드를 제거합니다.
   1. **콘텐츠 요소**&#x200B;를 클릭하고 새 섹션을 추가한 다음 섹션 이름을 추가합니다.
   1. 필드를 새 섹션에 추가합니다.
   1. **x** 아이콘을 클릭하여 **기본 섹션**&#x200B;을(를) 제거합니다.
1. 필드를 클릭한 다음 양식의 오른쪽 패널에 있는 컨트롤을 사용하여 해당 크기나 다음 정보 중 하나를 정의합니다.

   * **레이블**: 요청 양식에 표시되는 필드 이름입니다. 레코드 필드의 이름은 변경되지 않습니다.
   * **지침**: 필드에 대한 정보를 더 추가합니다.
   * **필수 필드 만들기**: 선택한 경우 필드에 값이 있어야 합니다. 그렇지 않으면 양식을 제출할 수 없습니다.
   * **논리 추가**: 필드가 표시되거나 숨겨지기 위해 충족되어야 하는 조건을 정의합니다.

   >[!TIP]
   >
   >   각 필드의 필드 유형은 양식에서 필드를 선택한 후 오른쪽 패널 상단에 표시됩니다.
   >     

1. (선택 사항) 양식 왼쪽에 있는 **콘텐츠 요소** 탭을 클릭하고 다음 요소를 추가합니다.

   * **설명 텍스트**
   * **섹션 구분**

   사용자 정의 양식 작성에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. (선택 사항) **미리 보기**&#x200B;를 클릭하여 다른 사용자가 새 레코드를 제출하는 데 사용할 양식을 표시할 방법을 확인합니다.
1. 양식에 대한 자세한 내용을 구성하려면 [구성 세부 정보 설정](#set-up-configuration-details)을 계속하거나 [요청 양식 작성 완료](#complete-request-form-creation)(으)로 이동하십시오.

#### 구성 세부 정보 설정

구성 탭에서 승인 프로세스를 설정하고 이 양식에서 만든 요청이 완료됨으로 표시되는 시기를 구성할 수 있습니다.

1. [요청 양식 만들기 시작](#begin-creating-a-request-form) 섹션에 설명된 대로 요청 양식을 만들거나 편집하십시오.

   선택한 레코드 유형에 대한 요청 양식이 양식 탭에서 열립니다.
1. (선택 사항) [양식 세부 정보 설정](#set-up-form-details)에 설명된 대로 양식 세부 정보를 설정합니다.

1. (선택 사항) 승인자를 추가하려면 **구성** 탭을 클릭한 다음 **승인자** 필드에 사용자 또는 팀을 하나 이상 추가하여 이 레코드 양식에 대한 새 요청을 승인하십시오.

   ![구성 탭](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * 한 명 또는 여러 명의 승인자를 요청 양식에 추가할 수 있습니다.
   * 최소 한 명 이상의 승인자가 요청을 거부하면 요청이 거부되고 레코드가 만들어지지 않습니다. 요청은 Workfront의 요청 영역에 있는 제출됨 섹션의 계획 탭에 남아 있습니다.
   * 두 명 이상의 승인자를 추가할 때 [하나의 결정만 필요] 옵션이 활성화되어 있지 않은 경우 요청이 승인 또는 거부되기 전에 모든 승인자가 결정을 내려야 합니다.
   * 팀이 승인자로 설정된 경우 팀에서 하나의 결정만 필요합니다.

   요청 양식에 승인을 추가하는 방법에 대한 자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

1. (조건부) 승인자 중 한 명이 레코드를 승인한 후 레코드를 만들려면 **한 개의 결정만 필요합니다** 확인란을 선택합니다.

1. 요청된 개체를 만들 때 이 양식에서 만든 요청을 완료됨으로 표시할지 또는 요청된 개체가 완료될 때 완료됨으로 표시할지 선택합니다.
1. (조건부) 요청된 객체가 완료될 때 요청이 완료로 표시되도록 선택한 경우 객체가 완료되는 시기를 나타내는 필드 및 값을 선택합니다. 예를 들어 생성된 객체의 상태가 완료로 설정된 경우 Status 필드와 Complete 값을 선택하여 요청을 완료할 수 있습니다.
1. <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[요청 양식 만들기 완료](#complete-request-form-creation)를 계속합니다.

<!--
 
<div class="preview">

#### Set up Automations

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. 

For information on creating automations in other areas of Workfront Planning, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. Currently, the only available trigger for request form automation is `When request object status equals pending creation`.

1. Update the following fields in the **Actions** section: 

   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Currently, the only available Action for request form automation is `Create record`.

     >[!TIP]
     >
     >After you saved the automation, you can no longer change the action selected in this field.
1. Continue to  [Complete request form creation](#complete-request-form-creation).


</div>

-->

### 요청 양식 작성 완료

1. [요청 양식 만들기 시작](#begin-creating-a-request-form) 및 [요청 양식에 대한 세부 정보 설정](#set-up-details-for-the-request-form)에 설명된 대로 양식을 만들고 설정합니다.
1. (선택 사항) 헤더의 양식 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 다음 **편집**&#x200B;을 클릭하여 양식 이름을 업데이트합니다.

1. 양식을 게시하고 고유한 링크를 얻으려면 **게시**&#x200B;를 클릭하십시오.

   다음과 같은 상황이 발생합니다.

   * **게시** 단추가 제거되었습니다.
   * **게시 취소** 단추가 양식에 추가됩니다. 클릭하면 양식에 액세스할 수 없습니다.
   * **공유** 단추가 양식에 추가됩니다.
   * 양식은 Workfront 주 메뉴의 요청 영역에서 사용할 수 있습니다.

1. 양식을 다른 사용자와 공유하려면 **공유**&#x200B;를 클릭하세요.

   요청 양식 공유에 대한 자세한 내용은 이 문서의 [요청 양식 공유](#share-a-request-form) 섹션을 참조하십시오
1. 머리글에서 양식 이름 왼쪽에 있는 왼쪽 화살표를 클릭하여 양식을 닫습니다.

   **요청 양식** 테이블 보기가 열리고 양식이 추가됩니다.

## 기존 요청 양식 관리


1. 요청 양식을 관리할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.

1. 페이지 헤더의 레코드 종류 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **요청 양식 관리**&#x200B;를 클릭합니다.

   레코드 유형과 연관된 모든 요청 양식이 테이블 보기에 표시됩니다.

1. (선택 사항) 테이블 보기에서 요청 양식 이름 위로 마우스를 가져간 후 양식 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭하고 다음 중 하나를 클릭합니다.

   * **양식 편집**: 양식에 대한 정보를 추가로 편집하려면 여기를 클릭하십시오.
   * **게시 취소**: Workfront의 요청 영역에서 양식을 제거하는 게시를 취소하려면 이 옵션을 클릭합니다.
   * **공유**: 양식에 액세스할 수 있는 사용자를 수정하려면 이 항목을 클릭하십시오.
   * **링크 복사**: 양식을 열지 않고 요청 양식의 링크를 빠르게 복사하려면 이 링크를 클릭하십시오.
   * **삭제**: 양식을 삭제하려면 이 항목을 클릭하십시오. 양식을 사용하여 추가된 모든 요청 및 레코드는 삭제되지 않습니다. 양식을 복구할 수 없습니다.

   ![요청 양식 목록의 요청 양식에 대한 추가 메뉴](assets/more-menu-on-request-form-from-request-forms-list.png)

1. 헤더의 **요청 양식** 왼쪽에 있는 왼쪽 화살표를 클릭하여 요청 양식 표를 닫습니다.

   레코드 유형 페이지가 열립니다.
1. (선택 사항 및 조건부) 헤더에서 레코드 형식 이름 오른쪽에 있는 **자세히** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 후 다음 중 하나를 수행합니다.

   1. **요청 양식 업데이트**&#x200B;를 클릭하여 요청 양식을 변경한 다음 요청 양식을 클릭하여 열고 편집합니다.
   1. **요청 양식에 대한 링크 복사**&#x200B;를 클릭하여 양식에 대한 링크를 다른 사용자와 공유합니다.

1. (선택 사항) Workfront의 **요청** 영역으로 이동하여 공유 양식을 찾아 요청을 제출합니다. 자세한 내용은 [레코드를 만들도록 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

## 요청 양식 공유

1. 이 문서의 [레코드 형식에 대한 요청 양식 만들기](#create-a-request-form-for-a-record-type) 섹션에 설명된 대로 요청 양식을 만듭니다.
1. 레코드 종류의 페이지에서 요청 양식 이름 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭합니다.
1. 양식을 다른 사용자와 공유하려면 **공유**&#x200B;를 클릭하세요.

1. 양식을 내부적으로 공유하려면 **내부 공유** 탭을 선택하고 **이 양식을 제출하기 위한 액세스 권한 부여** 필드에서 사용자, 팀, 작업 역할, 그룹 또는 회사의 이름을 검색한 다음 목록에 표시될 때 선택합니다. 각 엔터티에 대해 기본적으로 **제출** 권한이 선택됩니다.

   ![요청 양식에 대한 공유 상자](assets/share-box-for-request-form.png)

1. (선택 사항) 엔터티의 이름 뒤에 있는 드롭다운 메뉴를 클릭한 다음 **제거**&#x200B;를 클릭하여 목록에서 해당 엔터티를 제거하고 해당 엔터티와의 양식 공유를 중지합니다.

   >[!NOTE]
   >
   >팀, 그룹, 회사 및 작업 역할 외에도 Adobe Admin Console에 추가된 사용자와만 공유할 수 있습니다. Workfront 전용 사용자는 추가할 수 없습니다. 자세한 내용은 [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)를 참조하십시오.

1. **이 양식을 통해 요청을 제출할 수 있는 사용자** 섹션에서 다음 옵션 중 선택하여 이 양식에 액세스할 수 있는 사용자 유형을 표시합니다.

   * 초대된 사용자만 액세스 가능
   * 작업 영역에 대한 보기 이상의 액세스 권한이 있는 모든 사용자
   * 작업 영역에 대한 참여 이상의 액세스 권한이 있는 모든 사용자
1. (선택 사항) **링크 복사**&#x200B;를 클릭하여 양식에 대한 링크를 액세스 권한이 있는 사람과 공유합니다. 링크가 클립보드에 복사됩니다.
1. 양식을 공개적으로 공유하려면 **공개 공유** 탭을 선택한 다음 **공개 링크 만들기** 설정을 활성화하십시오.

   ![요청 양식에 대한 공개 공유](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* **공개 링크 만들기** 설정을 사용하면 조직 외부에 Workfront 계정이 없는 사람도 양식에 액세스하여 새 레코드를 제출할 수 있습니다.
   >
   >* 다음 필드 형식을 포함하는 양식은 공개적으로 공유할 수 없습니다.
   >
   >     * Workfront 또는 AEM Assets 연결
   >     * 사람
   >

1. **링크 만료 날짜**&#x200B;를 선택하세요.

   현재 날짜로부터 180일 이내에 미래 날짜를 선택할 수 있습니다.

   >[!TIP]
   >
   >공유 날짜가 만료되면 Workfront의 요청 영역에서 요청 양식을 더 이상 사용할 수 없고 다른 사용자와 공유한 링크에 더 이상 액세스할 수 없습니다.

   링크가 만료되면 사람들이 오류를 받게 되며 사람들이 양식에 다시 액세스하려면 링크 날짜를 업데이트하고 공유할 새 링크를 생성해야 합니다.


1. (선택 사항 및 조건부) 양식에 대한 공유 세부 정보를 저장하려면 **저장**&#x200B;을 클릭합니다.
1. (조건부) 양식을 이전에 저장한 경우 **링크 복사**&#x200B;를 클릭합니다.

   양식 공유 옵션이 저장되고 링크가 클립보드에 복사됩니다. 이제 다른 사용자와 공유할 수 있습니다.

   요청 양식에 대한 링크를 사용하여 레코드를 만드는 방법에 대한 자세한 내용은 [Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

1. **양식** 탭의 오른쪽 아래 모서리에 있는 **저장**&#x200B;을 클릭하여 양식을 저장합니다.
