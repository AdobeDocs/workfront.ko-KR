---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop에서 연결을 설정할 수 없음
description: Tableau Desktop을 Data Connect에 연결하려고 하면 오류가 발생합니다.
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Tableau Desktop에서 연결을 설정할 수 없음

## 문제

Tableau Desktop을 Data Connect에 연결하려고 하면 다음 오류가 표시됩니다.

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## 원인

이 오류는 Data Connect에서 데이터가 로드되지 않도록 하는 로컬 컴퓨터의 프록시 설정으로 인해 발생합니다.

Data Connect는 서드파티 Snowflake 클라우드 서비스를 통해 제공됩니다. Tableau를 사용하려면 Snowflake과 통신할 수 있도록 네트워킹을 열어 두어야 합니다.

## 솔루션

다음을 수행하여 이 문제를 해결할 수 있습니다.

* **보안 도구를 사용하지 않도록 설정하여 문제를 해결합니다**: Zscaler나 Cisco와 같은 보안 도구를 사용하지 않도록 설정하여 연결 문제를 해결하는지 확인하십시오. 이 방법으로 연결 문제가 해결되면 보안 도구가 최신 버전으로 업그레이드되었는지 확인하고 내부 네트워크 팀과 함께 VPN Snowflake에 Data Connect(허용 목록에 추가하다) IP 주소를 추가하십시오.

* **IP 주소를 허용 목록에 추가**: 방화벽 설정이 Data Connect에서 사용하는 IP 주소를 허용하는지 확인하십시오. 명령 `SYSTEM$ALLOWLIST()`을(를) 사용하여 IP 주소를 가져온 다음 VPN에서 허용 목록에 추가하다할 수 있습니다.

* **방화벽 및 프록시 설정 확인**: 네트워크에 있는 방화벽 또는 프록시 구성이 Snowflake 끝점에 대한 액세스를 차단하고 있는지 확인합니다. 필요한 Snowflake IP 주소를 회사 허용 목록 및 포트에 추가하려면 네트워크 관리자에게 문의해야 할 수 있습니다.

* **해결 방법 옵션**: Tableau의 데이터 Source 창 대신 워크시트 화면에서 추출을 만듭니다. 연결이 손실되지 않고 추출 프로세스가 완료됩니다.

