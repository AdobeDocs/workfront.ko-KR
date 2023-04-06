---
title: 양식 디자이너를 사용하여 양식 구성 및 미리 보기
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 양식 디자이너를 사용하여 사용자 지정 양식을 구성할 수 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# 양식 디자이너를 사용하여 양식 구성 및 미리 보기

양식 디자이너를 사용하여 사용자 지정 양식을 구성할 수 있습니다.

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
   <td>
   <p>현재 계획: 표준</p>
   <p>또는</p>
   <p>기존 계획: 계획</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>사용자 정의 양식에 대한 관리 액세스</p> <p>Workfront 관리자가 이 액세스 권한을 부여하는 방법에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## 섹션 브레이크 추가

사용자 지정 양식의 사용자 지정 필드 및 위젯을 제목이 있는 섹션으로 그룹화할 수 있습니다. 이 기능은 양식을 작성할 사용자에게 조직화된 경험을 제공하는 데 유용합니다. 또한 특정 사용자 지정 필드 및 위젯에 대한 액세스를 특정 사용자에게 제한해야 하는 경우 섹션에 배치한 다음 해당 사용자에게만 섹션에 대한 액세스 권한을 부여할 수 있습니다.

예를 들어, 시스템 관리자만 보거나 편집할 수 있는 중요한 정보를 추적해야 하는 경우, 관리 전용 권한으로 섹션 나누기를 만들고 해당 섹션에 중요 필드를 배치할 수 있습니다.

섹션에 대해 선택하는 액세스 설정은 사용자 지정 양식이 첨부된 Workfront 개체에 대해 사용자가 가지고 있는 권한에 직접 연결되어 있습니다. 사용자가 해당 개체를 보거나, 기여하거나, 관리할 액세스 권한이 있는지 여부에 따라 섹션을 숨기거나 표시할 수 있습니다. 또는 시스템 관리자 액세스 수준을 가진 사용자만 액세스할 수 있도록 섹션을 관리자 전용으로 설정할 수 있습니다.

객체에 대한 권한에 대한 자세한 내용은 [개체에 대한 권한 공유 개요](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

사용자 지정 양식의 사용자 지정 필드 및 위젯에 대한 자세한 내용은 [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### 사용자 지정 양식의 섹션에 대한 액세스 만들기 및 구성

1. 에 설명된 대로 사용자 지정 양식 만들기 또는 편집 및 필드 추가 작업을 시작합니다. [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 클릭 **섹션 나누기** 캔버스에서 원하는 위치로 드래그합니다.

1. 오른쪽 패널에서 섹션에 사용할 옵션을 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">레이블</td> 
      <td> <p>(필수) 섹션 위에 표시할 설명 레이블을 입력합니다. 언제든지 레이블을 변경할 수 있습니다.</p> <p><b>중요 사항</b>: 이 레이블에서 특수 문자를 사용하지 마십시오. 보고서에 올바로 표시되지 않습니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">설명</td> 
      <td>섹션이 무엇인지에 대해 사용자에게 설명하려면 텍스트를 입력합니다. 사용자 지정 양식에서 섹션의 레이블 아래에 표시됩니다.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>액세스 권한 부여</p> </td> 
      <td> <p> 이 섹션을 보고 해당 필드 값을 편집하려면 사용자 지정 양식이 첨부된 개체에서 사용자가 필요한 권한을 선택합니다. 
       <p>다음 권한은 <b>객체에 대한 액세스 권한이 있는 사용자는 필드 값을 볼 수 있습니다</b>:</p> 
         <ul>  
          <li><p><b>제한된 편집</b>: (개체가 프로젝트, 작업, 문제 또는 사용자인 경우에만 사용할 수 있습니다.)</p> 
          <p>프로젝트, 작업 또는 문제인 경우 사용자가 객체에 기여하도록 허용합니다.</p>
          <p>사용자가 프로필을 편집하거나 사용자의 경우 객체에 대한 프로필 권한을 소유할 수 있습니다.</p></li> 
          <li><b>편집</b>: 개체에 대한 권한 관리 </li> 
          <li><b>관리자만</b>: 시스템 관리자 액세스 수준</li> 
         </ul> </li> 
        <p>다음 권한은 <b>객체에 대한 액세스 권한이 있는 사용자는 필드 값을 편집할 수 있습니다</b>: </p> 
         <ul> 
          <li> <p><b>제한된 편집</b>: (개체가 프로젝트, 작업, 문제 또는 사용자인 경우에만 사용할 수 있습니다.)</p> 
           <p>객체에 프로젝트, 작업 또는 문제가 있는 경우 이 권한을 통해 사용자는 객체에 기여할 수 있습니다</p>
          <p>개체가 사용자일 경우 이 권한을 사용하여 프로필을 편집하거나 개체에 대한 프로필 권한을 소유할 수 있습니다.</p> 
          <li><b>편집</b>: 개체에 대한 권한 관리 </li> 
          <li><b>관리자만</b>: 시스템 관리자 액세스 수준</li> 
         </ul> </li> 
       </ul> 
       <p>객체에 대한 권한에 대한 자세한 내용은 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">개체에 대한 권한 공유 개요</a>.</p> 
       <p><b>메모</b>:  
       <ul> 
       <li> <p>여기서 지정한 권한이 없는 사용자는 섹션에서 사용자 지정 필드 및 위젯을 볼 수 없습니다. </p> <p>보고서에 필드 값을 표시하거나 텍스트 모드 보고의 계산된 필드에서 사용하는 경우에도 마찬가지입니다.</p> </li> 
       <li> <p>여러 객체 유형을 양식에 연결하면 이러한 단계에서 사용할 수 있는 보기 및 편집 권한이 변경될 수 있습니다. 자세한 내용은 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">여러 개체 유형이 사용자 지정 양식의 섹션 브레이크 권한에 영향을 주는 방식</a> 참조하십시오.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 하나 이상의 사용자 지정 필드 또는 위젯을 새 섹션에 드래그하거나 추가합니다. 섹션을 저장하기 전에 이 단축키가 필요합니다.

1. 클릭 **완료**.

   >[!TIP]
   >
   >을(를) 클릭합니다 **적용** 언제든지 사용자 지정 양식을 만들어 변경 사항을 저장하고 양식을 열어 둡니다.

### 여러 객체 유형이 섹션 브레이크 권한에 영향을 주는 방식 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

사용자 지정 양식 섹션에 대한 제한된 편집 권한은 프로젝트, 작업, 문제 및 사용자 개체 유형에만 사용할 수 있습니다.

제한된 편집 권한으로 구성된 섹션 브레이크가 있는 사용자 지정 양식에서는 양식에 다른 객체 유형(Portfolio, 프로그램, 문서, 회사, 청구 레코드, 이터레이션, 비용 또는 그룹) 중 하나를 추가하면 해당 객체 유형과 양식의 기존 객체 유형과 호환되는 편집 권한으로 전환하라는 메시지가 표시됩니다.

>[!INFO]
>
>**예:** 프로젝트 개체 유형과 연결된 사용자 지정 양식에서는 제한된 편집 권한으로 섹션 나누기가 구성됩니다.
>
>양식에 Portfolio 개체 유형을 추가합니다. 즉, 양식의 섹션 나누기에 더 이상 [편집 제한] 권한 옵션을 사용할 수 없습니다.
>
>Project 개체 유형 및 Portfolio 개체 유형과 호환되는 최소 사용 권한 수준인 Edit 권한으로 전환하라는 메시지가 화면에 표시됩니다.


## 사용자 지정 양식에 사용자 지정 필드 및 위젯을 배치합니다


1. 에 설명된 대로 사용자 지정 양식 만들기 또는 편집을 시작합니다. [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 사용자 지정 필드와 위젯을 같은 행에 배치하려면 그 사이에 줄이 나타날 때까지 다른 필드 옆에 하나씩 드래그합니다.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 를 사용할 수 있습니다 **미리 보기** 오른쪽 상단 모서리의 단추를 클릭하여 사용자 지정 필드 및 위젯이 양식에 표시되는 방법을 이해합니다.
>* 사용자가 볼 때 사용 가능한 화면 공간의 양에 따라 사용자 지정 필드 및 위젯이 항상 같은 방식으로 양식에 표시되는 것은 아닙니다. 예를 들어, 가로 공간이 제한된 경우 필드 행의 세 번째 필드가 다음 필드 행으로 줄 바꿈될 수 있습니다.


1. (선택 사항) 사용자 지정 필드 또는 위젯을 다른 필드 위나 아래에 배치하려면 항목 사이에 가로 파란색 선이 나타날 때까지 위나 아래로 드래그합니다.

1. 변경 사항을 저장하려면 **적용**

   또는

   클릭 **저장 후 닫기**.

## 사용자 지정 양식 미리 보기

1. 에 설명된 대로 사용자 지정 양식 만들기 또는 편집 및 필드 추가 작업을 시작합니다. [양식 디자인](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 클릭 **미리 보기** 왼쪽 상단 모서리에서 양식을 사용할 때 양식이 어떻게 표시되는지 확인한 다음 을 클릭합니다. **미리 보기 종료** 양식 편집으로 돌아갑니다.