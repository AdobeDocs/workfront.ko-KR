---
navigation-topic: notifications
title: 미리보기 샌드박스 환경에서 이메일 게재 활성화
description: 미리보기 샌드박스 환경에서 이메일 알림을 수신하려면 미리보기에 로그인하는 동안 사용자 설정에서 이 기능을 활성화해야 합니다.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# 미리보기 샌드박스 환경에서 이메일 게재 활성화

[!UICONTROL Adobe Workfront]은(는) 미리 보기 및 사용자 지정 새로 고침 샌드박스 환경에서 모든 전자 메일 통신을 사용하지 않도록 설정합니다. 미리 보기 샌드박스 환경에 대한 자세한 내용은 [Adobe Workfront 미리 보기 샌드박스 환경](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)을 참조하십시오. 사용자 지정 새로 고침 샌드박스 환경에 대한 자세한 내용은 [Adobe Workfront 사용자 지정 새로 고침 샌드박스 환경](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)을 참조하십시오.

미리보기 샌드박스 환경에서 다음 이메일 알림을 수신하려면 미리보기에 로그인하는 동안 사용자 설정에서 이 기능을 활성화해야 합니다.

* 이벤트 알림에 의해 트리거된 이메일 알림
* 미리 알림
* 자동 지연 또는 조기 미리 알림
* 이메일 초대

이 작업은 직접 수행하거나 편집할 수 있는 액세스 권한이 있는 모든 사용자에 대해 수행할 수 있습니다. 사용자 편집에 필요한 액세스 권한에 대한 자세한 내용은 [사용자에게 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)를 참조하십시오.

>[!NOTE]
>
>모바일 앱의 보고서 배달 및 푸시 알림은 미리보기 샌드박스 환경에 대해 항상 비활성화됩니다. 미리 보기 샌드박스 환경에 액세스할 때 사용자와 [!DNL Workfront] 관리자 모두 모바일 앱에 대해 보고서 배달이나 푸시 알림을 활성화할 수 없습니다.
>
>보고서 배달에 대한 자세한 내용은 [보고서 배달 개요](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)를 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스</strong></td> 
   <td> 
   <p>자신의 설정을 변경할 기여자 이상</p> <p>다른 사용자에 대한 설정을 편집하려면 표준</p> 
   또는
   <p> 자신의 설정을 변경하도록 요청 이상</p> <p>다른 사용자에 대한 설정 편집 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다.</p> </li> 
     <li> <p>액세스 수준에서 [!UICONTROL 사용자] 설정에 대해 [!UICONTROL 편집]을 선택해야 합니다. [!UICONTROL 사용자] 설정의 경우 [!UICONTROL 설정 미세 조정] <img src="assets/gear-icon-in-access-levels.png">에서 [!UICONTROL 만들기] 옵션과 두 [!UICONTROL 사용자 관리] 옵션 중 하나 이상을 활성화해야 합니다. </li> 
     <li>[!UICONTROL 사용자 관리자(그룹 사용자)] 옵션을 사용하는 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 미리보기 샌드박스 환경에서 이메일 게재 활성화

1. 미리보기 샌드박스 환경에 로그인합니다.
1. [!DNL Adobe Workfront]의 오른쪽 상단 모서리에서 프로필 사진을 클릭합니다. 그런 다음 **[!UICONTROL 자세히]** 메뉴를 클릭하고 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

   또는

   [!DNL Workfront]에서 사용자를 검색하고 해당 이름을 클릭합니다. 그런 다음 **[!UICONTROL 자세히]** 메뉴를 클릭하고 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

   또는

   여러 사용자의 경우: Workfront의 오른쪽 상단에 있는 **[!UICONTROL 기본 메뉴]** 아이콘 ![기본 메뉴 아이콘](assets/main-menu-icon.png)을 클릭한 다음 **[!UICONTROL 사용자]** ![사용자 아이콘](assets/users-icon-in-main-menu.png)을 클릭합니다.  그런 다음 여러 사용자를 선택하고 **[!UICONTROL 편집]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 환경 설정]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 이 테스트 환경에서 전자 메일 받기]**&#x200B;를 선택합니다.

   >[!NOTE]
   >
   >프로덕션 환경에서는 이 옵션을 사용할 수 없습니다.

1. **[!UICONTROL 변경 내용 저장]**&#x200B;을 클릭합니다.
