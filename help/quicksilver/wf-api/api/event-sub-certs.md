---
content-type: api
navigation-topic: api-navigation-topic
title: 이벤트 구독 인증서
description: 이벤트 구독 인증서
author: Becky
feature: Workfront API
source-git-commit: 53ef8f4fda22c912c274841d07ad865aa04141c8
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 이벤트 구독에 대한 클라이언트 TLS 구성

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

클라이언트 TLS를 사용하면 수신한 이벤트 구독 메시지가 실제로 Adobe Workfront에서 왔는지를 확인할 수 있습니다. 이 기능을 사용하려면 Workfront의 x509 인증서를 요청하고 확인하도록 서버를 구성해야 합니다.


## Workfront의 클라이언트 인증서 확인

이 절차에서는 서버가 TLS 연결을 허용하도록 구성되어 있다고 가정합니다. Workfront은 자체 서명된 인증서를 지원하지 않습니다.

일반적으로 서버에 대해 클라이언트 인증을 설정하는 데 필요한 단계는 다음과 같습니다.

1. DigiCert Global Root CA 인증서의 PEM 버전을 다운로드합니다.
1. 클라이언트 인증서 확인을 켜십시오.

   1단계의 CA 인증서를 트러스트된 것으로 지정합니다.

1. DigiCert Global Root CA에서 중간 CA인 DigiCert SHA2 Secure Server CA에 의해 인증서가 실제로 서명되었으므로 확인 깊이를 2로 설정하십시오.
1. 주체 도메인 이름을 검사하여 클라이언트 인증서가 Workfront에서 실제로 발생하는지 확인합니다.

## 서버 구성의 예

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

자세한 내용은 [ngx_http_ssl_module에 대한 NGiNX 설명서](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

자세한 내용은

* [클라이언트 인증 및 액세스 제어](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache 모듈 mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## 인증서 대 환경 매핑

| WF 환경 | 인증서 공통 이름 | 인증서 주체(DN) | | — | — | — | | 프로덕션 | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com| | 미리 보기 | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com | | 샌드박스 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com | | 샌드박스 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## 인증서 다운로드

다음 링크를 클릭하여 클라이언트 인증서를 다운로드합니다.

* [클라이언트 인증서 - 프로덕션 환경](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [클라이언트 인증서 - 미리 보기 환경](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [클라이언트 인증서 - 샌드박스 환경](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>두 샌드박스 환경 모두에 동일한 클라이언트 인증서를 사용할 수 있습니다.

