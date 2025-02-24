---
title: Adobe Workfront Planning에서 요청 양식 생성 및 관리
description: Adobe Workfront Planning 영역에서 레코드 유형을 선택한 후 요청 양식을 만들어 해당 레코드 유형과 연결할 수 있습니다. 그런 다음 다른 내부 또는 외부 사용자와 링크를 공유할 수 있습니다. 양식에 대한 링크가 있는 사용자는 해당 양식의 필드 값을 채울 수 있으며, 양식 제출을 통해 관련 레코드 유형에 대한 새 레코드를 추가할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 7fc2239de2488d2e3e5c434ab45e8a1d24c0b28f
workflow-type: tm+mt
source-wordcount: '1479'
ht-degree: 2%

---

# Adobe Workfront Planning에서 요청 양식 만들기 및 관리

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

요청 양식을 만들어 Adobe Workfront Planning에서 레코드 유형과 연결할 수 있습니다. 그런 다음 다른 내부 또는 외부 사용자와 링크를 공유할 수 있습니다.

양식에 대한 링크가 있는 사용자는 해당 양식의 필드 값을 업데이트하고 이를 제출하여 새 레코드를 추가할 수 있습니다.

이 문서에서는 작업 영역 관리자가 레코드 유형과 연결된 요청 양식을 만드는 방법에 대해 설명합니다.

레코드를 만들기 위해 레코드 형식에 요청을 제출하는 방법에 대한 자세한 내용은 [레코드를 만들기 위한 Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

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
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </td>

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
   <td>
   <p>표준</p>
   <p>기존 Workfront 라이선스에는 Workfront Planning을 사용할 수 없습니다.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>개체 권한</p></td>
   <td>
   <ul>
   <li><p>작업 공간에 대한 권한 관리</p></li>
    <li><p>시스템 관리자는 자신이 만들지 않은 작업 공간을 관리할 수 있습니다. </p></li>
    </ul>
   <p>Workfront Planning 객체의 권한 공유에 대한 자세한 내용은  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Adobe Workfront Planning의 공유 권한 개요</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다. </p>  
</td>
  </tr>
 </tbody>
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 유형에 대한 요청 양식 만들기

{{step1-to-planning}}

1. 레코드를 추가할 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.

1. 레코드 유형 카드를 클릭합니다. 레코드 종류 만들기에 대한 자세한 내용은 [레코드 종류 만들기](/help/quicksilver/planning/architecture/create-record-types.md)를 참조하세요.

   마지막으로 액세스한 보기에서 레코드 유형 페이지가 열립니다. 기본적으로 레코드 유형 페이지가 표 뷰에 열립니다.

1. 페이지 헤더의 레코드 형식 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **요청 양식 만들기**&#x200B;를 클릭합니다.
1. 요청 양식 이름을 업데이트합니다. 기본적으로 양식 이름은 **제목 없는 양식**&#x200B;입니다. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (선택 사항) 요청 양식에 대해 **설명**&#x200B;을(를) 추가합니다.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Click **Create**. 선택한 레코드 유형에 대한 요청 양식이 양식 탭에서 열립니다.

   ![](assets/campaigns-request-form-edit-mode.png)

   요청 양식에는 기본적으로 다음 정보가 포함되어 있습니다.

   * 선택한 레코드 유형의 표 보기에서 사용할 수 있는 레코드 필드입니다. <!--they are working on removing the limitation below-->

   <!-- when we go to prod, the Preview batch below will become the only batch-->

   >[!IMPORTANT]
   >
   >다음 유형의 필드가 요청 양식에 표시되지 않습니다.
   >
   >* 작성자 및 마지막 수정자
   >* 생성 날짜 및 마지막 수정 날짜
   >* 공식
   >* Workfront 개체의 조회 필드
   >* Workfront Planning 연결된 레코드의 조회 필드
   >

   <!--before release to prod: 
    > Depending on what environment you use to create a request form, the following scenarios exist:
   >
   >* Fields of the following types do not display in the request form in the Production environment: 
   >
   >    * Created by and Last modified by
   >    * Created date and Last modified date
   >    * Formula
   >    * People 
   >    * Workfront connected fields
   >    * Workfront objects' lookup fields
   >    * Workfront Planning records' connected fields
   >    * Workfront Planning connected records' lookup fields
   >    * AEM Assets connection fields-->

   * **기본 섹션**: Workfront이 요청 양식에 적용하는 기본 섹션 구분입니다. 모든 레코드 필드가 **기본 섹션** 영역에 표시됩니다.
   * **제목** 필드: Workfront에서 요청을 식별하는 필드입니다. 제목 필드의 구성 및 값을 편집할 수 없습니다.

     >[!TIP]
     >
     >**제목** 필드는 요청 양식에 표시되면 값이 필요합니다. 그러나 필요한 경우 **제목** 필드를 제거할 수 있으며 요청자가 요청을 제출할 때 양식에 표시되지 않습니다.

   * 레코드 유형과 연결된 모든 필드.

     요청 양식에 포함된 필드는 이 레코드 유형에 요청을 제출하는 모든 사람에게 표시됩니다.

1. (선택 사항) 제거할 양식의 필드 위에 마우스를 놓은 다음 **x** 아이콘을 클릭하여 제거합니다. 양식 왼쪽의 **필드** 탭에 추가됩니다.

   예를 들어 **제목** 필드는 Workfront Planning에 표시되지 않으므로 제거합니다. <!--remove this step when we connect intake with the Requests area in Workfront-->
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

   >[!NOTE]
   >
   >   각 필드의 필드 유형은 양식에서 필드를 선택한 후 오른쪽 패널 상단에 표시됩니다.
   >   
   >
   >   통화, 숫자 및 백분율 필드는 한 줄 텍스트 필드 유형으로 표시됩니다. 그러나 필드 형식은 유지되고 이러한 필드 내의 값은 통화, 숫자 및 백분율 값으로 표시됩니다.

1. (선택 사항) 양식 왼쪽에 있는 **콘텐츠 요소** 탭을 클릭하고 다음 요소를 추가합니다.

   * **설명 텍스트**
   * **섹션 구분**

   사용자 정의 양식 작성에 대한 자세한 내용은 [사용자 정의 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.

1. (선택 사항) **미리 보기**&#x200B;를 클릭하여 다른 사용자가 새 레코드를 제출하는 데 사용할 양식을 표시할 방법을 확인합니다.

1. (선택 사항) **구성** 탭을 클릭한 다음 **승인자** 필드에 사용자를 한 명 이상 추가하여 이 레코드 양식에 대한 새 요청을 승인합니다.

   ![](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * 요청 양식을 승인자와 연결하는 경우 새 레코드를 생성하기 전에 모든 승인자가 새 요청을 먼저 승인해야 합니다.
   * 한 명 또는 여러 명의 승인자를 요청 양식에 추가할 수 있습니다.
   * 최소 한 명 이상의 승인자가 요청을 거부하면 요청이 거부되고 레코드가 만들어지지 않습니다.
   * 요청이 승인 또는 거부되기 전에 모든 승인자는 결정을 내려야 합니다.

     요청 양식에 승인을 추가하는 방법에 대한 자세한 내용은 [요청 양식에 승인 추가](/help/quicksilver/planning/requests/add-approval-to-request-form.md)를 참조하십시오.

1. (선택 사항) 헤더의 양식 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭하여 양식 이름을 업데이트합니다.
1. 양식을 게시하고 고유한 링크를 얻으려면 **게시**&#x200B;를 클릭하십시오.

   다음과 같은 상황이 발생합니다.

   * **게시** 단추가 제거되었습니다.
   * **게시 취소** 단추가 양식에 추가됩니다. 클릭하면 양식에 액세스할 수 없습니다.
   * **공유** 단추가 양식에 추가됩니다.

1. 양식을 다른 사용자와 공유하려면 **공유**&#x200B;를 클릭하세요.

   ![](assets/share-box-for-request-form.png)

1. 이 양식에 액세스할 수 있는 사용자 유형을 나타내려면 다음 옵션 중에서 선택합니다.

   * 작업 영역에 대한 보기 이상의 액세스 권한이 있는 모든 사용자
   * 작업 영역에 대한 참여 이상의 액세스 권한이 있는 모든 사용자
   * 링크를 보유한 모든 사용자

   >[!WARNING]
   >
   >* **링크가 있는 모든 사용자**&#x200B;를 선택하면 조직 외부의 사람 중 Workfront 계정이 없는 사람도 양식에 액세스하여 새 레코드를 제출할 수 있습니다.
   >
   > * 다음 필드 형식을 포함하는 양식은 공개적으로 공유할 수 없습니다.
   >
   >     * Workfront 또는 AEM Assets 연결
   >     * 사용자
   >

1. (조건부) 이전 단계에서 **링크가 있는 모든 사용자**&#x200B;를 선택한 경우 사용 가능한 달력에서 **링크 만료 날짜**&#x200B;를 선택하십시오. 링크가 만료되면 사람들이 오류를 받게 되며 사람들이 양식에 다시 액세스하려면 링크 날짜를 업데이트하고 공유할 새 링크를 생성해야 합니다.

   현재 날짜로부터 180일 이내에 미래 날짜를 선택할 수 있습니다.

1. **링크 저장 및 복사**&#x200B;를 클릭하여 양식에 대한 공유 세부 정보를 저장합니다. 양식을 이전에 저장한 경우 **링크 복사**&#x200B;를 클릭합니다.

   양식 공유 옵션이 저장되고 링크가 클립보드에 복사됩니다. 이제 다른 사용자와 공유할 수 있습니다.

   요청 양식에 대한 링크를 사용하여 레코드를 만드는 방법에 대한 자세한 내용은 [Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

1. **양식** 탭의 오른쪽 아래 모서리에 있는 **저장**&#x200B;을 클릭하여 양식을 저장합니다.
1. 머리글에서 양식 이름 왼쪽에 있는 왼쪽 화살표를 클릭하여 양식을 닫습니다.

   레코드 유형 페이지가 열립니다.
1. (선택 사항) 헤더에서 레코드 형식 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 후 다음 중 하나를 수행합니다.
   * 요청 양식을 변경하려면 **요청 양식 업데이트**&#x200B;를 클릭하십시오.
   * **요청 양식에 대한 링크 복사**&#x200B;를 클릭하여 양식에 대한 링크를 다른 사용자와 공유합니다.

   >[!TIP]
   >
   >이러한 경우 링크가 공개적으로 공유된다는 표시가 있습니다.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
