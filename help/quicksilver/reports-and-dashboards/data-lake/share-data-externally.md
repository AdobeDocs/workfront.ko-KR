---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Workfront 데이터 레이크에 대한 연결 설정
description: Workfront 데이터 레이크를 사용하면 많이 사용되는 비즈니스 인텔리전스 도구를 사용하여 조직의 Workfront 데이터를 사용하거나 외부 데이터 웨어하우스에 저장할 수 있습니다.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# Workfront 데이터 레이크에 대한 연결 설정

Workfront 데이터 레이크를 사용하면 비즈니스 인텔리전스 도구를 사용하여 조직의 Workfront 데이터를 사용하거나 외부 데이터 웨어하우스에 저장할 수 있습니다.

Workfront 데이터 레이크 데이터를 외부 제품과 연결하려면에 설명된 대로 먼저 필요한 IP를 허용 목록에 추가하다에 추가해야 합니다 [허용 목록에 추가하다에 IP 추가](#add-ips-to-the-allowlist) 아래요. 또한 대부분의 제품에서 연결을 설정하려면 데이터 레이크에 대한 추가 정보가 필요합니다.

| 필드 이름 | 값 |
|---------------|-------------|
| 서버 | 를 제외한 연결 URL `https://` 부분(다음에서 찾음) **데이터 액세스** Workfront*)의 페이지 |
| 포트 | `443` |
| 데이터베이스 | `WORKFRONT` |
| 웨어하우스 | `READER_WH` |
| 스키마 | `WF` |
| 역할 | `READER_ROLE` |
| 사용자 이름 | 연결을 만들 때 선택한 사용자 이름( **데이터 액세스** Workfront*)의 페이지 |
| 암호 | 첫 번째 Snowflake 로그인 시 선택한 암호* |

*찾을 수 있는 위치에 대한 정보 **데이터 액세스** 데이터 레이크 연결이 포함된 페이지는 다음을 참조하십시오. [Snowflake을 위한 리더(서비스) 계정 만들기](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>한 항목이 IP 허용 목록에 추가되면 다른 모든 IP 주소는 더 이상 허용되지 않습니다. 시각화 도구를 사용하기 전에 시각화 도구의 작성 및 읽기 경험에 필요한 모든 IP 주소를 입력해야 합니다. 그렇지 않은 경우 잘못된 자격 증명에 대한 오류가 발생할 수 있습니다.

## 허용 목록에 추가하다에 IP 추가

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **설정**.

1. 왼쪽 패널에서 **시스템** > **데이터 액세스**.

1. 을(를) 클릭합니다 **허용된 IP** 탭을 클릭한 다음 **허용 목록에 추가하다 IP 주소를 IP에 추가** 단추를 클릭합니다.

1. 에 IP 주소 이름을 입력하십시오. **IP 주소 설명** 에서 사용할 도구의 IP 주소를 입력하십시오. **IP 주소**&#x200B;을 클릭한 다음 을 클릭합니다 **IP를 허용 목록에 추가**.

   ![IP 주소 추가](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 허용 목록에 추가하다에서 IP 주소 제거

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon.png) Adobe Workfront의 오른쪽 위 모서리에서 또는 (사용 가능한 경우) **[!UICONTROL 메인 메뉴]** 아이콘 ![메인 메뉴](/help/_includes/assets/main-menu-icon-left-nav.png) 왼쪽 상단 모서리에서 을(를) 클릭하고 **설정**.

1. 왼쪽 패널에서 **시스템** > **데이터 액세스**.

1. 을(를) 클릭합니다 **허용된 IP** 탭을 클릭한 다음 휴지통 아이콘을 클릭합니다 ![삭제 아이콘](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 제거할 IP 주소의 오른쪽에 있습니다.

1. 나타나는 창에서 상자를 선택하여 확인한 다음 을 클릭합니다. **삭제**.

## 비즈니스 인텔리전스 도구를 사용하여 데이터 공유

여러 가지 일반적인 비즈니스 인텔리전스 도구가 아래에 나와 있습니다. 링크를 클릭하면 서비스 설명서 사이트로 이동하여 데이터 레이크 연결에 대해 자세히 알아봅니다.

* [타블로](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [도모](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## 외부 데이터 웨어하우스에 데이터 저장

아래에 여러 개의 공통 데이터 웨어하우스가 나와 있습니다. 링크를 클릭하면 데이터 레이크 연결에 대해 자세히 알아볼 수 있는 각 서비스의 설명서 사이트로 이동합니다.

* [데이터 블록](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
