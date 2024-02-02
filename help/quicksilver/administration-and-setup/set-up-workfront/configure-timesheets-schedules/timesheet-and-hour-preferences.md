---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 타임시트 및 시간 환경 설정 구성
description: (으)로 [!DNL Adobe Workfront] 관리자는에서 타임시트 및 시간에 대한 환경 설정을 지정할 수 있습니다. [!DNL Workfront] 타임시트가 미리 채울 수 있는 항목과 사용자가 시간을 기록할 수 있는 항목을 정의하기 위한 것입니다.
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 66e6c96ca51a159f6e9a16178f06dd016217c7d8
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 0%

---

# 타임시트 및 시간 환경 설정 구성

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

(으)로 [!DNL Adobe Workfront] 관리자는에서 타임시트 및 시간에 대한 환경 설정을 지정할 수 있습니다. [!DNL Workfront] 타임시트가 미리 채울 수 있는 항목과 사용자가 시간을 기록할 수 있는 항목을 정의하기 위한 것입니다.

>[!IMPORTANT]
>
>이 문서에 설명된 조건에 따라 타임시트를 미리 채우는 항목 외에도 기본적으로 다음 항목이 타임시트에 표시됩니다.
>
>* 타임시트의 시간대 동안 시간을 기록한 항목
>* 타임시트에 고정된 항목
>* 검색하고 타임시트에 수동으로 추가하는 항목입니다. 수동으로 추가된 항목은 기본적으로 고정됩니다.
>
>자세한 내용은 [로그 시간](../../../timesheets/create-and-manage-timesheets/log-time.md) 및 [타임시트 개요](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).



타임시트의 변경 사항은 나중에 만들어지는 모든 타임시트에 영향을 줍니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td><p>현재:[!UICONTROL 계획]</p>
   또는
   <p>새로운 기능: 표준</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>다음이어야 합니다: [!DNL Workfront] 관리자.</p>  </td>
</tr> 
 </tbody> 
</table>

*자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 타임시트 및 시간 환경 설정 지정

{{step-1-to-setup}}

1. 클릭 **[!UICONTROL 타임시트 및 시간]** > **[!UICONTROL 환경 설정]**.

   [타임시트 및 시간 환경설정] 페이지가 표시됩니다.

1. (선택 사항) **시스템 타임시트 및 시간 환경 설정** 검색 상자에서 그룹 이름을 입력한 다음 목록에 표시될 때 선택합니다.

   ![](assets/search-for-group-box-in-timesheets-preferences-page.png)

   타임시트 및 시간 환경 설정 페이지가 선택한 그룹에 대한 환경 설정으로 업데이트됩니다. 그룹 수준 환경 설정을 수정하려면 시스템 수준 환경 설정 잠금을 해제해야 합니다. 자세한 내용은 섹션을 참조하십시오 [그룹에 대한 타임시트 및 시간 환경 설정 잠금 해제](#unlock-timesheet-and-hour-preferences-for-groups) 이 문서에서.

1. 다음에서 **[!UICONTROL 일반 환경 설정]** 섹션에서 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Log time for future dates]</td> 
      <td> <p>사용자가 시스템 전체에서 미래 날짜에 대한 시간을 기록할 수 있도록 해줍니다.</p> 
       <ul> 
        <li>로그 시간에 액세스할 수 있는 모든 프로젝트, 작업 및 문제</li> 
        <li>일반 시간으로서의 타임시트</li> 
       </ul> <p>이 기능은 사용자가 사무실을 비울 예정이고 해당 시간을 미리 기록하려는 경우 유용합니다.</p> <p><b>참고</b>:</p> 
       <p>마감 또는 취소된 작업 또는 문제에 사용자가 시간을 기록하는 것을 방지할 수 없습니다. 사용자가 완료 또는 중단된 프로젝트에 시간을 기록하지 못하도록 할 수만 있습니다. 작업 및 문제 목록에서 필터를 사용하여 완료되거나 취소된 작업을 사용자가 볼 수 없도록 제외하는 것이 좋습니다.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL 시간 항목에 수동으로 작업 역할 할당]</td> 
      <td> <p>사용자가 사용자 프로필에 할당되거나 객체에 할당된 작업 역할을 수동으로 선택할 수 있습니다.</p> <p><b>중요 사항</b>:  
        <ul> 
         <li>작업 역할을 시간 항목에 할당한 후 이 설정을 사용하지 않으면 사용자는 프로젝트, 작업 또는 문제의 [!UICONTROL 시간] 탭에서 다양한 역할에 기록된 시간을 조정해야 합니다.</li> 
         <li>사용자에게 프로필에 할당된 작업 역할이 없고 [!UICONTROL Advanced Assignments] 대화 상자에 [!UICONTROL Task Owner](으)로 할당된 작업이 있는 경우 사용자가 작업에 시간을 기록할 때 해당 작업 역할이 표시됩니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 타임시트 편집을 소유자 및 관리자로 제한]</td> 
      <td> <p>타임시트 소유자로 편집 제한 및 [!DNL Workfront] 관리자. 이 옵션이 비활성화되면 타임시트는 다음 작업으로도 편집할 수 있습니다.</p> 
       <ul> 
        <li> <p>타임시트에 대한 관리 액세스 권한과 액세스 수준의 시간이 있는 사용자</p> </li> 
        <li> <p>타임시트에서 "시간 편집 가능"이 활성화된 경우 타임시트 승인자</p> </li> 
        <li> <p>타임시트 소유자의 관리자</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 시간 편집을 소유자 및 관리자로 제한]</td> 
      <td>시간 및 시간을 입력하는 사용자로 편집 제한 [!DNL Workfront] 관리자. 이 설정은 프로젝트 또는 시간 보고서의 [!UICONTROL 시간] 탭에 적용됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 다음에서 **[!UICONTROL 사용자가 시간을 기록할 수 있는 위치]** 섹션에서 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto">
    <tr>
        <td>프로젝트에서 바로 [!UICONTROL]</td>
        <td>사용자가 프로젝트에 시간을 기록할 수 있습니다([!UICONTROL 업데이트] 탭과 타임시트 모두). 사용자가 프로젝트 수준에서 시간을 기록하지 않는 경우 이 옵션은 선택하지 않은 상태로 유지되어야 합니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 완료된 프로젝트에서]</td>
        <td>사용자가 완료로 표시된 프로젝트의 시간을 기록할 수 있습니다. 이 옵션이 비활성화되면 사용자는 [!UICONTROL 완료] 상태의 프로젝트에서 완료한 작업의 시간을 기록할 수 없습니다.</td>
    </tr>
    <tr>
        <td>[!UICONTROL 중단된 프로젝트에서]</td>
        <td>이 옵션이 활성화되면 사용자는 [!UICONTROL 중단] 상태인 프로젝트에 시간을 기록할 수 있습니다.</td>
    </tr>
   </table>

1. 다음에서 **[!UICONTROL 타임시트 미리 채우기]** 섹션에서 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">내에 있는 [!UICONTROL 작업] &lt;number of="" weeks=""&gt; 타임시트의 작업 범위에 대한 [!UICONTROL]</td> 
      <td> <p>사용자에게 할당된 작업 및 문제의 날짜가 포함된 타임시트의 날짜 범위 전후 주 수를 정의합니다.</p> 
      <p>기본 설정은 1주이며 이 범위를 4주로 확장할 수 있습니다.</p> 
      <p>즉, 범위에 대해 4주를 선택하는 경우, 타임시트의 일자 범위 전 4주부터 타임시트의 일자 범위 후 4주까지의 일자 범위가 있는 작업 및 문제로 타임시트가 미리 채워집니다. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 완료된 작업 및 문제]</td> 
      <td>일반적으로 여러 리소스가 단일 작업에 할당되는 경우 이 설정을 사용하는 것이 좋습니다. 즉, 한 리소스가 작업에 시간을 기록하고 완료로 표시하면 작업에 할당된 다른 리소스가 여전히 타임시트에서 작업 또는 문제를 찾아 시간을 기록할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 타임시트의 일자 범위에 계획된 일자가 있는 작업 및 문제]</td> 
      <td> <p>선택한 경우 타임시트에는 타임시트의 날짜 범위에 계획된 시작 일자 또는 완료 일자가 있는 작업 및 문제가 포함됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> 타임시트의 일자 범위에 예상 일자가 있는 [!UICONTROL 작업]</td> 
      <td> <p>이 옵션을 선택하면 문제나 작업의 계획된 일자가 타임시트 일자 범위를 벗어나는 경우에도 프로젝트의 기간 내에 예상 시작 일자 또는 완료 일자가 있는 작업이 타임시트에 포함됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 다음에서 **[!UICONTROL 프로젝트, 작업 및 문제 삭제됨]** 섹션에서 다음을 지정합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 프로젝트 삭제 시</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL 타임시트에 이미 추가된 로그 시간을 일반 시간으로 유지]</strong>: 이 프로젝트가 나중에 복원되면 타임시트에 시간이 유지됩니다.</li> 
        <li><strong>[!UICONTROL 기록된 시간을 모두 삭제]</strong>: 이 프로젝트가 나중에 복원되면 이미 기록된 시간이 프로젝트에 복원됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">작업 또는 문제 삭제 시</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL 기록된 시간을 프로젝트로 이동]</strong> 작업 또는 문제가 있는 위치: 이 작업 또는 문제가 나중에 복원되면 프로젝트에 시간이 유지됩니다.<br></li> 
        <li> <p><strong>[!UICONTROL 기록된 시간을 모두 삭제]</strong>: 이 작업 또는 문제가 나중에 복원되면 기록된 시간이 작업 또는 문제에 복원됩니다.</p> <p>이러한 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configure impact]을(를) 개체가 삭제되고 복원되는 시간에 설정</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 그룹에 대한 타임시트 및 시간 환경 설정 잠금 해제

조직의 그룹은 고유한 워크플로우에 대해 다르게 구성된 타임시트 또는 시간 환경 설정이 필요할 수 있습니다. 조직 전체에서 모든 그룹이 스스로 구성할 수 있도록 해당 그룹의 환경 설정을 잠금 해제할 수 있습니다.

환경 설정이 잠금 해제되고 그룹 관리자가 수정할 때 그룹이 홈 그룹인 경우 타임시트 소유자에게 영향을 줍니다.

그룹 관리자가 그룹에 대한 타임시트 및 시간 환경 설정을 구성하는 방법에 대한 자세한 내용은 [그룹에 대한 타임시트 및 시간 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>다음 이후 [!DNL Workfront] 관리자는 시스템 수준에서 환경 설정을 잠금 해제하고, 모든 그룹 관리자가 이를 구성한 다음 잠가서 그룹의 모든 사람과 아래의 하위 그룹이 동일한 구성을 사용하도록 할 수 있습니다. 이는 다음과 같은 기능과 병행됩니다. [!DNL Workfront] 관리자는 시스템 내의 모든 사용자에 대한 기본 설정을 구성하고 잠가야 합니다. 자세한 내용은 [그룹 타임시트 및 시간 환경 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

그룹이 구성할 수 있도록 프로젝트 환경 설정을 잠금 해제하려면 다음 작업을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 패널에서 **[!UICONTROL 타임시트 및 시간]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL 환경 설정]**.

1. 다음 중 하나를 수행합니다.

   * 그룹 관리자가 그룹에 대한 기본 설정을 구성할 수 있도록 하려면 **잠금 해제** 전환 ![](assets/unlock-toggle-button.png) 을 클릭하여 잠금을 해제합니다.
   * 모든 그룹이 환경 설정에 대한 구성을 사용하도록 하려면 전환이 잠겨 있는지 확인합니다 ![](assets/locked-preference-toggle.png) (기본값).

     >[!IMPORTANT]
     >
     >모든 요구 사항이 잠긴 기본 설정을 구성하는 방식으로 처리되도록 시스템 전체에서 그룹 관리자 및 사용자와 통신하는 것이 좋습니다.
     >
     >이 구성을 잠그면 시스템의 모든 그룹에서 해당 구성을 상속합니다. 또한 환경 설정이 일정 기간 동안 잠금 해제된 경우 구성은 그룹 관리자가 수행했을 수 있는 설정을 대체합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
