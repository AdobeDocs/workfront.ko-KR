---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 달력 보고서에서 사용자 정의 날짜 필드 사용
description: 달력 보고서는 작업의 시각적 표현을 제공하는 동적 보고서입니다. 작업, 문제 및 프로젝트에 대해 달력 보고서의 사용자 지정 날짜 필드를 사용할 수 있습니다.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 1%

---

# 달력 보고서에서 사용자 정의 날짜 필드 사용

A [!UICONTROL 달력] 보고서는 작업의 시각적 표현을 제공하는 동적 보고서입니다. 다음 개체에 대해 달력 보고서의 사용자 지정 날짜 필드를 사용할 수 있습니다.

* 작업
* 문제
* 프로젝트

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL 계획] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>[!UICONTROL 보고서], [!UICONTROL 대시보드] 및 [!UICONTROL 달력]에 대한 [!UICONTROL 편집] 액세스 권한</p> <p>참고: 여전히 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>달력 보고서에 대한 [!UICONTROL 관리] 액세스</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">오브젝트에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 전제 조건

1. 사용자 정의 날짜 필드가 있어야 하며 필드에 값을 입력할 수 있어야 합니다. [!DNL Workfront] 인스턴스. 사용자 정의 날짜를 사용하여 사용자 정의 양식을 설정하지 않은 경우 의 처음 두 섹션에 있는 지침을 따릅니다 [사용자 정의 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 달력에 추가하려는 프로젝트, 작업 또는 문제에 사용자 정의 양식을 첨부하고 날짜를 지정합니다. 자세한 내용은 [오브젝트에 사용자 정의 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 항목 그룹 설정

항목 그룹을 캘린더에 표시할 방법을 선택할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 캘린더]**.

1. 새 항목 그룹을 추가할 달력을 선택합니다.\
   또는\
   클릭 **[!UICONTROL + 새 캘린더]** 달력 이름을 입력합니다.

   >[!NOTE]
   >
   >다음을 수행해야 합니다. [!UICONTROL 편집] 액세스 대상: [!UICONTROL 보고서], [!UICONTROL 대시보드], 및 [!UICONTROL 캘린더] 을 클릭하여 캘린더 보고서를 만듭니다.

1. 왼쪽에서 **[!UICONTROL 캘린더에 추가]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 고급 항목 추가]**.

1. 다음을 지정합니다.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 이 항목 그룹의 이름을 지정합니다.]</strong></td>
      <td>항목 그룹의 이름을 입력합니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 색상]</strong></td>
      <td>항목 그룹의 색상을 선택합니다. 모든 항목이 달력 보고서에 선택한 색상으로 표시됩니다.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 날짜 필드]</strong></td>
      <td>선택 <strong>[!UICONTROL 사용자 지정 날짜]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 캘린더에서 표시]</strong></td>
      <td><p>날짜를 표시할 방법을 선택하십시오.</p>
       <ul>
        <li><strong>[!UICONTROL 단일 날짜]</strong>: 캘린더에 개체가 단일 날짜에 표시됩니다.</li>
        <li><strong>[!UICONTROL Duration](시작~끝)</strong>: 캘린더에 며칠 동안 개체가 표시됩니다.<br><p>참고: <strong>[!UICONTROL 기간]</strong>, 지정한 종료 날짜는 시작 날짜 이후여야 합니다. 그렇지 않으면 캘린더에 항목이 표시되지 않습니다.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL 사용자 지정 날짜]</strong></td>
      <td><p>추적할 개체에 첨부된 사용자 지정 날짜 이름을 입력합니다.</p><p><strong>참고:</strong> 성능 문제를 방지하기 위해 사용자 정의 날짜 이름 검색은 50개로 제한됩니다.</td>
     </tr>
    </tbody>
   </table>

1. 다음 섹션을 계속합니다.

## 항목 그룹에 개체 추가

항목을 표시할 방법을 설정한 후에는 달력에 표시할 객체를 그룹화에 추가해야 합니다.

1. 다음에서 **[!UICONTROL 캘린더에 무엇을 추가하시겠습니까?]** 섹션, 선택

   * **[!UICONTROL 작업]**
   * **[!UICONTROL 프로젝트]**
   * **[!UICONTROL 문제]**

1. 클릭 **[!UICONTROL 작업 추가]**, **[!UICONTROL 프로젝트 추가]**, 또는 **[!UICONTROL 문제 추가]**&#x200B;을 달력에 추가하는 객체 유형에 따라 달라집니다.\
   ![달력의 오브젝트 선택](assets/field-name.png)

1. 드롭다운 메뉴에서 필드 이름을 입력한 다음 캘린더에 표시할 개체의 필드 소스를 선택합니다(예: **[!UICONTROL 지연 작업]**).
1. 달력 그룹화에 대한 조건문을 설정합니다.

   ![Condition 문](assets/condition-statement-calendar.png)

   조건 설정에 대한 자세한 내용은 [필터 및 조건 수정자](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (선택 사항) 1-4단계를 반복하여 달력 그룹화에 대한 추가 객체를 지정합니다.
1. 다음에서 **[!UICONTROL 작업/프로젝트/문제 레이블을 다음으로 설정...]** 필드에서 이 달력 그룹화의 개체 레이블이 달력에서 어떻게 지정되는지 선택합니다.

   >[!NOTE]
   >
   >특정 객체에 대해 기본 레이블 옵션을 사용할 수 없는 경우 객체 이름이 대신 표시됩니다. 예를 들어 [!UICONTROL 상위 작업] 레이블이 선택되고 개체와 연관된 상위 작업이 없습니다. [!DNL Adobe Workfront] 달력에서 보고 있는 객체 이름이 표시됩니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
