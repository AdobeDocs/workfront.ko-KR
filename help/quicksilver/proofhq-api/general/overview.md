---
title: 개요
description: 개요
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# 개요

**Workfront 증명 API를 시작합니다**

Workfront 증명 API는 SSL을 사용하여 보안이 설정된 간단한 HTTP 서비스입니다. API는 고유한 애플리케이션에서 사용되는 모든 기능을 제공하는 것을 목표로 합니다.

## 지원되는 형식

공용 인터페이스는 WSDL 지원과 호환되는 SOAP 1.1입니다. 따라서 모든 요청은 HTTPS를 통해 XML을 사용하여 실행됩니다.

## API 버전 관리

기존 클라이언트 통합과의 호환성을 유지하기 위해 12.1 릴리스부터 API 버전 지정을 도입했습니다. 자세한 내용은  [API 업데이트](http://api.proofhq.com/new-updates) 페이지를 참조하십시오. 메서드 또는 매개 변수에 버전 정보가 없는 경우 표준 API의 일부로 이 정보를 찾을 수 있음을 의미합니다. 아래의 &quot;API 시작하기&quot; 섹션을 참조하십시오.

## API 시작하기

API 시작 지점:

`https://soap.proofhq.com/soap` (HTTPS의 사용에 유의하십시오.)

WSDL은 다음 위치에서 찾을 수 있습니다.

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**이 WSDL은 API 버전 지정을 도입한 후 12.1 릴리스까지 모든 변경 사항을 포함합니다. 다양한 WSDL 버전 및 예정된 변경 사항에 대한 자세한 내용은 API 업데이트 페이지를 참조하십시오**

모든 API 요청에는 세션 키가 필요합니다. 이 세션 키는 작업을 수행하는 Workfront 증명 사용자를 식별하고 doLogin() 메서드를 호출하고 사용자의 이메일 주소와 암호를 전달하여 가져옵니다. doLogin() 메서드는 API 요청 시퀀스 전에 한 번만 호출해야 합니다. 세션 키는 짧은 시간 동안 활성 상태로 유지되며 모든 메서드 호출 시 갱신됩니다. *곧 토큰 기반 인증에 대한 지원을 추가할 예정입니다.*

모든 요청에는 다음 봉투, 헤더 및 본문 형식이 사용됩니다.

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
	   ... API function and data inserted here ...
	</soapenv:Body>
	</soapenv:Envelope>
```

## FAQ

FAQ를 보려면 [이](http://api.proofhq.com/faqs) 페이지.
