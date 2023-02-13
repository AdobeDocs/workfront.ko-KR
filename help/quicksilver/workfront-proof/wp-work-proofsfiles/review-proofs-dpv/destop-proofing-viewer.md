---
content-type: overview
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-desktop-proofing-viewer
title: 데스크탑 교정 뷰어 이해
description: Desktop Proofing Viewer는 대화형 내용을 교정할 수 있도록 고안되었지만, 정적 및 비디오 내용을 교정할 수도 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 4610f24f-345a-4ebc-8a0c-382e34cac7b0
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 데스크탑 교정 뷰어 이해

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

Desktop Proofing Viewer는 대화형 내용을 교정할 수 있도록 고안되었지만, 정적 및 비디오 내용을 교정할 수도 있습니다.

Web Proofing Viewer와 달리 Desktop Proofing Viewer는 워크스테이션에서 실행되는 응용 프로그램입니다. 그러나 다음에서 액세스할 수 있습니다. [!DNL Workfront] 또는 [!DNL Workfront Proof] 증명을 실행하는 대신 독립형 애플리케이션으로 실행하는 경우(데스크톱 언어 교정 뷰어 설치에 대한 자세한 내용은 [데스크탑 교정 뷰어 설치](../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)).

## 데스크탑 교정 뷰어와 다른 언어 교정 뷰어 비교

* [데스크탑 교정 뷰어와 웹 교정 뷰어 비교](#desktop-proofing-viewer-vs-web-proofing-viewer)
* [데스크탑 교정 뷰어와 레거시 교정 뷰어 비교](#desktop-proofing-viewer-vs-legacy-proofing-viewer)

### 데스크탑 교정 뷰어와 웹 교정 뷰어 비교 {#desktop-proofing-viewer-vs-web-proofing-viewer}

두 가지 주요 특징은 Desktop Proofing Viewer와 Web Proofing Viewer를 구분합니다.

* 데스크탑 언어 교정 뷰어를 사용하면 웹 사이트, 스트리밍 비디오 또는 대화형 배너와 같은 대화형 컨텐츠를 검토할 수 있습니다. 웹 교정 뷰어를 사용하면 정적 및 비디오 증명만 검토할 수 있습니다.
* 데스크탑 언어 교정 뷰어는 로컬 컴퓨터에서 응용 프로그램으로 실행됩니다. 브라우저에서 웹 언어 교정 뷰어가 실행됩니다.

   >[!NOTE]
   >
   >   * 보안상의 이유로 조직에서 데스크탑 언어 교정 뷰어 앱을 사용할 수 없는 경우 [!DNL Workfront] 관리자는 Web Proofing Viewer에서 ZIP 아카이브 파일에 번들로 제공된 대화형 컨텐츠를 검토할 수 있도록 시스템을 구성할 수 있습니다.
   >   * 증명 만들기 및 증명 검색과 같은 증명 관리 작업은 [!DNL Workfront] 또는 [!DNL Workfront Proof]. 데스크탑 교정 뷰어는 증명을 검토할 용입니다.



다양한 언어 교정 뷰어의 기능에 대한 자세한 내용은 [Web Proofing Viewer와 Desktop Proofing Viewer 개요의 차이점](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)

### 데스크탑 교정 뷰어와 레거시 교정 뷰어 비교 {#desktop-proofing-viewer-vs-legacy-proofing-viewer}

대부분의 환경에서 더 이상 사용되지 않는 Flash에서 지원되므로 레거시 언어 교정 뷰어에 액세스할 수 없습니다.

Desktop Proofing Viewer에는 레거시 교정 뷰어에 대한 다음과 같은 개선 사항이 포함되어 있습니다.

* 보안(HTTPS) 사이트뿐만 아니라 보안되지 않은(HTTP) 사이트를 검토합니다.
* iFrame으로 보호된 사이트(iFrame 내에서 볼 수 없는 사이트)를 검토합니다.
* 다양한 장치에 대해 사전 구성된 해상도로 콘텐츠를 봅니다.\
   예를 들어, 다양한 표준 데스크탑 해상도나 iPhone 8과 같은 개별 장치에서 컨텐츠가 표시되는 방식을 확인할 수 있습니다.

레거시 언어 교정 뷰어가 [!DNL Workfront] ( 2018년 말 2018.3 릴리스 포함)

기존 언어 교정 뷰어는 고객이 획득하는 데 포함되지 않습니다 [!DNL Workfront] 2018년 7월 2018.2 릴리스 이후

## 데스크탑 교정 뷰어에서 비대화형 증명을 여는 사용자 설정

데스크탑 언어 교정 뷰어의 주요 목적은 대화형 컨텐츠에 교정을 제공하는 것이지만 정적 및 비디오 증명을 증명하기 위해 사용할 수도 있습니다.

사용자는 정적 및 비디오 증명을 포함하여 모든 종류의 증명을 열 때 자동으로 실행되도록 데스크탑 교정 뷰어를 구성할 수 있습니다. 자세한 내용은 [언어 교정 뷰어 설정 구성](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md).

## 증명 URL 입력

워크스테이션에서 직접 데스크탑 교정 뷰어를 시작하는 경우 증명 URL을 지정하여 증명을 열 수 있습니다. 이를 수행하려면 보려는 증명의 증명 URL이 있어야 합니다.

에서 직접 증명을 여는 것이 좋습니다 [!DNL Workfront]. 자세한 내용은 [증명 검토](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).
