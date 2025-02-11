---
product-area: projects
navigation-topic: use-lists
title: ' [!DNL Adobe Workfront]의 목록에서 항목을 인라인 편집합니다.'
description: 목록이나 보고서에 표시될 때 오브젝트를 인라인으로 편집할 수 있습니다. 목록이나 보고서에 표시된 객체에 대한 정보를 편집하면 객체가 즉시 업데이트됩니다.
feature: Get Started with Workfront
author: Nolan
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# [!DNL Adobe Workfront]의 목록에서 항목을 인라인 편집합니다.

<!--Audited: 11/2024-->

목록이나 보고서에 표시될 때 오브젝트를 인라인으로 편집할 수 있습니다. 목록이나 보고서에 표시된 객체에 대한 정보를 편집하면 객체가 즉시 업데이트됩니다.

오브젝트에 첨부되지 않은 사용자 정의 양식에 포함된 필드를 인라인 편집할 때 사용자 정의 양식이 자동으로 오브젝트에 추가됩니다. 필드가 여러 사용자 정의 양식에 있는 경우, 가장 최근에 업데이트된 사용자 정의 양식이 오브젝트에 첨부됩니다.

목록에 대한 자세한 내용은 [목록 시작 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)을 참조하세요.

목록이나 보고서에 표시된 대부분의 개체는 [!DNL Adobe Workfront]에서 인라인 편집할 수 있지만 다음과 같은 몇 가지 제한 사항이 있습니다.

* 계산 필드 또는 계산인 [!DNL Workfront] 기본 제공 필드는 편집할 수 없습니다.
* 목록의 오브젝트와 직접 연결된 필드만 편집할 수 있습니다. 목록의 객체와 연관된 객체에 속하는 필드는 편집할 수 없습니다.

  예를 들어 작업 보고서에서 작업의 상태를 편집할 수 있지만 동일한 보고서에서 작업이 연결된 프로젝트의 이름을 편집할 수는 없습니다. 프로젝트 보고서에서만 프로젝트의 이름을 편집할 수 있습니다.
* 목록에 대한 보기에 기본 통화가 표시되지 않으면 필드를 인라인 편집할 수 없습니다.

  기본 통화 표시에 대한 자세한 내용은 문서 [환율을 고유하게 사용하는 재무 데이터 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)의 [고유 통화를 사용하는 보고서 편집](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) 섹션을 참조하십시오.
* 목록에 표시되는 플래그 및 아이콘은 편집할 수 없습니다.
* 다른 보고서에서 가져온 보고서 필드는 인라인 편집할 수 없습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> 
    <p>신규:</p>
   <ul><li><p>기여자 이상 </p></li>
   </ul>

<p>현재:</p>
   <ul><li><p>요청 이상</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>목록이 있는 영역에 대한 [!UICONTROL 편집] 액세스 권한</p> <p>예를 들어 프로젝트에서 작업을 인라인 편집하려면 프로젝트에 대한 [!UICONTROL 편집] 액세스 권한이 필요합니다.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>[!UICONTROL 관리]</p> <p>사용자 정의 필드, 상태 등과 같은 특정 필드를 편집할 권한도 있어야 합니다.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 인라인 오브젝트 편집

1. 인라인 편집할 개체 목록으로 이동합니다.

   목록에는 목록에 있는 객체에 속하는 필드나 객체와 연관된 객체에 속하는 필드가 표시되어야 합니다.

1. 편집할 객체를 찾은 다음 목록의 필드 내부를 클릭합니다.

   >[!TIP]
   >
   >페이지가 여러 개인 경우 다음을 사용하여 객체를 찾을 수 있습니다.
   >
   >   * **페이지 매김**: 페이지 사이를 탐색하려면 뒤로 및 앞으로 화살표를 클릭하십시오.
   >     목록의 오른쪽 아래 모서리에 있는 [!UICONTROL 페이지 매김] 영역은 목록을 스크롤할 때 고정된 상태로 유지됩니다.
   >   * **빠른 필터**: 필터 아이콘을 클릭하거나 Alt+F를 입력하여 빠른 필터를 연 다음, 텍스트를 입력하여 입력한 텍스트가 포함된 항목만 표시합니다.
   >     빠른 필터는 목록 도구 모음에 있습니다. 자세한 내용은 [목록에 빠른 필터 적용](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)을 참조하십시오.

   필드를 편집할 수 있는 경우 필드 및 목록에 표시된 다른 모든 필드가 편집 가능한 셀로 바뀝니다.

   ![편집 가능한 셀](assets/nwe-editable-cells-350x131.png)

1. 이 셀의 정보를 편집한 다음 [!UICONTROL Enter]를 누르십시오.

   >[!NOTE]
   >
   >사용자 정의 필드가 서식을 허용하도록 구성된 경우 업데이트된 목록에서 필드를 인라인 편집할 때 텍스트를 굵게, 기울임꼴 또는 밑줄로 표시할 수 있습니다.
   >사용자 지정 필드의 서식 구성에 대한 자세한 내용은 [사용자 지정 양식 만들기](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)를 참조하십시오.
   >업데이트된 목록에 대한 자세한 내용은 문서 [목록 시작 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)의 &quot;업데이트된 목록과 기존 목록의 차이점&quot; 섹션을 참조하십시오.

1. 편집 가능한 다음 셀로 이동하려면 [!UICONTROL Tab]을 누릅니다.
1. (조건부) 편집 내용을 저장할 수 없고 셀이 빨간색으로 윤곽선이 표시되면 필드 내부를 클릭하여 셀 옆에 표시되는 유효성 검사 메시지를 검토하고 적절하게 업데이트합니다.

   가장 일반적으로 이 문제는 잘못된 포맷을 사용하거나 필수 필드를 비워 둔 경우에 발생합니다.

1. 모든 셀 수정이 끝나면 [!UICONTROL Enter]를 눌러 변경 내용을 저장합니다.
