---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 문제 해결 - [!DNL Workfront Proof] 증명 뷰어
description: 증명 콘텐츠가 로드되지 않고 빈 증명 뷰어만 표시되는 경우, 무언가가 이 작업을 로컬에서 차단하기 때문에 발생할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 39fdf5c2c2114a82c48f515c4a9f088596394045
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# 문제 해결 - [!DNL Workfront Proof] 증명 뷰어

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

증명 콘텐츠가 로드되지 않고 빈 증명 뷰어만 표시되는 경우, 무언가가 이 작업을 로컬에서 차단하기 때문에 발생할 수 있습니다. 아래에서 가능한 해결 방법을 시도해 보십시오.

## 브라우저 <!--and [!DNL Flash Player]--> 버전이 최신 버전인지 확인합니다.

모든 개발자는 애플리케이션을 지속적으로 작업하며 제품에 대한 새로운 기능과 수정 사항을 정기적으로 릴리스합니다. 사용자 경험을 개선하고 보안 수준을 유지하기 위한 것이므로 최신 버전만 사용하는 것이 좋습니다. 또한 애플리케이션 간의 충돌을 피하는 데 도움이 됩니다.

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### 브라우저 버전

일반적으로 대부분의 브라우저는 자동으로 업데이트되지만 문제가 발생하는 경우 사용 중인 버전을 확인하고 필요한 경우 업데이트를 수행하는 것이 좋습니다.

브라우저에서 [!UICONTROL 메뉴] (으)로 이동하여 [!UICONTROL 정보] 옵션을 찾습니다(경우에 따라 [!UICONTROL 도움말] 메뉴에 표시될 수 있음). [!UICONTROL 정보] 팝업에서 현재 브라우저 버전에 대한 정보와 업데이트를 업데이트/확인하는 옵션을 찾을 수 있습니다.

예를 들어 Chrome에서:

![Chrome 브라우저 버전](assets/proofview-3.png)

최신 브라우저 버전을 설치한 후 증명을 다시 열어 문제가 해결되었는지 확인하십시오.

<!--

## Ensure Your Local [!DNL Flash] Storage is Available

Our [!DNL Workfront Proof] Viewer is based on Flash, and we store some data about the proofs (i.e., comments, proof tiles, [!DNL Workfront Proof] Viewer settings) on your computer using [!DNL Flash Player]. If the [!DNL Workfront Proof] Viewer opens, but there is no content inside you will want to make sure that the Flash Storage is available on your machine and that [!DNL Workfront Proof] is allowed to use it.

If there is some storage allocated, but you're working with the bigger proofs with multiple pages and comments try to increase the [!DNL Flash] Storage and re-load your proof.

-->

## 문제의 위치 식별

* 증명이 다른 브라우저에서 열리나요?
* 매일 한 개의 브라우저를 사용하고 있는데 여기서 증명을 보는 데 문제가 있는 경우 컴퓨터의 다른 브라우저에서 동일한 증명을 열어 보십시오. 이렇게 하려면 기본 브라우저의 URL 표시줄에서 증명 링크를 복사하여 다른 브라우저에 붙여넣기만 하면 됩니다. 증명이 거기서 열리면 기본 브라우저 구성, 플러그인 및 확장을 검토하십시오. 방해가 될 수 있습니다.
* 기본 브라우저는 없지만 현재 브라우저에 성능 문제가 있는 경우 다른 브라우저로 전환하는 것이 좋습니다.
* 현재 위치의 다른 컴퓨터에서 증명이 열리고 있습니까?
증명이 컴퓨터의 브라우저에서 열리지 않는 경우 위치 및/또는 위치 외부의 다른 컴퓨터에서 열려고 합니다. 이렇게 하면 특정 컴퓨터에 문제가 있는지 또는 로컬 네트워크에 문제가 있는지 확인할 수 있습니다.
보안 수준이 높으면 [!DNL Workfront Proof] 연결이 다음에 의해 차단될 수 있습니다.

   * 로컬 AV 소프트웨어
   * 네트워크 보안 솔루션
   * DNS, 방화벽 또는 프록시 구성
   * 이것은 우리가 통제할 수 없는 설정입니다. 사용할 수 있는 다양한 보안 솔루션이 있으며, 네트워크에 구현된 보안 솔루션과 [!DNL Workfront Proof]에 대한 연결을 차단할 수 있는 보안 솔루션을 알 수 없습니다. 또한 내부 보안 구성을 결정하는 것은 [!DNL Workfront Proof]까지 할 수 없습니다. 위치/네트워크의 여러 컴퓨터에서 증명을 여는 데 문제가 있는 경우 IT 팀에 연락하여 네트워크 설정을 확인하고 필요한 경우 [!DNL Workfront Proof]을(를) 승인하거나 허용 목록에 추가하다에 추가하는 것이 좋습니다.

* 네트워크에서 [!DNL Workfront Proof] 연결이 허용됩니까?
증명 뷰어 내부에 페이지 조각인 타일이 로드됩니다. 이 콘텐츠가 사용자 측에서 제대로 로드되지 않으면 [!DNL Workfront Proof]에 대한 일부 연결이 네트워크에서 차단되었을 수 있습니다. 모든 연결 및 *.proofhq.com의 모든 콘텐츠가 허용 목록에 추가하다에 추가되었는지 확인해야 합니다. IT 팀이 이 확인을 지원할 수 있어야 합니다.

## 플러그인 검토

브라우저가 최신 상태이고 네트워크에서 [!DNL Workfront Proof]에 대한 연결을 차단하지 않는 경우 브라우저에 증명 보기에 영향을 주는 문제가 있을 수 있습니다. 브라우저에서 사용할 수 있는 플러그인과 확장이 여러 개인 경우가 있으며, 일부는 다른 플러그인과 간섭하거나 충돌할 수 있습니다.

가장 좋은 방법은 알 수 없는 추가 기능을 모두 제거하고 사용자가 사용하고 신뢰할 수 있는 추가 기능만 유지하는 것입니다. 각 브라우저는 플러그인 및 확장을 확인/수정/삭제할 수 있는 옵션을 제공해야 합니다. JavaScript을 사용하여 [!DNL Workfront Proof] 뷰어를 로드하므로 이에 영향을 줄 수 있는 플러그인을 특히 검토할 수 있습니다.

증명을 로드하는 데 방해가 되는 특정 추가 기능이 있는 경우 브라우저의 콘솔에서 세부 사항을 확인할 수 있습니다.

![브라우저 콘솔](assets/proofview-4.png)

대부분의 최신 브라우저에는 몇 가지 추가 개발자 도구가 있으며, 이를 사용하여 보다 고급 문제 해결을 수행할 수 있습니다.

증명을 보는 데 문제가 있는 경우:

* 브라우저의 콘솔을 열고 증명을 다시 로드합니다.
* 콘솔에 경고 또는 메시지가 있는지 확인합니다. 이러한 세부 정보는 문제의 근본 원인이 무엇인지 식별하는 데 도움이 될 수 있습니다.
* IT 팀이 결과를 분석하도록 합니다. 그들은 지역 문제를 해결하는 데 조언하고 도움을 줄 수 있어야 한다.
* 지원 팀과 결과를 공유합니다. 기꺼이 도와드리겠습니다.

## 혼합 콘텐츠 설정 확인

[!DNL Workfront Proof]에 대한 모든 연결이 HTTPS를 통해 이루어집니다. 그러나 [!DNL Workfront Proof] 뷰어에서는 HTTP를 통해 타일을 로드하며 데이터는 토큰으로 보호됩니다. 이렇게 하면 일부 브라우저 또는 보안 솔루션이 차단했을 수 있는 혼합 콘텐츠(기본적으로 또는 수동 구성)가 생성됩니다.

증명이 컴퓨터에서 열리지 않는 경우(브라우저의 콘솔에서 관련 경고를 볼 수 있어야 함) [!DNL Workfront Proof]에 대해 이러한 연결을 승인하거나 설정을 수정하여 컴퓨터에 수동 혼합 콘텐츠를 허용하십시오. 혼합된 콘텐츠는 정확한 원인을 파악하기 위해 브라우저, AV 소프트웨어 또는 네트워크 구성에 의해 차단될 수 있습니다. IT 팀/네트워크 관리자에게 연락해야 합니다. 컴퓨터에서 혼합 콘텐츠를 활성화하는 데에도 도움이 될 수 있습니다.


