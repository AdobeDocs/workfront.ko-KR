---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 기존 양식 빌더로 사용자 정의 양식에 사용자 정의 필드 추가
description: 사용자 정의 양식에서 작업할 때 새 사용자 정의 필드를 만들어 사용자 정의 양식에 추가할 수 있습니다. 다른 사용자 정의 양식에 이미 추가된 사용자 정의 필드를 추가할 수도 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 2%

---

# 기존 양식 빌더로 사용자 정의 양식에 사용자 정의 필드 추가

<!-- Audited: 02/2024 -->

사용자 정의 양식에서 작업할 때 새 사용자 정의 필드를 만들어 사용자 정의 양식에 추가할 수 있습니다.

다른 사용자 정의 양식에 이미 추가된 사용자 정의 필드를 추가할 수도 있습니다. 자세한 내용은 [사용자 정의 양식에서 사용자 정의 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

사용자 정의 양식에 자산 위젯을 추가하는 방법은 사용자 정의 필드를 추가하는 것과 유사합니다. [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>많은 사용자 정의 필드 또는 사용자 정의 필드의 수많은 다중 선택 옵션이 포함된 사용자 정의 양식에서 사용자는 해당 필드의 값을 추가하거나 변경할 때 성능이 저하될 수 있습니다. 예를 들어 100개의 사용자 정의 필드가 포함된 양식이나 200개 이상의 옵션이 있는 다중 선택 사용자 정의 필드는 사용자가 상호 작용할 때 속도가 느려질 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

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
   <td>사용자 정의 양식에 대한 관리 액세스 </td> 
  </tr>  
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 사용자 정의 양식에 사용자 정의 필드 추가 {#add-custom-field-to-custom-form}

1. 에 설명된 대로 사용자 정의 양식을 만들거나 편집하기 시작합니다. [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 다음 항목 선택 **필드 추가** 탭.

   ![필드 탭 추가](assets/add-a-field.jpg)

1. 포함 **새 필드** ![새 필드 아이콘](assets/new-field.jpg) 선택한 경우 다음 필드 유형 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">한 줄 텍스트 필드</td> 
      <td>사용자가 필드에 한 줄의 텍스트를 입력할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">단락 텍스트 필드</td> 
      <td>사용자가 필드에 여러 줄의 텍스트를 입력할 수 있습니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">포맷이 지정된 텍스트 필드</td> 
      <td>필드에 여러 줄의 텍스트를 입력하고 굵게, 기울임체, 밑줄, 글머리 기호, 번호 매기기, 하이퍼링크 및 블록 따옴표로 텍스트 서식을 지정할 수 있습니다. 이 기능은 홈, 업데이트 영역, 목록, Workfront 개체의 세부 정보 영역에서 사용할 수 있습니다. 문자 길이는 15,000자로 제한되어 있어 많은 텍스트와 서식을 사용할 수 있습니다.</p> <p>이 사용자 정의 필드 유형은 목록 및 보고서의 필터에서 지원되지 않습니다.</p> <p>API를 통해 이 필드에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">API의 리치 텍스트 필드 스토리지</a>.</p> <p><b>참고</b>: Workfront 모바일 앱에서는 서식이 있는 텍스트 필드를 사용할 수 없습니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">드롭다운</td> 
      <td>드롭다운 선택 사항 목록을 제공합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타이프 어헤드 </td> 
      <td>사용자가 Workfront에 있는 개체의 이름을 입력할 수 있습니다. 사용자가 입력을 시작하면 제안 목록이 나타납니다.
      이 필드 유형은 다음 개체를 지원합니다.
      <ul><li>사용자</li>
      <li>그룹</li>
      <li>작업 역할</li>
      <li>Portfolio</li>
      <li>프로그램</li>
      <li>프로젝트</li>
      <li>팀</li>
      <li>템플릿</li>
      <li>회사</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">계산됨</td> 
      <td>표현식을 정의하고 사용자 정의 양식에 결과를 표시할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">사용자 정의 양식에 계산된 데이터 추가</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">일자</td> 
      <td>사용자가 날짜 및 시간을 선택할 수 있는 달력을 표시합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">확인란</td> 
      <td>사용자가 여러 개의 선택 항목을 선택할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">라디오 버튼</td> 
      <td>사용자가 하나의 선택 항목만 선택해야 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명 텍스트</td> 
      <td>지침을 포함하고 Workfront 외부의 페이지에 연결할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">섹션 구분</td> 
      <td>섹션 구분은 실제로 필드가 아닙니다. 섹션 구분을 사용하여 사용자 정의 필드 및 위젯을 섹션으로 구성하고, 필요한 경우 각 섹션에 대해 서로 다른 보기 및 편집 권한을 구성할 수 있습니다. 섹션 구분 추가 및 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">사용자 정의 양식에 섹션 구분 추가</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >확인란 및 드롭다운과 같이 여러 항목을 선택할 수 있는 필드는 보고서에서 차트 및 그룹화하기 어렵습니다. 보고서에서 차트 및 그룹화를 보다 쉽게 수행할 수 있도록 각 선택 사항에 대해 별도의 필드(예: 한 줄 텍스트 필드)를 만들 수 있습니다.

1. 다음에서 **필드 설정** 탭에서 추가하는 사용자 정의 필드 유형에 사용할 수 있는 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 사용자 정의 필드 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에는 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 보고서, 홈 및 API 상호 작용과 같은 Workfront의 다양한 영역에 사용자 정의 필드를 추가할 때 시스템이 이 필드를 식별하는 방법입니다.</p> <p>사용자 정의 필드를 처음 구성할 때 레이블을 입력하면 이름 필드가 자동으로 채워집니다. 그러나 레이블 및 이름 필드는 동기화되지 않으므로 시스템에서 볼 수 있는 이름을 변경하지 않고도 사용자가 볼 수 있는 레이블을 자유롭게 변경할 수 있습니다.</p> 
      <p><b>중요 사항</b>:   
      <ul> 
      <li>그렇게 할 수도 있지만 본인이나 다른 사용자가 Workfront에서 사용자 정의 양식을 사용하기 시작한 후에는 이 이름을 변경하지 않는 것이 좋습니다. 이 필드를 선택하면 이제 Workfront의 다른 영역에서 참조될 수 있는 사용자 지정 필드가 시스템에서 더 이상 인식되지 않습니다. <p>예를 들어 사용자 지정 필드를 보고서에 추가하고 나중에 이름을 변경하면 Workfront은 보고서에서 이를 인식하지 못하며 새 이름을 사용하여 보고서에 다시 추가하지 않으면 제대로 작동하지 않습니다.</p> </li>
      <li> <p>기본 제공 Workfront 필드에 이미 사용된 이름은 입력하지 않는 것이 좋습니다.</p> </li>
      <li><p>Workfront의 다른 영역에서 필드를 사용할 때 오류를 방지하려면 사용자 지정 필드 이름에 마침표/점 문자를 사용하지 않는 것이 좋습니다.</p></li>
      </ul> <p>각 사용자 정의 필드 이름은 조직의 Workfront 인스턴스에서 고유해야 합니다. 이렇게 하면 다른 사용자 정의 양식에 대해 이미 만들어진 파일을 다시 사용할 수 있습니다. 자세한 내용은 <a href="#add-a-custom-field-to-a-custom-form">사용자 정의 양식에 사용자 정의 필드 추가</a> 이 문서에서.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>사용자 정의 필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 정의 양식을 작성할 때 물음표 아이콘 위로 마우스를 가져가 여기에 입력하는 정보가 포함된 도구 설명을 볼 수 있습니다.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">포맷</td> 
      <td> <p>사용자 정의 필드에 캡처할 데이터 유형을 선택합니다. 양식을 저장한 후 형식 선택을 변경할 수 있지만 새 형식은 입력한 값을 지원해야 합니다.</p>

   <p><strong>예:</strong> 하나 이상의 객체에 텍스트 형식의 필드 숫자 값을 저장하고 나중에 형식을 숫자 또는 통화로 변경하면 오류가 발생하지 않습니다. </p>
      <p>그러나 하나 이상의 개체에 텍스트 형식의 필드에 영숫자 값을 저장한 다음 형식을 숫자 또는 통화로 변경하려고 하면 저장된 영숫자 값이 숫자 또는 통화 형식과 호환되지 않으므로 오류가 발생합니다. </p>

   <p><strong>참고:</strong> 숫자 필드의 문자 길이는 16자로 제한됩니다. 텍스트 필드를 사용하여 숫자를 입력하고 제한을 피할 수도 있습니다.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">표시 유형</td> 
      <td>(드롭다운, 확인란 및 라디오 버튼만 해당) 필드에 대해 원하는 옵션 선택 유형을 전환합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">크기</td> 
      <td>(텍스트 필드만 해당) 필드의 너비를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간 표시(하루 기준)</td> 
      <td>(날짜 필드만 해당) 필드에 날짜와 함께 시간을 표시하려면 이 옵션을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">참조 오브젝트 유형</td> 
      <td> <p>(자동 완성 필드만 해당) 필드와 연결할 개체 유형을 선택합니다.</p> <p>적용 또는 저장+닫기를 클릭하면 필드의 오브젝트 유형을 변경할 수 없습니다.</p> <p><b>참고</b>:   
        <ul> 
         <li>Workfront 관리자가 Workfront 사용자 인터페이스에서 Portfolio, 프로그램 또는 프로젝트 이름을 사용자 지정한 경우 개체에 대한 기본 Workfront 이름이 사용자 지정한 이름이 아니라 이 드롭다운 목록에 표시됩니다. 이에 대한 도움이 필요한 경우 Workfront 관리자에게 문의하십시오.<br></li> 
         <li>iOS 및 Android Workfront Mobile 앱에서는 사용자, 회사, 그룹, 작업 역할, Portfolio, 프로그램, 프로젝트 및 템플릿과 같은 오브젝트 유형이 지원됩니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">필터 추가</td> 
      <td> <p>(자동 완성 필드만 해당) 사용자가 필드를 사용할 때 선택할 수 있는 객체를 제한하려면 객체 유형에 대한 필터를 추가합니다. </p> <p>예를 들어 사용자 이름이 다음 기준을 충족하는 경우에만 선택할 수 있도록 필드를 제한할 수 있습니다.</p> 
       <ul> 
        <li>지정한 그룹에 속합니다</li> 
        <li>지정한 역할 또는 직함과 연결됩니다</li> 
        <li>필드를 사용하는 사용자와 동일한 그룹에 속합니다</li> 
       </ul> <p>텍스트 모드 구문을 사용하여 선택한 객체 유형에 대한 필터를 정의해야 합니다. 텍스트 모드를 사용하여 필터를 만드는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">텍스트 모드를 사용하여 필터 편집</a>.</p>
       <p><b>참고</b>:   
        <ul> 
         <li>기존 사용자 정의 양식을 편집하는 경우 자동 완성 필드에 필터를 추가해도 사용자가 필드를 사용하여 이미 추가한 오브젝트가 제거되지 않습니다(필터의 범위 외부).</li> 
         <li>모바일 장치에서는 이 필터를 사용할 수 없습니다. 자동 완성 필드에 필터를 사용하는 경우 필드는 필터의 영향을 받지 않는 사용자의 모바일 장치에 표시됩니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명 텍스트</td> 
      <td>(설명 텍스트 필드만 해당) 사용자 정의 양식에 지침이나 링크를 제공하기 위해 표시할 텍스트를 입력합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하이퍼링크</td> 
      <td>(설명 텍스트 필드만 해당) 입력한 설명 텍스트에 하이퍼링크를 적용하려면 여기에 하이퍼링크를 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">필수 필드 만들기</td> 
      <td>사용자가 사용자 정의 양식을 작성하기 위해 필드를 요구하려면 이 옵션을 선택합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">업데이트 피드의 필드 변경 내용 추적</td> 
      <td><p>드롭다운 목록을 클릭한 다음 필드의 값 변경 사항을 자동으로 추적할 객체 유형을 선택합니다.</p> 
      <p><b>참고</b>: 다음에서는 이 옵션을 사용할 수 없습니다.</p> 
      <ul> 
      <li>경비, 회사, 반복, 청구 기록, 문서 및 그룹과 같은 객체 유형과 연관된 사용자 정의 양식입니다.</li> 
      <li>계산, 설명 텍스트 및 섹션 구분 필드 유형</li> 
      </ul>
      <p><b>중요 사항</b>: 여기에서 오브젝트 유형을 선택하거나 선택 취소하는 것은 선택한 오브젝트 유형과 연결되고 이 필드를 포함하는 모든 사용자 정의 양식에 영향을 줍니다. 예를 들어, 여기에서 오브젝트 유형을 선택 취소하고 사용자 정의 양식을 저장하는 경우 필드가 포함된 사용자 정의 양식의 해당 오브젝트 유형에 대해 필드의 값 변경 사항이 더 이상 추적되지 않습니다.</p>
       <p>여기에서 필드에 대한 오브젝트 유형을 선택하고 사용자 정의 양식을 저장하면 필드가 설정의 피드 업데이트 영역에 있는 사용자 정의 필드 탭에 표시됩니다.</p> 
       <p>반대로 설정의 피드 업데이트 영역에서 이 필드를 삭제하면 개체 유형과 연결되고 이 필드를 포함하는 모든 사용자 정의 양식에서 이 설정의 개체 유형이 선택 해제됩니다.</p> 
       <p>자세한 내용은 섹션을 참조하십시오 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#add-fields-you-want-workfront-to-track">Workfront에서 추적할 필드 추가</a> 이 문서에서 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md">시스템 업데이트 구성</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">논리 추가</td>
      <td>사용자가 기존 필드에서 선택한 사항을 기반으로 양식에 표시할 필드를 지정합니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">선택 항목 </td> 
      <td> <p>(드롭다운, 확인란 또는 라디오 버튼만 해당, 선택 사항)</p> 
       <ol> 
        <li> <p>클릭 <b>옵션</b>을 누르고 다음 중 하나를 활성화합니다.</p> 
           <ul> 
            <li><strong>값 표시</strong>: 필드에 있는 각 선택의 값을 표시합니다. 각 선택 항목의 레이블은 기본적으로 표시됩니다.</li> 
            <li><strong>선택 항목 정렬(A-Z)</strong>: 필드에서 추가하는 선택 항목을 알파벳순으로 정렬합니다.</li> 
           </ul> 
        </li> 
        <li> <p>사용자를 위해 추가하는 각 항목에 대해 톱니바퀴 아이콘을 클릭합니다 <img src="assets/gear-icon-settings.png">을(를) 클릭한 후 다음 옵션 중 하나를 선택합니다.</p> 
           <ul> 
            <li><strong>기본적으로 선택</strong>: 필드에서 기본적으로 선택을 선택합니다.</li> 
            <li> <p><strong>선택 항목 숨기기</strong>: 필드에서 선택 사항을 숨깁니다. 숨겨진 선택 사항은 보고서에서 계속 액세스할 수 있습니다.</p> </li> 
            <li> <p><strong>선택 항목 제거</strong>: 필드에서 선택 항목을 제거합니다.</p> <p><b>경고</b>: 이 선택 사항을 사용하는 현재 오브젝트가 있는 경우 필드에서 제거하지 마십시오. 삭제하면 내역 데이터가 손실됩니다. 대신 숨기려면 옵션을 선택합니다. 그러면 사용자가 나중에 선택할 수 없게 됩니다.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) 사용자 정의 양식에서 필드의 표시 유형을 변경하려면 **표시 유형** 드롭다운 메뉴를 클릭한 다음 원하는 유형을 클릭합니다.

   다음 필드 표시 유형 간에 전환할 수 있습니다.

   * **선택 유형 필드**: 확인란, 드롭다운, 라디오 버튼.
   * **텍스트 유형 필드**: 한 줄 텍스트 필드, 단락 텍스트 필드. (서식이 지정된 텍스트 필드를 다른 표시 유형으로 전환할 수 없습니다. 그러나 이를 제거하고 다른 유형의 필드를 추가할 수 있습니다.)

   예를 들어 확인란 필드를 만든 경우 드롭다운 필드 또는 라디오 단추 필드로 변경할 수 있습니다. 또는 한 줄 텍스트 필드를 만든 경우 단락 텍스트 필드로 변경할 수 있습니다.

   >[!NOTE]
   >
   >확인란 필드 또는 다중 선택 드롭다운 필드(두 개 이상의 옵션을 선택할 수 있는 드롭다운)에서 필드의 표시 유형을 단일 선택 필드 유형으로 변경하려면 다음 사항을 고려하십시오.
   >
   >* 라디오 단추로 변경하면 사용자가 변경하여 양식의 어떤 부분에서든 데이터를 저장할 때까지 Workfront에서는 사용자가 필드에 입력했을 수 있는 다중 선택 값을 유지합니다. 이때 다중 선택 유형 필드를 사용하여 선택한 모든 값은 선택한 라디오 단추 값으로 바뀝니다.
   >* 단일 선택 드롭다운으로 변경하면 Workfront에서는 사용자가 변경하여 필드에 저장할 때까지 사용자가 필드에 입력했을 수 있는 다중 선택 값을 유지합니다. 이때 다중 선택 유형 필드를 사용하여 선택한 모든 값은 선택한 드롭다운 값으로 바뀝니다.

1. (선택 사항) 3-5단계를 반복하여 사용자 정의 필드를 더 추가합니다.

   또는

   에 설명된 대로 조직에 대해 이미 생성된 필드를 추가합니다. [사용자 정의 양식에서 사용자 정의 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   >[!NOTE]
   >
   >단일 사용자 정의 양식에 최대 500개의 필드 및 위젯을 추가할 수 있습니다. 그러나 형식에 복잡성에 따라 100개가 넘는 값이 있을 경우 성능이 저하될 수 있습니다. 복잡한 양식의 예로는 계단식 매개 변수가 있는 양식, 계산된 사용자 정의 데이터 필드 및 단일 필드의 여러 값 옵션이 있습니다.

1. 클릭 **적용**.
1. 다른 방법으로 사용자 정의 양식을 계속 작성하려면 다음 문서 중 하나를 계속 진행하십시오.

   * [사용자 정의 양식에 사용자 정의 필드 및 위젯 배치](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 정의 양식에서 에셋 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 정의 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 정의 양식에 섹션 구분 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [사용자 정의 양식에서 기존의 계산된 사용자 정의 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [사용자 정의 양식에 표시 논리 및 건너뛰기 논리 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 정의 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
