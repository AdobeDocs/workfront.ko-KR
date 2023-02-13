---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: 을 사용하여 정적 웹 사이트 증명 만들기 [!DNL Workfront Proof]
description: 웹 페이지에서 정적 증명을 만들 수 있습니다. 또한 캡처의 화면 해상도를 정의하여 다양한 장치를 시뮬레이션할 수 있습니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 을 사용하여 정적 웹 사이트 증명 만들기 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

웹 페이지에서 정적 증명을 만들 수 있습니다. 또한 캡처의 화면 해상도를 정의하여 다양한 장치를 시뮬레이션할 수 있습니다.

## 정적 웹 사이트 증명 만들기

1. 를 엽니다. [!UICONTROL 새로운 증명] 에 설명된 대로 페이지를 페이지 페이지 페이지 페이지 페이지 페이지 페이지 페이지에 삽입됩니다. [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. 에 URL을 붙여넣거나 입력합니다 **www.shareyourlink.com** 상자.
1. 이 단계를 반복하여 여러 URL을 추가할 수 있습니다.
1. 이 상자 바로 아래에서 해상도(기본값 1366x768)를 클릭한 다음, **[!UICONTROL 화면 해상도]** 상자.
모바일 장치용 디자인을 증명한 다음 더 작은 해상도를 선택하십시오. 일반적으로 디자인은 화면/브라우저 창 해상도에 따라 로드됩니다.

1. 클릭 **[!UICONTROL 하위 페이지 찾기]** 입력한 URL과 동일한 도메인/하위 도메인에 있는 연결된 페이지를 포함하려는 경우,
   [!DNL Workfront Proof] 연결된 페이지를 검색하고 아래에 나열합니다. **[!UICONTROL 하위 페이지 찾기]** 선택 사항입니다. 포함할 페이지를 선택할 수 있습니다.

1. 사용 [!UICONTROL 증명 결합] 모든 웹 페이지를 하나의 다중 페이지 증명으로 제출할 수 있는 기능입니다.
1. 클릭 **[!UICONTROL 완료]**&#x200B;를 입력한 다음 다음에 설명된 대로 증명 구성을 완료합니다. [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 승인이 필요한 암호로 보호된 페이지 및 페이지 정보

[!DNL Workfront Proof] 암호로 보호된 웹 사이트를 정적 증명으로 캡처할 수 없습니다.

승인이 필요한 페이지에서 증명을 작성하려면 IT 팀이 웹 캡처 도구가 연결되는 회사허용 목록에 추가하다의 페이지에 다음 URL 중 하나를 추가해야 합니다.

**미국의 AWS 클러스터**: webcapture.proofhq.com

**미국의 GCP 클러스터**: webcapture.gcp.profhq.com

**EMEA 클러스터**: webcapture.proohq.eu

>[!NOTE]
>
>인증 및 암호로 보호된 웹 사이트를 요구하는 내부 페이지에 대해 정적 교정이 아닌 대화형 교정이 좋습니다. 자세한 내용은 [대화형 콘텐츠 증명 개요](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## 정적 웹 사이트 증명 처리 정보

* 애니메이션, 포함된 비디오, 스크립트 및 상호 작용은 정적 웹 사이트 증명에 포함할 수 없습니다. 대화형 컨텐츠를 증명하려면 다음을 참조하십시오 [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) in [에서 증명 생성 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* 증명 페이지는 일반적으로 페이지당 약 20초 비율로 캡처됩니다. 그러나 전체 준비 시간은 페이지가 호스팅된 서버에도 따라 다릅니다. 이 도구는 제출된 각 URL이 로드될 때까지 60초를 기다립니다. 대기 시간이 초과되면 증명에 실패합니다.
* 결합된 증명의 경우, URL이 캡처 도구에 응답하지 않는 경우 증명이 실패합니다.
* [!DNL Workfront Proof] 래스터화 후 최대 195인치 길이의 웹 페이지를 캡처합니다. 웹 페이지가 이보다 긴 경우 증명은 실패합니다.
* 모든 텍스트 요소에서 텍스트 추출을 사용할 수 있지만 이미지로 배치된 텍스트는 추출되지 않습니다.
* 증명에서 텍스트 하이퍼링크를 클릭하면 새 브라우저 탭에서 연결된 페이지가 열립니다.
* style=&quot;display:block&quot; 요소를 내에서 사용하는 경우 이미지의 하이퍼링크를 클릭할 수 없습니다 `<a>` 태그 사이에 Analytics JavaScript 코드를 배치했습니다. 페이지 디자인에서 이러한 부분을 조정하는 것이 좋습니다.
* 최상의 결과를 얻으려면 우수 코딩 사례 및 승인된 표준을 사용하여 페이지를 만드는 것이 좋습니다.
