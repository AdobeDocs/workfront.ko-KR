---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 시간 유형 관리
description: 시간 유형을 시간 항목과 연결할 수 있습니다. 시간 유형은 시간 항목을 정의하는 데 사용하는 레이블입니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 시간 유형 관리

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

시간 유형을 시간 항목과 연결할 수 있습니다. 시간 유형은 시간 항목을 정의하는 데 사용하는 레이블입니다.

시간 유형은 두 가지입니다.

* **프로젝트 특정 시간 유형**: 프로젝트, 작업 및 문제에 대해 로그온해야 합니다. 프로젝트 특정 시간 유형은 [!DNL Adobe Workfront] 프로젝트, 작업 및 문제에 대한 시간을 기록할 수 있는 위치입니다.

   로그인 시간 [!DNL Workfront], 사용할 수 있는 프로젝트별 시간 유형은 시스템, 프로젝트 및 사용자 수준에서 설정된 구성 옵션에 따라 다릅니다.

   다음의 기본 프로젝트별 시간 유형은 항상 사용할 수 있습니다.

   * 프로젝트 시간
   * 작업 이름
   * 문제 시간

   다음 [!DNL Workfront] 관리자는 [작업표의 시간 유형 및 가용성을 정의합니다.](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >프로젝트에서 특정 시간 유형을 사용할 수 있도록 [!DNL Workfront] 시스템의 각 프로젝트에서 하나 이상의 프로젝트별 시간 유형을 활성화해야 합니다. 시스템 수준에서 프로젝트별 시간 유형을 활성화할 수 없고 프로젝트 수준에서 사용할 수 있는 프로젝트 특정 시간 유형이 없습니다.

* **일반 시간 유형**: 일반 시간은 프로젝트, 작업 또는 문제와 연결할 수 없으며 작업표에 직접 기록됩니다. 로깅 시간에 대한 자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 계획</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>참고</b>: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 내장된 시간 유형

Workfront에는 내장된 시간 유형 세트가 포함되어 있습니다. 이러한 시간 유형은 편집할 수 없으며 숨길 수 없습니다.

와 함께 제공되는 시간 유형 [!DNL Workfront] 입니다.

* **[!UICONTROL 아픈 시간]**: 프로젝트, 작업 또는 문제의 시간 항목과 연결할 수 없는 일반적인 시간 유형입니다.
* **[!UICONTROL 휴가 시간]**: 프로젝트, 작업 또는 문제의 시간 항목과 연결할 수 없는 일반적인 시간 유형입니다.
* **[!UICONTROL 일반 간접비]**: 프로젝트, 작업 또는 문제의 시간 항목과 연결할 수 없는 일반적인 시간 유형입니다. 하지만 프로젝트 계획 프로세스에서 수익으로 계산될 수 있습니다.
* **[!UICONTROL 프로젝트 시간]**: 프로젝트의 시간 항목에만 연결할 수 있는 일반 시간 유형입니다.
* **[!UICONTROL 작업 시간]**: 작업의 시간 항목에만 연결할 수 있는 일반 시간 유형입니다.
* **[!UICONTROL 문제 시간]**: 문제에 대한 시간 항목에만 연결할 수 있는 일반 시간 유형입니다.

## 시간 유형 만들기

로서의 [!DNL Workfront] 관리자는 시스템 및 프로젝트 레벨 모두에서 조직의 새 시간 유형을 생성할 수 있습니다. 시스템 및 프로젝트 수준에서 시간 유형을 만든 후 사용자는 특정 프로젝트 및 사용자에게 사용할 수 있는 시간 유형을 정의할 수 있습니다. 자세한 내용은 [작업표의 시간 유형 및 가용성을 정의합니다.](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

새 시간 유형을 만들려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 작업표 및 시간]** > **[!UICONTROL 시간 유형]**.

1. 클릭 **[!UICONTROL 새 시간 유형].**
1. 다음 정보를 **[!UICONTROL 새 시간 유형]** 양식:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>새 시간 유형에 시스템에서 쉽게 인식할 수 있는 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>시간 유형에 대한 설명을 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위]</td> 
      <td> <p>드롭다운 메뉴에서 올바른 범위를 선택하여 시간 유형이 일반적인지 아니면 프로젝트별 시간 유형인지를 정의합니다.</p> <p>일반 시간 유형은 작업표에서만 표시되며 프로젝트, 작업 또는 문제와 연결할 수 없습니다.</p> <p><b>중요 사항</b>: 사용자 지정 시간 유형이 [!UICONTROL Project Specific]인 경우 [!UICONTROL General]로 변경하면 기존의 모든 작업, 문제 및 프로젝트 시간이 시스템 기본 유형으로 설정됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td>이 시간 유형과 연관된 시간 항목이 수익 계산에 영향을 미치도록 하려면 이 옵션을 선택합니다.</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 매출로 계산]**: 이 시간 유형과 연관된 시간 항목이 수익 계산에 영향을 미치도록 하려면 이 옵션을 선택합니다.

1. 클릭 **[!UICONTROL 시간 유형 만들기].**

## 시간 유형 비활성화

시간 유형이 더 이상 사용되지 않고 사용자가 해당 시간 항목을 더 이상 시간 항목과 연결하지 않게 하려는 경우 시간 유형을 비활성화할 수 있습니다.

시간 유형을 비활성화하면 의 어디에서든지 시간 유형이 숨겨집니다. [!DNL Workfront] 여기서 시간 유형이 표시됩니다.

시간 유형을 비활성화하려면

1. 클릭 **[!UICONTROL 설정]** 의 오른쪽 위 모서리 [!DNL Adobe Workfront] 를 클릭합니다.

1. 확장 **[!UICONTROL 작업표 및 시간 기본 설정]**&#x200B;를 클릭한 다음 **[!UICONTROL 시간 유형]**.

1. 비활성화할 시간 유형을 선택합니다.

1. 클릭 **[!UICONTROL 비활성화]**.
