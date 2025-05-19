---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 리소스 관리 환경 설정 구성
description: ' [!DNL Adobe Workfront] 관리자는 시스템에 대한 리소스 관리 기본 설정을 구성할 수 있습니다. 이러한 리소스 관리 환경 설정은  [!DNL Workfront] 리소스 예약 및 계획 도구에 대한 사용자 가용성 또는 용량 및 FTE를 계산하는 방법을 결정합니다.'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# [!UICONTROL 리소스 관리] 환경 설정 구성

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

[!DNL Adobe Workfront] 관리자는 시스템에 대한 [!UICONTROL 리소스 관리] 환경 설정을 구성할 수 있습니다. 이 환경 설정은 [!DNL Workfront] 리소스 일정 예약 및 계획 도구에 대한 사용자 시간 또는 FTE 가용성 또는 용량을 계산하는 방법을 결정합니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>새로운 기능: 표준</p>
   또는
   <p>현재: 플랜</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>시스템 관리자</td>
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 사용자의 수용작업량을 계산할 때 고려되는 정보

사용자의 용량을 계산할 때 Workfront은 다음 정보를 고려합니다.

* 사용자의 일정 또는 Workfront 시스템의 기본 일정에 정의된 예약 시간 수입니다.
* 일정 예외(사용되는 일정에 따라, 사용자 일정의 예외이거나 Workfront 기본 일정과 연관된 예외일 수 있음)
* 사용자의 휴무.
* 사용자의 FTE([!UICONTROL FTE]) 또는 [!DNL Workfront] 시스템의 FTE 값입니다. 사용자가 일정에 정의된 대로 전체 시간을 사용하는 경우 [!UICONTROL FTE]은(는) 1입니다.
* 사용자의 [!UICONTROL 작업 시간] 값(사용자가 프로젝트 관련 작업에 소요하는 시간을 나타냄). 여기에는 회의 및 훈련과 같은 오버헤드 시간은 포함되지 않습니다. [!UICONTROL 작업 시간]은(는) 사용자가 [!UICONTROL FTE] 또는 일정에 표시된 전체 시간 동안 작업에 사용할 수 있는 경우 1입니다. 즉, 모임 또는 교육과 같이 프로젝트와 관련되지 않은 작업에 시간을 사용하지 않습니다.


[!DNL Workfront]의 리소스 계획 및 예약에 대한 자세한 내용은 [리소스 관리 시작](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)을 참조하세요.


## [!UICONTROL 리소스 관리] 환경 설정 구성

>[!NOTE]
>
>이 설정은 전역 설정이므로 이 선택 사항은 모든 리소스 관리 도구에서 전체 시스템, 모든 사용자에 대한 모든 계산에 영향을 줍니다.

{{step-1-to-setup}}

1. **[!UICONTROL 리소스 관리]**&#x200B;를 클릭합니다.
1. [!DNL Workfront]에서 사용자의 사용 가능 여부를 계산하려면 다음 방법 중 하나를 선택하십시오.

   * **기본 일정**: [!DNL Workfront]은(는) 시스템의 기본 일정과 사용자의 개별 FTE를 사용하여 리소스 관리 도구에서 사용자의 사용 가능한 시간을 계산합니다.

     자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) 및 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

     이 옵션을 선택하면 Workfront은 다음 공식을 사용하여 사용자의 사용 가능한 시간을 계산합니다.


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >예를 들어, 기본 일정이 일주일에 40시간이고, 사용자 프로필의 FTE가 0.5이고, 1일 휴무가 1시간이고, 사용자 프로필의 [!UICONTROL 작업 시간]이 0.5이며, 사용자는 일주일에 9.5시간 동안 실제 프로젝트 작업에 사용할 수 있습니다.
     >
     >사용자에게 하루 1시간의 휴무가 있는 경우 사용 가능한 시간은 다음과 같이 계산됩니다.
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



     <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **사용자 일정**: [!DNL Workfront]은(는) 시스템의 [!UICONTROL 기본 일정]과 사용자 일정을 사용하여 리소스 관리 도구에서 사용자의 사용 가능한 [!UICONTROL FTE] 값을 계산합니다. 사용 가능한 시간은 사용자의 일정에 따라서만 계산되며 사용자의 [!UICONTROL FTE] 값은 무시됩니다. 기본 설정입니다.

     자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) 및 [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)을 참조하세요.

     >[!NOTE]
     >
     >사용자가 일정과 연결되어 있지 않으면 [!UICONTROL 기본 일정]만 사용하여 사용자의 사용 가능한 시간이 계산됩니다.

     사용자의 가용 시간은 다음 공식에 의해 계산됩니다.


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     사용자에 대해 사용 가능한 [!UICONTROL FTE]은(는) 다음 수식으로 계산됩니다.


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >예를 들어 [!UICONTROL 기본 일정]이 일주일에 40시간이고, 사용자의 일정이 일주일에 30시간이고, 사용자의 [!UICONTROL 작업 시간]이 0.5이고, 사용자의 [!UICONTROL FTE]이 0.35입니다.
     >
     >사용자에게 하루 휴무가 2시간인 경우 주별 사용 가능 시간 [!UICONTROL FTE]은(는) 다음과 같이 계산됩니다.
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
