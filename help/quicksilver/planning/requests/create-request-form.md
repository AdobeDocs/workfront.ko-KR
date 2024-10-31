---
title: Adobe Workfront Planning에서 요청 양식 생성 및 관리
description: Adobe Workfront Planning 영역에서 레코드 유형을 선택한 후 요청 양식을 만들어 해당 레코드 유형과 연결할 수 있습니다. 그런 다음 다른 내부 또는 외부 사용자와 링크를 공유할 수 있습니다. 양식에 대한 링크가 있는 사용자는 해당 양식의 필드 값을 채울 수 있으며, 양식 제출을 통해 관련 레코드 유형에 대한 새 레코드를 추가할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: a7cdee912e5047f1c8ef224aff6a41eaa3633df6
workflow-type: tm+mt
source-wordcount: '1375'
ht-degree: 2%

---

# Adobe Workfront Planning에서 요청 양식 만들기 및 관리

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

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
   <td role="rowheader"><p>Adobe Workfront 계획 계획*</p></td>
   <td>
<p>임의 </p>  
<p>각 Workfront Planning 계획에 포함된 사항에 대한 자세한 내용은 Workfront 계정 관리자에게 문의하십시오. </td>

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
1. 요청 양식 이름을 업데이트합니다. 기본적으로 양식 이름은 **제목 없는 요청 양식**&#x200B;입니다. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (선택 사항) 요청 양식에 대해 **설명**&#x200B;을(를) 추가합니다.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Click **Create**. 선택한 레코드 유형에 대한 요청 양식이 열립니다.

   ![](assets/campaigns-request-form-edit-mode.png)

   요청 양식에는 기본적으로 다음 정보가 포함되어 있습니다.

   * 선택한 레코드 유형의 표 보기에서 사용할 수 있는 레코드 필드입니다. <!--they are working on removing the limitation below-->

     >[!IMPORTANT]
     >
     > 요청 양식을 만드는 데 사용하는 환경에 따라 다음과 같은 시나리오가 있습니다.
     >
     >* 다음 형식의 필드가 미리 보기 </span> 또는 프로덕션 환경의 요청 양식 <span class="preview">에 표시되지 않습니다.
     >
     >    * 직원(작성자 및 마지막 수정자 포함)
     >    * 공식
     >    * 제작 일자
     >    * 마지막 수정일
     >    * Workfront 개체의 연결된 필드 또는 조회 필드
     >    * Workfront Planning의 연결된 조회 필드
     >* 다음 유형의 필드는 프로덕션 환경의 요청 양식에 표시되지 않습니다. <span class="preview">미리 보기 환경에 표시됩니다.</span>
     >    * <span class="preview"> Workfront Planning의 연결된 필드(Workfront 연결 및 Experience Manager 자산 포함)</span>


   * **기본 섹션**: Workfront이 요청 양식에 적용하는 기본 섹션 구분입니다. 기본 섹션의 이름을 변경하거나 제거할 수 없습니다.
   * **제목** 필드: Workfront에서 요청을 식별하는 필드입니다. 이 기능은 아직 사용할 수 없습니다. 제목 필드의 구성 및 값을 편집할 수 없습니다.
   * 레코드 유형과 연결된 모든 필드.

     요청 양식에 포함된 필드는 이 레코드 유형에 요청을 제출하는 모든 사람에게 표시됩니다.

1. (선택 사항) 제거할 양식의 필드 위에 마우스를 놓은 다음 **x** 아이콘을 클릭하여 제거합니다. 양식 왼쪽의 **필드** 탭에 추가됩니다.

   예를 들어 **제목** 필드는 Workfront Planning에 표시되지 않으므로 제거합니다. <!--remove this step when we connect intake with the Requests area in Workfront-->
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
1. (선택 사항) 헤더의 양식 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 다음 **편집**&#x200B;을(를) 클릭하여 양식 이름을 업데이트합니다.
1. 양식을 게시하고 고유한 링크를 얻으려면 **Publish**&#x200B;을(를) 클릭하십시오.

   다음과 같은 상황이 발생합니다.

   * **Publish** 단추가 제거되었습니다.
   * **게시 취소** 단추가 양식에 추가됩니다. 클릭하면 양식에 액세스할 수 없습니다.
   * **공유** 단추가 양식에 추가됩니다.

1. 양식을 다른 사용자와 공유하려면 **공유**&#x200B;를 클릭하세요.

   ![](assets/share-box-for-request-form.png)

1. 이 양식에 액세스할 수 있는 사용자 유형을 나타내려면 다음 옵션 중에서 선택합니다.

   * 작업 영역에 대한 보기 이상의 액세스 권한이 있는 모든 사용자
   * 작업 영역에 대한 참여 이상의 액세스 권한이 있는 모든 사용자
   * 링크를 보유한 모든 사용자

   >[!IMPORTANT]
   >
   >**링크가 있는 모든 사용자**&#x200B;를 선택하면 조직 외부의 사람 중 Workfront 계정이 없는 사람도 양식에 액세스하여 새 레코드를 제출할 수 있습니다.

1. (조건부) 이전 단계에서 **링크가 있는 모든 사용자**&#x200B;를 선택한 경우 사용 가능한 달력에서 **링크 만료 날짜**&#x200B;를 선택하십시오. 링크가 만료된 후 오류가 발생하며 양식 액세스 권한을 다시 부여받으려면 먼저 링크 날짜를 업데이트해야 합니다.

   현재 날짜로부터 180일 이내에 미래 날짜를 선택할 수 있습니다.

1. **링크 저장 및 복사**&#x200B;를 클릭하여 양식에 대한 공유 세부 정보를 저장합니다.

   양식 공유 옵션이 저장되고 링크가 클립보드에 복사됩니다. 이제 다른 사용자와 공유할 수 있습니다.

   요청 양식에 대한 링크를 사용하여 레코드를 만드는 방법에 대한 자세한 내용은 [Adobe Workfront Planning 요청 제출](/help/quicksilver/planning/requests/submit-requests.md)을 참조하십시오.

1. 화면 오른쪽 아래 모서리에 있는 **저장**&#x200B;을 클릭하여 양식을 저장합니다.
1. 머리글에서 양식 이름 왼쪽에 있는 왼쪽 화살표를 클릭하여 양식을 닫습니다.

   레코드 유형 페이지가 열립니다.
1. (선택 사항) 헤더에서 레코드 형식 이름 오른쪽에 있는 **자세히** 메뉴 ![](assets/more-menu.png)을(를) 클릭한 후 다음 중 하나를 수행합니다.
   * 요청 양식을 변경하려면 **요청 양식 업데이트**&#x200B;를 클릭하십시오.
   * **요청 양식에 대한 링크 복사**&#x200B;를 클릭하여 양식에 대한 링크를 다른 사용자와 공유합니다.

   >[!TIP]
   >
   >이러한 경우 링크가 공개적으로 공유된다는 표시가 있습니다.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
