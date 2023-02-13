---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 작업표 및 시간 환경 설정 구성
description: 로서의 [!DNL Adobe Workfront] 관리자는 작업표와 시간에 대한 기본 설정을 지정할 수 있습니다. [!DNL Workfront] 작업표에서 미리 채울 수 있는 항목과 사용자가 로그할 수 있는 항목을 정의하려면
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 1%

---

# 작업표 및 시간 환경 설정 구성

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

로서의 [!DNL Adobe Workfront] 관리자는 작업표와 시간에 대한 기본 설정을 지정할 수 있습니다. [!DNL Workfront] 작업표에서 미리 채울 수 있는 항목과 사용자가 로그할 수 있는 항목을 정의하려면

작업표에 대한 변경 사항은 나중에 생성되는 모든 작업표에 영향을 줍니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이선스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>넌 [!DNL Workfront] 관리자</p> <p><b>메모</b>

여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 작업표 및 시간 환경 설정 지정

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 작업표 및 시간]** > **[!UICONTROL 기본 설정]**.

1. 표시되는 페이지에서 **[!UICONTROL 일반 환경 설정]** 섹션에서 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 미래 날짜에 대한 로그 시간]</td> 
      <td> <p>다음 위치에서 시스템 전체에서 향후 날짜에 대한 시간을 기록할 수 있습니다.</p> 
       <ul> 
        <li>로그 시간에 액세스할 수 있는 모든 프로젝트, 작업 및 문제</li> 
        <li>일반 시간으로 작업표</li> 
       </ul> <p>이 기능은 사용자가 사무실을 비울 계획이며 해당 시간을 미리 기록하려는 경우 유용합니다.</p> <p><b>참고</b>: 사용자가 닫혀 있거나 취소된 작업이나 문제에 대해 시간을 기록하는 것을 방지할 수 없습니다. 사용자가 전체 또는 데드 프로젝트에 대한 시간을 기록하지 못하도록 할 수만 있습니다. 작업 및 문제 목록에서 필터를 사용하여 완료되었거나 취소된 작업이 사용자에게 표시되지 않도록 하는 것이 좋습니다.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL 작업 역할을 시간 항목에 수동으로 할당]</td> 
      <td> <p>사용자가 사용자 프로필에 할당되거나 객체에 할당된 작업 역할을 수동으로 선택할 수 있도록 허용합니다.</p> <p><b>중요 사항</b>:  
        <ul> 
         <li>작업 역할을 시간 항목에 할당한 후에 이 설정을 사용하지 않도록 설정하면 사용자는 프로젝트, 작업 또는 문제의 [!UICONTROL 시간] 탭에서 다양한 역할에 따라 기록된 시간을 조정해야 합니다.</li> 
         <li>사용자에게 프로필에 할당된 작업 역할이 없고 [!UICONTROL 고급 할당] 대화 상자에 [!UICONTROL 작업 소유자]로 할당된 작업이 있는 경우 사용자가 작업 시간을 기록하면 해당 작업 역할이 나타납니다.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 작업표 편집을 소유자 및 관리자로 제한]</td> 
      <td> <p>작업표 소유자 및 [!DNL Workfront] 관리자 이 옵션을 비활성화하면 작업표를 다음 방법으로 편집할 수도 있습니다.</p> 
       <ul> 
        <li> <p>작업표와 액세스 수준의 시간에 대한 관리자 액세스 권한이 있는 사용자</p> </li> 
        <li> <p>작업표에서 "시간 편집 가능"을 사용하는 경우 작업표 승인자</p> </li> 
        <li> <p>작업표 소유자의 관리자</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 소유자 및 관리자로 시간 편집 제한]</td> 
      <td>시간 및 시간을 입력하는 사용자로 편집 제한 [!DNL Workfront] 관리자 이 설정은 프로젝트 또는 시간 보고서의 [!UICONTROL 시간] 탭에 적용됩니다.</td> 
     </tr> 
    </tbody> 
   </table>

1. 에서 **[!UICONTROL 로깅 시간]** 섹션에서 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 프로젝트에서 직접 시간 기록]</td>
        <td>사용자가 프로젝트에 대한 시간을 기록할 수 있도록 합니다( [!UICONTROL 업데이트] 탭과 작업표). 사용자가 프로젝트 수준에서 시간을 기록하지 않는 경우 이 옵션은 선택 취소되어 있어야 합니다.</td>
    </tr>
    <tr>
        <td>완료된 프로젝트에 시간을 기록하십시오</td>
        <td>사용자가 완료된 것으로 표시된 프로젝트에 시간을 기록할 수 있습니다. 이 옵션을 비활성화하면 [!UICONTROL 완료] 상태의 프로젝트에서 완료된 작업에 대한 시간을 기록할 수 없습니다.</td>
    </tr>
    <tr>
        <td>중단된 프로젝트에 시간을 기록합니다</td>
        <td>이 옵션이 활성화되면 사용자는 [!UICONTROL 데드] 상태로 프로젝트에 대한 시간을 기록할 수 있습니다.</td>
    </tr>
   </table>

1. 에서 **[!UICONTROL 작업표를 미리 채우기]**&#x200B;섹션에서 &#x200B; 다음 옵션 중 하나를 구성합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 내에 있는 작업] &lt;number of="" weeks=""&gt; 작업표 작업 범위의 [!UICONTROL]</td> 
      <td> <p>사용자에게 할당된 작업 및 문제의 날짜가 포함된 작업표의 날짜 범위 전후의 주 수를 정의합니다. 기본 설정은 1주이며 이 범위를 4주로 확장할 수 있습니다. 즉, 작업표에 작업표의 날짜 범위 이전 4주 사이의 날짜가 있는 작업 및 문제로 미리 채워져 있습니다. 작업표의 날짜 범위 이후 최대 4주(해당 범위에 대해 4주를 선택하면) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 완료된 작업 및 문제]</td> 
      <td>일반적으로 여러 리소스가 단일 작업에 할당되는 경우 이 설정을 사용하는 것이 좋습니다. 즉, 한 리소스가 작업에 대해 시간을 기록하고 완료된 것으로 표시하면 작업에 할당된 다른 리소스가 작업 또는 문제를 작업표에서 찾아 해당 시간을 기록할 수 있습니다.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 작업표의 날짜 범위에 계획된 날짜가 있는 작업 및 문제]</td> 
      <td> <p>선택한 경우 작업표에 작업표의 날짜 범위 내에 있는 계획 시작 날짜나 완료 날짜가 있는 작업 및 문제가 포함됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL 작업표의 날짜 범위에 예상 날짜가 있는 작업]</td> 
      <td> <p>선택한 경우, 작업표에 예상 시작 날짜 또는 완료 날짜가 프로젝트의 시간 기간 내에 있는 작업이 포함되며, 해당 문제 또는 작업의 계획된 날짜가 작업표 날짜 범위를 벗어나는 경우에도 작업표에 포함된 작업이 포함됩니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 에서 **[!UICONTROL 프로젝트, 작업 또는 문제 삭제 환경 설정]** 섹션에서 다음을 지정합니다.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Better title would be Deleting projects, tasks, and issues</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 프로젝트 삭제 시]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL 로그인이 이미 작업표에 추가된 시간을 일반 시간으로 유지합니다.]</strong>: 이 프로젝트를 나중에 복원하면 작업표에 시간이 남아 있습니다.</li> 
        <li><strong>[!UICONTROL 기록된 모든 시간 삭제]</strong>: 이 프로젝트를 나중에 복원하면 이미 기록된 시간이 프로젝트에 복원됩니다.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 작업 또는 문제 삭제 시]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL 로그된 시간을 작업 또는 문제가 있는 프로젝트로 이동]</strong>: 이 작업이나 문제가 나중에 복원되면 시간이 프로젝트에 남아 있습니다.<br></li> 
        <li> <p><strong>[!UICONTROL 기록된 모든 시간 삭제]</strong>: 이 작업이나 문제가 나중에 복원되면 로그된 시간이 작업이나 문제로 복원됩니다.</p> <p>이러한 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configure Imperts]는 개체를 삭제하고 복원한 시간 후에 적용됩니다</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 그룹에 대한 작업표 및 시간 환경 설정 잠금 해제

조직의 그룹은 고유한 워크플로우에 대해 다르게 구성된 작업표 또는 시간 기본 설정이 필요할 수 있습니다. 조직 전체에서 모든 그룹에 대한 기본 설정을 잠금 해제하여 자신이 직접 구성할 수 있습니다.

기본 설정이 잠금 해제되어 그룹 관리자가 이를 수정하면, 해당 그룹이 홈 그룹인 경우 작업표 소유자에 영향을 줍니다.

그룹 관리자가 그룹의 작업표 및 시간 환경 설정을 구성하는 방법에 대한 자세한 내용은 [그룹에 대한 작업표 및 시간 환경 설정 구성](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>후 [!DNL Workfront] 관리자는 시스템 수준에서 기본 설정을 잠금 해제하면 모든 그룹 관리자가 해당 설정을 구성한 다음 잠근 후 해당 그룹의 모든 사람과 아래 하위 그룹이 동일한 구성을 사용하도록 할 수 있습니다. 이것은 [!DNL Workfront] 관리자는 시스템의 모든 사용자에 대한 환경 설정을 구성하고 잠그어야 합니다. 자세한 내용은 [그룹 작업표 및 시간 기본 설정 잠금 또는 잠금 해제](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

그룹이 프로젝트 환경 설정을 구성할 수 있도록 프로젝트 환경 설정을 잠금 해제하려면 다음을 수행하십시오.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe] Workfront을 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 왼쪽 패널에서 **[!UICONTROL 작업표 및 시간]**&#x200B;를 클릭한 다음 **[!UICONTROL 기본 설정]**.

1. 다음 중 하나를 수행합니다.

   * 그룹 관리자가 해당 그룹에 대한 환경 설정을 구성할 수 있도록 하려면 그룹 잠금을 해제하십시오 ![](assets/unlock-toggle-button.png).
   * 모든 그룹이 기본 설정에 대한 구성을 사용하려면 구성이 잠겼는지 확인합니다(기본값).

      >[!IMPORTANT]
      >
      >잠긴 기본 설정을 구성하는 방식으로 모든 요구 사항을 처리하도록 시스템 전체에서 관리자 및 그룹의 사용자와 통신하는 것이 좋습니다. 잠글 때 시스템의 모든 그룹에 의해 구성이 상속됩니다. 그리고 특정 기간 동안 기본 설정 잠금이 해제되어 있으면 해당 그룹 관리자가 만들 수 있는 구성 대신

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
