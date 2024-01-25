---
product-area: documents
navigation-topic: proofing-overview
title: 대화형 콘텐츠 증명 개요
description: 대화형 콘텐츠는 시청자를 유도하는 다양한 방법을 제공합니다. 에이전시는 이 콘텐츠에 대한 응답으로 수집한 분석을 사용하여 캠페인의 성공을 측정할 수 있습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# 대화형 콘텐츠 증명 개요

<!-- Audited: 01/2024 -->

대화형 콘텐츠는 시청자를 유도하는 다양한 방법을 제공합니다. 에이전시는 이 콘텐츠에 대한 응답으로 수집한 분석을 사용하여 캠페인의 성공을 측정할 수 있습니다.

대화형 콘텐츠의 예는 다음과 같습니다.

* 웹 사이트
* 임베디드 또는 스트리밍 비디오
* 대화형 배너
* HTML 애니메이션
* 마이크로사이트
* 대화형 이메일

## 대화형 콘텐츠에 대한 증명 만들기 기본 정보

다음 방법 중 하나로 대화형 콘텐츠에 대한 증명을 만들 수 있습니다.

* 대화형 컨텐츠가 포함된 ZIP 파일에서 증명을 만듭니다.

  Adobe Workfront은 ZIP 파일에서 콘텐츠를 압축 해제하여 Workfront 서버에 저장합니다. 이렇게 저장되므로 증명 검토 주기 동안 동일하게 유지되는 콘텐츠를 사용할 수 있습니다.

* 콘텐츠의 URL을 지정합니다.

  대화형 콘텐츠에 대한 증명을 만드는 가장 간단한 방법입니다. 또한 사용자가 인터넷에서 콘텐츠를 경험하므로 이를 대화식으로 검토할 수 있는 유일한 방법입니다.

  이 방법을 사용하면 Workfront에서 알 수 없는 외부 서버가 콘텐츠를 저장하고 호스팅합니다.

  대형 웹 사이트를 구성하는 모든 파일을 수집하기 어렵기 때문에 대형 웹 사이트에는 이 방법을 사용하는 것이 좋습니다. 그러나 증명 콘텐츠는 외부에 저장되므로 Workfront에서 해당 콘텐츠를 처리하는 개발자의 변경 내용으로부터 보호할 수 없으므로 증명 검토 주기 전반에 걸쳐 동일하게 유지되는 콘텐츠에 의존하지 못할 수 있습니다.

## 증명을 위해 ZIP 파일에서 대화형 콘텐츠 준비 정보

증명을 위해 ZIP 파일에 대화형 콘텐츠를 번들로 제공할 때 다음 사양이 포함되어 있는지 확인하십시오.

* CSS, JavaScript, 비디오, 사운드 및 이미지와 같은 모든 자산이 번들 파일에 포함되어야 합니다.
* 대화형 컨텐츠에는 기본 파일(index.html, index.htm)이 포함되어야 합니다. 이 파일이 루트 위치에 없으면 도구에서 자동으로 폴더를 검색하여 찾습니다. 기본 파일의 이름을 index.html/index.htm으로 지정할 필요는 없지만 기본 위치에 .html/.htm 파일이 하나만 있을 수 있습니다.
* 파일에는 최소 하나 이상의 정적 파일 웹 페이지가 있어야 합니다.
* 최대 번들 크기는 500MB입니다.
* iOS에서 만든 .zip 파일의 경우 이 도구는 콘텐츠가 있는 폴더를 자동으로 식별합니다.
* 대화형 프로젝트는 .zip 아카이브로만 지원됩니다. 표준 .zip 파일 제출이 실패합니다.
* 웹 사이트의 보안 유지(HTTPS)

  Desktop Proofing Viewer를 사용하는 경우에는 필수가 아닙니다.

  자세한 내용은 [Desktop Proofing 뷰어 이해](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* 웹 사이트는 iframe에서 볼 수 있어야 합니다.

  Desktop Proofing Viewer를 사용하는 경우에는 필수가 아닙니다.

  자세한 내용은 [Desktop Proofing 뷰어 이해](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## 대화형 증명 만들기 기본 정보

ZIP 번들 파일을 준비한 후 대화형 증명을 만듭니다.

자세한 내용은 [ZIP 파일에 대화형 컨텐츠에 대한 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

또는 Workfront 증명을 사용하는 경우 섹션 을 참조하십시오 [대화형 콘텐츠에 대한 증명 생성](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) 이 문서에서 [Workfront Proof에서 증명 생성](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 대화형 증명 검토 정보

독립형 데스크탑 증명 뷰어를 대화형 증명의 기본 뷰어로 사용하는 것이 좋습니다. 그러나 조직의 정책에서 Desktop Proofing Viewer 앱 사용을 허용하지 않는 경우 Workfront 관리자는 사용자가 ZIP 아카이브 파일에 번들로 제공된 대화형 컨텐츠를 웹 증명 뷰어에서 검토할 수 있도록 시스템을 구성할 수 있습니다. Desktop Proofing Viewer와 웹 증명 뷰어에 대한 비교 정보는 [웹 증명 뷰어와 데스크탑 증명 뷰어의 차이점 개요](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
