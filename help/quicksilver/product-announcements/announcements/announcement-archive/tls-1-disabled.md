---
content-type: reference
navigation-topic: announcements
title: Adobe Workfront에서 TLS 1.2 필요
description: 최적의 보안을 제공하기 위해 Adobe Workfront에서는 TLS 1.0 이하에 의존하는 모든 브라우저 연결 및 API 통합을 TLS 1.2를 사용하도록 업그레이드해야 합니다. 미리보기 환경에서 TLS 1.0은 이미 비활성화되어 있습니다.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Adobe Workfront에서 TLS 1.2 필요

최적의 보안을 제공하기 위해 Adobe Workfront에서는 TLS 1.0 이하에 의존하는 모든 브라우저 연결 및 API 통합을 TLS 1.2를 사용하도록 업그레이드해야 합니다. 미리보기 환경에서 TLS 1.0은 이미 비활성화되어 있습니다.

Workfront은 2018년 3월에 TLS 1.0에 대한 지원을 공식적으로 종료했습니다. TLS 1.0을 활용하는 모든 통합은 2019년 1월 9일부터 더 이상 작동하지 않습니다.  TLS 1.1은 2019년 4분기에 비활성화됩니다.

다음 섹션에서는 이러한 중요한 이정표에 대해 자세히 설명하고 조직에서 이 업그레이드를 준비하는 방법에 대해 자세히 설명합니다.

## Workfront, TLS 1.0에 대한 공식 지원 종료(2018년 3월 5일)

Workfront은 2018년 3월에 TLS 1.0에 대한 공식 지원을 종료했습니다.

TLS 1.0을 활용하는 브라우저 연결 및 API 통합은 여전히 작동하지만 Workfront은 TLS 1.0과 관련된 Workfront 애플리케이션의 문제를 해결하지는 않습니다.

## TLS 1.0을 사용하는 Workfront 통합 사용 안 함(2019년 1월 9일)

2019년 1월 9일에, TLS 1.0을 활용하는 모든 Workfront 브라우저 연결 및 API 통합이 TLS 1.1 이상을 사용하도록 업그레이드해야 합니다. TLS 1.0(인바운드 또는 아웃바운드 연결)을 계속 활용하는 브라우저 연결 및 API 통합은 이 시간 이후에는 더 이상 Workfront 애플리케이션과 통신할 수 없습니다. 

## TLS 1.1이 2019년 4분기에 비활성화됨

프로덕션 환경에서 TLS 1.1은 2019년 10월 21일에 비활성화되었습니다. 이 시간이 지나면 TLS 1.1을 사용하는 모든 통합이 더 이상 작동하지 않습니다.

이 변경 사항은 조직이 시스템 종료를 준비할 수 있도록 8월 7일에 미리보기 및 샌드박스 환경에서 적용됩니다.

## TLS 업그레이드 준비

* [브라우저를 통해 Workfront에 액세스할 때](#when-accessing-workfront-via-the-browser)
* [API를 통해 Workfront에 연결할 때](#when-connecting-to-workfront-via-the-api)

### 브라우저를 통해 Workfront에 액세스할 때 {#when-accessing-workfront-via-the-browser}

조직의 사용자가 지원되는 브라우저를 통해 Workfront에 액세스하고 있는지 확인합니다. 지원되는 브라우저에 대한 자세한 내용은 [Adobe Workfront 브라우저 요구 사항](../../../workfront-basics/workfront-browser-requirements.md)을 참조하십시오.

Workfront에서 지원하는 모든 브라우저는 TLS 1.2와 호환됩니다.

### API를 통해 Workfront에 연결할 때 {#when-connecting-to-workfront-via-the-api}

API(인바운드 또는 아웃바운드)를 통해 Workfront에 타사 애플리케이션을 통합하는 경우 통합에서 TLS 1.2(및 TLS 1.2 암호화 프로토콜)가 활성화되어 있는지 확인하십시오.
