---
filename: change-date-format-chrome
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 날짜 형식 변경 [!DNL Adobe Workfront]
description: 날짜의 날짜 형식을 변경하려면 [!DNL Adobe Workfront] 브라우저에서 언어 설정을 변경해야 합니다.
feature: Get Started with Workfront
exl-id: 9fac92fb-e3d1-4537-b324-4b35447cef28
source-git-commit: e9a96b6952ca3f128cc723df68787f40c8dcf604
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# 날짜 형식 변경 [!DNL Adobe Workfront]

<!--this article used to be called "Change the date format in Adobe Workfront when using Chrome". The team decieded to make it more generic and hide the steps. Also see drafted content below-->

날짜의 날짜 형식을 [!DNL Adobe Workfront], 예: [!UICONTROL 계획된 완료 일자], [!UICONTROL 실제 완료 일자], 또는 [!UICONTROL 예상 완료 일자].

예를 들어에서 날짜 형식을 변경할 수 있습니다 _DD/MM/YYYY_ 끝 _MM/DD/YYYY_ 또는 그 반대입니다.
또는 다음 날짜 형식에서 변경할 수 있습니다. _MM/DD/YY_ 끝 _YYYY년 월 DD일_.

보고자 하는 변경 내용과 변경 내용을 보려는 위치에 따라 다음과 같은 방법으로 Workfront의 날짜 형식을 변경할 수 있습니다.

* 의 모든 페이지에 대한 날짜 형식을 모두 변경하려면 [!DNL Workfront] 사용자의 위치 및 언어에 따라 브라우저에서 언어 설정을 변경해야 합니다.

  예를 들어 브라우저의 기본 언어가 로 설정된 경우 *[!UICONTROL 영어(미국)]*&#x200B;로 설정하면 날짜가 다음 형식으로 표시됩니다.

   * MM/DD/YYYY
   * YYY 년 월 DD 일

  에서 언어 설정을 변경하려면 [!DNL Chrome] 또는 다른 모든 브라우저에서 해당 브라우저의 설정을 수정해야 합니다. 브라우저 설정을 수정하는 단계는 브라우저마다 다릅니다. 브라우저의 [!UICONTROL 도움말], [!UICONTROL 환경 설정], 또는 [!UICONTROL 설정] 설정을 수정하는 방법을 배울 영역.

* 보고서와 보기의 날짜 형식만 변경하려면 [!UICONTROL 필드 형식] 에서 설정 [!UICONTROL 고급 옵션] 열 영역(보고서 또는 보기를 작성할 때). 위치나 언어에 따라 날짜 형식이 수정되지는 않습니다. 동일한 위치 또는 언어의 컨텍스트에서 날짜 형식을 수정합니다.

  ![](assets/field-format-in-advanced-options-of-a-view-highlighted.png)

  자세한 내용은 [사용자 지정 보고서 만들기](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* 전체 조직에 대한 모든 발신 이메일 알림의 날짜 형식을 변경하려면 다음을 업데이트해야 합니다. [!UICONTROL 기본 전자 메일 로케일] 에서 설정 [!UICONTROL 고객 정보] 영역 [!UICONTROL 설정].

  ![](assets/default-email-locale-field.png)

  자세한 내용은 [시스템에 대한 기본 정보 구성](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* 단일 사용자에 대한 모든 발신 전자 메일 알림의 모든 날짜 형식을 변경하려면 [!UICONTROL 이메일 로케일] 에서 설정 [!UICONTROL 사용자 편집] 상자(사용자 프로필을 편집할 때)

  ![](assets/email-locale-for-user-profile-highlighted.png)

  자세한 내용은 [사용자 프로필 편집](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--drafted because we should not document steps for a third-party application

To change your language settings in Chrome:

1. Click the 3-dots in the top right corner of your Chrome interface, then click **Settings**.
1. On the left area of the Settings page, expand **Advanced**, then click **Languages**.  
   Or  
   Search for *language*&nbsp;at the top of the Settings page, then click **Languages**.

1. In the **Language** list, locate the language and region that use your preferred date format.

   **Example:** If you speak English and you want the date format to be MM/DD/YYYY, you would select **English (United States)**. If you speak English and you want the date format to be DD/MM/YYY, you would select **English (United Kingdom)**.

1. (Conditional) If the language and region you want to use are not visible in the list, click **Add languages** to add it to the list.
1. Click the 3-dot menu next to the language and region you want to use, then click **Move to the top**.
1. Return to the Workfront interface, then refresh the page.  
   The date format is now updated in projects and other areas of Workfront that use MM/DD/YYYY or DD/MM/YYYY format when displaying dates.

   -->
