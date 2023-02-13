---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 에서 개인 시간 초과 구성 [!DNL Adobe Workfront]
description: Adobe Workfront은 개인 휴직을 관리, 발생 및 추적하기 위해 기존 시스템을 복제하거나 교체하도록 설계되지 않았습니다. 그러나 승인된 휴가가 발생하는 시점을 표시하는 것이 중요합니다. 왜냐하면 이 작업은 일정에 영향을 주고 지정된 작업의 계획 완료 날짜에 영향을 주기 때문입니다.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e87f2a459314b8059a3df634e97560b5c1dffac4
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 1%

---

# 에서 개인 시간 초과 구성 [!DNL Adobe Workfront]

[!DNL Adobe Workfront] 는 개인 휴직을 관리, 발생 및 추적하기 위해 기존 시스템을 복제하거나 교체하도록 설계되지 않았습니다.

하지만 승인된 시간이 발생하는 시점을 표시하는 것이 중요합니다. 왜냐하면 이것은 일정에 영향을 주고 [!UICONTROL 계획 완료 일자] 할당된 작업 중

예를 들어, 2주 정도 걸릴 예정인 작업에 할당되어 해당 시간 동안 3일 휴가를 받을 계획이라면, [!DNL Workfront] 해제 시간을 계산하기 위해 작업 타임라인에 3일을 추가합니다.

또한 자원 관리 도구에서는 개인 휴무를 사용하여 작업 일정을 예약할 수 있는 시기를 표시합니다.

>[!NOTE]
>
>오프하기로 예약한 날짜와 일치하지 않는 경우가 생기지 않도록 사용자 프로필의 시간대가 예약의 시간대와 일치하는지 확인하는 것이 좋습니다. 자세한 내용은 다음 문서를 참조하십시오.
>
>* [예약 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>




## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Work] 이상(개인 시간 설정)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td>[!UICONTROL Edit User] 액세스 권한이 있는 [!UICONTROL Manager](다른 사용자의 시간 제한 달력에 변경)</td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 에서 개인 시간 초과 구성 [!DNL Workfront]

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]을 클릭한 다음 프로필 사진 옆에 있는 사용자 이름을 클릭합니다.

1. 왼쪽 패널에서 **[!UICONTROL 해제 시간]**.
1. 개인 휴가에 대해 원하는 날짜를 선택합니다.
1. 선택 **[!UICONTROL 하루 종일]**&#x200B;하루 종일 쉬는 경우\
   하루 중 하루를 쉬고 있고, 쉬는 시간의 시작 및 종료 시간을 나타내는 경우 선택하지 않은 상태로 둡니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.\
   이제 쉬는 시간이 [!DNL Workfront] 시스템(리소스 그리드 등)을 참조하십시오. 이 시간 동안 작업이 할당되면 예약된 해제 시간을 사용자에게 알려주는 도구 설명이 나타납니다.
