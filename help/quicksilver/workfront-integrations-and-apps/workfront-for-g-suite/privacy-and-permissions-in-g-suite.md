---
product-area: workfront-integrations
keywords: google,doc,document,sheet,슬라이드
navigation-topic: workfront-for-g-suite
title: G Suite용 Workfront의 개인 정보 및 권한
description: G Suite용 Workfront의 개인 정보 및 권한
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 90d088846e72f1632274043c8d8ca7807ff05b4a
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# G Suite용 Workfront의 개인 정보 및 권한

고객 개인 정보가 중요하므로 Adobe Workfront은 Google 플러그인 앱의 타사 인증을 통해 생성되는 식별 고객 데이터를 저장하거나 수집하지 않습니다. Workfront for G Suite는 제한된 사용 요구 사항을 포함하여 Google API Services 사용자 데이터 정책을 준수합니다.

G Suite용 Workfront 플러그인이 최대 값을 제공할 수 있으려면 다음 권한이 필요합니다.

* **추가 기능이 실행 중일 때 이메일 메시지 보기**: G Suite용 Workfront 플러그인을 사용하면 이메일을 Workfront의 새로운 작업으로 변환하고 이메일의 제목과 본문으로 작업의 제목과 설명을 자동으로 채워서 수많은 중복 작업을 사용자에게 줄일 수 있습니다. 또한 플러그인을 사용하면 이메일을 Workfront에 새 주석으로 게시할 수 있습니다. 이 값을 제공하려면 추가 기능이 실행 중일 때 플러그인이 이메일 메시지를 확인해야 합니다.
* **Gmail 추가 기능으로 실행 / 민감하지 않음**: Gmail 환경에서 G Suite 추가 기능이 작동하려면 Workfront에 대한 권한이 필요합니다. 플러그인을 사용하려면 Gmail 환경이 작동해야 하므로 `Run as a Gmail add-on / non-sensitive` 권한.
* **추가 기능이 실행 중일 때 이메일 메시지 메타데이터 보기**: 워크플로우를 개선하기 위해 G Suite용 Workfront 플러그인은 이메일이 Workfront 알림인지 확인하고 Workfront 알림 유형(새 작업 요청, 승인 요청, 새 주석 등)을 식별합니다. 플러그인을 사용하려면 `View your email message metadata when the add-on is running` 이 값을 제공할 수 있는 권한.
* **플러그인은 달력 추가 기능/민감하지 않은 것으로 실행해야 합니다**: G Suite용 Workfront 플러그인은 캘린더에 연결되므로 작업이 일정에 미치는 영향을 시각화할 수 있습니다. 플러그인에는 다음이 필요합니다 `Run as a Calendar add-on / non-sensitive` 이 작업을 수행할 수 있는 권한.
* **외부 서비스 권한에 연결:** 궁극적으로 플러그인은 플러그인 값의 백본인 Workfront API에 연결해야 합니다. Workfront API는 Google 외부의 서비스이므로 플러그인을 사용하려면 `Connect to an external service permission` 플러그인을 작동하는 상태로 만듭니다.

Adobe Workfront의 고객 개인 정보 보호에 대한 헌신에 대한 자세한 내용은 [Workfront 개인 정보 보호 알림](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

자세한 내용은 [Google API 서비스 사용자 데이터 정책](https://developers.google.com/terms/api-services-user-data-policy).
