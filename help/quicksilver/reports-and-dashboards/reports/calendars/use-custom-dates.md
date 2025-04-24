---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 캘린더 보고서에서 사용자 정의 날짜 필드 사용
description: 달력 보고서는 작업의 시각적 표현을 제공하는 동적 보고서입니다. 작업, 문제 및 프로젝트에 대해 달력 보고서의 사용자 지정 날짜 필드를 사용할 수 있습니다.
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 5c0278607faf65b58abeb9b813e403f97032a965
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 1%

---

# 달력 보고서에서 사용자 정의 날짜 필드 사용

[!UICONTROL 달력] 보고서는 작업의 시각적 표현을 제공하는 동적 보고서입니다. 다음 개체에 대해 달력 보고서의 사용자 지정 날짜 필드를 사용할 수 있습니다.

* 작업
* 문제
* 프로젝트

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>새로운 기능: 표준</p>
       <p>또는</p>
       <p>현재: 플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!UICONTROL 보고서], [!UICONTROL 대시보드] 및 [!UICONTROL 달력]에 대한 [!UICONTROL 편집] 액세스 권한</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>달력 보고서에 대한 [!UICONTROL 관리] 액세스</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 전제 조건

1. [!DNL Workfront] 인스턴스에서 사용할 수 있는 필드 내에 사용자 지정 날짜 필드와 값이 있어야 합니다. 사용자 지정 날짜가 포함된 사용자 지정 양식이 설정되어 있지 않은 경우 [사용자 지정 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)의 지침을 따릅니다.
1. 달력에 추가하려는 프로젝트, 작업 또는 문제에 사용자 정의 양식을 첨부하고 날짜를 지정합니다. 자세한 내용은 [개체에 사용자 정의 양식 추가](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)를 참조하십시오.

## 항목 그룹 설정

항목 그룹을 캘린더에 표시할 방법을 선택할 수 있습니다.

{{step1-to-calendars}}

1. 새 항목 그룹을 추가할 일정을 선택하고 기타 메뉴를 클릭한 다음 **편집**을 클릭합니다.
또는
**[!UICONTROL + 새 일정]**&#x200B;을 클릭하고 프로젝트 이름을 입력한 다음 **[!UICONTROL 고급 항목 추가]**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >캘린더 보고서를 만들려면 액세스 수준에 [!UICONTROL 보고서], [!UICONTROL 대시보드] 및 [!UICONTROL 캘린더]에 대해 [!UICONTROL 편집] 액세스 권한이 있어야 합니다.

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
      <td><strong>[!UICONTROL 사용자 지정 날짜]</strong>을(를) 선택하십시오.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 캘린더에서 표시]</strong></td>
      <td><p>날짜를 표시할 방법을 선택하십시오.</p>
       <ul>
        <li><strong>[!UICONTROL Single Date]</strong>: 캘린더에 개체가 단일 날짜에 표시됩니다.</li>
        <li><strong>[!UICONTROL Duration](시작~끝)</strong>: 일정에서 일 범위에 걸쳐 개체를 표시합니다.<br><p>참고: <strong>[!UICONTROL Duration]</strong>을(를) 선택하는 경우 지정된 종료 날짜는 시작 날짜 이후여야 합니다. 그렇지 않으면 캘린더에 항목이 표시되지 않습니다.</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL 사용자 지정 날짜]</strong></td>
      <td><p>추적할 개체에 첨부된 사용자 지정 날짜 이름을 입력합니다.</p><p><strong>참고:</strong> 성능 문제를 방지하기 위해 사용자 지정 날짜 이름 검색은 50개의 결과로 제한됩니다.</td>
     </tr>
    </tbody>
   </table>

1. 다음 섹션을 계속합니다.

### 항목 그룹에 개체 추가

항목을 표시할 방법을 설정한 후에는 달력에 표시할 객체를 그룹화에 추가해야 합니다.

1. **[!UICONTROL 캘린더에 무엇을 추가하시겠습니까?]** 섹션, 선택

   * **[!UICONTROL 작업]**
   * **[!UICONTROL 프로젝트]**
   * **[!UICONTROL 문제]**

1. 캘린더에 추가하는 개체 유형에 따라 **[!UICONTROL 작업 추가]**, **[!UICONTROL 프로젝트 추가]**, **[!UICONTROL 문제 추가]** 또는 **휴무**&#x200B;를 클릭합니다.

1. 드롭다운 메뉴에서 필드 이름을 입력한 다음 캘린더에 표시할 개체의 필드 원본을 선택합니다(예: **[!UICONTROL 지연 작업]**).
1. 달력 그룹화에 대한 조건문을 설정합니다.


   조건 설정에 대한 자세한 내용은 [필터 및 조건 수정자](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)를 참조하세요.

   ![달력의 개체 선택](assets/calendar-field-name.png)

1. (선택 사항) 1-4단계를 반복하여 달력 그룹화에 대한 추가 객체를 지정합니다.
1. **[!UICONTROL 작업/프로젝트/문제 레이블을 다음으로 설정..]** 필드에서 이 일정 그룹화의 개체에 레이블을 지정하는 방법을 선택합니다.

   >[!NOTE]
   >
   >특정 객체에 대해 기본 레이블 옵션을 사용할 수 없는 경우 객체 이름이 대신 표시됩니다. 예를 들어 [!UICONTROL 상위 작업] 레이블을 선택하고 개체와 연결된 상위 작업이 없으면 [!DNL Adobe Workfront]에 캘린더에서 보고 있는 개체 이름이 표시됩니다.

   ![작업 레이블 설정](assets/set-task-labels.png)
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

