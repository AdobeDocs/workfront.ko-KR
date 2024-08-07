---
title: 개요
description: 개요
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# 개요

**Workfront Proof API 시작**

Workfront Proof API는 SSL을 사용하여 보호되는 간단한 HTTP 서비스입니다. API는 자체 애플리케이션에서 사용되는 모든 기능을 제공하는 것을 목표로 합니다.

## 지원되는 형식

공용 인터페이스는 WSDL 지원을 준수하는 SOAP 1.1입니다. 따라서 모든 요청은 HTTPS를 통해 XML을 사용하여 실행됩니다.

## API 버전 관리

기존 클라이언트 통합과의 호환성을 유지하기 위해 12.1 릴리스부터 API 버전 관리를 도입했습니다. 다음을 참조하십시오.  자세한 내용은 [API 업데이트](https://api.proofhq.com/new-updates.html) 페이지를 참조하십시오. 메서드나 매개 변수에 버전 정보가 없으면 표준 API의 일부로 이 메서드를 찾을 수 있다는 의미입니다. 아래의 &quot;API 시작하기&quot; 섹션을 참조하십시오.

## API 시작하기

API 진입점:

`https://soap.proofhq.com/soap`(HTTPS 사용 참고)

WSDL은 여기에서 찾을 수 있습니다.

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**이 WSDL에는 12.1 릴리스까지 모든 변경 내용이 포함되어 있으며 그 이후에는 API 버전 관리가 도입되었습니다. 다양한 WSDL 버전 및 향후 변경 사항에 대한 자세한 내용은 API 업데이트 페이지를 참조하십시오**

모든 API 요청에는 세션 키가 필요합니다. 이 세션 키는 작업을 수행하는 Workfront Proof 사용자를 식별하며 doLogin() 메서드를 호출하고 사용자의 이메일 주소와 암호를 전달하여 가져옵니다. doLogin() 메서드는 API 요청 시퀀스 전에 한 번만 호출하면 됩니다. 세션 키는 짧은 시간 동안 활성 상태로 유지되며 모든 메서드 호출 시 갱신됩니다. *토큰 기반 인증에 대한 지원을 곧 추가합니다.*

모든 요청은 다음 envelope, header 및 body 형식을 사용합니다.

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

