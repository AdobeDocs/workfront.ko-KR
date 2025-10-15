---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 달력 보고서에서 예상 일자 사용
description: 달력 보고서는 작업의 시각적 표현을 제공하는 동적 보고서입니다. 작업, 문제 및 프로젝트에 대해 달력 보고서의 예상 일자 필드를 사용할 수 있습니다.
author: Lisa
feature: Reports and Dashboards
exl-id: 39e16f0b-c10d-429e-9eb5-d4847c7e4ed9
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 1%

---

# 일정 보고서에서 [!UICONTROL 예상 일자] 사용

달력 보고서는 작업의 시각적 표현을 제공하는 동적 보고서입니다. 다음 객체에 대해 달력 보고서의 예상 일자 필드를 사용할 수 있습니다.

* 작업
* 문제
* 프로젝트

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p>
       <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>보고서, 대시보드 및 캘린더에 대한 액세스 편집</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td>캘린더 보고서에 대한 액세스 관리</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 항목 그룹 설정

항목 그룹을 캘린더에 표시할 방법을 선택할 수 있습니다.

{{step1-to-calendars}}

1. 새 항목 그룹을 추가할 일정을 선택하고 기타 메뉴를 클릭한 다음 **편집**&#x200B;을 클릭합니다.
또는
**[!UICONTROL + 새 일정]**&#x200B;을 클릭하고 프로젝트 이름을 입력한 다음 **[!UICONTROL 고급 항목 추가]**&#x200B;를 클릭합니다.

   >[!NOTE]
   >
   >캘린더 보고서를 만들려면 액세스 수준에 [!UICONTROL 보고서], [!UICONTROL 대시보드] 및 [!UICONTROL 캘린더]에 대해 [!UICONTROL 편집] 액세스 권한이 있어야 합니다.

1. 왼쪽의 **[!UICONTROL 일정에 추가]**&#x200B;를 클릭한 다음 **[!UICONTROL 고급 항목 추가]**&#x200B;를 클릭합니다.

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
      <td><p><strong>[!UICONTROL 예상 날짜]</strong>을(를) 선택하십시오. 예상 일자에 대한 자세한 내용은 </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">프로젝트 예상 시작 일자 개요</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">프로젝트, 작업 및 문제의 예상 완료 일자 개요</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 캘린더에서 표시]</strong></td>
      <td><p>날짜를 표시할 방법을 선택하십시오.</p>
       <ul>
        <li><strong>[!UICONTROL 시작 날짜만]</strong>: 캘린더에 개체가 단일 날짜에 표시됩니다.</li>
        <li><strong>[!UICONTROL 종료 날짜만]</strong>: 캘린더에 개체가 단일 날짜에 표시됩니다.</li>
        <li><strong>[!UICONTROL Duration] (시작~끝)</strong>: 일정에서 일 범위에 걸쳐 개체를 표시합니다.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL 사용 가능한 경우 실제 일자로 전환]</strong></td>
      <td><p>달력은 실제 날짜가 있는 경우 자동으로 해당 날짜로 전환합니다. <br>가능한 경우 실제 날짜로 전환하려면 <strong>[!UICONTROL 예]</strong> 또는 <strong>[!UICONTROL 아니요]</strong>를 선택하십시오. 실제 날짜에 대한 자세한 내용은</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">프로젝트의 실제 시작 일자 개요 </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">프로젝트 실제 완료 일자 개요 </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. 다음 섹션을 계속합니다.

## 항목 그룹에 개체 추가

항목을 표시할 방법을 설정한 후에는 달력에 표시할 객체를 그룹화에 추가해야 합니다.

1. **[!UICONTROL 캘린더에 무엇을 추가하시겠습니까?]** 섹션, 선택

   * **[!UICONTROL 작업]**
   * **[!UICONTROL 프로젝트]**
   * **[!UICONTROL 문제]**
   * **[!UICONTROL 휴무]**
1. 캘린더에 추가하는 개체 유형에 따라 **[!UICONTROL 작업 추가]**, **[!UICONTROL 프로젝트 추가]** 또는 **[!UICONTROL 문제 추가]**&#x200B;를 클릭합니다.

1. 드롭다운 메뉴에서 필드 이름을 입력한 다음 캘린더에 표시할 개체의 필드 원본을 선택합니다(예: **[!UICONTROL 지연 작업]**).
1. 달력 그룹화에 대한 조건문을 설정합니다.


   ![달력의 개체 선택](assets/calendar-field-name.png)
조건 설정에 대한 자세한 내용은 [필터 및 조건 수정자](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)를 참조하세요.

1. (선택 사항) 1-4단계를 반복하여 달력 그룹화에 대한 추가 객체를 지정합니다.
1. **[!UICONTROL 작업/프로젝트/문제 레이블을 다음으로 설정..]** 필드에서 이 일정 그룹화의 개체에 레이블을 지정하는 방법을 선택합니다.

   >[!NOTE]
   >
   >특정 객체에 대해 기본 레이블 옵션을 사용할 수 없는 경우 객체 이름이 대신 표시됩니다. 예를 들어 [!UICONTROL 상위 작업] 레이블을 선택하고 개체와 연결된 상위 작업이 없으면 [!DNL Adobe Workfront]에 캘린더에서 보고 있는 개체 이름이 표시됩니다.

   ![작업 레이블 설정](assets/set-task-labels.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

