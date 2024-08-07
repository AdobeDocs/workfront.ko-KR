---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 시간이 시간 단위로 기록되는지 또는 일 단위로 기록되는지 구성
description: 플랜 라이선스가 있는 사용자는 Adobe Workfront에 시간을 몇 시간 또는 며칠 단위로 기록할지 여부를 구성할 수 있습니다. 시스템 관리자는 개별 사용자 또는 조직의 여러 사용자에 대해 이 설정을 구성할 수 있습니다. 기본적으로 사용자는 시간을 시간 단위로 기록합니다.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 시간이 시간 단위로 기록되는지 또는 일 단위로 기록되는지 구성

플래너 라이선스를 가진 사용자는 Adobe Workfront에 시간을 몇 시간 단위로 기록할지 또는 며칠 단위로 기록할지 구성할 수 있습니다. 시스템 관리자는 개별 사용자 또는 조직의 여러 사용자에 대해 이 설정을 구성할 수 있습니다. 기본적으로 사용자는 시간을 시간 단위로 기록합니다. Workfront에서 시간을 기록하는 방법에 대한 자세한 내용은 [시간 기록](../../timesheets/create-and-manage-timesheets/log-time.md)을 참조하세요.

>[!NOTE]
>
>보고 정확성을 보장하기 위해 조직 전체에서 동일한 방법(시간 또는 일)으로 시간을 로깅하는 것이 좋습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이센스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>플래너는 스스로 시간을 구성할 수 있습니다. Workfront 관리자만 다른 사용자의 시간을 구성할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 확인하려면 Workfront 관리자에게 문의하십시오.

1. 목표와 시스템의 액세스 수준에 따라 다음 중 하나를 수행합니다.

   * **플래너 사용자 스스로 시간 로깅 구성:** Adobe Workfront 오른쪽 상단에 있는 **주 메뉴** 아이콘 ![](assets/main-menu-icon.png)을(를) 클릭한 다음 프로필 사진 옆에 있는 사용자 이름을 클릭합니다. 그런 다음 이름 옆에 있는 **자세히** 아이콘을 클릭하고 **편집**&#x200B;을 선택합니다.

   * **시스템 관리자가 다른 사용자에 대한 시간 로깅을 구성하는 중:** [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)에 설명된 대로 하나 이상의 사용자 계정을 편집하기 시작합니다.

1. 결과 대화 상자의 **리소스 계획** 섹션에서 **시간 기록** 옵션을 찾습니다.

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (조건부) 여러 사용자를 동시에 편집하는 시스템 관리자인 경우 **시간 기록**&#x200B;을 선택하십시오.
1. 로깅 시간에 대해 다음 옵션 중에서 선택합니다.

   | 옵션 | 설명 |
   |---|---|
   | **시간** | 사용자는 Workfront에서 시간을 기록할 때 시간을 지정합니다. |
   | **일** | 사용자는 Workfront에서 시간을 기록할 때 일을 지정합니다. |

1. (조건부) 일 단위로 시간을 기록하도록 선택한 경우 **전체 Workday에 해당하는 시간** 필드에 전일과 같은 시간 수를 입력합니다. 사용자의 타임시트에서 1일은 여기에 입력한 시간과 동일합니다.

   이 설정을 구성할 때는 다음 사항을 고려하십시오.

   * 시간을 시간 단위로 기록하도록 구성할 때는 이 옵션을 사용할 수 없습니다.
   * 이 옵션은 시간을 기록하기 위한 목적으로만 사용됩니다. 이 옵션은 사용자를 편집할 때도 사용할 수 있는 **일정** 옵션과 관련이 없습니다. **일정** 옵션은 타임라인과 Workfront의 다른 영역에서 시간을 계산할 때 사용됩니다. **일정** 옵션 사용에 대한 자세한 내용은 [일정 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)를 참조하십시오. 

1. **변경 내용 저장**&#x200B;을 클릭합니다.
