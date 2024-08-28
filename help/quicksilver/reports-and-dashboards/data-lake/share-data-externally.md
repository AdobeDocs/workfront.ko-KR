---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront 데이터 레이크에 대한 연결 설정
description: Workfront 데이터 레이크를 사용하면 많이 사용되는 비즈니스 인텔리전스 도구를 사용하여 조직의 Workfront 데이터를 사용하거나 외부 데이터 웨어하우스에 저장할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 1%

---

# Workfront Data Connect에 연결 설정

Workfront Data Connect를 사용하면 비즈니스 인텔리전스 도구를 통해 조직의 Workfront 데이터를 사용하거나 외부 데이터 웨어하우스에 저장할 수 있습니다.

Data Connect 데이터 레이크를 외부 제품과 연결하려면 먼저 아래 [허용 목록에 IP 추가](#add-ips-to-the-allowlist)에서 설명한 대로 필요한 IP를 허용 목록에 추가하다에 추가해야 합니다. 또한 대부분의 제품에서 연결을 설정하려면 데이터 레이크에 대한 추가 정보가 필요합니다.

| 필드 이름 | 값 |
|---------------|-------------|
| 서버 | `https://` 부분이 없는 연결의 URL(Workfront*의 **데이터 액세스** 페이지에 있음) |
| 포트 | `443` |
| 데이터베이스 | `WORKFRONT` |
| 웨어하우스 | `READER_WH` |
| 스키마 | `WF` |
| 역할 | `READER_ROLE` |
| 사용자 이름 | 연결을 만들 때 선택한 사용자 이름(Workfront*의 **데이터 액세스** 페이지에 있음) |
| 암호 | 첫 번째 Snowflake 로그인 시 선택한 암호* |

*Data Connect 연결이 포함된 **데이터 액세스** 페이지를 찾을 수 있는 위치에 대한 자세한 내용은 [Snowflake에 대한 판독기(서비스) 계정 만들기](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)를 참조하십시오.

>[!IMPORTANT]
>
>한 항목이 IP 허용 목록에 추가되면 다른 모든 IP 주소는 더 이상 허용되지 않습니다. 시각화 도구를 사용하기 전에 시각화 도구의 작성 및 읽기 경험에 필요한 모든 IP 주소를 입력해야 합니다. 그렇지 않은 경우 잘못된 자격 증명에 대한 오류가 발생할 수 있습니다.
>
>허용 목록에 추가하다에 IP 주소가 포함되어 있지 않지만 BI 도구에 연결하는 데 여전히 문제가 있는 경우 BI 도구에 대한 프록시 서버 구성을 확인하십시오.

## 허용 목록에 추가하다에 IP 추가

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 액세스**&#x200B;를 클릭합니다.

1. **허용된 IP** 탭을 클릭한 다음 **IP 주소를 허용 목록에 추가** 단추를 클릭합니다.

1. **IP 주소 설명**&#x200B;에 IP 주소 이름을 입력하고 **IP 주소**&#x200B;에서 사용할 도구의 IP 주소(또는 CIDR 블록)를 입력한 다음 **IP를 허용 목록에 추가**&#x200B;를 클릭합니다.

   ![IP 주소 추가](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 허용 목록에 추가하다에서 IP 주소 제거

1. Adobe Workfront의 오른쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon.png)을 클릭하거나(가능한 경우) 왼쪽 상단에 있는 **[!UICONTROL 주 메뉴]** 아이콘 ![주 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png)을 클릭한 다음 **설정**&#x200B;을 클릭합니다.

1. 왼쪽 패널에서 **시스템** > **데이터 액세스**&#x200B;를 클릭합니다.

1. **허용된 IP** 탭을 클릭한 다음 제거할 IP 주소의 오른쪽에 있는 휴지통 아이콘 ![삭제 아이콘](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)을 클릭합니다.

1. 표시되는 창에서 확인란에 확인 표시를 한 다음 **삭제**&#x200B;를 클릭합니다.

## 비즈니스 인텔리전스 도구를 사용하여 데이터 공유

여러 가지 일반적인 비즈니스 인텔리전스 도구가 아래에 나와 있습니다. 링크를 클릭하면 서비스 설명서 사이트로 이동하여 데이터 레이크 연결에 대해 자세히 알아봅니다.

* [타블로](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## 외부 데이터 웨어하우스에 데이터 저장

아래에 여러 개의 공통 데이터 웨어하우스가 나와 있습니다. 링크를 클릭하면 데이터 레이크 연결에 대해 자세히 알아볼 수 있는 각 서비스의 설명서 사이트로 이동합니다.

* [데이터 블록](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
