---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook 연결 테스트
description: Webhook 연결 테스트
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# Webhook 연결 테스트

문서 Webhook 구현이 올바르게 작동하는지 확인하려면 이 섹션에서 수동 테스트를 실행합니다. 이러한 단계는 Adobe Workfront 웹 인터페이스를 통과하여 Webhook 구현의 끝점을 간접적으로 공격합니다.

## 전제 조건

테스트를 실행하려면 다음 전제 조건이 필요합니다.

* ADM(Advanced Document Management)이 활성화된 Workfront 계정

* 시스템 관리자 권한이 있는 이 계정의 Workfront 사용자

* Workfront에 액세스할 수 있는 HTTP 끝점이 있는 문서 Webhook 인스턴스

또한 이러한 테스트에서는 Document Webhook 인스턴스가 등록되어 있다고 가정합니다. ( 설정 > 문서 > 사용자 정의 통합 아래의 Workfront에서 인스턴스를 등록할 수 있습니다.)

**테스트 1: 사용자를 위해 Document Webhook 서비스 제공**

OAuth 기반 웹후크 공급자에 대한 인증 URL 및 토큰 끝점 URL을 테스트합니다.

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. Add Documents 드롭다운을 클릭하고 Add Service 아래에서 Document Webhook 서비스를 선택합니다.
1. (OAuth 서비스만 해당) 이전 단계를 완료하면 서비스의 OAuth2 인증 페이지가 팝업 창에 로드됩니다. (참고: 먼저 서비스에 로그인하라는 메시지가 표시될 수 있습니다.) 인증 페이지에서 [신뢰] 또는 [허용] 단추를 클릭하여 Workfront에 사용자 계정에 대한 액세스 권한을 부여합니다.
1. 서비스가 문서 추가 드롭다운에 추가되었는지 확인합니다. 처음에 표시되지 않으면 브라우저를 새로 고침해 보십시오.

**테스트 2: Workfront에 문서 연결 /files, /metadata**

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. 문서 추가에서 Document Webhook 서비스를 선택합니다.
1. 모달에서 폴더 구조를 탐색합니다.
1. 폴더 구조를 탐색할 수 있는지 확인합니다.
1. 문서를 선택하여 Workfront에 연결

**테스트 3: 콘텐츠 관리 시스템의 문서로 이동**

/metadata(특히 viewLink) 끝점을 테스트합니다.

1. Workfront에 문서 연결
1. 문서를 선택하고 열기 링크를 클릭합니다.
1. 문서가 새 탭에서 열리는지 확인합니다.

**테스트 4: 콘텐츠 관리 시스템(로그인 포함)에서 문서로 이동**

/metadata(특히 viewLink) 끝점을 테스트합니다.

1. 컨텐츠 관리 시스템에서 로그아웃되었는지 확인합니다.
1. Workfront에 문서를 연결합니다.
1. 문서를 선택하고 열기 링크를 클릭합니다.
1. 컨텐츠 관리 시스템의 로그인 화면이 새 탭에 로드되는지 확인합니다.
1. 로그인하고 문서에 연결되었는지 확인합니다.

**테스트 5: 콘텐츠 관리 시스템에서 문서를 다운로드합니다**

다음 엔드포인트(특히 다운로드 링크)를 테스트합니다. /metadata 

1. Workfront에 문서를 연결합니다.
1. 문서를 선택하고 다운로드 링크를 클릭합니다.
1. 다운로드가 시작되는지 확인합니다.

**테스트 6: 콘텐츠 검색**

다음 끝점을 테스트합니다. /search

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. 문서 추가에서 Document Webhook 서비스를 선택합니다.
1. 모달에서 검색을 수행합니다.
1. 검색 결과가 올바른지 확인합니다.

**테스트 7: Workfront에서 컨텐츠 관리 시스템으로 문서 보내기**

/files, /uploadInit, /upload 끝점을 테스트합니다.

1. Workfront에서 상단 탐색 막대에 있는 문서 링크를 클릭하여 기본 문서 페이지로 이동합니다.
1. 컴퓨터에서 Workfront으로 문서 업로드
1. 문서 세부 정보 페이지로 이동
1. Document Actions 드롭다운에서 Send To...에 있는 Document Webhook 서비스를 선택합니다.
1. 원하는 대상 폴더로 이동하고 저장 버튼을 클릭합니다.
1. 문서가 컨텐츠 관리 시스템의 올바른 위치에 업로드되었는지 확인합니다.

**테스트 8: Workfront에서 썸네일 보기**

다음 끝점을 테스트합니다. /thumbnail

1. Workfront에 문서를 연결합니다.
1. 목록에서 문서를 선택합니다.
1. 축소판이 오른쪽 패널에 표시되는지 확인합니다.

**테스트 9: 콘텐츠 바이트 가져오기**

다음 끝점을 테스트합니다. /download

1. Workfront에 문서를 연결합니다.
1. 문서 세부 정보 페이지로 이동합니다.
1. [문서 작업] > [전송 대상...] > [Workfront]를 선택하여 Workfront으로 문서를 전송합니다. 이렇게 하면 Workfront에 새 문서 버전이 만들어집니다.
1. 다운로드 링크를 클릭하여 Workfront에서 문서를 다운로드합니다.

**테스트 10: 액세스 토큰 새로 고침(OAuth2 Webhook 공급자만 해당)**

다음 끝점을 테스트합니다. 토큰 끝점 URL

1. 사용자를 위한 Document Webhook 서비스 제공
1. 사용자의 액세스 토큰을 무효화하려면 1) 시간이 초과될 때까지 기다리거나, 2) 외부 시스템에서 수동으로 무효화하십시오.
1. Workfront에서 액세스 토큰을 새로 고칩니다. 예를 들어 문서를 Workfront에 연결하여 이 작업을 수행할 수 있습니다. 문서로 이동하여 연결할 수 있으면 액세스 토큰이 성공적으로 새로 고쳐졌다는 것을 알 수 있습니다.

>[!NOTE]
>
>현재 연결된 문서에는 전송 대상...을 사용할 수 없습니다. Workfront에서 추가합니다. Postman과 같은 REST 클라이언트를 사용하여 수동으로 끝점을 눌러 /download 끝점을 테스트할 수 있습니다. 또는 디지털 증명을 생성하여 /download 끝점을 테스트할 수 있습니다. 디지털 증명을 활성화하려면 Workfront에 문의하십시오.
