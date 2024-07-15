---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 시간 유형 관리
description: 시간 유형과 시간 항목을 연결할 수 있습니다. 시간 유형은 시간 항목을 정의하는 데 사용하는 레이블입니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 시간 유형 관리

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

시간 유형과 시간 항목을 연결할 수 있습니다. 시간 유형은 시간 항목을 정의하는 데 사용하는 레이블입니다.

시간 유형에는 두 가지 세트가 있습니다.

* **프로젝트별 시간 유형**: 프로젝트, 작업 및 문제에 로그온한 시간입니다. 프로젝트 특정 시간 유형은 프로젝트, 작업 및 문제에 시간을 기록할 수 있는 [!DNL Adobe Workfront]의 어디에서나 시간 항목과 연결할 수 있습니다.

  [!DNL Workfront]에서 시간을 기록할 때 사용할 수 있는 프로젝트별 시간 유형은 시스템, 프로젝트 및 사용자 수준에서 설정된 구성 옵션에 따라 다릅니다.

  다음 기본 프로젝트별 시간 유형은 항상 사용할 수 있습니다.

   * 프로젝트 시간
   * 작업 시간
   * 문제 시간

  [!DNL Workfront] 관리자는 [시간 형식 및 가용성 정의](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)에 설명된 대로 사용할 수 있는 프로젝트별 시간 형식을 결정합니다.

  >[!NOTE]
  >
  >[!DNL Workfront] 시스템에서 프로젝트별 시간 유형을 사용하는 경우 시스템의 각 프로젝트에서 프로젝트별 시간 유형을 하나 이상 사용해야 합니다. 시스템 수준에서 프로젝트별 시간 유형을 활성화할 수 없으며 프로젝트 수준에서 사용할 수 있는 프로젝트별 시간 유형이 없습니다.

* **일반 시간 유형**: 일반 시간은 프로젝트, 작업 또는 문제와 연결할 수 없으며 타임시트에 직접 로그인됩니다. 로깅 시간에 대한 자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md)을 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>[!DNL Workfront] 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. [!DNL Workfront] 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 기본 시간 유형

Workfront에는 기본 제공 시간 유형이 포함되어 있습니다. 이러한 시간 유형은 편집할 수 없으며 숨길 수 없습니다.

[!DNL Workfront]과(와) 함께 제공되는 시간 유형은 다음과 같습니다.

* **[!UICONTROL 병가 시간]**: 프로젝트, 작업 또는 문제의 시간 항목과 연결할 수 없는 일반적인 시간 형식입니다. 병가 시간은 수익으로 계산할 수 없습니다.
* **[!UICONTROL 휴가 시간]**: 프로젝트, 작업 또는 문제의 시간 항목과 연결할 수 없는 일반적인 시간 형식입니다. 휴가 시간은 수익으로 계산할 수 없습니다.
* **[!UICONTROL 일반 오버헤드]**: 프로젝트, 작업 또는 문제의 시간 항목과 연결할 수 없는 일반 시간 형식입니다. 하지만 프로젝트 계획 프로세스에서 수익으로 카운트될 수 있습니다.
* **[!UICONTROL 프로젝트 시간]**: 프로젝트의 시간 항목에만 연결할 수 있는 일반적인 시간 형식입니다.
* **[!UICONTROL 작업 시간]**: 작업의 시간 항목에만 연결할 수 있는 일반적인 시간 형식입니다.
* **[!UICONTROL 문제 시간]**:문제에 대한 시간 항목에만 연결할 수 있는 일반적인 시간 형식입니다.

## 시간 유형 만들기

[!DNL Workfront] 관리자는 시스템 수준과 프로젝트 수준 모두에서 조직에 대한 새 시간 유형을 만들 수 있습니다. 시스템 및 프로젝트 수준에서 시간 유형을 만든 후 사용자는 특정 프로젝트 및 사용자에 사용할 수 있는 시간 유형을 정의할 수 있습니다. 자세한 내용은 [시간 유형 및 가용성 정의](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)를 참조하십시오.

새 시간 유형을 만들려면:

1. [!DNL Adobe] Workfront의 오른쪽 위 모서리에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png)을(를) 클릭합니다.

1. **[!UICONTROL 타임시트 및 시간]** > **[!UICONTROL 시간 유형]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 새 시간 유형]을 클릭합니다.**
1. **[!UICONTROL 새 시간 형식]** 양식에 다음 정보를 지정하십시오.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 이름]</td> 
      <td>시스템에서 쉽게 인식할 수 있는 새 시간 이름을 지정합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 설명]</td> 
      <td>시간 유형에 대한 설명을 추가합니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 범위]</td> 
      <td> <p>드롭다운 메뉴에서 올바른 범위를 선택하여 시간 유형이 일반 또는 프로젝트별 시간 유형인지 여부를 정의합니다.</p> <p>일반 시간 유형은 타임시트에서만 볼 수 있으며 프로젝트, 작업 또는 문제와 연결할 수 없습니다.</p> <p><b>중요</b>: [!UICONTROL 프로젝트별] 사용자 지정 시간 유형이 있는 경우 [!UICONTROL 일반]으로 변경하면 기존의 모든 작업, 문제 및 프로젝트 시간이 시스템 기본 유형으로 설정됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td><p>이 시간 유형과 연관된 시간 항목이 수익 계산에 영향을 미치도록 하려면 이 옵션을 선택합니다.</p>
      <p>병가 시간과 휴가 시간은 수익으로 계산할 수 없습니다.</p>
      <p><b>메모</b></p>
      <p>일반 시간 유형이 매출로 계산되는 경우 시간을 기록하는 사용자의 프로필과 연결된 비용률은 시간 비용과 연결됩니다.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 매출로 계산]**: 이 시간 유형과 연결된 시간 항목이 매출액 계산에 영향을 미치도록 하려면 이 옵션을 선택하십시오.

1. **[!UICONTROL 시간 유형 만들기].**&#x200B;를 클릭합니다.

## 시간 유형 비활성화

시간 유형이 더 이상 사용되지 않는 경우 사용자가 시간 항목을 해당 시간 항목과 연결할 수 없게 되면 시간 유형을 비활성화할 수 있습니다.

시간 유형을 비활성화하면 시간 유형이 표시되는 [!DNL Workfront]의 모든 위치에서 시간 유형을 숨깁니다.

시간 유형을 비활성화하려면

1. 전역 탐색 모음에서 [!DNL Adobe Workfront]의 오른쪽 상단 근처에 있는 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 타임시트 및 시간 환경 설정]**&#x200B;을 확장한 다음 **[!UICONTROL 시간 유형]**&#x200B;을 클릭합니다.

1. 비활성화할 시간 유형을 선택합니다.

1. **[!UICONTROL 비활성화]**&#x200B;를 클릭합니다.
