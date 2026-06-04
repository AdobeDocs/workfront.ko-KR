---
content-type: reference
navigation-topic: announcements
title: 클러스터 1, 2 및 3의 고객은 Adobe Workfront 서비스가 차단되지 않도록 허용 목록에 추가하다 IP 블록을 업데이트해야 합니다
description: 핵심 인프라를 개선하고 개선하기 위해 클러스터 01, 02 및 03의 Adobe Workfront 고객을 AWS 공용 클라우드로 곧 마이그레이션할 예정입니다.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
TQID: https://experienceleague.adobe.com/I6EiM5bD37m-gC5wyB3DBaOscSTMX-18BpjogM1LcgU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 0%

---

# 클러스터 1, 2 및 3의 고객은 Adobe Workfront 서비스가 차단되지 않도록 허용 목록에 추가하다 IP 블록을 업데이트해야 합니다

핵심 인프라를 개선하고 개선하기 위해 클러스터 01, 02 및 03의 Adobe Workfront 고객을 AWS 공용 클라우드로 곧 마이그레이션할 예정입니다.

이 변경 사항의 일부로, Workfront 서비스가 차단되지 않도록 하려면 허용 목록에 추가하다 IP 블록에 다음 IP를 추가해야 합니다.

SSO 및 POP의 경우:

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

이메일의 경우

* 54.240.60.174
* 54.240.60.175

2019년 5월 13일까지 IP 블록을 업데이트했는지 확인하십시오. 자세한 내용은 [방화벽 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)을 참조하십시오.

고객에게 보다 안정적이고 강력한 경험을 제공하기 위해 노력하고 있는 Workfront에 대한 지속적인 지원에 감사드립니다.

추가 질문이 있는 경우 experience.workfront.com을 방문하거나 844.306.4357(미국) 또는 +44.1256.274200(EMEA)으로 전화하여 지원 팀에 문의하십시오.

## FAQ

### Workfront이 이러한 변화를 가져오는 이유는 무엇입니까?

Workfront은 고객에게 가능한 최상의 서비스를 일관되게 제공하기 위해 사용자 경험을 개선하기 위한 방법을 끊임없이 모색합니다. 이러한 변경으로 인해 최상의 경험을 제공하고 이미 강력한 보안 모델을 개선할 수 있는 새로운 기술을 사용할 수 있습니다.

### Workfront 관리자로서 나에게 필요한 작업은 무엇입니까?

위에 나열된 내부 IP 블록을 검토하고 IP 블록을 추가하는 데 도움이 필요하면 IT 또는 보안 부서에 문의하십시오.

### 이 변경을 수행하지 않을 경우 조직에서 기대할 수 있는 사항은 무엇입니까?

서비스를 새 IP로 마이그레이션할 때 Workfront 서비스에 액세스할 수 없습니다.
