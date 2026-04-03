---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Snowflake용 Reader 계정 만들기
description: Data Connect 데이터에 액세스하려면 먼저 Snowflake 리더 계정을 만들어야 합니다.
author: Courtney
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 1%

---

# Snowflake에 대한 Reader 계정 또는 연결 만들기

Data Connect 데이터에 액세스하려면 먼저 조직에 대한 Snowflake 리더(또는 서비스) 계정을 만든 다음 Data Connect에 액세스하려는 각 사용자 또는 도구에 대해 새 연결을 만들어야 합니다.

연결을 만든 후 기존 연결 탭 아래의 Data Connect 페이지(메인 메뉴 > 설정 > 시스템 > Data Connect)에서 해당 연결을 클릭하여 연결된 URL 및 사용자 이름을 찾을 수 있습니다.

외부 제품에 새로 만든 연결을 사용하는 방법에 대한 자세한 내용은 [Workfront Data Connect에 연결 설정](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)을 참조하십시오.

## 액세스 요구 사항

+++ 를 확장하여 액세스 요구 사항을 확인합니다. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>Ultimate</p>
    <p>워크플로 얼티밋</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p></td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 리더 계정 만들기

연결 만들기를 시작하려면 먼저 조직에 대한 새 Snowflake reader 계정을 만들어야 합니다.

>[!IMPORTANT]
>
>이 프로세스는 조직당 한 번만 완료해야 합니다. **Reader 계정 만들기** 단추가 아래 설명된 위치에 없으면 판독기 계정이 이미 만들어진 것입니다.

리더 계정을 만들려면:

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 연결**&#x200B;을 클릭합니다.

1. 조직의 Reader 계정을 만들려면 **Reader 계정 만들기** 단추를 클릭하십시오. 이 프로세스는 자동으로 진행되지만 완료하는 데 최대 24시간이 소요될 수 있습니다.

1. 완료되면 리더 계정이 이제 활성 상태임을 설명하는 대화 상자 창이 표시됩니다. 브라우저 페이지를 새로 고쳐 **새 연결 만들기** 단추에 액세스할 수 있습니다.

![Reader 계정을 만든 대화 상자](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## 연결 만들기

>[!IMPORTANT]
>
>2026년 6월에 다단계 인증(MFA)을 사용하려면 사용자 이름/암호 자격 증명이 필요합니다. Data Connect에서 인증 프로세스에서 MFA에서 작동하지 않는 서드파티 시각화 도구, 데이터 프로세서 및 스크립트로 데이터를 로드하는 데 사용되는 서비스 사용자 계정의 경우 RSA 또는 PAT 기반 인증으로 전환하는 것이 좋습니다.


1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 연결**&#x200B;을 클릭합니다.

1. **새 연결 만들기**&#x200B;를 클릭합니다.

1. 표시되는 창에서 연결 이름을 **연결 참조 설명**&#x200B;에 입력하고 사용자 이름을 **연결 사용자**&#x200B;에 입력한 다음 **연결 생성**&#x200B;을 클릭합니다.

   ![새 연결 만들기](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. 연결에 대한 인증 방법 선택:
   * [암호 인증](#password-authentication)
   * [프로그래밍 방식 액세스 토큰 인증](#programmatic-access-token-authentication)
   * [RSA 키 인증](#rsa-key-authentication)

### 암호 인증

1. **암호**&#x200B;를 클릭한 다음 **연결 생성**&#x200B;을 클릭합니다.

1. **기본 암호**&#x200B;와 Snowflake을 통해 데이터를 볼 수 있는 URL이 생성됩니다. Snowflake에 처음 로그인하기 위해 선택한 사용자 이름의 암호를 사용해야 하므로, 이 암호와 URL을 기록해야 합니다. 확인란을 선택하고 **닫기**&#x200B;를 클릭합니다.

   ![기본 계정 암호](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. 브라우저를 사용하여 Snowflake을 열고 이전 단계의 URL로 이동하고, 선택한 사용자 이름과 이전 단계의 기본 암호를 입력한 다음 **로그인**&#x200B;을 클릭합니다.

1. 처음 로그인하면 새 암호를 선택하라는 메시지가 표시됩니다. **새 암호**&#x200B;와 **암호 확인** 필드 모두에 선택한 암호를 입력한 다음 **제출**&#x200B;을 클릭합니다.

   ![Snowflake 암호 재설정](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. 이제 사용자 이름과 새 암호를 사용하여 Snowflake의 Data Connect 데이터 레이크 또는 선택한 비즈니스 시각화 도구에 액세스할 수 있습니다.

### 프로그래밍 방식 액세스 토큰 인증

1. **프로그래밍 방식 액세스 토큰**&#x200B;을 클릭합니다.

1. **만료 날짜** 필드에 토큰의 만료 날짜를 입력합니다. 만료 날짜는 향후 최대 365일까지 선택할 수 있습니다.

1. **연결 생성**&#x200B;을 클릭합니다.

1. 인증에 사용할 수 있는 PAT 토큰이 생성되고 Snowflake 환경 URL이 제공됩니다. 제공한 PAT 및 사용자 이름을 사용하여 타사 시각화 도구 또는 데이터 프로세서에서 Snowflake에 연결할 수 있습니다. URL과 함께 기록을 유지해야 합니다. 확인란을 선택하고 **닫기**&#x200B;를 클릭합니다.

   ![프로그래밍 방식 액세스 토큰 대화 상자](/help/quicksilver/reports-and-dashboards/data-lake/assets/pat-test.png)


### RSA 키 인증

1. **RSA 키**&#x200B;를 클릭합니다.

1. **RSA 공개 키** 필드에 RSA 공개 키를 입력합니다.

1. **연결 생성**&#x200B;을 클릭합니다.

1. 연결이 생성되고 Snowflake 환경 URL이 제공됩니다. 제공한 RSA 키 및 사용자 이름을 사용하여 서드파티 시각화 도구 또는 데이터 프로세서에서 Snowflake에 연결할 수 있습니다.



Snowflake에 로그인하기 위해 선택한 사용자 이름과 함께 RSA 키를 사용해야 하므로 이 키와 URL에 대한 기록이 있어야 합니다. 확인란을 선택하고 **닫기**&#x200B;를 클릭합니다.

![RSA 키 대화 상자](assets/rsa-test.png)

## 리더 계정 취소

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 액세스**&#x200B;를 클릭합니다.

1. 해지하려는 계정의 오른쪽에 있는 휴지통 아이콘 ![삭제 아이콘](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)을 클릭합니다.

1. 표시되는 창에서 확인란에 확인 표시를 한 다음 **삭제**&#x200B;를 클릭합니다.
