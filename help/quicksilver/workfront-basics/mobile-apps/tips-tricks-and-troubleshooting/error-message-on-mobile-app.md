---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: " [!DNL Adobe Workfront] 모바일 앱에서 오류 메시지: '계정이 API를 사용할 수 없습니다.'"
description: " [!DNL Adobe Workfront] 모바일 앱에서 오류 메시지: '계정이 API를 사용할 수 없습니다.'"
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# [!DNL Adobe Workfront] 모바일 앱에 오류 메시지: &quot;[!UICONTROL 계정이 API를 사용할 수 없습니다.]&quot;

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td> 
   <td> <p> 임의</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 라이선스</strong></td> 
   <td> <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>[!UICONTROL 시스템 관리자] </p> </td> 
  </tr> 
 </tbody> 
</table>

## 문제

[!DNL Adobe Workfront] 모바일 앱에 로그인하려고 하면 다음 오류가 표시됩니다. *[!UICONTROL 계정이 API를 사용할 수 없습니다. 시스템 관리자에게 알려주면 설정이 완료됩니다. 죄송합니다.]*

## 원인

[!DNL Workfront] 관리자가 모바일 장치에서 액세스할 수 있도록 [!DNL Workfront] 환경을 활성화하지 않았습니다.

## 솔루션

1. [!DNL Workfront] 웹 응용 프로그램에 [!DNL Workfront] 관리자로 로그인합니다.
1. **[!UICONTROL 설정]** 영역으로 이동합니다.
1. **[!UICONTROL 시스템]** 메뉴를 확장한 다음 **[!UICONTROL 기본 설정]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 보안]** 섹션에서 **[!UICONTROL 사람들이 [!DNL Workfront]의 모바일 응용 프로그램과 [!DNL Workfront Outlook] 추가 기능]** 옵션을 사용하여 사용하도록 설정합니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.\
   이제 시스템의 모든 사용자가 모바일 앱 및 [!DNL Outlook]에서 [!DNL Workfront]에 액세스할 수 있습니다.
