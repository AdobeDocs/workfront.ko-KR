---
title: 레코드 편집
description: Adobe Workfront 계획 기능에서 레코드 정보를 편집할 수 있습니다. 레코드 만들기 및 편집을 시작하려면 먼저 레코드 유형을 만들어야 합니다.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# 레코드 편집

{{maestro-important-intro}}

레코드와 연결된 필드의 값을 편집하여 Adobe Workfront 계획 기능에서 레코드 정보를 편집할 수 있습니다.

레코드 만들기 및 편집을 시작하려면 먼저 레코드 유형을 만들어야 합니다.

자세한 내용은 [레코드 유형 만들기](../architecture/create-record-types.md).

레코드 만들기에 대한 자세한 내용은 [레코드 만들기](/help/quicksilver/maestro/records/create-records.md).

&lt;!— 여기에서 세부 사항 보기의 필드가 표 보기의 필드와 동일하다고 언급하십시오. 이 문서는 레코드 관리 보기에서 연결되어 이 정보를 참조합니다—>

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
<td>
   <p> 제품</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 계약</p></td>
   <td>
<p>Adobe Workfront 계획 기능 비공개 베타 프로그램에 조직을 등록해야 합니다. 이 새 제품에 대해 문의하려면 계정 담당자에게 문의하십시오. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 플랜</p></td>
   <td>
<p>임의</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td>
   <td>
   <p>새로운 기능: 밝게 또는 높음</p>
   또는
   <p>현재: 작업 시간 이상</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>액세스 수준 구성</p></td>
   <td> <p>Adobe Workfront 계획 기능에 대한 액세스 제어가 없습니다 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>권한</p></td>
   <td> <p>작업 영역에 대한 상위 권한 기여</a> </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>레이아웃 템플릿</p></td>
   <td> <p>Workfront 또는 그룹 관리자는 레이아웃 템플릿에 마에스트로 영역을 추가해야 합니다. 자세한 내용은 <a href="../access/access-overview.md">액세스 개요</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 레코드 편집에 대한 고려 사항

* 작업 영역에 대한 권한이 부여된 경우 직접 만든 레코드나 다른 사용자가 만든 레코드를 편집할 수 있습니다.
* 다음 영역에서 레코드 필드를 편집할 수 있습니다.

   * 레코드 보기에서 레코드의 세부 정보 상자.
   * 레코드의 세부 정보 페이지입니다.
   * 테이블 보기에서 인라인입니다.

* 다음 유형의 필드는 자동으로 업데이트되며, 해당 값을 수동으로 편집할 수 없습니다.
   * 다른 레코드의 연결된 필드
   * 공식 유형 필드
   * 시스템 필드(생성자, 생성일, 마지막 수정자, 마지막 수정일)
* 표시되는 레코드가 다른 레코드에 연결되어 있는 경우 편집 중인 레코드의 새 정보가 연결된 레코드에 반영됩니다.
* 레코드를 일괄적으로 편집할 수 없습니다. <!--this will probably change-->
* URL은 http://, https://, ftp:// 또는 www로 시작하는 경우에만 한 줄 텍스트 필드 유형에서 링크로 인식됩니다. .

## 레코드 편집

다음 영역에서 레코드를 편집할 수 있습니다.

* [레코드 유형의 테이블 보기에서](#edit-a-record-from-the-table-view-of-a-record-type)
* [레코드의 세부 정보 페이지에서](#edit-a-record-from-the-records-details-page)

### 레코드 유형의 표 보기에서 인라인 레코드 편집

{#step1-to-maestro}

마지막으로 액세스한 작업 영역이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.
1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.
1. (조건부) 테이블 보기의 탭을 클릭하거나 **+ 보기** 테이블 뷰를 생성합니다. 마지막으로 액세스할 때 다른 유형의 보기에서 레코드 유형을 보지 않은 경우 테이블 보기는 기본 보기여야 합니다.

   선택한 레코드 유형과 연관된 레코드가 테이블 뷰에 표시됩니다.
1. 레코드 행 내부를 클릭하여 인라인 레코드에 대한 정보 편집을 시작합니다.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!NOTE]
   >
   >  다음 필드는 읽기 전용이고 Workfront에서 자동으로 업데이트하므로 해당 필드에 대한 정보는 편집할 수 없습니다.
   >  
   >  * 레코드 종류를 연결하여 만든 연결된 필드. 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).
   >  * 생성자, 생성일, 마지막 수정자, 마지막 수정일, 공식 필드 유형의 필드.

1. (선택 사항 및 조건부) 단락 유형 필드를 편집할 때 다음을 사용합니다 **리치 텍스트** 서식 옵션:

   * 볼드체
   * 이탤릭체
   * 밑줄
   * 링크 추가
   * 글머리 기호 목록 추가
   * 번호 매기기 목록 추가

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (선택 사항) 연결된 레코드 필드를 두 번 클릭하여 연결된 레코드나 개체를 다른 레코드에 추가합니다. 자세한 내용은 [레코드 연결](/help/quicksilver/maestro/records/connect-records.md).
1. 누르기 **입력** 키보드에서 를 클릭하거나 행 외부를 클릭하여 변경 내용을 저장합니다. 변경 사항은 자동으로 저장됩니다. A **저장됨** 변경 사항이 저장되었음을 보여 주는 표시기가 표 보기의 오른쪽 위 모서리에 잠시 표시됩니다.


1. (선택 사항) 한 필드에서 다른 필드로 정보를 복사하여 붙여넣으려면 다음 중 하나를 수행합니다.

   * 필드의 기존 값을 하나 이상 복사한 다음 다른 레코드의 같은 유형의 필드에 붙여 넣습니다.
   * 열의 열 헤더를 클릭하여 선택하고 복사한 다음 다른 열의 열 헤더를 클릭하고 복사한 열의 내용을 붙여넣습니다. 열에는 유사한 필드 유형이 포함되어야 합니다.
   * Shift 키를 누른 상태에서 을 클릭하여 테이블의 여러 행을 선택하고 선택한 행의 정보를 복사한 다음 다른 행을 클릭하고 선택한 정보를 새 행 및 그 다음 행에 붙여넣습니다.

   >[!NOTE]
   >
   >다음 사항을 고려하십시오.
   >
   >* 정보를 복사하고 붙여넣으려면 다음 키보드 단축키를 사용하십시오.
   >   * 복사: CTRL + C (Mac의 경우 ⌘ + C)
   >   * 붙여넣기: CTRL + V(Mac의 경우 ⌘ + V)
   >* 정보를 붙여넣은 필드와 같은 유형의 레코드 필드 이외의 다른 소스에서 정보를 복사할 수 없습니다.
   >
   >* 레코드의 세부 정보 영역에는 필드 값을 복사하여 붙여넣을 수 없습니다. 이 기능은 레코드 종류의 표 보기에서만 지원됩니다.
   >* 다음 필드 유형에 대한 필드 값을 복사하여 붙여넣을 수 없습니다.
   >
   >
   >    * 레코드 종류를 연결하여 만든 연결된 필드. 연결된 레코드 필드를 복사하여 붙여 넣을 수 있습니다. 자세한 내용은 [레코드 유형 연결](../architecture/connect-record-types.md).
   >    * 생성자, 생성일, 마지막 수정자, 마지막 수정자 유형의 필드

1. (선택 사항) 다음 키보드 단축키를 사용하여 레코드 정보 편집 또는 복사 및 붙여넣기를 실행 취소하거나 재실행할 수 있습니다.

   * CTRL+Z(Mac의 경우 ⌘+Z)
   * 변경 내용을 재실행하려면 CTRL+Shift+Z(Mac의 경우 ⌘+Shift+Z)

   >[!TIP]
   >
   >    키보드 단축키를 한 번에 여러 번 사용하여 여러 변경 내용을 실행 취소할 수 있습니다.

1. (선택 사항) 레코드에 썸네일을 추가합니다. 자세한 내용은 [레코드에 썸네일 추가](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### 보기의 기록 세부 정보 상자에서 레코드 편집

모든 보기의 세부 정보 상자에서 레코드를 편집할 수 있습니다.

{{step1-to-maestro}}

마지막으로 액세스한 작업공간이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 모든 유형의 보기에서 레코드 이름을 클릭합니다

   또는

   테이블 테이블 보기에서 **세부 정보 열기** 아이콘 ![](assets/open-details-icon-in-table-name-field.png) 레코드 이름의 왼쪽에 있거나 레코드 이름을 클릭합니다. 다음 **세부 사항** 상자가 뷰에 열립니다.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >다음을 볼 수 있습니다. **세부 정보 열기** 테이블 보기에서 레코드의 이름 필드 왼쪽에 있는 아이콘은 이름 필드가 기본 필드인 경우에만 해당됩니다.

1. 에서 필드 정보 편집을 시작합니다. **세부 사항** 상자. Workfront은 변경 사항을 자동으로 저장합니다.

1. (선택 사항) **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 의 오른쪽 위 모서리 **세부 사항** 레코드를 여는 상자 **세부 사항** 새 탭에서 페이지를 만듭니다. 에 설명된 대로 레코드를 계속 편집합니다. [레코드의 세부 정보 페이지에서 레코드 편집](#edit-a-record-from-the-records-details-page) 이 문서의 섹션.

### 레코드의 세부 정보 페이지에서 레코드 편집

세부 정보 페이지에서 레코드를 편집할 수 있습니다.

{{step1-to-maestro}}

마지막으로 액세스한 작업공간이 열립니다.

1. (선택 사항) 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 클릭하여 레코드를 업데이트할 작업 영역을 선택합니다.

1. 레코드 유형 카드를 클릭합니다.

   레코드 유형 페이지가 열립니다.

1. 다음 중 하나를 수행하십시오.

   * 모든 보기에서 다음에 설명된 대로 세부 정보 상자에 액세스합니다. [보기의 기록 세부 정보 상자에서 레코드 편집](#edit-a-record-from-the-records-details-box-in-a-view)이 문서의 섹션. 그런 다음 **새 탭에서 열기** 아이콘 ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> 의 오른쪽 위 모서리 **세부 사항** 레코드를 여는 상자 **세부 사항** 새 탭에서 페이지를 만듭니다.

   * 다음에서 **표** 보기, 레코드 이름 위로 마우스를 가져간 다음 **자세히** 메뉴 ![](assets/more-menu.png)을 클릭한 다음 을 클릭합니다 **보기**

     ![](assets/contextual-menu-for-record-row.png)

     레코드 **세부 사항** 페이지가 열립니다.

     ![](assets/details-page.png)

1. 다음을 클릭합니다. **자세히** 메뉴 ![](assets/more-menu.png) 레코드 이름 오른쪽에서 **편집**

   또는

   세부 정보 페이지의 편집 가능한 필드 내부를 클릭하여 정보를 편집합니다.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. 클릭 **변경 내용 저장**.