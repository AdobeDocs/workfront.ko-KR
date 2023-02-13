---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 리소스 관리 환경 설정 구성
description: 로서의 [!DNL Adobe Workfront] 관리자는 시스템에 대한 리소스 관리 기본 설정을 구성할 수 있습니다. 이러한 자원 관리 환경설정은 사용자 가용성 또는 능력 및 FTE가 [!DNL Workfront] 리소스 예약 및 계획 도구
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 80ad604330e8b55037f1607b754cc8bb34f6a3ec
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 구성 [!UICONTROL 리소스 관리] 환경 설정

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<!--drafted for Work time field: <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

로서의 [!DNL Adobe Workfront] 관리자는 다음을 구성할 수 있습니다 [!UICONTROL 리소스 관리] 시스템에 대한 기본 설정입니다. 이러한 기본 설정은 사용자 시간 또는 FTE 가용성 또는 능력이 [!DNL Workfront] 리소스 예약 및 계획 도구

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

이 문서의 절차를 수행하려면 다음 사항이 있어야 합니다.

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
   <td> <p>시스템 관리자 액세스 수준</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> <p><b>메모</b>:

여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
 </tbody> 
</table>

<!--drafted for Work time field: 

## Information taken into account when calculating user's capacity

When calculating a user's capacity, Workfront takes into account the following information:

* The number of scheduled hours, as defined in either the Schedule of the user or the Workfront system's [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (depending on which [!UICONTROL Schedule] is used, it can be the exceptions of the user's schedule, or those associated with the [!DNL Workfront] [!UICONTROL Default Schedule])
* User's time off
* The value of the Full Time Equivalent ([!UICONTROL FTE]) of the user or that of the [!DNL Workfront] system. The [!UICONTROL FTE] equals 1 when the user works full time, as defined in the schedule. 

<!-drafted for Work Time field  

* <span class="preview">The value of [!UICONTROL Work Time] for the user which refers to time that the user spends on project-related work. This does not include overhead time, like meetings and training. The [!UICONTROL Work Time] equals 1 when the user is available for work the entire time as indicated by the [!UICONTROL FTE] or the schedule, which means they don't spend any time in non-project-related work like meetings or trainings.</span>

-->

의 자원 계획 및 스케줄링에 대한 정보 [!DNL Workfront]를 참조하십시오. [리소스 관리 시작](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

—>

## 구성 [!UICONTROL 리소스 관리] 환경 설정

>[!NOTE]
>
>전역 설정이므로 이 옵션은 전체 시스템, 모든 사용자, 모든 리소스 관리 도구 및 모든 리소스 풀에 대한 모든 계산에 영향을 줍니다.

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).
1. 클릭 **[!UICONTROL 리소스 관리]**.
1. 다음 방법 중 하나를 선택하여 [!DNL Workfront]:

   * **기본 예약**: [!DNL Workfront] 시스템의 기본 일정 및 사용자의 개별 FTE를 사용하여 리소스 관리 도구에서 사용자의 사용 가능한 시간을 계산합니다.

      예약에 대한 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      사용자 값에 대한 자세한 정보 [!UICONTROL FTE]를 참조하십시오.  [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront은 Workfront 관리자가 [다음]을 선택하면 다음 공식을 사용하여 사용자의 [사용 가능한 시간]을 계산합니다 [!UICONTROL 기본 예약]:

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > 예를 들어 [!UICONTROL 기본 예약] 일주일에 40시간이고 [!UICONTROL FTE] 사용자의 프로필은 0.5이며, 사용자는 일주일에 20시간 동안 작업할 수 있습니다.
      >사용자에게 하루 중 1시간 비우기 시간이 있는 경우 사용 가능한 시간은 다음과 같이 계산됩니다.
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
   <!--drafted for Work Time field

      <div class="preview">
      
      In the Preview environment: 

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >For example, if the Default Schedule is 40 hours a week,  the FTE in the profile of the user is 0.5, the user has 1 hour of Time off one day, and the [!UICONTROL Work Time] in the profile of the user is 0.5, the user is available for actual project work for 9.5 hours a week.
      >
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>

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

   * **사용자 일정**: [!DNL Workfront] 는 사용자의 일정과 [!UICONTROL 기본 예약] 사용 가능 [!UICONTROL FTE] 리소스 관리 도구에서 사용자의 값입니다. 사용 가능한 시간은 사용자의 예약에만 따라 계산됩니다. 의 값 [!UICONTROL FTE] 의 경우 무시됩니다. 기본 설정입니다.

      예약에 대한 자세한 내용은 [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      사용자의 [!UICONTROL 예약]를 참조하십시오.  [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >사용자가 예약과 연관되지 않은 경우, 사용자의 사용 가능한 시간은 [!UICONTROL 기본 예약].

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      사용 가능한 [!UICONTROL FTE] 의 경우, 사용자는 다음 공식을 사용하여 계산됩니다.

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >예를 들어 [!UICONTROL 기본 예약] 는 일주일에 40시간이고 사용자의 일정은 일주일에 30시간, 즉 [!UICONTROL FTE] 의 값은 0.70입니다.
      >  
      >사용자에게 하루 중 2시간 휴가 있는 경우 해당 주별 사용 가능 [!UICONTROL FTE] 는 다음과 같이 계산됩니다.
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <!--drafted for Work Time field:

      <div class="preview">

      In the Preview environment: 
      
      The Available hours for the user is calculated by the following formula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) * [!UICONTROL Work Time]
      ```    

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week, the schedule of the user is 30 hours a week, and the user's [!UICONTROL Work Time] is 0.5 the [!UICONTROL FTE] of the user is 0.35.
      >
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      >
      >```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```
      (************ checking this second other with Dev/ Artur - not sure where Exceptions fit in **********)

      </div>
      -->
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
