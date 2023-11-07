---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: 웹후크 개요
description: 웹후크 개요
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# 웹후크 개요

Adobe Workfront Document Webhooks는 Workfront이 외부 문서 공급자에 대해 승인된 API 호출을 수행하는 API 엔드포인트 세트를 정의합니다. 이를 통해 모든 문서 스토리지 공급자에 대한 미들웨어 플러그인을 생성할 수 있습니다.

![](assets/mceclip0-350x262.png)

Webhook 기반 통합을 위한 사용자 경험은 Google Drive, Box 및 Dropbox과 같은 기존 문서 통합의 사용자 경험과 유사합니다. 예를 들어 Workfront 사용자는 다음 작업을 수행할 수 있습니다.

* 외부 문서 공급자의 폴더 구조 탐색
* 파일 검색
* Workfront에 파일 연결
* 외부 문서 공급자에 파일 업로드
* 문서의 축소판 보기

**참조 구현**

새 웹후크 구현의 개발을 바로 시작할 수 있도록 Workfront에서는 참조 구현의 예를 제공합니다. 이러한 예는 다음에서 찾을 수 있습니다. [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). 예제는 Java 기반이며 Workfront에서 네트워크 파일 시스템의 문서를 연결할 수 있도록 해줍니다. 

>[!NOTE]
>
>GitHub의 리소스는 예시일 뿐이며 구현을 실행할 수 없습니다.

## 버전

* 버전 1.0(릴리스 날짜 - 2015년 5월): 초기 사양

* 버전 1.1(릴리스 날짜 - 2015년 6월). 업데이트된 /uploadInit - 추가된 documentId 및 documentVersionId

* 버전 1.2(릴리스 날짜 - 2015년 10월): /createFolder 추가됨

* 예정된 버전(릴리스 날짜 - 미정):

   * /delete 추가됨
   * /rename이 추가되었습니다.
   * /serviceInfo 추가됨
   * /customAction 추가됨
   * /search에 페이지 매김 및 parentId 추가
