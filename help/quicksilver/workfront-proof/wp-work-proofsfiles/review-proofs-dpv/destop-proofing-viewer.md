---
content-type: overview
product-previous: workfront-proof
product-area: documents
navigation-topic: review-proofs-desktop-proofing-viewer
title: Desktop Proofing 뷰어 이해
description: Desktop Proofing Viewer는 대화형 컨텐츠의 교정을 위해 설계되었지만 정적 및 비디오 컨텐츠의 교정을 위해서도 사용할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 4610f24f-345a-4ebc-8a0c-382e34cac7b0
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Desktop Proofing 뷰어 이해

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

Desktop Proofing Viewer는 대화형 컨텐츠의 교정을 위해 설계되었지만 정적 및 비디오 컨텐츠의 교정을 위해서도 사용할 수 있습니다.

웹 증명 뷰어와 달리 데스크탑 증명 뷰어는 워크스테이션에서 실행되는 애플리케이션입니다. 그러나 증명을 실행할 때는 독립 실행형 응용 프로그램으로 실행하지 않고 [!DNL Workfront] 또는 [!DNL Workfront Proof]에서 액세스할 수 있습니다. 데스크톱 증명 뷰어 설치에 대한 자세한 내용은 [데스크톱 증명 뷰어 설치](../../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)를 참조하십시오.

## 데스크탑 증명 뷰어와 다른 증명 뷰어 비교

* [데스크탑 증명 뷰어와 웹 증명 뷰어](#desktop-proofing-viewer-vs-web-proofing-viewer)
* [데스크탑 증명 뷰어와 레거시 증명 뷰어](#desktop-proofing-viewer-vs-legacy-proofing-viewer)

### 데스크탑 증명 뷰어와 웹 증명 뷰어 {#desktop-proofing-viewer-vs-web-proofing-viewer}

다음 두 가지 주요 특성은 Desktop Proofing Viewer와 Web Proofing Viewer를 구분합니다.

* Desktop Proofing Viewer를 사용하면 웹 사이트, 스트리밍 비디오 또는 대화형 배너와 같은 대화형 컨텐츠를 검토할 수 있으며, Web Proofing Viewer를 사용하면 정적 및 비디오 증명만 검토할 수 있습니다.
* Desktop Proofing Viewer는 로컬 컴퓨터에서 응용 프로그램으로 실행되고 Web Proofing Viewer는 브라우저에서 실행됩니다.

  >[!NOTE]
  >
  >   * 보안상의 이유로 조직에서 Desktop Proofing Viewer 앱을 사용할 수 없는 경우 [!DNL Workfront] 관리자는 사용자가 웹 증명 뷰어에서 ZIP 보관 파일에 번들로 제공된 대화형 콘텐츠를 검토할 수 있도록 시스템을 구성할 수 있습니다.
  >   * 증명 만들기 및 탐색 등의 증명 관리 작업은 [!DNL Workfront] 또는 [!DNL Workfront Proof]에서 수행됩니다. Desktop Proofing Viewer는 증명을 검토하는 용도로만 사용됩니다.


다양한 증명 뷰어의 기능에 대한 자세한 내용은 [웹 증명 뷰어와 데스크톱 증명 뷰어의 차이점](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)을 참조하십시오.

### 데스크탑 증명 뷰어와 레거시 증명 뷰어 {#desktop-proofing-viewer-vs-legacy-proofing-viewer}

레거시 증명 뷰어는 대부분의 환경에서 더 이상 사용되지 않는 Flash에서 지원하므로 액세스 권한이 없을 수도 있습니다.

Desktop Proofing Viewer에는 기존 증명 뷰어에 대한 다음과 같은 개선 사항이 포함되어 있습니다.

* 보안(HTTPS) 사이트뿐만 아니라 비보안(HTTP) 사이트를 검토합니다.
* iFrame으로 보호된 사이트(iFrame 내에서 볼 수 없는 사이트)를 검토합니다.
* 다양한 디바이스에 대해 미리 구성된 해상도로 콘텐츠를 볼 수 있습니다.\
   예를 들어 다양한 표준 데스크탑 해상도나 iPhone 8과 같은 개별 디바이스에서 콘텐츠가 표시되는 방식을 확인할 수 있습니다.

레거시 증명 뷰어는 2018년 연말에 2018.3 릴리스를 통해 [!DNL Workfront]에서 제거됩니다.

2018년 7월 2018.2 릴리스 이후 [!DNL Workfront]을(를) 가져오는 고객의 경우 레거시 증명 뷰어가 포함되지 않습니다.

## 데스크탑 증명 뷰어에서 비대화형 증명을 열기 위한 사용자 설정

Desktop Proofing Viewer의 주요 목적은 증명 대화형 컨텐츠이지만 이를 사용하여 정적 및 비디오 증명을 수행할 수도 있습니다.

사용자는 정적 증명 및 비디오 증명을 포함한 모든 종류의 증명을 열 때 자동으로 시작되도록 데스크톱 증명 뷰어를 구성할 수 있습니다. 자세한 내용은 [증명 뷰어 설정 구성](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)을 참조하십시오.

## 증명 URL 입력

워크스테이션에서 바로 데스크톱 증명 뷰어를 시작하면 증명 URL을 지정하여 증명을 열 수 있습니다. 이를 수행하려면 보려는 증명의 증명 URL이 있어야 합니다.

[!DNL Workfront]에서 직접 증명을 여는 것이 좋습니다. 자세한 내용은 [증명 검토](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md)를 참조하십시오.
