---
title: 사용자 정의 양식 만들기
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 양식 디자이너를 사용하여 사용자 정의 양식을 디자인할 수 있습니다. 다른 Workfront 개체에 사용자 정의 양식을 첨부하여 해당 개체에 대한 데이터를 캡처할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: b95d536bc251c2575b105f38691a66bde67502b8
workflow-type: tm+mt
source-wordcount: '6589'
ht-degree: 5%

---

# 사용자 정의 양식 만들기

<!-- Audited: 6/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->

Adobe Workfront에서 양식 디자이너를 사용하여 사용자 정의 양식을 디자인할 수 있습니다. 다른 Workfront 개체에 사용자 정의 양식을 첨부하여 해당 개체에 대한 데이터를 캡처할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>새로운 기능: 표준</p>
   <p>또는</p>
   <p>현재: 플랜</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> </td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자 정의 양식 디자인 시작

{{step-1-to-setup}}

1. 왼쪽 패널에서 **사용자 지정 Forms**&#x200B;을 클릭한 다음 **Forms**&#x200B;을(를) 선택합니다.

1. **새 사용자 정의 양식을 클릭합니다.**
1. 사용자 정의 양식을 첨부할 개체 유형을 선택한 다음 **계속**&#x200B;을 클릭합니다.

   ![개체 유형 선택](assets/choose-object-type.jpg)

1. **양식 이름 추가** 영역에 사용자 지정 양식 제목을 입력합니다.
1. (선택 사항) 더 많은 개체에 첨부할 수 있도록 양식에 더 많은 개체 형식을 추가하려면 **개체 형식** 옆에 있는 ![추가](assets/add-objects-icon.png) 아이콘 **개체 추가 아이콘**&#x200B;을 클릭한 다음 표시되는 메뉴에서 원하는 형식을 선택합니다. 이 단계를 반복하여 원하는 만큼 객체 유형을 추가할 수 있습니다.

   양식에 두 개 이상의 개체가 추가되면 개체 유형에서 X를 클릭하여 양식에서 삭제할 수 있습니다.

   >[!CAUTION]
   >
   >사용자 정의 양식을 삭제하면 해당 양식과 관련된 오브젝트의 모든 사용자 정의 데이터도 삭제됩니다. 삭제된 데이터는 복구할 수 없습니다. 또는 더 이상 사용하지 않는 사용자 정의 양식을 비활성화하여 연결된 모든 내역 데이터를 유지할 수 있습니다.
   >
   >자세한 내용은 [기존 사용자 정의 양식에서 개체 형식 추가 또는 삭제](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) 및 [사용자 정의 양식 비활성화 또는 다시 활성화](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md)를 참조하십시오.


1. 그런 다음 사용자 정의 양식에 필드를 추가할 수 있습니다. 자세한 내용은 다음 섹션을 참조하십시오.
   * [다른 사용자 정의 양식에서 이미 사용된 기존 필드 또는 위젯 재사용](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [필드 이름 및 레이블에 대한 참고 사항](#notes-on-field-names-and-labels)
   * [텍스트 필드 추가](#add-text-fields)
   * [계산된 필드 추가](#add-calculated-fields)
   * [라디오 버튼, 확인란 그룹 및 드롭다운 추가](#add-radio-buttons-checkbox-groups-and-drop-downs)
   * [자동 완성 및 날짜 필드 추가](#add-typeahead-and-date-fields)
   * [외부 조회 필드 추가](#add-external-lookup-fields)
   * [이미지, PDF 및 비디오 추가](#add-images-pdfs-and-videos)
   * [Workfront 기본 필드 추가](#add-workfront-native-fields)
   * [Adobe XD 파일 추가](#add-adobe-xd-files)
   * [Planning 연결 필드 추가](#add-planning-connection-fields)

## 사용자 정의 양식에 새 필드 또는 기존 필드 추가

사용자 정의 양식을 디자인할 때 새 필드 또는 기존 필드를 사용할 수 있습니다.

사용자 정의 양식은 500개의 필드로 제한됩니다. 왼쪽 하단의 카운터는 폼에 사용되는 필드 수를 표시하며 폼 디자이너 내에서 스크롤할 때 항상 표시됩니다.

### 다른 사용자 정의 양식에서 이미 사용된 기존 필드 또는 위젯 재사용

1. 화면 왼쪽 상단에서 **필드 라이브러리**&#x200B;를 클릭합니다.

1. 원하는 필드 또는 위젯을 캔버스로 드래그하여 놓습니다. 다른 필드 또는 위젯을 추가하려면 이 단계를 반복합니다.

   >[!NOTE]
   >
   >단일 사용자 정의 양식에 최대 500개의 필드 및 위젯을 추가할 수 있습니다. 그러나 형식에 복잡성에 따라 100개가 넘는 값이 있을 경우 성능이 저하될 수 있습니다.
   >
   >
   >복잡한 양식의 예로는 계단식 매개 변수가 있는 양식, 계산된 사용자 정의 데이터 필드 및 단일 필드의 여러 값 옵션이 있습니다.

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

### 필드 이름 및 레이블에 대한 참고 사항 {#notes-on-field-names-and-labels}

레이블은 대부분의 필드에 사용할 수 있습니다. 사용자 정의 양식의 필드 또는 위젯 위에 표시되는 설명 레이블입니다. 언제든지 레이블을 변경할 수 있습니다.

>[!NOTE]
>
>보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오.

모든 필드에는 이름이 필요합니다. 이 이름은 보고서, 홈 및 API 상호 작용과 같은 Workfront 전체의 다양한 영역에 사용자 정의 필드를 추가할 때 시스템이 이 필드를 식별하는 방법입니다. 필드나 위젯을 처음 구성할 때 레이블을 입력하면 이름 필드가 자동으로 채워져 일치합니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.

각 사용자 정의 필드 이름은 조직의 Workfront 인스턴스에서 고유해야 합니다. 이렇게 하면 다른 사용자 정의 양식에 대해 이미 만들어진 파일을 다시 사용할 수 있습니다.

>[!NOTE]
>
>그렇게 할 수도 있지만 본인이나 다른 사용자가 Workfront에서 사용자 정의 양식을 사용하기 시작한 후에는 이 이름을 변경하지 않는 것이 좋습니다. 이 필드를 선택하면 이제 Workfront의 다른 영역에서 참조될 수 있는 사용자 지정 필드가 시스템에서 더 이상 인식되지 않습니다.
>&#x200B;>예를 들어 사용자 지정 필드를 보고서에 추가하고 나중에 이름을 변경하면 Workfront은 보고서에서 이를 인식하지 못하며 새 이름을 사용하여 보고서에 다시 추가하지 않으면 제대로 작동하지 않습니다.
>
>기본 제공 Workfront 필드에 이미 사용된 이름은 입력하지 않는 것이 좋습니다.
>
>Workfront의 다른 영역에서 필드를 사용할 때 오류를 방지하기 위해 사용자 지정 필드 이름에 마침표/점 문자를 사용하지 않는 것이 좋습니다.

사용자 정의 필드 레이블 및 이름에서는 다음 특수 문자가 지원되지 않습니다.

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* :
* `{`
* `}`

### 텍스트 필드 추가

사용자 정의 양식에 여러 개의 다른 텍스트 필드를 추가할 수 있습니다.

+++ 를 확장하여 사용 가능한 텍스트 필드에 대한 설명을 확인합니다.

* **한 줄 텍스트 필드**: 사용자가 필드에 한 줄 텍스트를 입력할 수 있습니다.
* **단락 필드**: 사용자가 필드에 여러 줄의 텍스트를 입력할 수 있습니다.
* **서식 있는 텍스트 필드**: 필드에 여러 줄의 텍스트를 입력하고 굵게, 기울임꼴, 밑줄, 글머리 기호, 번호 매기기, 하이퍼링크 및 블록 따옴표로 텍스트 서식을 지정할 수 있습니다. 문자 길이는 15,000자로 제한되어 있어 많은 텍스트와 서식을 사용할 수 있습니다.

  이 사용자 정의 필드 유형은 목록 및 보고서의 필터에서 지원되지 않습니다.

  API를 통해 이 필드에 액세스하는 방법에 대한 자세한 내용은 [API의 서식 있는 텍스트 필드 저장소](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md)를 참조하십시오.

  >[!NOTE]
  >
  >Workfront 모바일 앱에서는 서식이 있는 텍스트 필드를 사용할 수 없습니다(향후 릴리스에서 사용 가능).

* **설명 텍스트**: 지침을 포함하고 Workfront 외부의 페이지에 연결할 수 있습니다.

+++

텍스트 필드를 추가하려면:

1. 화면 왼쪽의 **새 필드** 탭에서 다음 텍스트 필드 중 하나를 찾아 캔버스의 섹션으로 끌어서 놓습니다.

   * 한 줄 텍스트
   * 단락
   * 서식 포함 텍스트
   * 설명 텍스트

   ![필드를 섹션으로 드래그](assets/drag-field-to-section.png)

1. 화면 오른쪽에서 추가하려는 사용자 정의 필드 유형에 사용할 수 있는 옵션을 구성합니다.

   <table>
    <tr>
    <td>에 입력</td>
    <td>설명</td>
    <td>다음에 사용 가능: </td>
    </tr>
    <tr>
    <td>크기</td>
    <td><p>(선택 사항) 양식의 텍스트 필드 크기를 변경합니다.<p>
   </td>
    <td><ul>
    <li>한 줄 텍스트</li>
    <li>단락</li>
    <li>서식 포함 텍스트</li>
    <li>설명 텍스트</li>
    </ul></td>
    </tr>
    <tr>
    <td>레이블</td>
    <td><p>(필수) 필드 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.<p>
    <p><b>중요</b>: 보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오. 자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p></td>
    <td><ul>
    <li>한 줄 텍스트</li>
    <li>단락</li>
    <li>서식 포함 텍스트</li>
    </ul></td>
    </tr>
    <tr>
     <td>이름</td>
    <td><p>(필수) 이 이름은 시스템이 필드를 식별하는 방법입니다. 위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.</p>
    <p>자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p>
    </td>
    <td><ul>
    <li>한 줄 텍스트</li>
    <li>단락</li>
    <li>서식 포함 텍스트</li>
    <li>설명 텍스트</li>
    </ul></td>
    </tr>
    <tr>
    <td>지침</td>
    <td>필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>한 줄 텍스트</li>
    <li>단락</li>
    <li>서식 포함 텍스트</li>
    </ul></td>
    </tr>
    <tr>
    <td>형식</td>
    <td><p>사용자 정의 필드에 캡처할 데이터 유형을 선택합니다.</p> <p><b>참고</b>:   
    <ul> 
    <li>양식을 저장한 후에는 이 필드를 편집할 수 없습니다. 수학 계산에서 필드를 사용하려면 숫자 또는 통화 형식을 선택해야 합니다.</li> 
    <li>숫자 또는 통화를 선택하면 0으로 시작하는 숫자가 자동으로 잘립니다.</li>
    <li>숫자 필드의 문자 길이는 16자로 제한됩니다. 텍스트 필드를 사용하여 숫자를 입력하고 제한을 피할 수도 있습니다.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>한 줄 텍스트</li>
    <li>단락</li>
    </ul></td>
    </tr>
    <tr>
    <td>표시 유형</td>
    <td>한 줄과 단락 텍스트 필드 간에 전환합니다.</td>
    <td><ul>
    <li>한 줄 텍스트</li>
    <li>단락</li>
    </ul></td>
    </tr>
    <tr>
    <td>하이퍼링크</td>
    <td> 입력한 설명 텍스트에 하이퍼링크를 적용하려면 여기에 하이퍼링크를 추가합니다. 설명 텍스트는 양식이 첨부된 개체에 대한 링크로 표시됩니다.</td>
    <td><ul><li>설명 텍스트</li></ul></td>
    </tr>
    <tr> 
      <td role="rowheader">필수 필드 만들기</td>
      <td><p>사용자가 사용자 정의 양식을 작성하기 위해 필드를 요구하려면 이 옵션을 선택합니다.</p></td>
    <td><ul>
    <li>한 줄 텍스트</li>
    <li>단락</li>
    <li>서식 포함 텍스트</li>
    </ul></td> 
    </tr> 
   </table>

1. (선택 사항) 다른 필드 또는 위젯을 추가하려면 이전 단계를 반복합니다.

   또는

   필드를 복사하려면 필드 위로 마우스를 가져간 다음 복사 아이콘을 클릭합니다.

   ![복사 아이콘](assets/copy-field.png)

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

### 계산된 필드 추가

사용자 정의 양식에서 사용자 정의 양식을 오브젝트에 첨부할 때 기존 데이터를 사용하는 계산된 사용자 정의 필드를 추가하여 새 데이터를 생성할 수 있습니다.

계산된 필드를 추가하려면 [양식 디자이너를 사용하여 계산된 필드 추가](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)를 참조하십시오.

### 라디오 버튼, 확인란 그룹 및 드롭다운 추가

사용자 정의 양식에 라디오 버튼, 확인란 그룹, 드롭다운 및 다중 선택 드롭다운을 추가할 수 있습니다.

+++ 를 확장하여 사용 가능한 필드에 대한 설명을 확인합니다.

* **라디오 단추**: 사용자가 하나의 선택 항목만 선택해야 합니다.
* **확인란 그룹**: 사용자가 여러 개의 선택 항목을 선택할 수 있도록 허용합니다.
* **단일 선택 드롭다운**: 드롭다운 선택 항목 목록을 제공합니다.
* **다중 선택 드롭다운**: 사용자가 드롭다운 목록에서 여러 항목을 선택할 수 있습니다.

+++

>[!NOTE]
>
>확인란 그룹 및 다중 선택 드롭다운과 같이 여러 항목을 선택할 수 있는 필드는 보고서에서 차트 및 그룹화하기 어렵습니다. 보고서에서 차트 및 그룹화를 보다 쉽게 수행할 수 있도록 각 선택 항목에 대해 별도의 필드(예: 한 줄 텍스트 필드)를 만들 수 있습니다.

라디오 단추, 확인란 그룹 및 드롭다운을 추가하려면 다음을 수행합니다.

1. 화면 왼쪽의 **새 필드** 탭에서 다음 필드 중 하나를 찾아 캔버스의 섹션으로 끌어서 놓습니다.

   * 라디오 버튼
   * 확인란 그룹
   * 단일 선택 드롭다운
   * 다중 선택 드롭다운

   ![필드를 캔버스로 드래그](assets/drag-field-to-section.png)

1. 화면 오른쪽에서 추가하려는 사용자 정의 필드 유형에 사용할 수 있는 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>에 입력</td>
    <td>설명</td>
    <td>다음에 사용 가능: </td>
    </tr>
    <tr> 
     <td role="rowheader">레이블</td> 
     <td> <p>(필수) 사용자 정의 필드 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오. 자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td> 
     <td><ul>
    <li>라디오 버튼</li>
    <li>확인란 그룹</li>
    <li>단일 선택 드롭다운</li>
    <li>다중 선택 드롭다운</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">이름</td> 
     <td> <p>(필수) 이 이름은 시스템이 필드를 식별하는 방법입니다. 위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.</p> 
    <p>자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td>
     <td><ul>
    <li>라디오 버튼</li>
    <li>확인란 그룹</li>
    <li>단일 선택 드롭다운</li>
    <li>다중 선택 드롭다운</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">지침</td> 
    <td> <p>사용자 정의 필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>라디오 버튼</li>
    <li>확인란 그룹</li>
    <li>단일 선택 드롭다운</li>
    <li>다중 선택 드롭다운</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">형식</td> 
    <td> <p>사용자 정의 필드에 캡처할 데이터 유형을 선택합니다.</p> <p><b>참고</b>:   
     <ul> 
    <li>양식을 저장한 후에는 이 필드를 편집할 수 없습니다. 수학 계산에서 필드를 사용하려면 숫자 또는 통화 형식을 선택해야 합니다.<br></li> 
    <li>숫자 또는 통화를 선택하면 0으로 시작하는 숫자가 자동으로 잘립니다.</li>
    <li>숫자 필드의 문자 길이는 16자로 제한됩니다. 텍스트 필드를 사용하여 숫자를 입력하고 제한을 피할 수도 있습니다.</li>
     </ul></p></td> 
     <td><ul>
    <li>라디오 버튼</li>
    <li>확인란 그룹</li>
    <li>단일 선택 드롭다운</li>
    <li>다중 선택 드롭다운</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">표시 유형</td> 
    <td>라디오 버튼, 확인란 그룹, 단일 선택 드롭다운 또는 다중 선택 드롭다운 간 전환</td> 
    <td><ul>
    <li>라디오 버튼</li>
    <li>확인란 그룹</li>
    <li>단일 선택 드롭다운</li>
    <li>다중 선택 드롭다운</li>
    </ul></td>
    </tr> 
    <td role="rowheader">선택 항목 </td> 
    <td> 
    <p>다음 옵션 중 하나를 선택합니다.</p> 
    <ul> 
    <li><strong>값 표시</strong>: 필드에 있는 각 선택 값을 표시합니다. 각 선택 항목의 레이블은 기본적으로 표시됩니다.</li>
   <li><strong>선택 항목 정렬 A-Z</strong>: 필드에서 추가하는 선택 항목을 알파벳순으로 정렬합니다.</li>
    </ul>
     <p>사용자를 위해 추가하는 각 옵션에 대해 톱니바퀴 아이콘 <img src="assets/gear-icon-settings.png">을(를) 클릭한 후 다음 옵션 중 하나를 선택합니다.</p> 
    <ul> 
    <li><strong>기본적으로 선택</strong>: 필드에서 기본적으로 선택을 선택합니다.</li> 
    <li> <p><strong>선택 항목 숨기기</strong>: 필드에서 선택 항목을 숨깁니다. 숨겨진 선택 사항은 보고서에서 계속 액세스할 수 있습니다.</p> </li> 
    <li> <p><strong>선택 항목 제거</strong>: 필드에서 선택 항목을 제거합니다.</p> <p><b>경고</b>: 이 선택 항목을 사용하는 현재 개체가 있는 경우 필드에서 제거하지 마십시오. 삭제하면 내역 데이터가 손실됩니다. 대신 숨기려면 옵션을 선택합니다. 그러면 사용자가 나중에 선택할 수 없게 됩니다.</p> </li> 
    </ul>   
    <p><b>참고:</b> 선택할 수 있는 선택 항목 수에 제한이 없습니다. </p>    
    </td> 
    <td><ul>
    <li>라디오 버튼</li>
    <li>확인란 그룹</li>
    <li>단일 선택 드롭다운</li>
    <li>다중 선택 드롭다운</li>
    </ul>
    </td>
     </tr> 
          <tr> 
    <td role="rowheader">필수 필드 만들기</td> 
    <td>사용자가 사용자 정의 양식을 작성하기 위해 필드를 요구하려면 이 옵션을 선택합니다. </td> 
    <td><ul>
    <li>라디오 버튼</li>
    <li>확인란 그룹</li>
    <li>단일 선택 드롭다운</li>
    <li>다중 선택 드롭다운</li>
    </ul></td>
     </tr> 
    <tr> 
    </tbody> 
    </table>

1. (선택 사항) 다른 필드 또는 위젯을 추가하려면 이전 단계를 반복합니다.

   또는

   필드를 복사하려면 필드 위로 마우스를 가져간 다음 복사 아이콘을 클릭합니다.

   ![복사 아이콘](assets/copy-field.png)

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

### 자동 완성 및 날짜 필드 추가

자동 완성 및 날짜 필드를 사용자 정의 양식에 추가할 수 있습니다.

+++ 를 확장하여 사용 가능한 필드에 대한 설명을 확인합니다.

* **Typeahead**: 사용자가 Workfront에 있는 개체의 이름을 입력할 수 있습니다. 사용자가 입력을 시작하면 제안 목록이 나타납니다. 이 필드 유형은 다음 개체를 지원합니다.
   * 사용자
   * 그룹
   * 작업 역할
   * 포트폴리오
   * 프로그램
   * 프로젝트
   * 팀
   * 템플릿
   * 회사
* **날짜**: 사용자가 날짜 및 시간을 선택할 수 있는 달력을 표시합니다.

+++

자동 완성 및 날짜 필드를 추가하려면:

1. 화면 왼쪽의 **새 필드** 탭에서 다음 필드 중 하나를 찾아 캔버스의 섹션으로 끌어서 놓습니다.

   * 타이프 어헤드
   * 일자

   ![필드를 섹션으로 드래그](assets/drag-field-to-section.png)

1. 화면 오른쪽에서 추가하려는 사용자 정의 필드 유형에 사용할 수 있는 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>필드 설정</td>
    <td>설명</td>
    <td>다음에 사용 가능: </td>
    </tr>
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 사용자 정의 필드 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오. 자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td> 
       <td><ul>
    <li>타이프 어헤드</li>
    <li>일자</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 시스템이 필드를 식별하는 방법입니다. 위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.</p> 
      <p>자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td>
    <td><ul>
    <li>타이프 어헤드</li>
    <li>일자</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>사용자 정의 필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>타이프 어헤드</li>
    <li>일자</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">시간 표시(하루 기준)</td> 
      <td>필드에 날짜와 함께 시간을 표시하려면 이 옵션을 선택합니다.</td> 
         <td><ul>
    <li>일자</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">참조 오브젝트 유형</td> 
      <td> <p>필드와 연결할 객체 유형을 선택합니다.</p> <p><b>적용</b> 또는 <b>저장 및 닫기</b>를 클릭하면 필드의 개체 유형을 변경할 수 없습니다.</p> <p><b>참고</b>:   
        <ul> 
         <li>Workfront 관리자가 Workfront 사용자 인터페이스에서 포트폴리오, 프로그램 또는 프로젝트 이름을 사용자 지정한 경우 개체에 대한 기본 Workfront 이름이 사용자 지정한 이름이 아니라 이 드롭다운 목록에 표시됩니다. 이에 대한 도움이 필요한 경우 Workfront 관리자에게 문의하십시오.<br></li> 
         <li>iOS 및 Android Workfront Mobile 앱에서는 사용자, 회사, 그룹, 작업 역할, Portfolio, 프로그램, 프로젝트 및 템플릿과 같은 오브젝트 유형이 지원됩니다.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>타이프 어헤드</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">필터 추가</td>
      <td><p>사용자가 필드를 사용할 때 선택할 수 있는 개체를 제한하기 위해 개체 유형에 대한 필터를 추가합니다. </p> <p>예를 들어 사용자 이름이 다음 기준을 충족하는 경우에만 선택할 수 있도록 필드를 제한할 수 있습니다.</p> 
       <ul> 
        <li>지정한 그룹에 속합니다.</li> 
        <li>지정한 역할 또는 직위와 연결되어 있습니다.</li> 
        <li>필드를 사용하는 사용자와 동일한 그룹에 속합니다.</li> 
       </ul>
       <p>텍스트 모드 구문을 사용하여 선택한 객체 유형에 대한 필터를 정의해야 합니다. 텍스트 모드를 사용하여 필터를 만드는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">텍스트 모드를 사용하여 필터 편집</a>을 참조하십시오.</p>
       <p><b>팁:</b> 자동 완성 필드에 필터를 직접 추가하기 전에 필터를 테스트하는 보고서를 만들 수 있습니다. 이렇게 하면 필터가 올바른 개체를 반환하는지 확인하는 데 도움이 됩니다. 그런 다음 보고서에서 텍스트 모드로 전환하고 텍스트 모드 문을 복사하여 자동 완성 필터에 추가할 수 있습니다.</p>
       <p><b>참고</b>:
       <ul> 
        <li>기존 사용자 정의 양식을 편집하는 경우 자동 완성 필드에 필터를 추가해도 사용자가 필드를 사용하여 이미 추가한 오브젝트가 제거되지 않습니다(필터의 범위 외부).</li> 
        <li>모바일 장치에서는 이 필터를 사용할 수 없습니다. 자동 완성 필드에 필터를 사용하는 경우 해당 필드는 필터의 영향을 받지 않는 사용자의 모바일 장치에 표시됩니다.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>타이프 어헤드</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">필수 필드 만들기</td> 
      <td>사용자가 사용자 정의 양식을 작성하기 위해 필드를 요구하려면 이 옵션을 선택합니다. </td> 
       <td><ul>
    <li>타이프 어헤드</li>
    <li>일자</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 다른 필드 또는 위젯을 추가하려면 이전 단계를 반복합니다.

   또는

   필드를 복사하려면 필드 위로 마우스를 가져간 다음 복사 아이콘을 클릭합니다.

   ![복사 아이콘](assets/copy-field.png)

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

### 외부 조회 필드 추가

외부 조회 필드는 외부 API를 호출하고 드롭다운 필드에 값을 옵션으로 반환합니다. 사용자 정의 양식이 첨부된 오브젝트로 작업하는 사용자는 드롭다운에서 이러한 옵션 중 하나 이상을 선택할 수 있습니다. 외부 조회 필드는 목록 및 보고서에서도 사용할 수 있습니다.

외부 조회 필드를 사용하여 Workfront 또는 공개 API의 동일한 인스턴스를 호출하는 예제는 [사용자 지정 양식의 외부 조회 필드 예제](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)를 참조하십시오.

>[!NOTE]
>
>* 외부 조회 필드는 Outlook 플러그인에서 지원되지 않습니다.
>* 필드가 다른 필드에 종속된 경우 목록에서 외부 조회 필드를 사용할 수 없습니다.

외부 조회를 추가하려면:

1. 화면 왼쪽의 **새 필드** 탭에서 **외부 조회**&#x200B;를 찾아 캔버스의 섹션으로 끕니다.
1. 화면 오른쪽에서 사용자 정의 필드에 대한 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 사용자 정의 필드 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오. 자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 시스템이 필드를 식별하는 방법입니다. 위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 그러나 레이블 및 이름 필드는 동기화되지 않으므로 시스템에 표시되는 이름을 변경하지 않고도 사용자가 볼 수 있는 레이블을 변경할 수 있습니다.</p>
      <p>자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td>
     </tr> 
      <td role="rowheader">지침</td> 
      <td> <p>사용자 정의 필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">형식</td>
      <td><p>사용자 정의 필드에 캡처할 데이터 유형을 선택합니다.</p>
      <p><strong>참고:</strong></p>
      <ul><li>양식을 저장한 후 형식 유형을 변경할 수 있습니다. 한 가지 제한 사항은 개체의 기존 모든 값을 새 유형으로 변환할 수 있어야 한다는 것입니다. (예를 들어, 형식 유형이 텍스트이고 객체가 "abc" 값을 저장하는 경우 필드를 변환할 수 없으며 "abc"를 숫자/통화로 변환할 수 없다는 오류가 발생합니다.) 수학 계산에서 필드를 사용하려면 숫자 또는 통화 형식을 선택해야 합니다.</li>
      <li>숫자 또는 통화를 선택하면 0으로 시작하는 숫자가 자동으로 잘립니다.</li>
      <li>숫자 필드의 문자 길이는 16자로 제한됩니다. 텍스트 필드를 사용하여 숫자를 입력하고 제한을 피할 수도 있습니다.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">기본 API URL</td> 
      <td><p>API에 대한 URL을 입력하거나 붙여넣습니다.</p><p>API URL은 드롭다운에 표시하려는 옵션의 JSON 콘텐츠를 반환해야 합니다. JSON 경로 필드를 사용하여 반환된 JSON에서 드롭다운 옵션으로 특정 값을 선택할 수 있습니다.</p><p>API URL을 입력할 때 URL에 다음 값을 선택적으로 전달할 수 있습니다.</p>
      <ul>
      <li>$$HOST - 현재 Workfront 호스트를 나타내며 Workfront API에 대한 API 호출을 생성/검색하는 데 사용할 수 있습니다. 이 와일드카드를 사용하면 인증이 처리되고 사용자가 인증 헤더를 보낼 필요가 없습니다. (예를 들어 사용자는 기본 URL <code>$$HOST/attask/api/task/search</code>을(를) 사용하여 작업을 검색할 수 있으며, 이를 통해 작업을 검색하고 반환된 작업 목록에서 값을 선택할 수 있습니다.)</li>
      <li><p>$$QUERY - 최종 사용자가 필드에 입력하는 검색 텍스트를 나타내며, 이를 통해 최종 사용자에 대한 쿼리 필터링을 구현할 수 있습니다. (사용자가 드롭다운에서 값을 검색합니다.)</p>
      <p>참조 중인 API에서 허용하는 경우 검색 쿼리에 수정자를 포함하여 검색이 작동하는 방식을 식별할 수 있습니다. 예를 들어, 다음을 기본 API URL로 사용하여 사람들이 특정 텍스트가 포함된 Workfront 프로젝트를 검색할 수 있도록 할 수 있습니다. <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p><a href="/help/quicksilver/wf-api/general/api-basics.md">API 기본 사항</a>에서 Workfront 검색 수정자에 대해 자세히 알아보세요.</p>
      <p><strong>참고:</strong> $$QUERY를 사용하지 않고 검색 상자에 사용자 유형 텍스트를 입력하면 이미 선택한 항목의 범위가 좁혀집니다. 그러나 $$QUERY를 사용하고 사용자가 원하는 것을 입력하면 API에 대한 새 네트워크 호출이 수행됩니다. 따라서 API에 2000개 이상의 값이 있고 API가 쿼리를 지원하는 경우 $$QUERY를 활용하여 기존 2000개 값뿐만 아니라 좁혀진 옵션이 있는 원본 API에서도 검색할 수 있습니다.</p></li>
      <li><p>{fieldName} - 여기서 fieldName은 Workfront의 사용자 지정 또는 네이티브 필드입니다. 이 방법으로 이미 선택한 필드의 값을 외부 조회 필드에 전달하여 옵션을 필터링할 때 계단식 드롭다운 옵션 필터를 구현할 수 있습니다. (예를 들어 지역 필드가 양식에 이미 있고 API의 국가 목록을 특정 지역에 있는 국가로 좁히고 있습니다.)</p>
      <p>{fieldName} 구문을 사용하여 다른 필드에 종속되는 외부 조회 필드의 경우 API에서 반환되는 옵션은 다른 필드에 입력한 문자열이나 값과 일치하는 옵션으로 제한됩니다. (이 기능은 목록 및 보고서에서 지원되지 않습니다.)</p></li>
      <li>{referenceObject}.{fieldName} - 필드가 개체의 일부인 경우. 이 구문은 사용자 정의 표현식과 유사합니다. (예: portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>팁:</strong> 정의할 수 있는 특정 쿼리에 대해 작업 중인 API에 대한 설명서를 검토하십시오.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP 메서드</td> 
      <td>메서드에 대해 <strong>Get</strong>, <strong>Post</strong> 또는 <strong>Put</strong>을 선택합니다.</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON 경로</td>
      <td><p>API에 대한 JSON 경로를 입력하거나 붙여넣습니다.</p> <p>이 옵션을 사용하면 API URL에서 반환되는 JSON에서 데이터를 추출할 수 있습니다. JSON 내에서 드롭다운 옵션에 표시할 값을 선택하는 데 사용됩니다.</p><p>예를 들어 API URL이 다음 형식으로 JSON을 반환하는 경우 "$.data[*].name"을 사용하여 미국과 캐나다를 드롭다운 옵션으로 선택할 수 있습니다.</br>
      <pre>
      &lbrace;
       데이터: &lbrace;
         { name: "미국"},
         { name: "Canada"}
       &rbrace;
      &rbrace;
      </pre>
      </p>
     <p>JSON 경로와 올바른 JSON 경로를 작성하는 방법에 대한 자세한 내용은 <a href="https://jsonpath.com/">https://jsonpath.com/</a>을(를) 참조하십시오.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">헤더</td>
      <td><p><strong>헤더 추가</strong>를 클릭한 다음 API를 사용한 인증에 필요한 키-값 쌍을 입력하거나 붙여 넣습니다.</p><p><strong>참고:</strong> 머리글 필드는 자격 증명을 저장할 수 있는 안전한 위치가 아니므로 입력하고 저장하는 것에 주의해야 합니다.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">다중 선택 드롭다운</td>
      <td><p>사용자가 드롭다운에서 두 개 이상의 값을 선택할 수 있도록 하려면 이 옵션을 선택합니다.</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">필수 필드 만들기</td>
      <td><p>사용자가 사용자 정의 양식을 작성하기 위해 필드를 요구하려면 이 옵션을 선택합니다.</p></td>
     </tr>       
    </tbody>
   </table>

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

>[!NOTE]
>
>다음 항목은 외부 API 호출의 기술적 제한입니다.
>
>* 최대 옵션 수는 2000개입니다(반환된 JSON의 처음 2000개의 고유 옵션만 표시됨).
>* 시간 초과: 30초
>* 재시도 횟수: 3
>* 재시도 사이의 대기 기간: 500ms
>* 예상 응답 상태: 2xx

### 이미지, PDF 및 비디오 추가

사용자 정의 양식에 이미지, PDF 및 비디오를 추가할 수 있습니다. 사용자 정의 양식이 첨부된 오브젝트로 작업하는 사용자는 다음 영역에서만 이미지, PDF 또는 비디오를 볼 수 있습니다.

* 객체의 세부 정보 영역(예: 프로젝트의 경우 프로젝트 세부 정보 영역).
* 새로운 Adobe Workfront 경험 모양과 느낌이 있는 객체의 편집 상자(예: 프로젝트 편집 및 작업 편집 상자)입니다.

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ 를 확장하여 사용 가능한 필드에 대한 설명을 확인합니다.

* **이미지**: 사용자가 이미지 파일을 추가할 수 있도록 허용합니다.
* **PDF**: 사용자가 PDF를 추가할 수 있도록 허용
* **비디오**: 사용자가 비디오 파일을 추가할 수 있도록 허용합니다.

+++

이미지, PDF 또는 비디오를 추가하려면:

1. 화면 왼쪽의 **새 필드** 탭에서 다음 필드 중 하나를 찾아 캔버스의 섹션으로 끌어서 놓습니다.

   * 이미지
   * PDF
   * 비디오

   ![필드를 섹션으로 드래그](assets/drag-field-to-section.png)

1. 위젯에 대해 다음 속성 중 하나를 입력하거나 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">크기</td> 
      <td>(선택 사항) 필요한 경우 위젯의 표시 크기를 변경합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 위젯 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오. 자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 시스템이 위젯을 식별하는 방법입니다. 위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.</p> <p>자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(필수) 인터넷에서 저장된 위젯의 URL을 입력하거나 붙여넣습니다.</p> 
      <p>비디오 위젯을 추가하는 경우 현재 URL 상자에 다음을 추가하여 추가할 수 있습니다.</p> 
      <ul> 
      <li> <p>YouTube 또는 Vimeo 링크</p> </li> 
      <li> <p>Google 드라이브 비디오 링크</p> </li> 
      <li> <p>MP4 및 MOV 확장으로 비디오에 연결</p> </li> 
      <li> <p>Workfront 인스턴스의 문서 영역에 이미 업로드된 비디오에 대한 링크입니다. 자세한 내용은 이 문서의 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">문서 영역에서 사용자 지정 양식에 비디오 위젯을 추가</a>를 참조하십시오.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>위젯에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >PDF의 경우 위젯 표시 크기에 대해 크게 를 사용하는 것이 좋습니다.
   >브라우저의 PDF 뷰어는 사용자의 디스플레이에 영향을 미치며 PDF 디스플레이가 최적이 아닌 경우 창 크기 및 브라우저 확대/축소 비율을 조정해야 할 수 있습니다.

1. (선택 사항) 다른 필드 또는 위젯을 추가하려면 이전 단계를 반복합니다.

   또는

   필드를 복사하려면 필드 위로 마우스를 가져간 다음 복사 아이콘을 클릭합니다.

   ![복사 아이콘](assets/copy-field.png)

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

#### 문서 영역에서 사용자 정의 양식에 비디오 추가{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>이러한 방식으로 사용자 정의 양식에 비디오를 추가하면 사용자가 오브젝트의 양식에 액세스할 때 문서 영역에 설정된 권한이 비디오에 적용됩니다.

1. [웹 사이트 또는 기타 웹 콘텐츠에 대한 대화형 증명 만들기](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md)에 설명된 대로 문서 영역의 비디오로 이동하여 증명을 생성합니다.
1. 증명을 엽니다.
1. 비디오의 아무 곳이나 마우스 오른쪽 단추로 클릭한 다음 **비디오 주소 복사**&#x200B;를 선택합니다.
1. 비디오 위젯을 추가하는 사용자 정의 양식에서 복사한 주소를 **URL** 상자에 붙여 넣습니다.
1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

### Workfront 기본 필드 추가

사용자 정의 양식에 Workfront 기본 필드를 추가할 수 있습니다. 사용자 정의 양식을 오브젝트에 첨부하면 필드가 오브젝트 데이터에서 채워집니다. 예를 들어 프로젝트에 첨부된 사용자 정의 양식의 설명 필드는 프로젝트 설명을 가져옵니다. (데이터가 없는 경우 필드에 &quot;N/A&quot;가 표시될 수 있습니다.)

+++ 를 확장하면 지원되는 기본 필드 목록이 표시됩니다.

이 표에는 사용자 정의 양식의 특정 Workfront 개체에 사용 가능한 기본 필드가 나열되어 있습니다.

| 필드 이름 | 프로젝트 | 작업 | 문제 | 템플릿 | 템플릿 작업 | 포트폴리오 | 프로그램 | 그룹 |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| 실제 완료 일자 기준 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 실제 기간 | ✓ |   |   |   |   |   |   |   |
| 실제 근로시간 | ✓ |   | ✓ |   |   |   |   |   |
| 실제 시작 일자 기준 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 회사 | ✓ |   |   | ✓ |   |   |   |   |
| 조건 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 상태 유형 | ✓ |   |   | ✓ |   |   |   |   |
| 설명 | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| 기간 |   | ✓ |   |   | ✓ |   |   |   |
| 기간 유형 |   | ✓ |   |   | ✓ |   |   |   |
| 기간 단위 |   | ✓ |   |   | ✓ |   |   |   |
| 작성자 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| 입력 일자 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| 그룹 | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| 마지막으로 업데이트한 사람 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 마지막 업데이트 날짜 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 이름 | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| 소유자 | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| 계획된 완료 일자 기준 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 계획된 기간 | ✓ |   |   | ✓ |   |   |   |   |
| 계획된 시간 | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| 계획된 시작 일자 | ✓ |   |   |   |   |   |   |   |
| 포트폴리오 | ✓ |   |   | ✓ |   |   | ✓ |   |
| 우선순위 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 프로그램 | ✓ |   |   | ✓ |   |   |   |   |
| 예상 완료 일자 기준 | ✓ | ✓ |   |   |   |   |   |   |
| 예상 기간(분) |   | ✓ |   |   |   |   |   |   |
| 예상 시작 일자 기준 | ✓ | ✓ |   |   |   |   |   |   |
| 참조 번호 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 일정 모드 | ✓ |   |   | ✓ |   |   |   |   |
| 심각도 |   |   | ✓ |   |   |   |   |   |
| 스폰서 | ✓ |   |   | ✓ |   |   |   |   |
| 상태 | ✓ | ✓ |   |   |   |   |   |   |
| 스토리 포인트 |   | ✓ |   |   |   |   |   |   |
| 템플릿 | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. 화면 왼쪽의 **새 필드** 탭에서 **기본 필드 참조**&#x200B;을(를) 찾아 캔버스의 섹션으로 끌어서 놓습니다.
1. 화면 오른쪽에서 사용자 정의 필드에 대한 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">크기</td> 
      <td>(선택 사항) 필요에 따라 필드의 표시 크기를 변경합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 필드 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오. 자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td>
      <td> <p>(필수) 이 이름은 시스템이 필드를 식별하는 방법입니다. 필드를 처음 구성할 때 레이블을 입력하면 이름 필드가 자동으로 채워집니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.</p>
      <p>자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">참조 필드</td> 
      <td><p>(필수) Workfront 기본 필드를 선택합니다.<p><p>양식 개체에 대한 네이티브 필드만 사용할 수 있습니다. 예를 들어 양식 디자이너 상단의 개체 유형 목록에 프로젝트가 표시되면 프로젝트에 대한 기본 필드는 선택할 수 있지만 작업에만 해당하는 필드는 선택할 수 없습니다.</p></td>
     </tr>
     <tr>
      <td role="rowheader">필터 추가</td>
      <td><p>참조 필드에 대한 필터를 추가하여 사용자가 필드를 사용할 때 선택할 수 있는 항목 목록을 제한합니다. </p> <p>예를 들어 사용자 이름이 다음 기준을 충족하는 경우에만 선택할 수 있도록 필드를 제한할 수 있습니다.</p> 
       <ul>
        <li>지정한 그룹에 속합니다.</li> 
        <li>지정한 역할 또는 직위와 연결되어 있습니다.</li> 
        <li>필드를 사용하는 사용자와 동일한 그룹에 속합니다.</li> 
       </ul>
       <p>텍스트 모드 구문을 사용하여 선택한 참조 필드의 필터를 정의해야 합니다. 자세한 내용은 <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">텍스트 모드를 사용하여 필터 편집</a>을 참조하세요.</p>
       <p><b>참고</b>:
       <ul> 
        <li>필터 옵션은 Portfolio, 회사 또는 소유자와 같은 기본 자동 완성 필드를 참조하는 경우에만 사용할 수 있습니다.</li>
        <li>기존 사용자 정의 양식을 편집하는 경우 기본 필드에 필터를 추가해도 사용자가 필드를 사용하여 이미 추가한 오브젝트(필터의 범위 밖)는 제거되지 않습니다.</li> 
        <li>모바일 장치에서는 이 필터를 사용할 수 없습니다. 기본 필드에 대한 필터를 사용하는 경우 필드는 필터의 영향을 받지 않는 사용자의 모바일 장치에 표시됩니다.</li> 
        </ul></p></td> 
      <td>
     </tr>
     <tr> 
      <td role="rowheader">필수 필드 만들기</td>
      <td><p>사용자가 사용자 정의 양식을 작성하기 위해 필드를 요구하려면 이 옵션을 선택합니다.</p></td>
     </tr> 
    </tbody> 
   </table>

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

### Adobe XD 파일 추가

Adobe XD 프로토타입을 사용자 정의 양식에 직접 추가할 수 있습니다. 사용자 정의 양식이 첨부된 오브젝트로 작업하는 사용자는 다음 영역에서만 Adobe XD 파일을 볼 수 있습니다.

* 객체의 세부 정보 영역(예: 프로젝트의 경우 프로젝트 세부 정보 영역)
* 새로운 Adobe Workfront 경험 모양과 느낌이 있는 객체의 편집 상자(예: 프로젝트 편집 및 작업 편집 상자)

Adobe XD 파일을 추가하려면:

1. 화면 왼쪽의 **새 필드** 탭에서 **Adobe XD**&#x200B;을(를) 찾아 캔버스의 섹션으로 끌어서 놓습니다.
1. 위젯에 대해 다음 속성 중 하나를 입력하거나 편집합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">크기</td> 
      <td>(선택 사항) 필요한 경우 위젯의 표시 크기를 변경합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 위젯 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 보고서에 특수 문자가 올바르게 표시되지 않으므로 이 레이블에 특수 문자를 사용하지 마십시오. 자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 시스템이 위젯을 식별하는 방법입니다. 위젯을 처음 구성하는 경우 레이블을 입력하면 이름 필드가 위젯과 일치하도록 자동으로 채워집니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.</p>
    <p>자세한 내용은 <a href="design-a-form.md#notes-on-field-names-and-labels">필드 이름 및 레이블에 대한 참고</a>을 참조하세요.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(필수) 유효한 XD 프로토타입 링크를 입력하거나 붙여넣습니다.</p> 
      <p><b>참고</b>: Adobe XD의 공유 탭에 있는 링크 액세스 설정은 링크가 있는 모든 사용자에게 설정되어야 합니다. 그렇지 않으면 사용자가 프로토타입을 볼 수 없습니다. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>위젯에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (선택 사항) 다른 필드 또는 위젯을 추가하려면 이전 단계를 반복합니다.

   또는

   필드를 복사하려면 필드 위로 마우스를 가져간 다음 복사 아이콘을 클릭합니다.

   ![복사 아이콘](assets/copy-field.png)

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

### Planning 연결 필드 추가

>[!IMPORTANT]
>
>이 섹션의 정보는 Adobe Workfront의 추가 기능인 Adobe Workfront Planning에 나와 있습니다.
>
>Workfront Planning에 액세스하려면 다음 항목이 있어야 합니다.
>
>* 새로운 Workfront 플랜 및 라이선스. 기존 Workfront 계획 또는 라이선스에는 Workfront Planning을 사용할 수 없습니다.
>* Workfront Planning을 위한 추가 패키지
>* 조직의 Workfront 인스턴스는 Adobe 통합 경험에 온보딩되어야 합니다.
>
> Workfront Planning에 액세스하기 위한 전체 요구 사항 목록은 [Adobe Workfront Planning 액세스 개요](/help/quicksilver/planning/access/access-overview.md)를 참조하십시오.
> 
>Workfront Planning에 대한 자세한 내용은 [Adobe Workfront Planning 개요](/help/quicksilver/planning/general/planning-overview.md)를 참조하십시오.

Planning 연결 사용자 정의 필드를 객체의 사용자 정의 양식에 추가하여 Workfront Planning에서 연결된 레코드를 Workfront 객체의 사용자 정의 필드에서 볼 수 있습니다.

모든 개체의 사용자 정의 양식에 Planning 연결 필드를 추가할 수 있습니다. 하지만 Workfront Planning에서 연결할 수 있는 Workfront 객체와 연결된 사용자 정의 양식에만 연결된 레코드를 표시할 수 있습니다.

>[!NOTE]
>
>사용자 정의 필드에서 정보를 보는 사용자는 Workfront Planning 및 Workfront 객체에 연결된 레코드 유형이 포함된 작업 공간에 액세스할 수 있어야 합니다.

Planning 연결 필드를 추가하려면

1. 화면 왼쪽의 **새 필드** 탭에서 **계획 연결**&#x200B;을 찾아 캔버스의 섹션으로 끌어서 놓습니다.
1. 화면 오른쪽에서 사용자 정의 필드에 대한 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">크기</td> 
      <td>(선택 사항) 필요한 경우 위젯의 표시 크기를 변경합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 필드 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 이 레이블에 특수 문자를 사용하지 마십시오.</p> 
      <p>Planning 레코드의 출처를 쉽게 식별하는 데 도움이 되는 레이블을 선택하는 것이 좋습니다. 작업 공간 이름 또는 레코드 유형 이름과 같은 정보를 추가합니다. </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td>
      <td> <p>(필수) 이름은 시스템이 필드를 식별하는 방법입니다. 필드를 처음 구성할 때 레이블을 입력하면 이름 필드가 자동으로 채워집니다. 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에 표시되는 이름을 변경하지 않고도 사용자에게 표시되는 레이블을 변경할 수 있는 옵션이 제공됩니다.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>(권장) 필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p>
      <p>여기에서 연결하는 레코드와 개체에 대한 자세한 정보를 추가할 수 있습니다. </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">오브젝트 유형</td> 
      <td><p>(필수) Workfront Planning의 레코드 유형에 연결된 Workfront 객체 유형을 선택합니다.</p>
      다음 객체 유형 중에서 선택할 수 있습니다.
      <ul><li> 프로젝트</li>
      <li> 포트폴리오</li><li> 프로그램</li><li> 회사</li><li> 그룹</li></ul>
       <p>양식의 오브젝트 유형에 대한 Workfront 오브젝트 유형만 사용할 수 있습니다.</p> <p> 예를 들어, 양식 디자이너 상단의 개체 유형 목록에 프로젝트가 표시되면 포트폴리오가 아닌 이 필드에서만 프로젝트를 선택할 수 있습니다. 단, 포트폴리오를 레코드 유형에 연결할 수도 있습니다.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">작업 영역</td> 
      <td> <p>(필수) Workfront에 표시할 레코드의 출처가 되는 Planning 작업 영역을 선택합니다.</p> <p> 객체 유형 필드에서 선택한 객체 유형에 연결된 작업공간만 표시됩니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">레코드 유형</td> 
      <td><p>(필수) Workfront 개체 유형과 연결된 Workfront Planning 레코드 유형을 선택합니다.</p><p>객체 유형 필드에서 선택한 객체 유형에 대한 연결이 있는 레코드 유형만 표시됩니다. </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">연결 필드</td> 
      <td><p>(필수) Workfront 객체에 표시할 선택한 Planning 레코드 유형과 Workfront 객체 유형 간의 연결 필드를 선택합니다. </p> <p> <b>참고</b>: 같은 개체와 레코드 종류 사이에 여러 연결 필드가 있을 수 있지만 필드를 하나만 선택할 수 있습니다.</p>  </td> 
     </tr>

<tr> 
      <td role="rowheader">레코드 유형 필드</td> 
      <td><p>(선택 사항) 연결된 레코드 유형에서 최대 7개의 조회 필드를 선택하여 사용자 정의 양식에 표시합니다. 기본 필드는 기본적으로 선택되어 있으며 편집할 수 없습니다. </p> <p> 선택한 연결된 레코드의 필드가 사용자 정의 양식의 표 보기에 표시됩니다. 양식이 Workfront 개체에 첨부된 경우 테이블 보기는 읽기 전용입니다. </p>  
    <img src="assets/planning-connections-field-with-table-on-form-preview.png"></td> 
     </tr>
      </tbody> 
   </table>

1. (선택 사항) 다른 필드를 추가하려면 이전 단계를 반복하십시오.

   또는

   필드를 복사하려면 필드 위로 마우스를 가져간 다음 복사 아이콘을 클릭합니다.

   ![복사 아이콘](assets/copy-field.png)

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하고 다른 섹션으로 이동하여 양식을 계속 작성하십시오.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

   이제 Workfront Planning에서 연결된 오브젝트에 양식을 첨부하고 다음 중 하나를 수행할 수 있습니다.

   * Workfront 개체에 연결된 Workfront Planning 레코드 유형(있는 경우)을 봅니다.
   * Workfront 개체에서 레코드를 연결하거나 연결을 끊습니다.

   자세한 내용은 [Workfront 개체에서 레코드 연결 관리](/help/quicksilver/planning/records/manage-records-in-planning-section.md)를 참조하십시오.

## 양식 디자이너를 사용하여 양식 구성 및 미리 보기

섹션 구분을 사용하여 사용자 정의 양식을 구성하고 양식의 미리 보기를 확인하는 방법에 대한 자세한 내용은 [양식 디자이너를 사용하여 양식 구성 및 미리 보기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)를 참조하십시오.



