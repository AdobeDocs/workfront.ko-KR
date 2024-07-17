---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: ' [!DNL Workfront Proof]을(를) 사용하여 정적 웹 사이트 증명 만들기'
description: 웹 페이지에서 정적 증명을 만들 수 있습니다. 또한 캡처의 화면 해상도를 정의하여 다양한 디바이스를 시뮬레이션할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# [!DNL Workfront Proof]을(를) 사용하여 정적 웹 사이트 증명 만들기

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

웹 페이지에서 정적 증명을 만들 수 있습니다. 또한 캡처의 화면 해상도를 정의하여 다양한 디바이스를 시뮬레이션할 수 있습니다.

## 정적 웹 사이트 증명 만들기

1. [증명 생성 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)에 설명된 대로 [!UICONTROL 새 증명] 페이지를 엽니다.
1. **www.shareyourlink.com** 상자에 URL을 붙여 넣거나 입력하십시오.
1. 이 단계를 반복하여 여러 URL을 추가할 수 있습니다.
1. 이 상자 바로 아래에 있는 해상도(기본값은 1366x768)를 클릭한 다음 **[!UICONTROL 화면 해상도]** 상자에서 원하는 해상도를 선택합니다.
모바일 장치용 디자인을 증명하려면 더 작은 해상도를 선택하십시오. 일반적으로 디자인은 화면/브라우저 창 해상도에 따라 로드됩니다.

1. 입력한 URL과 동일한 도메인/하위 도메인에 있는 연결된 페이지를 포함하려면 **[!UICONTROL 하위 페이지 찾기]**를 클릭합니다.
   [!DNL Workfront Proof]이(가) 연결된 페이지를 검사하여 **[!UICONTROL 하위 페이지 찾기]** 옵션 아래에 표시합니다. 포함할 페이지를 선택할 수 있습니다.

1. [!UICONTROL 증명 결합] 기능을 사용하면 모든 웹 페이지를 하나의 다중 페이지 증명으로 제출할 수 있습니다.
1. **[!UICONTROL 완료]**&#x200B;를 클릭한 다음 [증명 생성 위치 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)에 설명된 대로 증명 구성을 완료합니다.

## 암호로 보호된 페이지 및 권한 부여가 필요한 페이지 정보

[!DNL Workfront Proof]은(는) 암호로 보호된 웹 사이트를 정적 증명으로 캡처할 수 없습니다.

승인이 필요한 페이지에서 증명을 만들려면 IT 팀은 웹 캡처 도구가 연결되는 회사의 허용 목록에 다음 URL 중 하나를 추가해야 합니다.

**미국의 AWS 클러스터**: webcapture.proofhq.com

**미국에 있는 GCP 클러스터**: webcapture.gcp.proofhq.com

**EMEA 클러스터**: webcapture.proofhq.eu

>[!NOTE]
>
>승인이 필요한 내부 페이지 및 암호로 보호된 웹 사이트에는 정적 증명 대신 대화형 증명을 사용하는 것이 좋습니다. 자세한 내용은 [대화형 콘텐츠 증명 개요](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)를 참조하십시오.

## 정적 웹 사이트 증명 처리 기본 정보

* 애니메이션, 포함된 비디오, 스크립트 및 상호 작용은 정적 웹 사이트 증명에 포함할 수 없습니다. 대화형 내용을 증명하려면 [증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)에서 [증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)을 참조하세요.

* 증명 페이지는 일반적으로 페이지당 약 20초의 속도로 캡처되도록 준비됩니다. 그러나 전체 준비 시간은 페이지가 호스팅된 서버에도 따라 다릅니다. 이 도구는 제출된 각 URL이 로드될 때까지 60초 동안 기다립니다. 이 대기 시간을 초과하면 증명이 실패합니다.
* 결합된 증명의 경우 URL 중 캡처 도구에 응답하지 않는 URL이 있으면 증명이 실패합니다.
* [!DNL Workfront Proof]은(는) 래스터화 후 최대 195인치 길이의 웹 페이지를 캡처합니다. 웹 페이지가 이보다 길면 증명이 실패합니다.
* 텍스트 추출은 모든 텍스트 요소에서 사용할 수 있지만 이미지로 배치된 텍스트는 추출되지 않습니다.
* 교정에서 텍스트 하이퍼링크를 클릭할 수 있고 링크된 페이지가 새 브라우저 탭에서 열립니다.
* `<a>` 태그 내에 style=&quot;display:block&quot; 요소를 사용하면 이미지의 하이퍼링크를 클릭할 수 없습니다. 페이지 디자인에서 이러한 부분을 조정하는 것이 좋습니다.
* 최상의 결과를 얻으려면 우수 코딩 사례 및 승인된 표준을 사용하여 페이지를 만드는 것이 좋습니다.
