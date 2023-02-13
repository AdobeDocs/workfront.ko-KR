---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: "오류 메시지 [!DNL Adobe Workfront] 모바일 앱: '계정이 API가 활성화되지 않았습니다.'"
description: "오류 메시지 [!DNL Adobe Workfront] 모바일 앱: '계정이 API가 활성화되지 않았습니다.'"
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# 오류 메시지 [!DNL Adobe Workfront] 모바일 앱: &quot;[!UICONTROL 계정이 API가 활성화되지 않았습니다.]&quot;

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td> 
   <td> <p> 모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 라이선스</strong></td> 
   <td> <p>플랜</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>[!UICONTROL System 관리자] </p> </td> 
  </tr> 
 </tbody> 
</table>

## 문제

에 로그인하려고 할 때 [!DNL Adobe Workfront] 모바일 앱에서는 다음 오류가 표시됩니다. *[!UICONTROL 계정이 API가 활성화되지 않았습니다. 시스템 관리자에게 문의하여 설정을 받으십시오. 미안해]*

## 원인

사용자 [!DNL Workfront] 관리자가 활성화되지 않았습니다. [!DNL Workfront] 모바일 장치에서 액세스할 수 있는 환경입니다.

## 솔루션

1. 에 로그인합니다. [!DNL Workfront] 웹 애플리케이션 [!DNL Workfront] 관리자
1. 로 이동합니다. **[!UICONTROL 설정]** 영역.
1. 를 확장합니다. **[!UICONTROL 시스템]** 메뉴를 클릭한 다음 **[!UICONTROL 기본 설정]**.

1. 아래에 **[!UICONTROL 보안]** 섹션에서 **[!UICONTROL 사용자 사용 허용 [!DNL Workfront]의 모바일 애플리케이션 및 [!DNL Workfront Outlook] 추가 기능]** 옵션을 활성화하면 됩니다.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.\
   이제 시스템의 모든 사용자가 [!DNL Workfront] 모바일 앱으로부터, [!DNL Outlook].
