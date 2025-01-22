---
title: 레코드 연결
description: 레코드 종류 간에 연결을 만든 후에는 개별 레코드를 서로 연결할 수 있습니다. 레코드를 연결할 때 한 레코드의 정보를 다른 레코드에 표시할 수 있습니다.
recommendations: noDisplay, noCatalog
feature: Workfront Planning
role: User, Admin
author: Alina
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '2912'
ht-degree: 1%

---


# 기록 연결

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning 레코드를 서로 연결하거나 다른 응용 프로그램의 객체에 연결할 수 있습니다. 레코드를 연결할 때 한 레코드의 정보를 다른 레코드에 표시할 수 있습니다.

이 문서에서는 레코드를 연결하는 방법에 대해 설명합니다. 레코드 연결에 대한 일반 정보는 [연결된 레코드 개요](/help/quicksilver/planning/records/connected-records-overview.md)를 참조하십시오.

먼저 두 레코드 형식을 서로 연결하거나 다른 응용 프로그램의 개체 형식에 레코드 형식을 연결해야 합니다. 이렇게 하면 연결된 레코드 필드가 만들어집니다. 그런 다음 연결된 레코드 필드를 사용하여 레코드를 서로 연결하거나 레코드를 다른 응용 프로그램의 다른 개체에 연결할 수 있습니다.

레코드를 연결하는 것은 다른 응용 프로그램의 개체에 레코드를 연결하는 것과 비슷합니다.

레코드 형식을 서로 연결하거나 다른 응용 프로그램의 개체 형식에 연결하는 방법에 대한 자세한 내용은 [레코드 형식 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하십시오.

레코드 종류를 연결하는 예제는 [레코드 종류 및 레코드를 연결하는 예제](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md)를 참조하십시오.

다음을 연결할 수 있습니다.

* Adobe Workfront 계획 레코드
* Adobe Workfront Planning은 다른 응용 프로그램의 객체를 사용하여 레코드를 기록합니다.

  다음 응용 프로그램에서 아래 나열된 형식의 개체에 레코드를 연결할 수 있습니다.

   * Adobe Workfront

      * 프로젝트
      * 포트폴리오
      * 프로그램
      * 회사
      * 그룹

   * Adobe Experience Manager Assets

      * 이미지 파일
      * 폴더

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <li><p> Adobe Workfront 계획<p></li>
   <li><p>Adobe Experience Manager Assets, AEM assets를 Planning 레코드와 연결하려면<p>
   <p>Adobe Experience Manager Assets 라이선스가 있어야 하며 AEM Assets과 Workfront 간의 통합이 있어야 합니다.
    자세한 내용은 <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Experience Manager Assets 및 Assets Essentials용 Adobe Workfront: 문서 색인</a>을 참조하세요. </p>
   </li>  
   </ul></td> 
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
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>레코드를 연결할 작업 영역에 대한 권한 관리 </p>  
   <p>작업공간에 대한 또는 그 이상의 권한을 보고 다른 응용 프로그램에서의 액세스와 관계없이 다른 응용 프로그램의 개체 및 필드에 대한 모든 연결을 볼 수 있습니다. </p>
   <p>Workfront 또는 Experience Manager Assets에서 연결할 개체에 대한 이상의 권한을 봅니다. </p>
   <p>시스템 관리자에게는 작성하지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한이 있습니다.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>레이아웃 템플릿</p></td> 
   <td> <p>Workfront 관리자를 포함한 모든 사용자에게 메인 메뉴의 계획 영역을 포함하는 레이아웃 템플릿을 할당해야 합니다 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 레코드 연결에 대한 고려 사항

* 레코드를 다른 레코드나 개체와 연결하려면 다음이 필요합니다.

   * 하나 이상의 작업 공간, 레코드 유형 및 레코드.

  자세한 내용은 다음 문서를 참조하십시오.

   * [작업 공간 만들기](/help/quicksilver/planning/architecture/create-workspaces.md)
   * [레코드 유형 만들기](/help/quicksilver/planning/architecture/create-record-types.md)
   * [레코드 만들기](/help/quicksilver/planning/records/create-records.md)

   * 레코드 유형 간 또는 레코드 유형과 다른 응용 프로그램의 개체 간 연결입니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.

* 하나 또는 여러 개의 레코드나 개체를 서로 연결할 수 있습니다. 레코드 또는 개체 유형을 연결할 때 선택한 연결 유형에 따라 다릅니다. 자세한 내용은 [레코드 종류 연결 개요](/help/quicksilver/planning/architecture/connect-record-types-overview.md)를 참조하십시오.

## Workfront Planning에서 레코드 연결

Workfront Planning에서 Planning 레코드의 다음 영역에 있는 레코드를 연결할 수 있습니다.

* 테이블 보기의 연결된 레코드 필드입니다.
* 세부 정보 탭의 연결된 레코드 필드에 있는 레코드의 미리 보기 또는 페이지입니다.
* 연결 탭의 레코드 미리 보기 또는 페이지입니다.

### 테이블 보기 또는 세부 정보 영역에서 Adobe Workfront Planning 레코드 연결

{{step1-to-planning}}

1. 연결할 레코드가 있는 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. 테이블 뷰의 이름을 클릭하여 엽니다.
1. (선택 사항) 테이블에 새 행을 추가하여 선택한 레코드 유형에 레코드를 추가합니다. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
1. (조건부) 선택한 레코드 유형을 다른 레코드 유형과 연결한 후 연결된 레코드 열로 이동하여 다른 레코드와 연결할 레코드에 해당하는 셀을 두 번 클릭합니다.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. 다음 중 하나를 수행하십시오.

   * 목록에서 연결된 레코드의 이름을 클릭하여 선택한 레코드에 추가합니다. 레코드가 자동으로 추가됩니다.
   * 레코드의 이름을 입력하고 목록에 표시될 때 클릭합니다. 레코드가 자동으로 추가됩니다.

   >[!TIP]
   >
   >레코드 유형이 연결되어 있을 때 표시할 레코드 이미지만 선택한 경우 연결된 필드에 레코드의 축소판이나 아이콘만 표시됩니다. 자세한 내용은 [레코드 종류 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하세요.
   >

1. (조건부) 레코드 유형을 연결할 때 연결 유형에 대해 일대다 또는 일대일을 선택한 경우 다른 곳에 이미 연결되어 있는 레코드나 개체를 연결하려고 하면 다시 연결하면 원래 연결에서 해당 레코드가 제거된다는 경고가 표시됩니다. 제거를 허용하고 레코드를 연결하려면 **연결**&#x200B;을 클릭하고 필드로 돌아가서 다른 레코드를 선택하려면 **취소**&#x200B;를 클릭하십시오.
1. (선택 사항) 연결할 레코드 또는 개체를 찾을 수 없고 해당 개체를 추가하려면 **+ 추가**&#x200B;를 클릭하여 새 레코드를 추가합니다. 자세한 내용은 문서 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)의 &quot;연결할 때 레코드 만들기&quot; 섹션을 참조하십시오.

   >[!TIP]
   >
   >    표 보기에서 다음을 수행하여 레코드의 페이지를 열고 다른 레코드를 연결할 수 있습니다.
   >1. 보기에서 레코드 이름을 클릭합니다.
   >1. 연결된 레코드 필드를 찾아 필드를 두 번 클릭합니다(이미 연결된 레코드가 있는 경우).
   >또는
   >연결된 레코드 또는 개체 형식에서 레코드를 추가하려면 **레코드 연결**(필드가 비어 있는 경우)을 클릭합니다.
   >
   >![](assets/connect-records-from-record-page-field.png)

1. (선택 사항) 모든 레코드를 표시하려면 **모두 보기**&#x200B;를 클릭합니다.

1. (조건부) 이전 단계에서 **모두 보기**&#x200B;를 클릭한 경우 **개체 연결** 상자가 표시됩니다.

   ![](assets/connected-objects-table-for-records.png)

1. 검색 상자에 레코드 이름을 입력한 다음 목록에 표시될 때 선택합니다

   또는

   상자에서 하나 이상의 레코드 이름을 선택한 다음 **개체 연결**&#x200B;을 클릭합니다.

   다음이 추가됩니다.

   * 연결된 레코드는 이전 단계에서 선택한 레코드의 연결된 레코드 필드에 표시됩니다.
   * 레코드 유형을 연결할 때 연결된 조회 필드를 추가한 경우 연결된 필드는 연결된 레코드의 정보로 채워집니다.

   연결된 레코드를 업데이트하면 연결되는 레코드의 연결된 필드가 자동으로 업데이트됩니다. 연결된 필드는 수동으로 편집할 수 없습니다.

   >[!TIP]
   >
   >* &quot;연결된 필드&quot;와 &quot;조회 필드&quot;를 서로 교환하여 사용합니다.
   >
   >* 레코드 유형을 연결할 때 여러 레코드에 연결하도록 선택하면 여러 개체의 필드 값이 쉼표로 구분되어 표시되거나 레코드 유형을 연결할 때 선택한 집계자에 따라 집계됩니다.

1. (선택 사항) 레코드 유형 페이지를 닫고 선택한 작업 영역으로 이동합니다.
1. 연결한 레코드 종류의 카드를 클릭합니다.

   예를 들어 **Campaign** 레코드를 제품 레코드와 연결한 경우 **Product** 카드를 클릭합니다.

   레코드 유형 카드가 표 보기에서 열립니다. 그렇지 않으면 테이블 뷰를 선택합니다.

   **Campaign** 연결된 레코드 필드에는 제품 레코드 종류 페이지에서 제품에 연결한 캠페인의 이름이 표시됩니다. Campaign 정보를 업데이트하면 제품 레코드 유형에 대한 Campaign 연결 레코드 필드가 자동으로 업데이트됩니다.

### 테이블 보기 또는 레코드의 세부 정보 페이지에서 Adobe Workfront Planning 레코드를 Workfront 객체에 연결

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

레코드 형식과 Workfront 개체 형식 간에 연결을 만든 후 개별 레코드를 Workfront의 개체에 연결할 수 있습니다. 연결한 Workfront 필드는 개체를 연결할 레코드에서 자동으로 채워집니다.

>[!NOTE]
>
>Workfront에서 Workfront 개체 유형을 Workfront Planning 레코드 유형과 연결할 수 없습니다.


{{step1-to-planning}}

1. 연결할 레코드가 있는 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 카드로 표시됩니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. **보기** 드롭다운 메뉴에서 **테이블** 보기를 선택하십시오.

1. 선택한 레코드 종류에 개별 레코드를 추가하려면 **새 레코드**&#x200B;을(를) 클릭하십시오. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.

1. (조건부) 선택한 레코드 유형을 Workfront 개체 유형과 연결한 후 연결된 개체 열로 이동하여 Workfront의 개체와 연결할 레코드에 해당하는 셀을 두 번 클릭합니다.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. 다음 중 하나를 수행하십시오.

   * 목록에서 개체를 클릭하여 선택한 레코드에 추가합니다. 객체는 알파벳순으로 나열됩니다. 개체가 자동으로 추가됩니다.
   * 객체의 이름을 입력하고 목록에 표시될 때 클릭합니다. 개체가 자동으로 추가됩니다.

   >[!TIP]
   >
   >보기에서 레코드의 페이지를 열거나 연결된 레코드 필드를 두 번 클릭하거나 필드에서 **연결**&#x200B;을 클릭하여 연결된 개체 형식의 개체를 추가할 수 있습니다.

1. (선택 사항) 연결할 개체를 찾을 수 없고 개체를 추가하려면 **+ 추가**&#x200B;를 클릭하여 새 프로젝트 또는 포트폴리오를 만들고 추가하십시오.

   자세한 내용은 [Workfront Planning에서 Workfront 개체 만들기](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)를 참조하십시오.

1. (선택 사항) 적어도 볼 수 있는 권한이 있는 모든 개체를 표시하려면 **모두 보기**&#x200B;를 클릭합니다.

   이전 단계에서 **모두 보기**&#x200B;를 클릭한 경우 **개체 연결** 상자가 표시됩니다.

   ![](assets/connect-objects-box-to-select-projects.png)

1. 검색 상자에 Workfront 개체 이름을 입력한 다음 목록에 표시될 때 선택합니다

   또는

   상자에서 하나 이상의 개체 이름을 선택한 다음 **개체 연결**&#x200B;을 클릭합니다.

   >[!IMPORTANT]
   >
   >* 보기 액세스 권한이 있는 Workfront 개체만 추가할 수 있습니다.
   >
   >* Workfront 개체를 추가하면 작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자가 Workfront에서의 권한 또는 액세스 권한에 관계없이 Workfront 개체 및 해당 필드 정보를 볼 수 있습니다.

   다음이 추가됩니다.

   * 선택한 Workfront 개체가 연결된 레코드 필드에 추가됩니다.
   * 레코드 종류를 Workfront에 연결할 때 추가한 경우, Workfront 개체의 연결된 필드(또는 조회 필드)는 Workfront의 정보로 자동으로 채워집니다.

   다른 응용 프로그램의 개체와 레코드 형식을 연결하는 방법에 대한 자세한 내용은 [레코드 형식 연결](/help/quicksilver/planning/architecture/connect-record-types.md)을 참조하십시오.

1. (선택 사항) 테이블 보기의 연결된 필드 또는 레코드 페이지의 연결된 필드에서 Workfront Planning 레코드에 연결된 Workfront 개체의 이름을 클릭합니다.

   이 경우 객체에 대한 보기 권한이 적어도 있으면 Workfront에서 Workfront 객체가 열립니다.

   >[!TIP]
   >
   >* 레코드 유형을 연결할 때 여러 레코드를 연결하도록 선택하면 조회 필드의 값이 쉼표로 구분되어 표시되거나 선택한 집계기에 따라 집계됩니다.
   >
   >* Workfront의 연결된 Workfront 개체에 대해 연결된 레코드 필드가 만들어지지 않습니다.

1. (선택 사항) 레코드 종류의 테이블 보기에서 연결된 Workfront 개체의 열 머리글 위로 마우스를 가져간 다음 드롭다운 메뉴를 클릭한 다음 **조회 필드 편집**&#x200B;을 클릭합니다.

1. **선택하지 않은 필드** 영역에서 Workfront 개체 필드 추가

   또는

   **선택한 필드** 영역에서 Workfront 개체 필드를 제거합니다.

   이렇게 하면 Workfront Planning 레코드에서 연결된 필드가 추가되거나 제거됩니다. 제거된 필드와 관련된 정보는 Workfront에 남아 있습니다.


### 레코드 페이지의 테이블 보기 또는 세부 정보 탭에서 Workfront Planning 레코드를 Adobe Experience Manager 개체에 연결합니다.

<!--when we will have more applications to link to from Planning, change the title to something like: Connect Workfront Planning records to objects from other applications-->

>[!IMPORTANT]
>
>Adobe Experience Manager Assets 라이선스가 있어야 하며, Workfront Planning 레코드를 Adobe Experience Manager Assets에 연결하려면 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.
>
>Adobe Admin Console 온보딩에 대한 질문이 있는 경우 [통합 경험 Adobe FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md)를 참조하십시오.

레코드 종류와 Adobe Experience Manager Assets 간에 연결을 만들면 개별 레코드를 Experience Manager 에셋에 연결할 수 있습니다. 연결을 만들 때 Experience Manager Assets에서 연결한 에셋 필드는 연결한 레코드 종류에 자동으로 채워집니다.

>[!NOTE]
>
>Workfront 관리자가 Experience Manager Assets과 Adobe Experience Manager Assets 간의 통합을 통해 메타데이터 매핑을 구성할 때 Workfront에서 Planning 레코드 및 해당 필드에 액세스할 수 있습니다. 자세한 내용은 [Adobe Workfront과 Experience Manager Assets 간의 에셋 메타데이터 매핑 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)을 참조하십시오.

레코드를 Experience Manager 에셋과 연결하려면 다음 작업을 수행하십시오.

{{step1-to-planning}}

1. 연결할 레코드가 있는 작업 영역을 클릭합니다.

   작업공간이 열리고 레코드 유형이 표시됩니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. 레코드 종류 페이지의 오른쪽 위 모서리에 있는 **보기** 드롭다운 메뉴에서 **테이블** 보기를 선택하십시오.

1. (선택 사항) 선택한 레코드 형식에 새 레코드를 추가하려면 **새 레코드**&#x200B;을 클릭합니다. 자세한 내용은 [레코드 만들기](/help/quicksilver/planning/records/create-records.md)를 참조하세요.
1. (조건부) 선택한 레코드 종류를 Experience Manager Assets에 연결한 후 연결된 개체 열로 이동하여 Experience Manager에서 다른 개체와 연결할 레코드에 해당하는 셀을 마우스로 가리킨 다음 **+** 아이콘을 클릭합니다.

   >[!TIP]
   >
   >  레코드 페이지의 연결된 개체 필드에서 **+** 아이콘을 클릭하여 자산을 레코드에 연결할 수 있습니다.

   **Assets 선택** 상자가 표시됩니다. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. 를 클릭하여 다음 유형의 자산 중 일부를 선택합니다.

   * 이미지
   * 폴더

   여러 자산을 선택할 수 있습니다.

   >[!IMPORTANT]
   >
   > Experience Manager에서 볼 수 있는 액세스 권한이 있는 에셋만 연결할 수 있습니다. 연결되면 모든 Workfront Planning 사용자는 Experience Manager Assets에서의 액세스 권한에 관계없이 Workfront Planning에서 에셋을 볼 수 있습니다.

1. **선택**&#x200B;을 클릭합니다. <!-- we might change this to Connect-->

   다음이 추가됩니다.

   * 선택한 Experience Manager 에셋이 연결된 레코드 필드에 추가됩니다.
   * 연결된 필드(또는 조회 필드)는 Experience Manager 연결된 자산의 정보로 채워집니다.

     Experience Manager 에셋 필드의 기존 정보는 연결된 필드 또는 조회 필드에 자동으로 표시됩니다.

     >[!TIP]
     >
     >* 레코드 유형을 연결할 때 여러 레코드를 연결하도록 선택하면 선택한 집계기에 따라 여러 개체의 값이 쉼표로 구분되거나 집계되어 표시됩니다.
     >
     >* Workfront Planning 연결 레코드에 대한 연결된 레코드 필드는 Experience Manager Assets 애플리케이션에서 연결된 Experience Manager 자산에 대해 생성되지 않습니다.

1. (선택 사항) Experience Manager Assets에 연결한 레코드 유형으로 이동하고 연결된 레코드 필드에서 에셋의 이름을 클릭합니다. 에셋의 Experience Manager 세부 정보가 팝업 창에 표시됩니다.

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   이미지 파일에 대해 다음 필드가 표시됩니다.

   * 이미지의 축소판
   * 이미지 파일 이름
   * 차원
   * 크기
   * 설명
   * Experience Manager의 파일 경로
   * 에셋 유형
   * 제작일
   * 수정일

1. (선택 사항) Experience Manager에서 에셋 Experience Manager 레코드 페이지를 열려면 연결하려는 레코드의 레코드 종류 페이지로 이동하고 연결된 레코드 필드에서 에셋 이름을 클릭하여 팝업 창을 연 다음 **AEM에서 열기** 아이콘 ![](assets/open-asset-icon.png)을 클릭하여 에셋을 엽니다.

   이렇게 하면 Adobe Experience Manager Assets에서 Experience Manager 에셋이 열립니다.

1. (선택 사항) 레코드 종류의 테이블 보기에서 연결된 Experience Manager 에셋의 열 머리글 위로 마우스를 가져간 다음 드롭다운 메뉴를 클릭한 다음 **조회 필드 편집**&#x200B;을 클릭합니다.

1. **선택하지 않은 필드** 영역에서 Experience Manager Assets 개체 필드 추가

   또는

   **선택한 필드** 영역에서 Workfront 개체 필드를 제거합니다.

   이렇게 하면 레코드에서 연결된 필드가 추가되거나 제거됩니다. 제거된 필드와 관련된 정보는 Experience Assets Adobe에 남아 있습니다.

### 레코드 페이지의 연결 탭에서 Workfront Planning 레코드를 다른 레코드 또는 개체와 연결합니다.

1. 다른 Planning 레코드 유형 또는 다른 응용 프로그램의 객체 유형에 연결된 레코드 유형의 모든 뷰로 이동합니다.
1. 이전 하위 섹션에 설명된 단계에 따라 다른 레코드나 오브젝트와 연결할 레코드를 뷰에서 찾습니다.
1. 레코드 이름을 클릭합니다.

   미리보기 페이지가 열립니다.
1. (선택 사항) **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png)을 클릭하여 레코드 페이지를 엽니다.
1. 레코드의 미리 보기 또는 페이지에서 **연결** 탭을 클릭합니다.

   ![](assets/connections-tab-on-record-in-workfront-planning.png)

   선택한 레코드 유형에 연결된 모든 레코드 또는 개체 유형이 섹션으로 표시됩니다. 연결된 레코드 또는 개체는 카드의 레코드 또는 개체 유형 이름 아래에 표시됩니다.

   >[!TIP]
   >
   >    기본적으로 개별 레코드가 연결된 연결된 연결된 레코드만 표시됩니다.

1. (선택 사항) 연결된 레코드가 없는 레코드 종류를 포함하여 연결된 모든 레코드 종류를 표시하려면 **모든 연결 표시**&#x200B;를 클릭합니다.

1. (선택 사항) 축소하려면 섹션의 왼쪽에 있는 아래쪽 방향 화살표를 클릭합니다.

1. (조건부) 같은 형식의 레코드나 개체를 더 추가하려면 **연결**&#x200B;을 클릭합니다.
1. 이전 섹션에서 설명한 단계에 따라 Workfront Planning의 레코드 또는 Workfront 또는 Experience Manager Assets의 개체를 연결합니다.
레코드와 개체가 즉시 추가됩니다.
1. (선택 사항) 레코드 또는 개체의 연결된 카드 위에 마우스를 놓은 다음 **레코드 연결 끊기** 아이콘 ![](assets/disconnect-icon-with-tooltip.png)을 클릭하여 선택한 레코드에서 연결을 끊습니다.

   ![](assets/disconnect-record-icon-with-tooltip-on-connections-tab.png)

   레코드는 Workfront Planning의 모든 영역 또는 연결된 것으로 표시될 수 있는 다른 응용 프로그램에서 즉시 연결이 끊어집니다. 모든 조회 필드 값도 제거됩니다.

## Workfront 개체에서 레코드 연결

Workfront 객체에서 Workfront Planning 레코드를 연결하려면 다음이 있어야 합니다.

* 레코드 유형과 Workfront Planning에서 설정된 Workfront 객체 유형 간의 연결입니다.
* Workfront 또는 그룹 관리자는 레이아웃 템플릿의 Workfront 프로젝트, 포트폴리오 및 프로그램에 계획 섹션을 추가해야 합니다.

자세한 내용은 [Adobe Workfront 개체의 계획 섹션에서 레코드 관리](/help/quicksilver/planning/records/manage-records-in-planning-section.md)를 참조하십시오.
