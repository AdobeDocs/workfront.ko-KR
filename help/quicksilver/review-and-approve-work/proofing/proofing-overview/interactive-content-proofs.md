---
product-area: documents
navigation-topic: proofing-overview
title: 대화형 콘텐츠 증명 개요
description: 대화형 콘텐츠는 뷰어를 사로잡는 여러 방법을 제공합니다. 에이전시는 이 컨텐츠에 대한 응답에서 수집된 분석을 사용하여 캠페인의 성공을 측정할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 대화형 콘텐츠 증명 개요

대화형 콘텐츠는 뷰어를 사로잡는 여러 방법을 제공합니다. 에이전시는 이 컨텐츠에 대한 응답에서 수집된 분석을 사용하여 캠페인의 성공을 측정할 수 있습니다.

대화형 컨텐츠의 예는 다음과 같습니다.

* 웹 사이트
* 포함된 비디오 또는 스트리밍 비디오
* 대화형 배너
* HTML5 애니메이션
* 마이크로사이트
* 대화형 이메일

이 문서에서는 대화형 콘텐츠 교정에 대해 다음과 같이 설명합니다.

## 대화형 컨텐츠에 대한 증명 만들기 정보

다음 방법 중 하나로 대화형 컨텐츠에 대한 증명을 만들 수 있습니다.

* 대화형 컨텐츠가 들어 있는 ZIP 파일에서 증명을 만듭니다.

   Adobe Workfront은 ZIP 파일에서 컨텐츠를 압축 해제한 후 Workfront 서버에 저장합니다. 이러한 방식으로 저장되므로 증명 검토 주기 내내 동일한 콘텐츠를 유지할 수 있습니다.

* 컨텐츠의 URL을 지정합니다.

   이는 대화형 컨텐츠에 대한 증명을 만드는 가장 간단한 방법입니다. 사용자가 인터넷에서 경험하는 것처럼 이 방법만이 콘텐츠를 대화식으로 검토할 수 있습니다.

   이 방법을 사용하면 Workfront에 알 수 없는 외부 서버가 컨텐츠를 저장하고 호스팅합니다.

   대형 웹 사이트를 구성하는 모든 파일을 수집하기 어려우므로 대형 웹 사이트에 대해 이 방법을 사용하는 것이 좋습니다. 그러나 증명 컨텐츠는 외부에 저장되므로 Workfront은 증명 컨텐츠를 작업하는 개발자의 변경 사항에서 이를 보호할 수 없으므로 증명 검토 주기 내내 동일하게 유지되는 컨텐츠를 사용하지 못할 수 있습니다.

## ZIP 파일에서 언어 교정을 위한 대화형 컨텐츠 준비 정보

교정을 위해 대화형 컨텐츠를 ZIP 파일로 번들로 구성하는 경우 다음 사양을 포함해야 합니다.

* CSS, JavaScript, 비디오, 사운드 및 이미지와 같은 모든 자산은 번들 파일에 포함되어야 합니다.
* 대화형 컨텐츠에는 기본 파일(index.html, index.htm)이 포함되어야 합니다. 이 파일이 루트 위치에 배치되지 않으면 이 도구는 폴더를 자동으로 검색하여 찾습니다. 기본 파일의 이름은 index.html/index.htm이 아니지만 기본 위치에 .html/.htm 파일이 하나만 있을 수 있습니다.
* 파일에 정적 파일 웹 페이지가 하나 이상 있어야 합니다.
* 최대 번들 크기는 500MB입니다.
* iOS에서 만든 .zip 파일의 경우, 도구는 컨텐츠가 있는 폴더를 자동으로 식별합니다
* 대화형 프로젝트는 .zip 아카이브로만 지원됩니다. 표준 .zip 파일 제출이 실패합니다.
* 웹 사이트의 보안(HTTPS)이 있어야 합니다.

   데스크톱 언어 교정 뷰어를 사용할 때는 이 작업이 필요하지 않습니다.

   자세한 내용은 [데스크탑 교정 뷰어 이해](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* 웹 사이트를 iframe에서 볼 수 있어야 합니다.

   데스크톱 언어 교정 뷰어를 사용할 때는 이 작업이 필요하지 않습니다.

   자세한 내용은 [데스크탑 교정 뷰어 이해](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## 대화형 증명 만들기 정보

ZIP 번들 파일을 준비한 후 대화형 증명을 만듭니다.

자세한 내용은 [ZIP 파일에서 대화형 컨텐츠에 대한 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

또는 Workfront 증명을 사용하는 경우 섹션을 참조하십시오 [대화형 컨텐츠에 대한 증명 생성](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generati) 기사 [Workfront 증명에서 증명 생성](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 대화형 증명 검토 정보

대화형 증명을 위한 기본 뷰어로 독립형 데스크탑 언어 교정 뷰어를 사용하는 것이 좋습니다. 그러나 조직의 정책에 따라 데스크탑 언어 교정 뷰어 앱을 사용할 수 없는 경우 Workfront 관리자가 웹 언어 교정 뷰어에서 ZIP 아카이브 파일에 번들로 제공된 대화형 컨텐츠를 검토할 수 있도록 시스템을 구성할 수 있습니다. Desktop Proofing Viewer 및 Web Proofing Viewer에 대한 비교 정보는 다음을 참조하십시오 [Web Proofing Viewer와 Desktop Proofing Viewer 개요의 차이점](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
