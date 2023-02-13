---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhooks 개요
description: Webhooks 개요
author: John
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Webhooks 개요

Adobe Workfront Document Webhooks는 Workfront에서 외부 문서 공급자에 인증된 API 호출을 수행하는 API 엔드포인트 집합을 정의합니다. 이렇게 하면 누구나 문서 저장소 공급자에 대한 미들웨어 플러그인을 만들 수 있습니다.

![](assets/mceclip0-350x262.png)

웹 후크 기반 통합에 대한 사용자 경험은 Google 드라이브, 상자, Dropbox과 같은 기존 문서 통합의 사용자 경험과 비슷합니다. 예를 들어 Workfront 사용자는 다음 작업을 수행할 수 있습니다.

* 외부 문서 공급자의 폴더 구조 탐색
* 파일 검색
* Workfront에 파일 연결
* 외부 문서 공급자에 파일 업로드
* 문서의 축소판 보기

**참조 구현**

새 웹 후크 구현 개발을 시작하는 데 도움이 되도록 Workfront에서 참조 구현을 제공합니다. 이에 대한 코드는 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . 이 구현은 Java 기반이며, Workfront에서 네트워크 파일 시스템에서 문서를 연결할 수 있도록 합니다. 

## 버전

* 버전 1.0(릴리스 날짜 - 2015년 5월): 초기 사양

* 버전 1.1(릴리스 날짜 - 2015년 6월). /uploadInit 업데이트 - documentId 및 documentVersionId가 추가되었습니다.

* 버전 1.2(릴리스 날짜 - 2015년 10월): /createFolder 를 추가했습니다.

* 예정된 버전(릴리스 날짜 - TBD):

   * 추가/삭제
   * 추가/이름 바꾸기
   * /serviceInfo가 추가되었습니다.
   * /customAction 추가
   * /search에 페이지 매김 및 parentId 추가
