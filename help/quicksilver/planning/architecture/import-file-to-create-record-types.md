---
title: CSV 또는 Excel 파일에서 정보를 가져와 레코드 유형 만들기
description: 레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 CSV 또는 Excel 파일에서 정보를 가져와서 조직의 라이프사이클에 필요한 작업 항목을 설명하는 사용자 정의 레코드 유형을 만들 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# CSV 또는 Excel 파일에서 정보를 가져와서 레코드 유형 만들기

<span class="preview">이 페이지의 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 모든 고객을 위한 미리보기 환경에서만 사용할 수 있습니다. 월별 프로덕션 릴리스 이후 빠른 릴리스를 활성화한 고객을 위해 프로덕션 환경에서도 동일한 기능을 사용할 수 있습니다. </span>

<span class="preview">빠른 릴리스에 대한 자세한 내용은 [조직의 빠른 릴리스 사용 또는 사용 안 함](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)을 참조하세요. </span>

{{planning-important-intro}}

레코드 유형은 Adobe Workfront Planning의 객체 유형입니다. Workfront Planning에서 CSV 또는 Excel 파일에서 정보를 가져와서 조직의 라이프사이클에 필요한 작업 항목을 설명하는 사용자 정의 레코드 유형을 만들 수 있습니다.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다.

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
<p>Workfront Planning에 액세스하려면 조직의 Workfront 인스턴스가 Adobe 통합 경험에 온보딩되어야 합니다.</p> 
<p>자세한 내용은 <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront용 Adobe 통합 환경</a>을 참조하십시오. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이센스*</p></td> 
   <td><p> 표준</p>
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
   <td>   <p>작업 영역</a>에 대한 권한 관리 </p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>

</tbody> 
</table>

*Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++


## Excel 또는 CSV 파일을 사용하여 레코드 유형 가져오기에 대한 고려 사항

* Excel 파일의 각 시트는 레코드 유형이 됩니다. 시트의 이름은 레코드 유형의 이름이 됩니다.
* 시트가 한 개만 있거나 CSV 파일을 가져오는 경우, 파일의 이름은 레코드 유형의 이름이 됩니다.
* 각 시트의 열 머리글은 각 레코드 유형과 연결된 필드가 됩니다.
* 필드는 해당 레코드 유형에 대해 고유합니다.
* 각 시트의 각 행은 해당 레코드 유형과 연관된 고유한 레코드가 됩니다.
* Excel 파일의 각 시트는 다음을 초과할 수 없습니다.
   * 25,000행
   * 500열
* 파일은 5MB보다 크지 않아야 합니다.
* 빈 시트는 지원되지 않습니다.
* 다음 유형의 필드는 지원되지 않으며 가져오기 시트의 필드에 매핑할 수 없습니다.

   * Workfront 및 AEM Assets 개체 유형에 대한 연결 필드입니다.
   * 연결된 Planning 레코드 또는 Workfront 및 AEM Assets 개체의 조회 필드
   * 공식 필드
   * 만든 날짜, 만든 사람
   * 마지막 수정 날짜, 마지막 수정자
   * <span class="preview">승인 날짜, 승인자</span>
   * 사용자

Excel 또는 CSV 파일을 사용하여 레코드 유형을 가져오려면 다음을 수행합니다.

{{step1-to-planning}}

1. 레코드 유형을 만들 작업 영역을 클릭합니다.

   또는

   작업 영역에서 기존 작업 영역 이름의 오른쪽에 있는 아래쪽 방향 화살표를 확장하고 작업 영역을 검색한 다음 목록에 표시될 때 선택합니다.
1. **레코드 종류 추가**&#x200B;를 클릭합니다.
1. **파일에서 업로드**&#x200B;를 클릭합니다.
1. 이전에 컴퓨터에 저장한 Excel 또는 CSV 파일을 끌어서 놓거나 **CSV 또는 Excel 파일 선택**&#x200B;을 클릭하여 찾은 다음 선택합니다.
1. **미리 보기 및 편집**&#x200B;을 클릭합니다.

   **미리 보기 및 편집** 상자에 다음 정보가 표시됩니다.

   * 시트 이름 또는 이후 레코드 유형이 왼쪽 패널에 표시됩니다. Workfront Planning에서는 기본적으로 각 새 레코드 유형에 대해 아이콘과 색상을 선택합니다.
   * 첫 번째 시트 또는 레코드 유형이 선택되고 연관된 필드의 이름이 열 머리글로 표시됩니다. 각 필드의 유형은 기본적으로 선택됩니다.
   * 각 행은 새 레코드를 나타냅니다. 처음 10개의 레코드만 [미리 보기 및 편집] 상자에 표시됩니다.

   ![미리 보기 및 편집 상자](assets/preview-and-edit-box.png)

1. (선택 사항) 왼쪽 패널에서 각 시트의 이름을 클릭하여 포함된 정보를 검토합니다.

   >[!NOTE]
   >
   >비어 있는 시트는 지원되지 않으며 흐리게 표시됩니다.

1. (선택 사항) 왼쪽 패널에서 가져오지 않을 시트는 선택 취소합니다.

   ![선택하지 않은 상태로 가져올 시트 선택](assets/select-sheets-to-import-drop-down-with-unselected.png)

   선택을 취소한 시트는 회색 배경과 함께 표시됩니다.

1. (선택 사항) 열 머리글 오른쪽의 아래쪽 화살표를 클릭하여 **필드** 탭에서 다음 중 하나를 수행합니다.

   레코드 종류 매핑 가져오기 상자의 ![필드 탭](assets/field-tab-on-record-type-import-mapping-box.png)

   * 필드 중 하나의 이름을 변경합니다
   * **필드 형식** 변경
   * 필드 **설명** 업데이트

1. (선택 사항) 열의 정보를 다른 레코드 종류의 연결된 필드에 매핑하려면 **연결** 탭을 클릭합니다.

   ![레코드 종류 가져오기 매핑 상자의 연결 탭](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >Workfront Planning 연결된 레코드의 필드에만 매핑할 수 있습니다. Workfront 또는 AEM Assets 연결의 필드에 매핑할 수 없습니다. 자세한 내용은 이 문서의 [Excel 또는 CSV 파일을 사용하여 레코드 형식을 가져오는 데 대한 고려 사항](#considerations-about-importing-record-types-using-an-excel-or-csv-file) 섹션을 참조하십시오.

1. (조건부) 필드에 대한 정보를 업데이트한 후 **저장**&#x200B;을 클릭합니다.

1. 파일을 가져올 준비가 되면 **가져오기**&#x200B;를 클릭합니다.

   다음 정보는에서 Workfront Planning으로 가져옵니다.

   * 새 레코드 유형
   * 각 레코드 유형과 연결된 새 필드
   * 각 레코드 유형과 연결된 새 레코드

   레코드 유형 페이지에서 필드 및 레코드 관리를 시작할 수 있습니다.

   이제 Workfront Planning 및 작업 영역에 대한 액세스 권한이 있는 모든 사람이 가져온 레코드 유형 및 해당 정보를 보고 편집할 수 있습니다.
