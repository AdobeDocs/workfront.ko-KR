---
product-area: projects
navigation-topic: use-lists
title: 의 목록에 있는 인라인 편집 항목 [!DNL Adobe Workfront]
description: 객체들이 목록이나 보고서에 표시될 때 인라인 객체를 편집할 수 있습니다. 목록이나 보고서에 표시된 객체에 대한 정보를 편집하면 객체가 즉시 업데이트됩니다.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 의 목록에 있는 인라인 편집 항목 [!DNL Adobe Workfront]

객체들이 목록이나 보고서에 표시될 때 인라인 객체를 편집할 수 있습니다. 목록이나 보고서에 표시된 객체에 대한 정보를 편집하면 객체가 즉시 업데이트됩니다.

인라인 편집을 할 때는 객체에 첨부되지 않은 사용자 지정 양식에 포함된 필드를 편집하면 사용자 지정 양식이 객체에 자동으로 추가됩니다. 여러 사용자 지정 양식에 필드가 있는 경우 가장 최근에 업데이트된 사용자 지정 양식이 개체에 첨부됩니다.

목록에 대한 자세한 내용은 [에서 목록 시작 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

목록이나 보고서에 표시되는 대부분의 개체는 인라인으로 편집할 수 있습니다 [!DNL Adobe Workfront]에는 다음과 같은 몇 가지 제한 사항이 있습니다.

* 계산된 필드를 편집하거나 [!DNL Workfront] 계산되는 기본 제공 필드.
* 목록의 객체에 직접 연결된 필드만 편집할 수 있습니다. 목록의 객체와 연관된 객체에 속하는 필드는 편집할 수 없습니다.\
   예를 들어 작업 보고서에서 작업 상태를 편집할 수 있지만 동일한 보고서에서 작업이 연결된 프로젝트의 이름은 편집할 수 없습니다. 프로젝트 이름은 프로젝트 보고서에서만 편집할 수 있습니다.
* 목록에 대한 보기에 기본 통화가 표시되지 않으면 편집 필드를 인라인 편집할 수 없습니다.\
   기본 통화 표시에 대한 자세한 내용은 섹션을 참조하십시오 [고유한 통화로 보고서 편집](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) 기사 [고유한 환율을 사용하여 재무 데이터 보고서 만들기](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* 목록에 표시되는 플래그와 아이콘은 편집할 수 없습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Review] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>목록이 있는 영역에 대한 [!UICONTROL 편집] 액세스</p> <p>예를 들어, 프로젝트에서 편집 작업을 인라인 편집하려면 프로젝트에 [!UICONTROL 편집] 액세스 권한이 있어야 합니다.</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우<br>자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>개체 권한</strong></td> 
   <td> <p>[!UICONTROL Manage]</p> <p>또한 사용자 지정 필드, 상태 등과 같은 특정 필드를 편집할 수 있는 권한이 있어야 합니다.</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 인라인 개체 편집

1. 인라인 편집하려는 개체 목록으로 이동합니다.

   목록에 객체 또는 목록에 속하는 필드가 목록에 있는 객체와 연관된 객체에 속해야 합니다.

1. 편집할 개체를 찾은 다음 목록의 필드 안을 클릭합니다.

   >[!TIP]
   >
   >여러 페이지가 있는 경우 다음을 사용하여 개체를 찾을 수 있습니다.
   >
   >   
   >   
   >   * **페이지 매김**: 페이지 간을 탐색하려면 뒤로 및 앞으로 화살표를 클릭합니다.\
      >     목록의 오른쪽 아래 모서리에 있는 [!UICONTROL 페이지 매김] 영역을 스크롤할 때 고정된 상태로 유지됩니다.
   >   * **빠른 필터**: 필터 아이콘을 클릭하거나 Alt+F를 입력하여 빠른 필터를 연 다음 텍스트를 입력하여 입력한 텍스트가 포함된 항목만 표시합니다.\
      >     빠른 필터는 목록 도구 모음에 있습니다. 자세한 내용은 [목록에 빠른 필터 적용](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   필드를 편집할 수 있으면 목록에 표시된 필드 및 기타 모든 필드가 편집 가능한 셀로 바뀝니다.

   ![](assets/nwe-editable-cells-350x131.png)

1. 이 셀 내의 정보를 편집한 다음 키를 누릅니다 [!UICONTROL Enter 키].

   >[!NOTE]
   >
   >사용자 지정 필드가 서식을 허용하도록 구성된 경우 업데이트된 목록에서 필드를 인라인 편집할 때 텍스트를 굵게, 기울임체 또는 밑줄을 지정할 수 있습니다.\
   >사용자 지정 필드에 대한 서식 구성에 대한 자세한 내용은 [사용자 지정 양식 만들기 또는 편집](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >업데이트된 목록에 대한 자세한 내용은 문서의 &quot;업데이트된 목록과 레거시 목록 간의 차이&quot; 섹션을 참조하십시오 [에서 목록 시작 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. 누르기 [!UICONTROL 탭] 편집 가능한 다음 셀로 이동합니다.
1. (조건부) 편집 내용을 저장할 수 없고 셀의 윤곽이 빨간색으로 표시되어 있는 경우 필드 내부를 클릭하여 셀 옆에 표시되는 유효성 검사 메시지를 검토하고 적절한 업데이트를 수행합니다.

   일반적으로 잘못된 형식을 사용하거나 필수 필드를 비워 두면 발생합니다.

1. 모든 셀을 수정한 후 키를 누릅니다 [!UICONTROL Enter 키] 변경 사항을 저장하려면 을 클릭합니다.
