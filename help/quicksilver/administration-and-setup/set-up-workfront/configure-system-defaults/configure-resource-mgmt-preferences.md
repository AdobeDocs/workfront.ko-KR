---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 리소스 관리 환경 설정 구성
description: (으)로 [!DNL Adobe Workfront] 관리자 시스템의 리소스 관리 기본 설정을 구성할 수 있습니다. 이러한 자원 관리 환경설정은 다음에 대한 사용자 가용성 또는 능력 및 FTE를 계산하는 방법을 결정합니다. [!DNL Workfront] 자원 스케줄링 및 계획 툴.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# 구성 [!UICONTROL 리소스 관리] 환경 설정

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

(으)로 [!DNL Adobe Workfront] 관리자 다음을 구성할 수 있습니다. [!UICONTROL 리소스 관리] 시스템에 대한 환경 설정. 이러한 환경 설정은 다음에 대한 사용자 시간 또는 FTE 가용성 또는 용량을 계산하는 방법을 결정합니다. [!DNL Workfront] 자원 스케줄링 및 계획 툴.

## 액세스 요구 사항

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

이 문서의 단계를 수행하려면 다음이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>모든</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>시스템 관리자 액세스 수준</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p> <p><b>메모</b>:

아직 액세스 권한이 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에 추가 제한을 설정하는 경우. 자세한 내용: [!DNL Workfront] 관리자가 액세스 수준을 수정할 수 있습니다. 다음을 참조하십시오. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## 사용자의 수용작업량을 계산할 때 고려되는 정보

사용자의 용량을 계산할 때 Workfront은 다음 정보를 고려합니다.

* 사용자 일정 또는 Workfront 시스템에 정의된 예약 시간 수 [!UICONTROL 기본 일정]
* [!UICONTROL 예약] [!UICONTROL 예외] (다음에 따라) [!UICONTROL 예약] 를 사용합니다. 사용자 일정의 예외이거나 와 연관된 예외일 수 있습니다. [!DNL Workfront] [!UICONTROL 기본 일정])
* 사용자 휴무
* Full Time Equivalent( 값[!UICONTROL FTE])을 설정하는 것이 좋습니다. [!DNL Workfront] 시스템. 다음 [!UICONTROL FTE] 사용자가 일정에 정의된 대로 전체 시간을 작업할 때 가 1이 됩니다.
* 값: [!UICONTROL 작업 시간] (프로젝트 관련 작업에 사용자가 소요하는 시간을 나타내는 사용자) 여기에는 회의 및 훈련과 같은 오버헤드 시간은 포함되지 않습니다. 다음 [!UICONTROL 작업 시간] 은 사용자가 다음에 표시된 전체 시간을 작업할 수 있는 경우 1입니다. [!UICONTROL FTE] 또는 일정, 즉 회의 또는 교육 등 프로젝트 관련 이외의 작업에 시간을 전혀 사용하지 않습니다.


의 리소스 계획 및 스케줄링에 대한 자세한 내용 [!DNL Workfront], 참조 [리소스 관리 시작](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## 구성 [!UICONTROL 리소스 관리] 환경 설정

>[!NOTE]
>
>이 설정은 전역 설정이므로 이 선택 사항은 모든 리소스 관리 도구에서 전체 시스템, 모든 사용자에 대한 모든 계산에 영향을 줍니다.

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 클릭 **[!UICONTROL 리소스 관리]**.
1. 다음 방법 중 하나를 선택하여 의 사용자 가용성을 계산합니다. [!DNL Workfront]:

   * **기본 일정**: [!DNL Workfront] 시스템의 기본 일정 및 사용자의 개별 FTE를 사용하여 리소스 관리 도구에서 사용자의 사용 가능한 시간을 계산합니다.

      일정에 대한 자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      사용자 값 찾기에 대한 자세한 정보 [!UICONTROL FTE], 참조  [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront은 Workfront 관리자가 다음을 선택할 때 다음 공식을 사용하여 사용자의 사용 가능한 시간을 계산합니다. [!UICONTROL 기본 일정]:


      `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


      >[!INFO]
      >
      >예를 들어 기본 일정이 일주일에 40시간이고 사용자 프로필의 FTE가 0.5이며 1일 1시간의 휴무가 있는 경우 [!UICONTROL 작업 시간] 사용자의 프로필이 0.5이면 사용자는 주 9.5시간 동안 실제 프로젝트 작업에 참여할 수 있습니다.
      >
      >사용자에게 하루 1시간의 휴무가 있는 경우 사용 가능한 시간은 다음과 같이 계산됩니다.
      >
      >
      >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`

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

   * **사용자의 일정**: [!DNL Workfront] 사용자의 일정과 [!UICONTROL 기본 일정] 사용 가능 여부 계산 시스템 [!UICONTROL FTE] 리소스 관리 도구의 사용자 값입니다. 사용자의 일정에 따라서만 사용 가능한 시간이 계산됩니다. 값 [!UICONTROL FTE] 의 사용자는 무시됩니다. 기본 설정입니다.

      일정에 대한 자세한 내용은 [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      사용자의 [!UICONTROL 예약], 참조  [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >사용자가 일정과 연결되어 있지 않으면 사용자의 사용 가능한 시간은 [!UICONTROL 기본 일정].

      사용자의 가용 시간은 다음 공식에 의해 계산됩니다.


      `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


      사용 가능한 [!UICONTROL FTE] 사용자의 경우 다음 공식에 의해 계산됩니다.


      `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


      >[!INFO]
      >
      >예를 들어 [!UICONTROL 기본 일정] 은 일주일에 40시간이고, 사용자의 일정은 일주일에 30시간이며, 사용자의 [!UICONTROL 작업 시간] 은(는) 0.5임 [!UICONTROL FTE] 사용자의 은(는) 0.35입니다.
      >
      >사용자가 하루 2시간의 휴무를 사용하는 경우 해당 주별 사용 가능 [!UICONTROL FTE] 는 다음과 같이 계산됩니다.
      >
      >
      >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`

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
