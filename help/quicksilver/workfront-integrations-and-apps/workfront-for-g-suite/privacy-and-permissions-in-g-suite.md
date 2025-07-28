---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Google Workspace용 Workfront의 개인 정보 및 권한
description: Google Workspace용 Workfront의 개인 정보 및 권한
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Google Workspace용 Workfront의 개인 정보 및 권한

>[!IMPORTANT]
>
>보다 안정적이고 확장 가능한 통합을 제공하기 위해 Workfront 자동화 및 통합(Fusion)을 사용하는 현대적이고 유연한 통합 접근 방식으로 전환하고 있습니다. 이 전환 프로세스의 일부로 다음 Google Workspace용 Workfront 기능은 **2026년 2월 28일** 이후에 사용할 수 없습니다.
>
>* Workfront 내에서 Google Workspace 기능 액세스
>
>* Gmail 또는 Google Calendar 사이트 패널에서 Workfront 작업 보기 및 관리
>
>조직의 Google Workspace 통합 요구 사항에 맞게 Workfront 자동화 및 통합을 사용하는 것이 좋습니다.
>
>Workfront 자동화 및 통합에 대한 개요는 [Adobe Workfront Fusion 개요](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)를 참조하십시오.
>
>Google Workspace용 Workfront 자동화 및 통합 모듈의 특정 기능에 대한 자세한 내용은 [Gmail 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) 및 [Google 달력 모듈](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)을 참조하십시오.

고객 개인 정보가 중요하기 때문에 Adobe Workfront은 Google 플러그인 앱의 서드파티 인증으로 인해 발생하는 식별 고객 데이터를 저장하거나 수집하지 않습니다. Google용 Workfront Workspace이 Google API에서 받은 정보를 사용하고 다른 앱으로 전송하면 사용 제한 요구 사항을 포함하여 [Google API 서비스 사용자 데이터 정책](https://developers.google.com/terms/api-services-user-data-policy)을 준수합니다.

Workfront for Google Workspace 플러그인이 최대 가치를 제공할 수 있으려면 다음 권한이 필요합니다.

* **추가 기능이 실행되고 있을 때 전자 메일 메시지 보기**: Google Workspace용 Workfront 플러그인을 사용하면 전자 메일을 Workfront의 새 작업으로 변환하고 작업의 제목과 설명을 전자 메일의 제목과 본문으로 자동으로 채워 사용자가 수 시간 동안 중복적인 작업을 할 필요가 없습니다. 또한 플러그인을 사용하면 이메일을 Workfront에 새로운 주석으로 게시할 수 있습니다. 이 값을 게재하려면 추가 기능이 실행 중일 때 플러그인이 이메일 메시지를 확인해야 합니다.
* **Gmail 추가 기능으로 실행/민감하지 않음**: Google용 Workfront Workspace 추가 기능이 Gmail 환경에서 작동하려면 권한이 필요합니다. 플러그인을 사용하려면 Gmail 환경이 필요하므로 `Run as a Gmail add-on / non-sensitive` 권한이 필요합니다.
* **추가 기능이 실행되고 있을 때 전자 메일 메시지 메타데이터를 봅니다**: 워크플로를 개선하기 위해 Google Workspace용 Workfront 플러그인은 전자 메일이 Workfront 알림인지 확인하고 Workfront 알림의 유형(새 작업 요청, 승인 요청, 새 댓글 등)을 식별합니다. 이 값을 전달하려면 플러그인에 `View your email message metadata when the add-on is running` 권한이 필요합니다.
* **플러그 인을 일정 추가 기능/민감하지 않게 실행해야 함**: Google Workspace용 Workfront 플러그 인이 일정에 연결되므로 작업이 일정에 미치는 영향을 시각화할 수 있습니다. 이 작업을 수행하려면 플러그인에 `Run as a Calendar add-on / non-sensitive` 권한이 필요합니다.
* **외부 서비스 권한에 연결:** 궁극적으로 플러그인은 플러그인 값의 백본인 Workfront API에 연결해야 합니다. Workfront API는 Google의 외부 서비스이므로 플러그인이 작동하려면 `Connect to an external service permission`이(가) 필요합니다.

Adobe Workfront의 고객 개인 정보 보호에 대한 자세한 내용은 [Workfront의 개인 정보 보호 알림](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf)을 참조하십시오.

자세한 내용은 [Google API 서비스 사용자 데이터 정책](https://developers.google.com/terms/api-services-user-data-policy)을 참조하세요.
