---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 문제 해결 - [!DNL Workfront Proof] 증명 뷰어
description: 증명 콘텐츠가 로드되지 않고 빈 증명 뷰어만 표시되는 경우, 무언가가 이 작업을 로컬에서 차단하기 때문에 발생할 수 있습니다. 아래에서 가능한 해결 방법을 시도해 보십시오.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 0%

---

# 문제 해결 - [!DNL Workfront Proof] 증명 뷰어

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품의 기능에 대해 설명합니다 [!DNL Workfront Proof]. 내부 교정에 대한 정보 [!DNL Adobe Workfront], 참조 [증명](../../../review-and-approve-work/proofing/proofing.md).

증명 콘텐츠가 로드되지 않고 빈 증명 뷰어만 표시되는 경우, 무언가가 이 작업을 로컬에서 차단하기 때문에 발생할 수 있습니다. 아래에서 가능한 해결 방법을 시도해 보십시오.

## 브라우저 및 [!DNL Flash Player] 버전이 최신입니다.

모든 개발자는 애플리케이션을 지속적으로 작업하며 제품에 대한 새로운 기능과 수정 사항을 정기적으로 릴리스합니다. 사용자 경험을 개선하고 보안 수준을 유지하기 위한 것이므로 최신 버전만 사용하는 것이 좋습니다. 또한 애플리케이션 간의 충돌을 피하는 데 도움이 됩니다.

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### 브라우저 버전

요즘은 대부분의 브라우저가 자동으로 업데이트되지만 문제가 발생하는 경우 사용 중인 버전을 확인하고 필요한 경우 업데이트를 수행하는 것이 좋습니다.

브라우저에서 로 이동합니다. [!UICONTROL 메뉴] 및 를 찾습니다. [!UICONTROL 정보] option(경우에 따라 아래에 표시될 수 있음) [!UICONTROL 도움말] 메뉴)를 참조하십시오. 다음에서 [!UICONTROL 정보] 팝업에서 현재 브라우저 버전에 대한 정보와 업데이트를 업데이트/확인하는 옵션을 확인할 수 있습니다.

Chrome에서 다음을 참조하십시오.

![ProofView_3.png](assets/proofview-3-350x206.png)

최신 버전을 구하면 [!DNL Flash Player] 플러그인과 설치된 브라우저 버전이 증명을 다시 열어 문제가 해결되었는지 확인합니다.

## 로컬 항목 확인 [!DNL Flash] 저장소 사용 가능

당사 [!DNL Workfront Proof] Viewer는 Flash을 기반으로 하며 증명에 대한 일부 데이터(예: 댓글, 증명 타일)를 저장합니다. [!DNL Workfront Proof] (뷰어 설정)을 사용하여 컴퓨터의 [!DNL Flash Player]. 다음과 같은 경우 [!DNL Workfront Proof] 뷰어가 열리지만 내부에 컨텐츠가 없습니다. 컴퓨터에서 Flash 저장소를 사용할 수 있는지 확인하고 [!DNL Workfront Proof] 사용할 수 있습니다.

할당된 저장소가 있지만 여러 페이지와 댓글이 있는 더 큰 교정본을 사용하여 작업하는 경우 [!DNL Flash] 증명을 저장하고 다시 로드합니다.

다음을 참조하십시오. [증명 보기 문제 - [!DNL Flash] 공유 오브젝트 설명](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) 자세한 지침을 참조하십시오.

## 문제의 위치 식별

* 증명이 다른 브라우저에서 열리나요?
* 매일 한 개의 브라우저를 사용하고 증명을 보는 데 문제가 있는 경우 컴퓨터의 다른 브라우저에서 동일한 증명을 열어 보십시오. 이렇게 하려면 기본 브라우저의 URL 표시줄에서 증명 링크를 복사하여 다른 브라우저에 붙여넣기만 하면 됩니다. 거기에서 증명이 열리면 기본 브라우저 구성, 플러그인 및 확장이 방해가 될 수 있으니 검토하십시오.
* 선호하는 브라우저는 없지만 현재 브라우저에 성능 문제가 있는 경우 다른 브라우저로 전환하는 것이 좋습니다.
* 현재 위치의 다른 컴퓨터에서 증명이 열리고 있습니까?
증명이 컴퓨터의 브라우저에서 열리지 않는 경우 위치 및/또는 위치 외부의 다른 컴퓨터에서 열려고 합니다. 이렇게 하면 특정 컴퓨터에 문제가 있는지 또는 로컬 네트워크에 문제가 있는지 확인할 수 있습니다.
보안 수준이 보다 높은 경우 [!DNL Workfront Proof] 다음에 의해 차단될 수 있음:

   * 로컬 AV 소프트웨어
   * 네트워크 보안 솔루션
   * DNS, 방화벽 또는 프록시 구성
   * 이것은 우리가 통제할 수 없는 설정입니다. 사용할 수 있는 다양한 보안 솔루션이 있으며 네트워크에 구현된 보안 솔루션과 연결이 차단될 수 있는 보안 솔루션을 파악할 수 없습니다 [!DNL Workfront Proof]. 또한 다음을 충족하지 않습니다. [!DNL Workfront Proof] 내부 보안 구성을 결정합니다. 위치/네트워크의 여러 컴퓨터에서 증명을 여는 데 문제가 있는 경우 IT 팀에 연락하여 네트워크 설정을 확인하고 다음을 승인하거나 추가하는 것이 좋습니다. [!DNL Workfront Proof] 필요한 경우 허용 목록에 추가하다으로

* 다음에 대한 연결입니다. [!DNL Workfront Proof] 네트워크에서 허용됩니까?
증명 뷰어 내부에 페이지 조각인 타일이 로드됩니다. 이 콘텐츠가 끝에서 제대로 로드되지 않는 경우 일부 연결이 [!DNL Workfront Proof] 네트워크에서 차단되었습니다. 모든 연결 및 *.proofhq.com의 모든 콘텐츠가 허용 목록에 추가하다에 추가되었는지 확인해야 합니다. IT 팀이 이 확인을 지원할 수 있어야 합니다.

## 리뷰 플러그인

브라우저 및 [!DNL Flash Player] 플러그인이 최신 상태이며 네트워크가 (으)로의 연결을 차단하지 않습니다. [!DNL Workfront Proof] 브라우저에 증명 보기에 영향을 주는 것이 있을 수 있습니다. 현재 브라우저에서 사용할 수 있는 여러 플러그인과 확장이 있으며, 일부 플러그인은 다른 플러그인과 간섭하거나 충돌합니다.

가장 좋은 방법은 알 수 없는 추가 기능을 모두 제거하고 사용자가 사용하고 신뢰할 수 있는 추가 기능만 유지하는 것입니다. 각 브라우저는 플러그인 및 확장을 확인/수정/삭제할 수 있는 옵션을 제공해야 합니다. 당사 [!DNL Workfront Proof] 뷰어는 다음을 기반으로 함 [!DNL Flash] 또한 JavaScript를 사용하여 뷰어를 로드하므로 여기에 영향을 줄 수 있는 플러그인을 특히 검토해 보겠습니다.

증명을 로드하는 데 방해가 되는 특정 추가 기능이 있는 경우 브라우저의 콘솔에서 세부 사항을 확인할 수 있습니다.

![ProofView_4.png](assets/proofview-4-350x57.png)

대부분의 최신 브라우저에는 사용 가능한 몇 가지 추가 개발자 도구가 있으며 고급 문제 해결에 사용할 수 있습니다.

증명을 보는 데 문제가 있는 경우:

* 브라우저의 콘솔을 열고 증명을 다시 로드합니다.
* 콘솔에 경고 또는 메시지가 있는지 확인합니다. 이러한 세부 정보는 문제의 근본 원인이 무엇인지 식별하는 데 도움이 될 수 있습니다.
* IT 팀이 결과를 분석하도록 합니다. 그들은 지역 문제를 해결하는 데 조언하고 도움을 줄 수 있어야 한다.
* 지원 팀과 결과를 공유합니다. 기꺼이 도와드리겠습니다.


## 혼합 콘텐츠 설정 확인

에 대한 모든 연결 [!DNL Workfront Proof] 은 HTTPS를 통해 전달됩니다. 그러나 [!DNL Workfront Proof] 뷰어는 HTTP를 통해 타일을 로드하며 데이터는 토큰으로 보호됩니다. 이렇게 하면 일부 브라우저 또는 보안 솔루션이 차단할 수 있는 혼합 콘텐츠가 만들어집니다(기본적으로 또는 수동 구성에 따라).

이 때문에 컴퓨터에서 증명이 열리지 않는 경우(브라우저의 콘솔에서 관련 경고를 볼 수 있어야 함) 다음 항목에 대한 해당 연결을 승인합니다. [!DNL Workfront Proof] 또는 컴퓨터에 수동 혼합 콘텐츠를 허용하도록 설정을 수정합니다. 혼합된 콘텐츠는 브라우저, AV 소프트웨어, 네트워크 구성 등에 의해 차단될 수 있습니다. 정확한 원인을 확인하려면 IT 팀/네트워크 관리자에게 문의하십시오. 컴퓨터에서 혼합 콘텐츠를 활성화하는 데에도 도움이 될 수 있습니다.


