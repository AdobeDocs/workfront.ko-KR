---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 시간 또는 일 단위로 로그인 여부 구성
description: 플랜 라이센스가 있는 사용자는 Adobe Workfront에서 시간을 몇 시간 또는 며칠 단위로 기록하는지를 구성할 수 있습니다. 시스템 관리자는 개별 사용자 또는 조직의 여러 사용자에 대해 이 설정을 구성할 수 있습니다. 기본적으로 사용자는 시간을 시간 단위로 기록합니다.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 시간 또는 일 단위로 로그인 여부 구성

계획자 라이센스가 있는 사용자는 Adobe Workfront에서 시간을 몇 시간 또는 며칠 단위로 기록하는지를 구성할 수 있습니다. 시스템 관리자는 개별 사용자 또는 조직의 여러 사용자에 대해 이 설정을 구성할 수 있습니다. 기본적으로 사용자는 시간을 시간 단위로 기록합니다. Workfront에서 시간을 기록하는 방법에 대한 자세한 내용은 [로그 시간](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>보고 정확도를 위해 조직 전체에서 시간 또는 일과 같은 방식으로 로깅 시간을 사용하는 것이 좋습니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>플랜 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>기획자들은 스스로 시간을 구성할 수 있다. Workfront 관리자만 다른 사용자에 대한 시간을 구성할 수 있습니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

1. 시스템의 목표 및 액세스 수준에 따라 다음 중 하나를 수행합니다.

   * **계획자 사용자가 직접 시간 로깅을 구성합니다.** 을(를) 클릭합니다. **기본 메뉴** 아이콘 ![](assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 프로필 사진 옆에 있는 사용자 이름을 클릭합니다. 그런 다음 **자세히** 이름 옆에 있는 아이콘을 선택하고 **편집**.

   * **시스템 관리자가 다른 사용자에 대해 시간 로깅을 구성하는 중:** 에 설명된 대로 하나 이상의 사용자 계정 편집을 시작합니다. [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 결과 대화 상자의 **리소스 계획** 섹션에서 **로그인 시간** 선택 사항입니다.

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (조건부) 여러 사용자를 동시에 편집하는 시스템 관리자는 **로그인 시간**.
1. 로깅 시간을 위해 다음 옵션 중에서 선택합니다.

   | 옵션 | 설명 |
   |---|---|
   | **시간** | 사용자는 Workfront에서 시간을 로깅할 때 시간을 지정합니다. |
   | **일** | 사용자는 Workfront에서 시간을 기록할 때 일수를 지정합니다. |

1. (조건부) 일 단위로 시간을 기록하도록 선택한 경우, **전체 Workday에 해당하는 시간** 필드, 하루 동안의 시간 수를 입력합니다. 사용자의 작업표에 나오는 하루는 여기에서 입력하는 시간과 같습니다.

   이 설정을 구성할 때는 다음 사항을 고려하십시오.

   * 이 옵션은 구성 시 시간 단위로 로그인할 수 없습니다.
   * 이 옵션은 로깅 시간에만 사용됩니다. 이 옵션은 **예약** 옵션을 사용할 수도 있습니다. 다음 **예약** 옵션은 타임라인과 Workfront의 다른 영역에서 계산할 때 사용됩니다. (사용 방법에 대한 자세한 정보 **예약** 옵션을 참조하십시오. [예약 만들기](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)) 

1. 클릭 **변경 내용 저장**.
