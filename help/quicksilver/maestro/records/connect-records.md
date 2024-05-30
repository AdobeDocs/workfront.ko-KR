---
title: 기록 연결
description: 레코드 종류 간에 연결을 만든 후에는 개별 레코드를 서로 연결할 수 있습니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 1%

---

<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# 기록 연결

{{planning-important-intro}}

Adobe Workfront Planning 레코드를 서로 연결하거나 다른 응용 프로그램의 객체에 연결할 수 있습니다.

먼저 두 레코드 형식을 서로 연결하거나 다른 응용 프로그램의 개체 형식에 레코드 형식을 연결해야 합니다. 이렇게 하면 연결된 레코드 필드가 만들어집니다. 그런 다음 연결된 레코드 필드를 사용하여 레코드를 서로 연결하거나 레코드를 다른 응용 프로그램의 다른 개체에 연결할 수 있습니다.

레코드를 연결하는 것은 다른 응용 프로그램의 개체에 레코드를 연결하는 것과 비슷합니다.

레코드 형식을 서로 연결하거나 다른 응용 프로그램의 개체 형식에 연결하는 방법에 대한 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

레코드 종류 연결에 대한 예는 [레코드 종류 및 레코드 연결의 예](../architecture/example-connect-record-types-and-records.md).

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

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>제품</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Adobe Workfront Planning 레코드를 Experience Manager Assets과 연결하려면 Adobe Experience Manager Assets 라이선스가 있어야 하며, 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다. 자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 통합 경험 Adobe</a>.</p>
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Workfront Planning의 조기 액세스 단계에 조직을 등록해야 합니다. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td>
   <td>
   <p>임의</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Workfront Planning에 대한 액세스 수준 제어가 없습니다.</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>레코드를 연결할 작업 영역에 대한 권한 관리 </p>  
   <p>다른 응용 프로그램의 액세스 권한에 관계없이 다른 응용 프로그램의 개체 및 필드에 대한 모든 연결을 볼 수 있는 작업공간에 대한 이상의 권한을 봅니다. </p>
   <p>시스템 관리자에게는 작성하지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한이 있습니다.</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 계획 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 레코드 연결에 대한 고려 사항

* 레코드 유형을 연결하면 연결된 레코드 유형이 연결된 레코드 유형의 테이블 및 해당 레코드 페이지에서 연결된 레코드 필드로 표시됩니다.
* 연결된 레코드 필드에서 연결된 레코드와 개체 유형의 레코드와 개체를 찾아보고 추가할 수 있습니다.
* 연결된 레코드 유형의 필드를 연결 중인 레코드 유형의 테이블에 추가할 수 있습니다.
* 연결 중인 레코드의 연결된 필드 값은 수동으로 업데이트할 수 없습니다.

  연결된 레코드의 연결된 필드 값은 원본 레코드나 개체에서 자동으로 연결되는 Workfront Planning 레코드를 채웁니다.

* Workfront 계획 및 보기에 대한 액세스 권한 또는 작업 공간에 대한 상위 권한이 있는 모든 사용자는 레코드 간 또는 레코드와 다른 응용 프로그램의 개체 간에 수행하는 연결을 볼 수 있습니다. 연결하려는 응용 프로그램의 사용 권한에 관계없이 연결된 레코드와 개체를 볼 수 있습니다.
* 연결된 레코드가 있는 작업 영역에 대한 관리 권한이 있는 경우 다른 사용자의 연결을 보고 편집할 수 있습니다.
* 한 레코드를 다른 응용 프로그램에서 하나 또는 여러 개체에 연결할 수 있습니다.
* 레코드를 다른 레코드나 개체와 연결하려면 다음이 필요합니다.

   * 하나 이상의 작업 공간, 레코드 유형 및 레코드.

     자세한 내용은 다음 문서를 참조하십시오.

      * [작업 공간 만들기](../architecture/create-workspaces.md)
      * [레코드 유형 만들기](../architecture/create-record-types.md)
      * [레코드 만들기](../records/create-records.md)

   * 레코드 유형 간 또는 레코드 유형과 다른 응용 프로그램의 개체 간 연결입니다. 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md)
* Workfront에서 다음 영역의 Workfront Planning 레코드로 객체를 연결할 수 있습니다.
   * Workfront Planning의 Planning 레코드에서.
   * Workfront 객체의 Planning 섹션에서 다음을 수행합니다.

## Workfront Planning에서 레코드 연결

### Adobe Workfront 계획 레코드 연결

{{step1-to-maestro}}

기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드를 연결할 작업 영역을 선택합니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. 선택 **표** 다음에서 보기 **보기** 레코드 유형 페이지의 오른쪽 위 모서리에 있는 드롭다운 메뉴.
1. (선택 사항) 테이블에 새 행을 추가하여 선택한 레코드 유형에 레코드를 추가합니다. 자세한 내용은 [레코드 만들기](../../maestro/records/create-records.md).
1. (조건부) 선택한 레코드 종류를 다른 레코드 종류와 연결한 후 연결된 레코드 열로 이동하여 다른 레코드와 연결할 레코드에 해당하는 셀을 두 번 클릭합니다.

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. 다음 중 하나를 수행하십시오.

   * 목록에서 연결된 레코드의 이름을 클릭하여 선택한 레코드에 추가합니다. 레코드가 자동으로 추가됩니다.
   * 레코드의 이름을 입력하고 목록에 표시될 때 클릭합니다. 레코드가 자동으로 추가됩니다.
   * 클릭 **모두 보기** 모든 레코드를 표시합니다.

1. (조건부) 을 클릭한 경우 **모두 선택** 이전 단계에서 **오브젝트 연결** 상자가 표시됩니다.

   ![](assets/connected-objects-table-for-records.png)

1. 검색 상자에 레코드 이름을 입력한 다음 목록에 표시될 때 선택합니다

   또는

   상자에서 하나 이상의 레코드 이름을 선택한 다음 **오브젝트 연결** 을 클릭합니다.

   >[!TIP]
   >
   >    레코드의 페이지를 열고 연결된 레코드 필드를 찾은 다음 **레코드 연결** 연결된 레코드 또는 개체 유형에서 레코드를 추가할 수 있습니다.
   >
   >![](assets/connect-records-from-record-page-field.png)

   다음이 추가됩니다.

   * 연결된 레코드는 6단계에서 선택한 레코드의 연결된 레코드 필드에 표시됩니다. <!--accurate?-->
   * 레코드 유형을 연결할 때 연결된 조회 필드를 추가한 경우 연결된 필드는 연결된 레코드의 정보로 채워집니다.

   연결된 레코드를 업데이트하면 연결되는 레코드의 연결된 필드가 자동으로 업데이트됩니다. 연결된 필드는 수동으로 편집할 수 없습니다.

   >[!TIP]
   >
   >* &quot;연결된 필드&quot;와 &quot;조회 필드&quot;를 서로 교환하여 사용합니다.
   >
   >* 을 활성화한 경우 **여러 레코드 허용** 레코드 유형을 연결하면 선택한 여러 개체의 필드 값이 쉼표로 구분되어 표시되거나 선택한 집계기에 따라 집계됩니다.

1. (선택 사항) 레코드 유형 페이지를 닫고 선택한 작업 영역으로 이동합니다.
1. 연결한 레코드 종류의 카드를 클릭합니다.

   예를 들어 를 연결한 경우 **캠페인** 제품 레코드와 함께 레코딩하려면 **제품** 카드.

   레코드 유형 카드가 표 보기에서 열립니다. 그렇지 않으면 테이블 뷰를 선택합니다.

   다음 사항에 주목하십시오. **캠페인** 연결된 레코드 필드는 제품 레코드 유형 페이지에서 제품에 연결한 캠페인의 이름을 표시합니다. Campaign 정보를 업데이트하면 제품 레코드 유형에 대한 Campaign 연결 레코드 필드가 자동으로 업데이트됩니다.

### Adobe Workfront Planning 레코드를 Workfront 객체에 연결

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

레코드 형식과 Workfront 개체 형식 간의 연결을 만든 후에는 개별 레코드를 Workfront의 개체에 연결할 수 있습니다. 연결한 Workfront 필드는 개체를 연결할 레코드에서 자동으로 채워집니다.

>[!NOTE]
>
>Workfront에서 Workfront 개체 유형을 Workfront Planning 레코드 유형과 연결할 수 없습니다.


{{step1-to-maestro}}

기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드를 연결할 작업 영역을 선택합니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. 선택 **표** 다음에서 보기 **보기** 드롭다운 메뉴.

1. 클릭 **새 레코드**  선택한 레코드 유형에 개별 레코드를 추가할 수 있습니다. 자세한 내용은 [레코드 만들기](../../maestro/records/create-records.md).
1. (조건부) 선택한 레코드 종류를 Workfront 개체 형식과 연결한 후 연결된 개체 열로 이동하여 Workfront의 개체와 연결할 레코드에 해당하는 셀을 두 번 클릭합니다.

   ![](assets/connect-projects-smaller-box-in-table-view.png)

1. 다음 중 하나를 수행하십시오.

   * 목록에서 개체를 클릭하여 선택한 레코드에 추가합니다. 객체는 알파벳순으로 나열됩니다. 개체가 자동으로 추가됩니다.
   * 객체의 이름을 입력하고 목록에 표시될 때 클릭합니다. 개체가 자동으로 추가됩니다.
   * 클릭 **모두 보기** 최소한 볼 수 있는 권한이 있는 모든 개체를 표시합니다.

1. (조건부) 을 클릭한 경우 **모두 보기** 이전 단계에서 **오브젝트 연결** 상자가 표시됩니다.

   ![](assets/connect-objects-box-to-select-projects.png)

1. 검색 상자에 Workfront 개체 이름을 입력한 다음 목록에 표시될 때 선택합니다

   또는

   상자에서 하나 이상의 개체 이름을 선택한 다음 **오브젝트 연결** 을 클릭합니다.

   >[!IMPORTANT]
   >
   >* 보기 액세스 권한이 있는 Workfront 개체만 추가할 수 있습니다.
   >
   >* Workfront 개체를 추가하면 작업 영역에 대한 보기 이상의 권한이 있는 모든 사용자가 Workfront에서의 권한 또는 액세스 권한에 관계없이 Workfront 개체 및 해당 필드 정보를 볼 수 있습니다.

   다음이 추가됩니다.

   * 선택한 Workfront 개체가 연결된 레코드 필드에 추가됩니다.
   * 레코드 종류를 Workfront에 연결할 때 추가한 경우, Workfront 개체의 연결된 필드(또는 조회 필드)는 Workfront의 정보로 자동으로 채워집니다.

   >[!TIP]
   >
   >레코드의 페이지를 열고 연결된 레코드 필드를 찾은 다음 **+** 연결된 객체 유형에서 객체를 추가하는 필드의 아이콘.

   다른 응용 프로그램의 개체와 레코드 형식을 연결하는 방법에 대한 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).

1. (선택 사항) 테이블 보기의 연결된 필드 또는 레코드 페이지의 연결된 필드에서 Workfront Planning 레코드에 연결된 Workfront 개체의 이름을 클릭합니다.

   연결된 Workfront 개체에 대한 읽기 전용 Workfront Planning 레코드 페이지가 열립니다. 레코드 유형을 Workfront 개체와 연결할 때 조회 필드로 선택한 필드가 Workfront Planning 레코드 페이지에 표시됩니다.

   >[!TIP]
   >
   >* 여러 레코드 허용 설정을 사용하면 조회 필드 값이 쉼표로 구분되어 표시되거나 선택한 집계기에 따라 집계됩니다.
   >
   >* Workfront의 연결된 Workfront 개체에 대해 연결된 레코드 필드가 만들어지지 않습니다.

1. (선택 사항) Workfront에서 연결된 Workfront 개체를 열려면 **소스로 이동** Workfront 개체의 레코드 페이지의 오른쪽 상단 모서리에서 참조할 수 있습니다.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   적어도 개체를 볼 수 있는 보기 권한이 있는 경우 Workfront 개체 페이지가 열립니다. 권한이 있는 경우 Workfront 개체에 대한 정보를 편집할 수 있습니다.

1. (선택 사항) 레코드 유형의 테이블 보기에서 연결된 Workfront 개체의 열 헤더를 마우스로 가리킨 다음 드롭다운 메뉴를 클릭한 다음 **조회 필드 편집**.

1. 에서 Workfront 개체 필드 추가 **선택하지 않은 필드** 영역

   또는

   에서 Workfront 개체 필드 제거 **선택된 필드** 영역입니다.

   이렇게 하면 Workfront Planning 레코드에서 연결된 필드가 추가되거나 제거됩니다. 제거된 필드와 관련된 정보는 Workfront에 남아 있습니다.


### Workfront Planning 레코드를 Adobe Experience Manager 객체에 연결

<!--when we will have more applications to link to from Maestro, change the title to something like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>Adobe Experience Manager Assets 라이선스가 있어야 하며, Workfront Planning 레코드를 Adobe Experience Manager Assets에 연결하려면 조직의 Workfront 인스턴스가 Adobe 비즈니스 플랫폼 또는 Adobe Admin Console에 온보딩되어야 합니다.
>
>Adobe Admin Console 온보딩에 대한 질문이 있는 경우 [통합 경험 FAQ Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

레코드 종류와 Adobe Experience Manager Assets 간에 연결을 만들면 개별 레코드를 Experience Manager 에셋에 연결할 수 있습니다. 연결을 만들 때 Experience Manager Assets에서 연결한 에셋 필드는 연결한 레코드 종류에 자동으로 채워집니다.

{{step1-to-maestro}}

기본적으로 마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 레코드를 연결할 작업 영역을 선택합니다.
1. 레코드 유형의 카드를 클릭하여 레코드 유형 페이지를 엽니다.
1. 선택 **표** 다음에서 보기 **보기** 레코드 유형 페이지의 오른쪽 위 모서리에 있는 드롭다운 메뉴.

1. (선택 사항) **새 레코드** 선택한 레코드 유형에 새 레코드를 추가합니다. 자세한 내용은 [레코드 만들기](../../maestro/records/create-records.md).
1. (조건부) 선택한 레코드 종류를 Experience Manager Assets에 연결한 후 연결된 개체 열로 이동하여 Experience Manager의 다른 개체와 연결할 레코드에 해당하는 셀을 마우스로 가리킨 다음 **+** 아이콘.

   >[!TIP]
   >
   >  다음을 추가할 수 있습니다. **+** 레코드 페이지의 연결된 개체 필드에 있는 아이콘으로 자산을 레코드에 연결합니다.

   다음 **에셋 선택** 상자가 표시됩니다. <!--we might change this to Connect assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

1. 를 클릭하여 다음 유형의 자산 중 일부를 선택합니다.

   * 이미지
   * 폴더

   여러 자산을 선택할 수 있습니다.

   >[!IMPORTANT]
   >
   > Experience Manager에서 볼 수 있는 액세스 권한이 있는 에셋만 연결할 수 있습니다. 연결되면 모든 Workfront Planning 사용자는 Experience Manager Assets에서의 액세스 권한에 관계없이 Workfront Planning에서 에셋을 볼 수 있습니다.

1. 클릭 **선택**. <!-- we might change this to Connect-->

   다음이 추가됩니다.

   * 선택한 Experience Manager 에셋이 연결된 레코드 필드에 추가됩니다.
   * 연결된 필드(또는 조회 필드)는 Experience Manager 연결된 자산의 정보로 채워집니다.

     Experience Manager 에셋 필드의 기존 정보는 연결된 필드 또는 조회 필드에 자동으로 표시됩니다.

     >[!TIP]
     >
     >* 복수 레코드 허용 설정을 활성화한 경우 선택한 집계기에 따라 여러 객체 값이 쉼표로 구분되거나 집계되어 표시됩니다.
     >
     >* Workfront Planning 연결 레코드에 대한 연결된 레코드 필드는 Experience Manager Assets 애플리케이션에서 연결된 Experience Manager 자산에 대해 생성되지 않습니다.

1. (선택 사항) Experience Manager Assets에 연결한 레코드 유형으로 이동하고 연결된 레코드 필드에서 에셋의 이름을 클릭합니다. 에셋의 Experience Manager 세부 정보가 팝업 창에 표시됩니다. <!--update screen shot with hi-rez picture-->

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

1. (선택 사항) Experience Manager에서 에셋 레코드 Experience Manager 페이지를 열려면 연결하려는 레코드의 레코드 유형 페이지로 이동하고 연결된 레코드 필드에서 에셋 이름을 클릭하여 팝업 창을 연 다음 **열기** 아이콘 ![](assets/open-asset-icon.png) 를 클릭하여 자산을 엽니다.

   이렇게 하면 Adobe Experience Manager Assets에서 Experience Manager 에셋이 열립니다.

1. (선택 사항) 레코드 유형의 테이블 보기에서 연결된 Experience Manager 에셋의 열 헤더 위로 마우스를 가져간 다음 드롭다운 메뉴를 클릭하고 **조회 필드 편집**.

1. 에서 Experience Manager Assets 개체 필드 추가 **선택하지 않은 필드** 영역

   또는

   에서 Workfront 개체 필드 제거 **선택된 필드** 영역입니다.

   이렇게 하면 레코드에서 연결된 필드가 추가되거나 제거됩니다. 제거된 필드와 관련된 정보는 Experience Assets Adobe에 유지됩니다.

## Workfront 개체에서 레코드 연결

Workfront 객체에서 Workfront Planning 레코드를 연결하려면 다음이 있어야 합니다.

* 레코드 유형과 Workfront 객체 유형 간의 연결입니다.
* 레코드와 Workfront 개체 간 최소 하나 이상의 연결.
* Workfront 또는 그룹 관리자는 Planning 레코드 유형에 연결할 수 있는 Workfront 객체 유형에 Planning 섹션을 추가해야 합니다.

자세한 내용은 [Adobe Workfront 오브젝트의 계획 섹션에서 레코드 관리](/help/quicksilver/maestro/records/manage-records-in-planning-section.md).
