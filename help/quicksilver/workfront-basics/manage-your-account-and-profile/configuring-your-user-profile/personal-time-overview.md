---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 개인 휴무 구성
description: 승인된 휴무는 일정에 영향을 주고 할당된 작업의 계획된 완료 일자에 영향을 주기 때문에 Adobe Workfront에 시간을 표시하는 것이 중요합니다.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 1%

---

# 개인 휴무 구성

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront]은(는) 개인 휴무를 관리, 계산 및 추적하기 위해 기존 시스템을 복제하거나 대체하도록 설계되지 않았습니다.

그러나 승인된 휴무가 발생하는 시기를 표시하는 것이 중요합니다. 이는 사용자의 일정과 할당된 작업의 [!UICONTROL 계획된 완료 일자]에 모두 영향을 미치기 때문입니다.

예를 들어, 2주가 걸릴 예정인 작업에 할당되어 있고 해당 시간 동안 3일을 쉴 계획이라면, [!DNL Workfront]은(는) 휴무를 고려하여 작업 타임라인에 3일을 추가합니다.

또한 자원 관리 도구는 개인 휴무를 사용하여 작업 일정을 잡을 수 있는 시기를 나타냅니다.

>[!NOTE]
>
>휴무를 예약하는 날짜와 불일치가 발생하지 않도록 사용자 프로필의 시간대가 예약의 시간대와 일치하는 것이 좋습니다. 자세한 내용은 다음 문서를 참조하십시오.
>
>* [일정 만들기](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [사용자 프로필 편집](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 라이센스</td> 
   <td> <p>새로운 기능: 표준(개인 휴무 구성)</p>
        <p>또는</p>
        <p>현재: 회사 또는 그 이상(개인 휴무 구성)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>[!UICONTROL Edit User] 액세스 권한이 있는 [!UICONTROL Manager](다른 사용자의 휴무 달력을 변경하기 위해)<br>
   <strong>참고:</strong> 관리자가 다른 사용자의 개인 휴무 일정을 편집하면 모든 항목이 관리자의 표준 시간대가 아니라 사용자의 표준 시간대로 표시됩니다.</td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## [!DNL Workfront]에서 개인 휴무 구성

{{step1-click-profile-pic}}

1. 왼쪽 패널에서 **[!UICONTROL 휴무]**&#x200B;를 클릭합니다.
1. 개인 휴무에 대해 원하는 날짜를 선택합니다.

   ![개인 휴무 일정](assets/personal-time-off-calendar.png)

1. 하루 종일 쉬려면 **[!UICONTROL 하루 종일]**&#x200B;을 선택하세요.

   하루 미만의 휴무를 수행하는 경우 확인란을 선택 취소한 상태로 두고 휴무 시작 및 종료 시간을 나타냅니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 리소스 플래너 및 업무 균형자 같은 리소스 관리 도구의 [!DNL Workfront] 시스템에서 휴무를 볼 수 있습니다. 이 시간 동안 작업에 할당되면 도구 팁은 사용자에게 휴무가 예약되었음을 알려줍니다.
