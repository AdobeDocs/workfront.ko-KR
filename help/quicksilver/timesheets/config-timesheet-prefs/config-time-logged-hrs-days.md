---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 시간이 시간 단위로 기록되는지 또는 일 단위로 기록되는지 구성
description: 플랜 라이선스가 있는 사용자는 Adobe Workfront에 시간을 몇 시간 또는 며칠 단위로 기록할지 여부를 구성할 수 있습니다. 시스템 관리자는 개별 사용자 또는 조직의 여러 사용자에 대해 이 설정을 구성할 수 있습니다. 기본적으로 사용자는 시간을 시간 단위로 기록합니다.
author: Lisa
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b0a3a11a3c04a0969bee99f8e1cea231911f0e6a
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# 시간이 시간 단위로 기록되는지 또는 일 단위로 기록되는지 구성

Standard 또는 Plan 라이선스를 가진 사용자는 Adobe Workfront에서 시간을 몇 시간 또는 며칠 단위로 기록할지 구성할 수 있습니다. 시스템 관리자는 개별 사용자 또는 조직의 여러 사용자에 대해 이 설정을 구성할 수 있습니다. 기본적으로 사용자는 시간을 시간 단위로 기록합니다. Workfront에서 시간을 기록하는 방법에 대한 자세한 내용은 [시간 기록](../../timesheets/create-and-manage-timesheets/log-time.md)을 참조하세요.

>[!NOTE]
>
>보고 정확성을 보장하기 위해 조직 전체에서 동일한 방법(시간 또는 일)으로 시간을 로깅하는 것이 좋습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td><p>표준 및 플랜 사용자는 자신을 위한 시간을 구성할 수 있습니다. Workfront 관리자만 다른 사용자의 시간을 구성할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

1. 목표와 시스템의 액세스 수준에 따라 다음 중 하나를 수행합니다.

   * **표준 또는 플랜 사용자가 스스로 시간 기록을 구성합니다.** Adobe Workfront 오른쪽 상단의 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](assets/main-menu-icon.png)를 클릭한 다음 프로필 사진 옆에 있는 사용자 이름을 클릭합니다. 또는(가능한 경우) 위쪽 탐색 영역에서 프로필 사진을 클릭한 다음 **[!UICONTROL Workfront 프로필]**&#x200B;을 클릭합니다. 그런 다음 이름 옆에 있는 **자세히** 아이콘을 클릭하고 **편집**&#x200B;을 선택합니다.

   * **시스템 관리자가 다른 사용자에 대한 시간 로깅을 구성하는 중:** [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)에 설명된 대로 하나 이상의 사용자 계정을 편집하기 시작합니다.

1. 결과 대화 상자의 **리소스 계획** 섹션에서 **시간 기록** 옵션을 찾습니다.

   ![옵션에 시간 기록](assets/user-profile-log-time-options.png)

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
