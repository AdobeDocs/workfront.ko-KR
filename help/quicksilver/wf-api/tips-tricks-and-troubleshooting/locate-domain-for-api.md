---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Adobe Workfront API 호출에 대한 도메인 형식
description: Adobe Workfront API에서 사용할 도메인을 찾습니다
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# Adobe Workfront API 호출에 대한 도메인 형식

Workfront API에 대한 API를 호출하면 호출에서 조직의 도메인을 사용합니다. 이 도메인 URL의 형식은 조직이 Adobe 통합 셸에 온보딩되었는지 여부에 따라 다릅니다.

조직이 Adobe 통합 셸에 있는지 확인하려면 Workfront 페이지를 볼 때 표시되는 URL을 검사합니다.

| Workfront URL의 시작 문자: | API 호출용 URL: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

도메인을 찾으려면:

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **[!UICONTROL 설정]** ![설정 아이콘](/help/_includes/assets/gear-icon-setup.png)을 클릭합니다.
1. **시스템**&#x200B;을 선택한 다음 **고객 정보**&#x200B;을 선택합니다.

   화면 오른쪽에 도메인이 나열됩니다.

   ![도메인](assets/domain.png)

