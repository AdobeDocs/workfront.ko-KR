---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Snowflake을 위한 리더(서비스) 계정 만들기
description: Workfront 데이터 레이크의 데이터에 액세스하려면 먼저 Snowflake에 대한 리더 계정을 만들어야 합니다.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Snowflake을 위한 리더(서비스) 계정 만들기

Workfront 데이터 레이크 데이터에 액세스하려면 먼저 각 새 연결에 대한 Snowflake 판독기(또는 서비스) 계정을 만들어야 합니다. 연결을 만든 후 **기존 연결** 탭 아래의 **데이터 액세스** 페이지(**기본 메뉴** > **설정** > **시스템** > **데이터 액세스**)에서 연결을 클릭하여 연결된 URL과 사용자 이름을 찾을 수 있습니다.

외부 제품에 새로 만든 연결을 사용하는 방법에 대한 자세한 내용은 [Workfront 데이터 레이크에 연결 설정](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)을 참조하십시오.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>TBD</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

## 리더 계정 만들기

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 액세스**&#x200B;를 클릭합니다.

1. **새 연결 만들기** 클릭

1. 표시되는 창에서 연결 이름을 **연결 참조 설명**&#x200B;에 입력하고 사용자 이름을 **연결 사용자**&#x200B;에 입력한 다음 **연결 생성**&#x200B;을 클릭합니다.

   ![판독기 계정 만들기](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. **기본 암호**&#x200B;와 Snowflake을 통해 데이터를 볼 수 있는 URL이 생성됩니다. Snowflake에 처음 로그인하기 위해 선택한 사용자 이름과 함께 암호를 사용해야 하므로 이 암호와 URL을 기록해야 합니다. 확인란을 선택하고 **닫기**&#x200B;를 클릭합니다.

   ![기본 계정 암호](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. 브라우저를 사용하여 Snowflake을 열어 이전 단계의 URL로 이동하고, 선택한 사용자 이름과 이전 단계의 기본 암호를 입력한 다음 **로그인**&#x200B;을 클릭합니다.

1. 처음 로그인하면 새 암호를 선택하라는 메시지가 표시됩니다. **새 암호**&#x200B;와 **암호 확인** 필드 모두에 선택한 암호를 입력한 다음 **제출**&#x200B;을 클릭합니다.

   ![Snowflake 암호 재설정](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. 이제 사용자 이름과 새 암호를 사용하여 Snowflake의 Workfront 데이터 레이크 또는 선택한 비즈니스 시각화 도구에 액세스할 수 있습니다.

## 리더 계정 취소

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 액세스**&#x200B;를 클릭합니다.

1. 해지하려는 계정의 오른쪽에 있는 휴지통 아이콘 ![삭제 아이콘](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)을 클릭합니다.

1. 표시되는 창에서 확인란에 확인 표시를 한 다음 **삭제**&#x200B;를 클릭합니다.
