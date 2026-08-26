---
product-area: documents
navigation-topic: documents-navigation-topic
title: Adobe Workfront의 C2PA 메타데이터
description: C2PA 메타데이터의 의미와 사용자가 업로드, 저장 및 다운로드하는 문서에서 Adobe Workfront이 메타데이터를 보존하는 방법에 대해 알아봅니다.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 3510218fb179a0852ad22abe2a753ccdb261205a
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 0%

---

# Adobe Workfront의 C2PA 메타데이터

C2PA 메타데이터는 콘텐츠와 함께 이동하는 안전하고 변조가 불가능한 정보입니다. 생성 AI(GenAI)를 사용하여 이미지, 비디오 또는 오디오 파일을 만들거나 변경하면 C2PA 메타데이터는 해당 사실을 기록하여 파일을 받은 누구나 작성 방법을 볼 수 있도록 합니다.

C2PA 메타데이터는 개방형 [C2PA](https://c2pa.org/) 표준을 기반으로 합니다.

## C2PA 메타데이터에 포함된 내용

C2PA 메타데이터에는 다음이 포함됩니다.

* GenAI 도구를 제공한 공급자의 이름입니다.
* 콘텐츠를 만들거나 변경하는 데 사용되는 GenAI 시스템의 이름 및 버전 번호입니다.
* 콘텐츠가 생성 또는 변경된 날짜 및 시간입니다.
* 고유 식별자.

C2PA 메타데이터에는 PII(개인 식별 정보)가 포함되어 있지 않습니다.

## Workfront에서 C2PA 메타데이터를 처리하는 방법

Adobe Workfront은 사용자가 작업하는 파일의 메타데이터를 수정하지 않습니다. 이미 C2PA 메타데이터를 전달하는 파일을 업로드할 때 Workfront에서는 해당 파일이 Workfront에 저장되고 다운로드되므로 이 정보를 그대로 유지합니다.

메타데이터는 파일 자체에 포함되어 있으므로 Workfront 워크플로를 통해 그대로 유지되므로 Workfront에서 나갈 때 증명 정보가 콘텐츠와 함께 유지됩니다.
