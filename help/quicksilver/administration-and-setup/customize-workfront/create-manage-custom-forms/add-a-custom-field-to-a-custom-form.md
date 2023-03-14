---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 기존 양식 빌더를 사용하여 사용자 지정 양식에 사용자 지정 필드 추가
description: 사용자 지정 양식에서 작업하는 경우 새 사용자 지정 필드를 만들어 사용자 지정 양식에 추가할 수 있습니다. 다른 사용자 지정 양식에 이미 추가된 사용자 지정 필드를 추가할 수도 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '2208'
ht-degree: 2%

---

# 기존 양식 빌더를 사용하여 사용자 지정 양식에 사용자 지정 필드 추가

사용자 지정 양식에서 작업하는 경우 새 사용자 지정 필드를 만들어 사용자 지정 양식에 추가할 수 있습니다.

다른 사용자 지정 양식에 이미 추가된 사용자 지정 필드를 추가할 수도 있습니다. 자세한 내용은 [사용자 지정 양식에서 사용자 지정 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

사용자 지정 필드를 추가하는 것과 유사한 프로세스인 사용자 지정 양식에 자산 위젯을 추가하는 방법에 대한 내용은 [사용자 지정 양식에서 자산 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>사용자 지정 필드가 많은 사용자 지정 양식이나 사용자 지정 필드의 다중 선택 옵션이 포함된 사용자 지정 양식에서는 해당 필드에 값을 추가하거나 변경할 때 성능이 저하될 수 있습니다. 예를 들어 사용자 지정 필드가 100개 포함된 양식이나 옵션이 200개 이상인 다중 선택 사용자 지정 필드가 사용자 상호 작용할 때 속도가 느려질 수 있습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td>플랜</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;보유한 계획, 라이선스 유형 또는 액세스 수준 구성을 알아보려면 Workfront 관리자에게 문의하십시오.

## 사용자 지정 양식에 사용자 지정 필드 추가

1. 에 설명된 대로 사용자 지정 양식 만들기 또는 편집을 시작합니다. [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 를 엽니다. **필드 추가** 탭.

   ![](assets/add-a-field.jpg)

1. 사용 **새 필드** ![](assets/new-field.jpg) 선택한 경우 아래에 나열된 필드 유형 중 하나를 선택합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">한 줄 텍스트 필드</td> 
      <td>사용자가 필드에 단일 텍스트 행을 입력할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">단락 텍스트 필드</td> 
      <td>필드에 여러 줄의 텍스트를 입력할 수 있습니다.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">포맷이 지정된 텍스트 필드</td> 
      <td>필드에 여러 줄의 텍스트를 입력하고 굵게, 기울임체, 밑줄, 글머리 기호, 번호 매기기, 하이퍼링크 및 블록 따옴표로 텍스트 서식을 지정할 수 있습니다. 이 기능은 Workfront 개체의 홈, 업데이트 영역, 목록 및 세부 정보 영역에서 사용할 수 있습니다. 15,000자로 제한되면 많은 텍스트와 서식을 사용할 수 있습니다.</p> <p>API를 통해 이 필드에 액세스하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">API의 리치 텍스트 필드 저장소</a>.</p> <p><b>참고</b>: 서식이 있는 텍스트 필드는 Workfront 모바일 앱에서 사용할 수 없습니다(향후 릴리스에서 사용 가능). </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">드롭다운</td> 
      <td>드롭다운 선택 사항 목록을 제공합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">타이프 어헤드 </td> 
      <td>사용자가 Workfront에 있는 개체의 이름을 입력할 수 있습니다. 사용자가 입력을 시작하면 추천 목록이 표시됩니다.
      이 필드 유형은 다음 개체를 지원합니다.
      <ul><li>사용자</li>
      <li>그룹</li>
      <li>작업 역할</li>
      <li>포트폴리오</li>
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
      <td>표현식을 정의하고 결과를 사용자 지정 양식에 표시할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">사용자 지정 양식에 계산된 데이터 추가</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">일자</td> 
      <td>사용자가 날짜와 시간을 선택할 수 있는 달력을 표시합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">확인란</td> 
      <td>사용자가 여러 선택 사항을 선택할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">라디오 버튼</td> 
      <td>사용자는 하나만 선택해야 합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명 텍스트</td> 
      <td>Workfront 외부의 페이지에 대한 지침 및 링크를 포함할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">섹션 구분</td> 
      <td>섹션 브레이크는 실제로 필드가 아닙니다. 섹션 나누기를 사용하여 사용자 지정 필드 및 위젯을 섹션으로 구성하고, 필요한 경우 각 섹션에 대해 다른 보기 및 편집 권한을 구성할 수 있습니다. 섹션 나누기 추가 및 구성에 대한 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">사용자 지정 양식에 섹션 브레이크 추가</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 설정 **필드 설정** 탭에서 추가 중인 사용자 지정 필드 유형에 사용할 수 있는 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 사용자 지정 필드 위에 표시할 수사적 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에서 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">이름</td> 
      <td> <p>(필수) 이 이름은 Workfront 전체에서 보고서, 홈 및 API 상호 작용과 같은 다양한 영역에 사용자 지정 필드를 추가할 때 시스템에서 사용자 지정 필드를 식별하는 방법입니다.</p> <p>처음으로 사용자 지정 필드를 구성하고 레이블을 입력하면 이름 필드가 자동으로 채워져서 일치합니다. 그러나 레이블 및 이름 필드는 동기화되지 않습니다. 이렇게 하면 시스템에서 표시되는 이름을 변경하지 않고도 사용자가 보는 레이블을 변경할 수 있습니다.</p> 
      <p><b>중요 사항</b>:   
      <ul> 
      <li>가능하지만 사용자나 다른 사용자가 Workfront에서 사용자 지정 양식을 사용하기 시작한 후에는 이 이름을 변경하지 않는 것이 좋습니다. 이 경우 시스템은 이제 Workfront의 다른 영역에서 참조할 수 있는 사용자 지정 필드를 더 이상 인식하지 못합니다. <p>예를 들어, 보고서에 사용자 지정 필드를 추가하고 나중에 해당 이름을 변경하면 Workfront이 보고서에서 사용자 지정 필드를 인식하지 못하며, 새 이름을 사용하여 보고서에 다시 추가하지 않으면 해당 기능에서 제대로 작동하지 않습니다.</p> </li>
      <li> <p>기본 제공 Workfront 필드에 이미 사용되는 이름을 입력하지 않는 것이 좋습니다.</p> </li>
      <li><p>Workfront의 다른 영역에서 필드를 사용할 때 오류를 방지하기 위해 사용자 지정 필드 이름에 기간/점 문자를 사용하지 않는 것이 좋습니다.</p></li>
      </ul> <p>각 사용자 지정 필드 이름은 조직의 Workfront 인스턴스에서 고유해야 합니다. 이렇게 하면 다른 사용자 지정 양식에 대해 이미 생성된 양식을 다시 사용할 수 있습니다. 자세한 내용은 <a href="#Add" class="MCXref xref">사용자 지정 양식에 사용자 지정 필드 추가</a> 참조하십시오.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">지침</td> 
      <td> <p>사용자 지정 필드에 대한 추가 정보를 입력합니다. 사용자가 사용자 지정 양식을 작성하면 물음표 아이콘을 마우스로 가리키면 여기에 입력하는 정보가 포함된 도구 설명이 표시됩니다.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">포맷</td> 
      <td> <p>사용자 지정 필드에 캡처할 데이터 유형을 선택합니다.</p> <p><b>메모</b>:   
        <ul> 
         <li>양식을 저장한 후에는 이 필드를 편집할 수 없습니다. 필드를 수학 계산에서 사용하려면 숫자 또는 통화 형식을 선택해야 합니다.<br></li> 
         <li>번호 또는 통화를 선택하면 0으로 시작하는 숫자가 자동으로 잘립니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">표시 유형</td> 
      <td>(드롭다운, 확인란 및 라디오 단추만 해당) 필드에 원하는 옵션 선택 유형을 전환합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">크기</td> 
      <td>(텍스트 필드만 해당) 필드의 너비를 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">시간 표시(하루 기준)</td> 
      <td>(날짜 필드만) 날짜 및 시간을 필드에 표시하려면 이 옵션을 선택합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">참조 오브젝트 유형</td> 
      <td> <p>(Typeahead 필드만) 필드와 연결할 객체 유형을 선택합니다.</p> <p>적용 또는 저장+닫기를 클릭한 후에는 필드의 개체 유형을 변경할 수 없습니다.</p> <p><b>메모</b>:   
        <ul> 
         <li>Workfront 관리자가 Workfront 사용자 인터페이스에서 Portfolio, 프로그램 또는 프로젝트의 이름을 사용자 지정한 경우 개체의 기본 Workfront 이름이 사용자 지정된 이름이 아니라 이 드롭다운 목록에 표시됩니다. 도움이 필요한 경우 Workfront 관리자에게 문의하십시오.<br></li> 
         <li>다음 개체 유형은 iOS 및 Android Workfront 모바일 앱에서 지원됩니다. 사용자, 회사, 그룹, 작업 역할, Portfolio, 프로그램, 프로젝트 및 템플리트.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">필터 추가</td> 
      <td> <p>(필드 유형만) 사용자가 필드를 사용할 때 선택할 수 있는 객체를 제한하기 위해 객체 유형에 대한 필터를 추가합니다. </p> <p>예를 들어 다음 기준을 충족하는 경우에만 사용자 이름을 선택할 수 있도록 필드를 제한할 수 있습니다.</p> 
       <ul> 
        <li>지정된 그룹 또는 그룹에 속합니다</li> 
        <li>이 구성 요소는 지정한 역할이나 직책에 연결됩니다</li> 
        <li>이 그룹은 필드를 사용하는 사람과 동일한 그룹에 속합니다</li> 
       </ul> <p>텍스트 모드 구문을 사용하여 선택한 개체 유형에 대한 필터를 정의해야 합니다. 텍스트 모드를 사용하여 필터를 만드는 방법에 대한 자세한 내용은 섹션을 참조하십시오 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">필터에서 텍스트 모드 편집</a> 기사 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">텍스트 모드 개요</a>. </p> <p><b>메모</b>:   
        <ul> 
         <li>기존 사용자 지정 양식을 편집하는 경우, Typeahead 필드에 필터를 추가하면 사용자가 해당 필드를 사용하여 이미 추가한 개체(필터 범위 외)가 제거되지 않습니다.</li> 
         <li>이 필터는 모바일 장치에서 사용할 수 없습니다. Typeahead 필드에 필터를 사용하는 경우 해당 필드는 필터의 영향을 받지 않는 사용자의 모바일 장치에 나타납니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명 텍스트</td> 
      <td>(설명 텍스트 필드만 해당) 표시할 텍스트를 입력하여 사용자 지정 양식에 지침이나 링크를 제공합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">하이퍼링크</td> 
      <td>(설명 텍스트 필드만) 입력한 설명 텍스트에 하이퍼링크를 적용하려면 여기에 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">필수 필드 만들기</td> 
      <td>사용자가 사용자 지정 양식을 완료하기 위해 필드를 필수 필드로 사용하려면 이 옵션을 선택합니다. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">업데이트 피드의 필드 변경 내용 추적</td> 
      <td><p>드롭다운 목록을 클릭한 다음 필드의 값 변경 사항을 자동으로 추적할 객체 유형을 선택합니다.</p> 
      <p><b>참고</b>: 이 옵션은 다음과 같은 경우에는 사용할 수 없습니다.</p> 
      <ul> 
      <li>다음 개체 유형과 연결된 사용자 지정 양식: 비용, 회사, 이터레이션, 청구 레코드 및 그룹</li> 
      <li>다음 필드 유형: 계산된 , 설명 텍스트 및 섹션 나누기</li> 
      </ul>
      <p><b>중요 사항</b>: 여기서 객체 유형을 선택하거나 선택 취소하면 선택한 객체 유형과 연관되어 있고 이 필드가 포함된 모든 사용자 정의 양식이 영향을 받습니다. 예를 들어, 여기에서 객체 유형을 선택 취소하고 사용자 지정 양식을 저장하면 해당 필드를 포함하는 사용자 지정 양식에서 해당 객체 유형에 대해 더 이상 필드의 값 변경 사항이 추적되지 않습니다.</p>
       <p>여기에 필드에 대한 개체 유형을 선택하고 사용자 지정 양식을 저장하면 필드가 설정의 피드 업데이트 영역의 사용자 지정 필드 탭에 표시됩니다.</p> 
       <p>반대로, [설정]의 [피드 업데이트] 영역에서 이 필드가 삭제되면 개체 유형과 연결되고 이 필드가 포함된 모든 사용자 지정 양식에서 이 설정의 개체 유형이 선택 취소됩니다.</p> 
       <p>자세한 내용은 섹션을 참조하십시오 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">Workfront에서 추적할 필드 추가</a> 기사 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">시스템 업데이트 구성</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">논리 추가</td> 
      <td>기존 필드에서 사용자가 선택한 내용을 기준으로 양식에 표시할 필드를 지정합니다. 자세한 내용은 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">선택 항목 </td> 
      <td> <p>(드롭다운, 확인란 또는 라디오 단추만 해당) 선택 사항)</p> 
       <ol> 
        <li> <p>클릭 <b>옵션</b>를 활성화한 후 다음 중 하나를 활성화합니다.</p> 
           <ul> 
            <li><strong>값 표시</strong>: 필드에 각 선택 항목의 값을 표시합니다. 각 선택 항목의 레이블은 기본적으로 표시됩니다.</li> 
            <li><strong>선택 항목 A-Z 정렬</strong>: 필드에서 알파벳순으로 추가하는 선택 사항을 정렬합니다.</li> 
           </ul> 
        </li> 
        <li> <p>사용자에 대해 추가하는 각 선택 사항에 대해 톱니바퀴 아이콘을 클릭합니다 <img src="assets/gear-icon-settings.png">를 선택한 다음, 다음 옵션 중 하나를 선택합니다.</p> 
           <ul> 
            <li><strong>기본적으로 선택</strong>: 필드에서 기본적으로 옵션을 선택합니다.</li> 
            <li> <p><strong>선택 숨기기</strong>: 필드에서 선택 사항을 숨깁니다. 숨겨진 선택 사항은 보고서에서 액세스할 수 있습니다.</p> </li> 
            <li> <p><strong>선택 항목 제거</strong>: 필드에서 선택 항목을 제거합니다.</p> <p><b>경고</b>: 이 옵션을 사용하는 현재 개체가 있는 경우 필드에서 해당 개체를 제거하지 마십시오. 이를 제거하면 기록 데이터가 손실됩니다. 대신 옵션을 선택하여 숨기면 나중에 사용자가 선택할 수 없게 됩니다.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (조건부) 사용자 지정 양식에서 필드의 표시 유형을 변경하려면 **표시 유형** 드롭다운 메뉴를 클릭한 다음 원하는 유형을 클릭합니다.

   다음 필드 표시 유형 간을 전환할 수 있습니다.

   * **선택 유형 필드**: 확인란, 드롭다운, 라디오 단추.
   * **텍스트 유형 필드**: 단일 행 텍스트 필드, 단락 텍스트 필드. 서식 있는 텍스트 필드를 다른 표시 형식으로 전환할 수 없습니다. 그러나 제거하고 다른 유형의 필드를 추가할 수 있습니다.)

   예를 들어 확인란 필드를 만든 경우 드롭다운 필드 또는 라디오 단추 필드로 변경할 수 있습니다. 또는 단일 행 텍스트 필드를 만든 경우 단락 텍스트 필드로 변경할 수 있습니다.

   >[!NOTE]
   >
   >확인란 필드 또는 다중 선택 드롭다운 필드(두 개 이상의 옵션을 선택할 수 있는 드롭다운)에서 필드의 표시 유형을 단일 선택 필드 유형으로 변경하려면 다음 사항을 고려하십시오.
   >
   >* 라디오 단추로 변경하는 경우 사용자가 변경 및 양식 일부에 데이터를 저장할 때까지 Workfront은 사용자가 필드에 입력한 다중 선택 값을 유지합니다. 이때 다중 선택 유형 필드를 사용하여 선택한 모든 값은 선택한 라디오 단추 값으로 대체됩니다.
   >* 단일 선택 드롭다운으로 변경하는 경우 Workfront에서는 사용자가 변경하고 필드에 값을 저장할 때까지 사용자가 필드에 입력한 다중 선택 값을 유지합니다. 이때 다중 선택 유형 필드를 사용하여 선택한 모든 값은 선택한 드롭다운 값으로 대체됩니다.


1. (선택 사항) 2-6단계를 반복하여 다른 사용자 지정 필드를 추가합니다.

   또는

   에 설명된 대로 조직에 대해 이미 생성된 필드를 추가합니다. [사용자 지정 양식에서 사용자 지정 필드 또는 위젯 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >단일 사용자 지정 양식에 최대 500개의 필드와 위젯을 추가할 수 있습니다. 그러나 양식에 100개 이상이 있을 경우 그 복잡성에 따라 성능이 저하될 수 있습니다. 복잡한 양식의 예로는 계단식 매개 변수가 있는 양식, 계산된 사용자 지정 데이터 필드 및 단일 필드에 여러 값 옵션이 있습니다.

1. 클릭 **적용**.
1. 사용자 지정 양식을 다른 방식으로 계속 빌드하려면 다음 문서 중 하나를 계속 진행합니다.

   * [사용자 지정 양식에 사용자 지정 필드 및 위젯을 배치합니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [사용자 지정 양식에서 자산 위젯 추가 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [사용자 지정 양식에 계산된 데이터 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [사용자 지정 양식에 섹션 브레이크 추가](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [사용자 지정 양식에서 기존의 계산된 사용자 지정 필드 재사용](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [표시 논리를 추가하고 논리를 사용자 지정 양식에 건너뜁니다](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [사용자 지정 양식 미리 보기 및 완료](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
