---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion 릴리스 활동: 2020년 11월 16일의 주'
description: 이 페이지에서는 2020년 11월 16일이 있는 주의 Adobe Workfront Fusion에서 향상된 기능을 모두 설명합니다.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Workfront Fusion 릴리스 활동: 2020년 11월 16일의 주

이 페이지에서는 2020년 11월 16일이 있는 주의 Adobe Workfront Fusion에서 향상된 기능을 모두 설명합니다.

최근 변경 사항 목록을 보려면 [Adobe Workfront Fusion 릴리스 활동](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion의 최근 버그 수정 목록에 대해서는 다음을 참조하십시오. [Workfront 유지 관리 업데이트](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) 페이지를 방문하여 Workfront Fusion Maintenance Update라는 업데이트를 확인하십시오.

## Jira Cloud 커넥터 업데이트

Jira Cloud 커넥터를 사용할 수 있는 방법을 확장하기 위해 세 가지 새로운 모듈을 추가했습니다.

* 스프린트에 문제 추가
* 목록 레코드
* 레코드 검색

또한 &quot;Sprint&quot; 개체 유형을 지원하도록 기존 모듈을 업데이트했습니다. 이전에는 사용자 지정 API 호출 모듈을 통해서만 &quot;Sprint&quot; 개체에 액세스할 수 있었습니다.

자세한 내용은 [Jira 소프트웨어 모듈](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## 이제 시나리오의 매핑에 실행 ID를 사용할 수 있습니다

이제 시나리오에 대한 실행 ID를 매핑 패널에서 사용할 수 있습니다. 이 ID는 시나리오의 특정 실행을 나타내며 메타데이터로 사용할 수 있습니다. 예를 들어 실행 ID를 Fusion에서 생성하는 레코드로 저장할 수 있으므로 나중에 어떤 Fusion 실행에서 레코드를 만들었는지 확인할 수 있습니다. 매핑 패널에서 일반 함수 아래의 실행 ID를 찾을 수 있습니다.

시나리오 실행에 대한 자세한 내용은 [Adobe Workfront Fusion의 시나리오 실행, 주기 및 단계](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Workfront Fusion 2.0 시나리오에 대한 키보드 단축키

시나리오 빌드를 보다 편리하게 하기 위해 몇 가지 키보드 단축키를 추가했습니다.

* Ctrl/Cmd+Shift+Enter: 시나리오 실행
* Ctrl/Cmd + Shift + S: 시나리오 저장

Workfront Fusion 2.0 시나리오 빌드에 대한 자세한 내용은 [Adobe Workfront Fusion에서 시나리오 만들기](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## Office 365 Excel 커넥터 업데이트

Office 365 Excel 커넥터를 사용할 수 있는 방법을 확장하기 위해 몇 가지 새로운 모듈을 추가했습니다. 이제 다음을 수행할 수 있습니다.

* 통합 문서 변경 사항에서 모듈을 트리거합니다
* 통합 문서 검색 또는 다운로드
* 워크시트, 워크시트 행, 테이블 또는 테이블 행 나열
* 테이블 또는 워크시트 행 업데이트
* 테이블 또는 워크시트 행 삭제
* 테이블에 대한 메타데이터 검색
* 사용자 지정 API 호출 만들기

이전에 사용 가능한 모듈이 여전히 앱에 있습니다.

자세한 내용은 [Microsoft Office 365 Excel 모듈](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## Workfront 앱 연결에서 OAuth 2.0 사용

OAuth 2.0을 사용하도록 Workfront 커넥터를 업데이트했습니다. 이 업데이트는 Workfront 앱 연결을 더 쉽게 변경할 수 있음을 의미합니다. 예를 들어, 연결 변경 사항(예: 암호)이 발생하는 경우 시나리오에서는 각 개별 연결을 더 이상 업데이트할 필요가 없습니다. 또한 OAuth2는 보안 향상 및 SSO(Single Sign-on)를 사용하는 기능 등의 다른 이점을 제공합니다.

현재 기존 연결을 변경할 필요가 없습니다. 그러나 OAuth 2.0의 이점을 활용하려는 경우 기존 연결을 재인증할 수 있습니다.

자세한 내용은 [Adobe Workfront 모듈](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
