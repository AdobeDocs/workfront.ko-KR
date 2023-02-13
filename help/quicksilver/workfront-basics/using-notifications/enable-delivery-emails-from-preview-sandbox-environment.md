---
navigation-topic: notifications
title: 미리 보기 샌드박스 환경에서 전자 메일 게재 활성화
description: 미리 보기 샌드박스 환경에서 이메일 알림을 받으려면 미리 보기에 로그인한 동안 사용자 설정에서 이 기능을 활성화해야 합니다.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# 미리 보기 샌드박스 환경에서 전자 메일 게재 활성화

[!UICONTROL Adobe Workfront] 미리 보기 및 사용자 지정 새로 고침 샌드박스 환경 모두에서 모든 이메일 통신을 비활성화합니다. 미리 보기 샌드박스 환경에 대한 자세한 내용은 [Adobe Workfront 미리 보기 샌드박스 환경](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). 사용자 지정 새로 고침 샌드박스 환경에 대한 자세한 내용은 [Adobe Workfront 사용자 지정 새로 고침 샌드박스 환경](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

미리 보기 샌드박스 환경에서 다음 이메일 알림을 수신하려면 미리 보기에 로그인한 동안 사용자 설정에서 이 기능을 활성화해야 합니다.

* 이벤트 알림에 의해 트리거된 이메일 알림
* 미리 알림
* 자동 지연 또는 조기 미리 알림
* 이메일 초대

직접 또는 편집할 수 있는 액세스 권한이 있는 모든 사용자에 대해 이 작업을 수행할 수 있습니다. 사용자 편집에 필요한 액세스에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>모바일 앱의 보고서 전달 및 푸시 알림은 항상 미리 보기 샌드박스 환경에 대해 비활성화됩니다. 너도 아니고 [!DNL Workfront] 관리자는 샌드박스 환경 미리 보기에 액세스할 때 모바일 앱에 대한 보고서 전달 또는 푸시 알림을 활성화할 수 있습니다.
>
>보고서 게재에 대한 자세한 내용은 [보고서 배달 개요](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>고유한 설정을 변경하려면 [!UICONTROL Request] 이상</p> <p>[!UICONTROL Plan] - 다른 사용자에 대한 설정을 편집합니다.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다.</p> <p> 이 액세스 수준에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> </li> 
     <li> <p>액세스 수준에서 [!UICONTROL 사용자] 설정에 대해 [!UICONTROL 편집]을 선택해야 합니다. 그리고 [!UICONTROL 사용자] 설정의 경우 [!UICONTROL 설정 세부 조정]에서 설정을 조정합니다. <img src="assets/gear-icon-in-access-levels.png"> , [!UICONTROL 만들기] 옵션과 두 [!UICONTROL 사용자 관리] 옵션 중 하나 이상을 활성화해야 합니다. </p> <p>[!UICONTROL 사용자 관리(그룹 사용자)] 옵션을 사용하는 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>액세스 수준의 [!UICONTROL 사용자] 설정에 대한 자세한 내용은 다음을 참조하십시오 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
    </ul> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우 자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 수정할 수 있습니다. <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 미리 보기 샌드박스 환경에서 전자 메일 게재를 활성화합니다

1. 미리 보기 샌드박스 환경에 로그인합니다.
1. 의 오른쪽 위 모서리에서 프로필 사진을 클릭합니다. [!DNL Adobe Workfront]. 그런 다음 **[!UICONTROL 자세히]** 메뉴 및 선택 **[!UICONTROL 편집]**.

   또는

   에서 사용자 검색 [!DNL Workfront] 이름을 클릭합니다. 그런 다음 **[!UICONTROL 자세히]** 메뉴 및 선택 **[!UICONTROL 편집]**.

   또는

   여러 사용자의 경우: 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) Workfront의 오른쪽 위 모서리에서 을(를) 클릭하고 **[!UICONTROL 사용자]** ![](assets/users-icon-in-main-menu.png).  그런 다음 여러 사용자를 선택하고 **[!UICONTROL 편집]**.

1. 클릭 **[!UICONTROL 기본 설정]**.
1. 선택 **[!UICONTROL 이 테스트 환경에서 전자 메일 받기]**.

   >[!NOTE]
   >
   >프로덕션 환경에 있는 경우에는 이 옵션을 사용할 수 없습니다.

1. 클릭 **[!UICONTROL 변경 내용 저장]**.
