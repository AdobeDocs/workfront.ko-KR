---
title: 양식 Designer으로 양식 구성 및 미리 보기
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 양식 Designer으로 사용자 정의 양식을 구성할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 28961cda48ce4eec84ed272e660be6ba938be370
workflow-type: tm+mt
source-wordcount: '1285'
ht-degree: 0%

---

# 양식 디자이너를 사용하여 양식 구성 및 미리 보기

양식 디자이너를 사용하여 사용자 정의 양식을 구성하고 미리 보기하여 제대로 설정되었는지 확인할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront 플랜*</p> </td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td>
   <p>새 플랜: 표준</p>
   <p>또는</p>
   <p>현재 플랜: 플랜</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>를 참조하십시오.</p> </td> 
  </tr>  
 </tbody> 
</table>

## 섹션 구분 추가

사용자 정의 양식의 사용자 정의 필드 및 위젯을 제목이 있는 섹션으로 그룹화할 수 있습니다. 이 기능은 양식을 작성할 사용자에게 구성된 경험을 제공하는 데 유용합니다. 또한 특정 사용자 정의 필드 및 위젯에 대한 액세스를 특정 사용자로 제한해야 하는 경우 섹션에 배치한 다음 해당 사용자에게만 섹션에 대한 액세스 권한을 부여할 수 있습니다.

예를 들어 시스템 관리자만 보거나 편집할 수 있어야 하는 중요한 정보를 추적해야 하는 경우 관리자 전용 권한으로 섹션 구분을 만들고 해당 섹션에 중요한 필드를 배치할 수 있습니다.

섹션에 대해 선택하는 액세스 설정은 사용자 정의 양식이 첨부된 Workfront 개체에서 사용자가 갖는 권한에 직접 연결되어 있습니다. 사용자가 해당 개체를 보거나, 기여하거나, 관리할 수 있는 액세스 권한을 가지고 있는지 여부에 따라 섹션을 숨기거나 표시할 수 있습니다. 또는 시스템 관리자 액세스 수준이 있는 사용자만 액세스할 수 있도록 섹션을 관리 전용으로 설정할 수 있습니다.

개체에 대한 사용 권한에 대한 자세한 내용은 [개체에 대한 사용 권한 공유 개요](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)를 참조하십시오.

사용자 정의 양식의 사용자 정의 필드 및 위젯에 대한 자세한 내용은 [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)을 참조하십시오.

### 사용자 정의 양식의 섹션에 대한 액세스 만들기 및 구성

1. [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)에 설명된 대로 사용자 정의 양식을 만들거나 편집하고 필드를 추가하십시오.

1. **섹션 구분**&#x200B;을 클릭하고 캔버스에서 원하는 위치로 끕니다.

1. 오른쪽 패널에서 섹션에 사용할 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 섹션 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요</b>: 이 레이블에 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>섹션의 용도를 사용자에게 설명하려면 텍스트를 입력합니다. 사용자 정의 양식에서 섹션의 레이블 아래에 표시됩니다.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>액세스 권한 부여</p> </td> 
      <td> <p> 이 섹션을 보고 해당 필드 값을 편집하려면 사용자 정의 양식이 첨부된 오브젝트에서 사용자에게 필요한 권한을 선택하십시오. 
       <p>다음 권한은 <b>개체에 대한 액세스 권한이 있는 사용자가 필드 값을 볼 수 있습니다</b>:</p> 
         <ul>
          <li><strong>보기</strong>: 개체에 대한 사용 권한을 봅니다.</li>
          <li><p><b>제한된 편집</b>: (개체가 프로젝트, 작업, 문제 또는 사용자인 경우에만 사용 가능):</p> 
          <p>프로젝트, 작업 또는 문제인 경우 사용자가 오브젝트에 기여할 수 있도록 허용합니다.</p>
          <p>사용자가 프로필을 편집하거나, 사용자의 경우 개체에 대한 프로필 권한을 소유할 수 있습니다.</p></li> 
          <li><b>편집</b>: 개체에 대한 권한을 관리합니다. </li> 
          <li><b>관리자만</b>: 시스템 관리자 액세스 수준</li> 
         </ul> </li> 
        <p>다음 권한은 <b>개체에 대한 이 액세스 권한이 있는 사용자가 필드 값을 편집할 수 있습니다</b>: </p> 
         <ul> 
          <li> <p><b>제한된 편집</b>: (개체가 프로젝트, 작업, 문제 또는 사용자인 경우에만 사용 가능):</p> 
           <p>객체가 프로젝트, 작업 또는 문제인 경우 이 권한을 사용하여 사용자가 객체에 기여할 수 있습니다</p>
          <p>개체가 사용자인 경우 이 권한을 사용하여 사용자가 프로필을 편집하거나 개체에 대한 프로필 권한을 소유할 수 있습니다.</p> 
          <li><b>편집</b>: 개체에 대한 권한을 관리합니다. </li> 
          <li><b>관리자만</b>: 시스템 관리자 액세스 수준</li> 
         </ul> </li> 
       </ul> 
       <p>개체에 대한 사용 권한에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">개체에 대한 사용 권한 공유 개요</a>를 참조하십시오.</p> 
       <p><b>참고</b>:  
       <ul> 
       <li> <p>여기에서 지정한 권한이 없는 사용자는 섹션에서 사용자 정의 필드 및 위젯을 볼 수 없습니다. </p> <p>이는 보고서의 필드 값을 표시하거나 텍스트 모드 보고의 계산된 필드에서 사용하는 경우에도 마찬가지입니다.</p> </li> 
       <li><p>요청/문제 사용자 정의 양식의 경우: 섹션 구분에서 필드를 보려면 보기 권한이 필요하지만 필드를 편집하려면 관리자 권한이 필요한 경우 양식을 작성할 때 섹션과 해당 필드의 모든 항목이 관리자가 아닌 사용자에게 표시되지 않습니다. 요청이 생성되면 보기 액세스 권한이 있는 사용자가 섹션의 필드를 볼 수 있습니다.</p></li>
       <li> <p>여러 객체 유형을 양식과 연결하면 다음 단계에서 사용할 수 있는 보기 및 편집 권한이 변경될 수 있습니다. 자세한 내용은 이 문서에서 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">여러 개체 유형이 사용자 정의 양식의 섹션 구분 권한에 미치는 영향</a>을 참조하십시오.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>논리 추가</p></td> 
      <td><p>표시 논리를 사용하여 사용자가 양식을 작성할 때 다중 선택 사용자 정의 필드에서 선택한 항목에 따라 섹션을 양식에 표시할지 여부를 지정합니다.</p><p><strong>참고:</strong> 섹션 구분 아래의 모든 개별 필드에 표시 논리가 적용되어 있고 논리의 결과로 해당 필드가 모두 숨겨져 있으면 사용자 지정 양식에서 전체 섹션이 숨겨집니다. 이 문제는 표시 논리가 섹션 구분에 적용되지 않는 경우에도 발생합니다.</p><p>자세한 내용은 <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">양식 디자이너를 사용하여 표시 논리 추가 및 건너뛰기 논리 추가</a>를 참조하십시오.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 하나 이상의 사용자 정의 필드 또는 위젯을 새 섹션으로 드래그하거나 추가합니다. 섹션을 저장하기 전에 필요합니다.

1. **완료**&#x200B;를 클릭합니다.

   >[!TIP]
   >
   >사용자 정의 양식을 만드는 동안 언제든지 **적용**&#x200B;을 클릭하여 변경 내용을 저장하고 양식을 열어 둘 수 있습니다.

### 여러 객체 유형이 섹션 구분 권한에 미치는 영향 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

사용자 정의 양식 섹션 구분에 대한 제한된 편집 권한은 프로젝트, 작업, 문제 및 사용자 객체 유형에 대해서만 사용할 수 있습니다.

제한된 편집 권한으로 구성된 섹션 구분이 있는 사용자 정의 양식에서 다른 객체 유형 중 하나(Portfolio, 프로그램, 문서, 회사, 청구 기록, 반복, 경비 또는 그룹)를 양식에 추가하는 경우 해당 객체 유형 및 양식의 기존 객체 유형 모두와 호환되는 편집 권한으로 전환하라는 메시지가 표시됩니다.

>[!INFO]
>
>**예:** 프로젝트 개체 형식과 연결된 사용자 지정 양식에서 제한된 편집 권한으로 섹션 나누기를 구성합니다.
>
>Portfolio 개체 유형을 양식에 추가하면 양식의 섹션 구분에 대해 제한된 편집 권한 옵션을 더 이상 사용할 수 없습니다.
>
>[편집] 권한으로 전환하라는 메시지가 화면에 표시됩니다. 이 권한은 프로젝트 객체 유형 및 Portfolio 객체 유형 모두와 호환되는 가장 낮은 수준의 권한입니다.


## 사용자 정의 양식에 사용자 정의 필드 및 위젯 배치


1. [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)에 설명된 대로 사용자 정의 양식을 만들거나 편집하십시오.

1. 사용자 정의 필드와 위젯을 동일한 행에 배치하려면 사이에 선이 나타날 때까지 한 필드를 다른 행 옆에 드래그합니다.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 오른쪽 상단의 **미리 보기** 단추를 사용하여 사용자 정의 필드 및 위젯이 양식에 표시되는 방식을 파악할 수 있습니다.
>* 사용자 정의 필드 및 위젯은 사용자가 볼 때 사용할 수 있는 화면 공간의 크기에 따라 양식에서 항상 동일한 방식으로 표시되지 않을 수 있습니다. 예를 들어, 수평 공간이 제한되는 경우 필드 행의 세 번째 필드는 다음 필드 행으로 래핑될 수 있다.

1. (선택 사항) 사용자 정의 필드 또는 위젯을 다른 필드 위 또는 아래에 배치하려면 항목 사이에 가로 파란색 선이 나타날 때까지 위 또는 아래로 드래그합니다.

1. 변경 내용을 저장하려면 **적용**&#x200B;을 클릭하세요.

   또는

   **저장 후 닫기**&#x200B;를 클릭합니다.

## 사용자 정의 양식 미리 보기

1. [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)에 설명된 대로 사용자 정의 양식을 만들거나 편집하고 필드를 추가하십시오.

1. 오른쪽 상단의 **미리 보기**&#x200B;를 클릭하여 양식 사용 시 표시되는 모양을 확인한 다음 **미리 보기 종료**&#x200B;를 클릭하여 양식 편집으로 돌아갑니다.

