---
content-type: reference
navigation-topic: announcements
title: 클러스터 1, 2 및 3의 고객은 Adobe Workfront 서비스허용 목록에 추가하다가 차단되지 않도록 모든 IP 블록을 업데이트해야 합니다
description: 핵심 인프라를 향상시키고 개선하기 위해 곧 Adobe Workfront 고객을 클러스터 01, 02 및 03 로 AWS 공용 클라우드로 마이그레이션할 예정입니다.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 4%

---

# 클러스터 1, 2 및 3의 고객은 Adobe Workfront 서비스허용 목록에 추가하다가 차단되지 않도록 모든 IP 블록을 업데이트해야 합니다

핵심 인프라를 향상시키고 개선하기 위해 곧 Adobe Workfront 고객을 클러스터 01, 02 및 03 로 AWS 공용 클라우드로 마이그레이션할 예정입니다.

이 변경의 일부로, Workfront 서비스의 차단을 방지하려면 다음 IP를 IP 블록에 추가해야 허용 목록에 추가하다 합니다.

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

이메일의 경우:

* 54.240.60.174
* 54.240.60.175

IP 허용 목록에 추가하다 블록이 2019년 5월 13일까지 업데이트되었는지 확인하십시오. 자세한 내용은 [방화벽 허용 목록에 추가하다 구성](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Adobe에서 보다 안정적이고 강력한 고객 경험을 만들기 위해 노력하고 있는 Workfront을 계속 지원해 주셔서 감사합니다.

추가 질문 사항은 experience.workfront.com을 방문하거나 844.306.4357(미국) 또는 +44.1256.274200(EMEA)로 전화하여 지원 팀에 문의하십시오.

## FAQ

### Workfront이 이 변경 작업을 수행하는 이유는 무엇입니까?

Workfront은 고객에게 최상의 서비스를 지속적으로 제공하기 위한 노력의 일환으로 사용자 경험을 개선할 수 있는 방법을 끊임없이 모색하고 있습니다. 이러한 변경 사항으로 인해 최상의 경험을 제공하고 이미 강력한 보안 모델을 개선할 수 있는 새로운 기술을 사용할 수 있습니다.

### Workfront 관리자로서 제가 필요로 하는 작업은 무엇입니까?

IP 블록을 검토하고 위에 나열된 IP를 추가하는 허용 목록에 추가하다 데 도움이 필요하면 내부 IT 또는 보안 부서에 문의하십시오.

### 이 변경을 수행하지 않을 경우 조직에서 예상할 수 있는 것은 무엇입니까?

서비스를 새 IP로 마이그레이션하면 Workfront 서비스에 액세스할 수 없습니다.
