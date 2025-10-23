---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 개인 휴무 구성
description: 승인된 휴무는 일정에 영향을 주고 할당된 작업의 계획된 완료 일자에 영향을 주기 때문에 Adobe Workfront에 시간을 표시하는 것이 중요합니다.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e25ea757129e9645f7b5f0729cd498d5947f49f2
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 개인 휴무 구성

<!-- Audited: 12/2023 -->

<span class="preview">이 페이지에서 강조 표시된 정보는 아직 일반적으로 사용할 수 없는 기능을 참조합니다. 미리 보기 샌드박스 환경에서만 사용할 수 있으며 프로덕션에 단계적으로 롤아웃할 때 릴리스됩니다.</span>

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

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Adobe Workfront 패키지</td> 
   <td><p>임의</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront 라이선스</td> 
   <td> <p>개인 휴무를 구성하려면 다음을 수행해야 합니다.</p>
        <p>표준(개인 휴무 구성)</p>
        <p>회사 또는 그 이상(개인 휴무 구성)</p> </td>
  </tr> 
  <tr> 
   <td>액세스 수준 구성</td> 
   <td><p>다른 사용자의 휴무 달력을 변경하려면 해당 사용자의 관리자여야 하며 사용자 편집 액세스 권한이 있어야 합니다.</p>
   <p><strong>참고:</strong> 관리자가 다른 사용자의 개인 휴무 일정을 편집하면 모든 항목이 관리자의 표준 시간대가 아니라 사용자의 표준 시간대로 표시됩니다.</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## [!DNL Workfront]에서 개인 휴무 구성

{{step1-click-profile-pic}}

>[!NOTE]
>
>Adobe 통합 경험을 사용하는 경우 상단 탐색 영역에서 Workfront 계정 메뉴(프로필 사진)를 클릭한 다음 Workfront 프로필을 선택하여 Adobe 프로필에 액세스할 수 있습니다.
>
>![workfront 프로필](assets/aue-profile.png)

1. 왼쪽 패널에서 **[!UICONTROL 휴무]**&#x200B;를 클릭합니다.
1. 개인 휴무에 대해 원하는 날짜를 선택합니다.

   <span class="preview">미리 보기 환경의 샘플 이미지:</span>
   ![개인 휴무 일정](assets/personal-time-off-calendar-0925.png)

   프로덕션 환경의 샘플 이미지:
   ![개인 휴무 일정](assets/personal-time-off-calendar.png)

1. 하루 종일 쉬려면 **[!UICONTROL 하루 종일]**&#x200B;을 선택하세요.

   하루 미만의 휴무를 수행하는 경우 확인란을 선택 취소한 상태로 두고 휴무 시작 및 종료 시간을 나타냅니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

   이제 리소스 플래너 및 업무 균형자 같은 리소스 관리 도구의 [!DNL Workfront] 시스템에서 휴무를 볼 수 있습니다. 이 시간 동안 작업에 할당되면 도구 팁은 사용자에게 휴무가 예약되었음을 알려줍니다.
