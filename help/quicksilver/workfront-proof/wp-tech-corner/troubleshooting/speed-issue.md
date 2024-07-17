---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: ' [!DNL Workfront Proof]의 속도 문제'
description: 이 도움말 페이지에서는  [!DNL Workfront Proof] 을(를) 사용할 때 발생할 수 있는 속도 문제가 ISP 또는  [!DNL Workfront Proof]의 콘텐츠 전달 네트워크와 관련이 있는지 확인하는 데 도움이 됩니다.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# [!DNL Workfront Proof]의 속도 문제

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

이 도움말 페이지에서는 [!DNL Workfront Proof]을(를) 사용할 때 발생할 수 있는 속도 문제가 ISP 또는 [!DNL Workfront Proof]의 콘텐츠 전달 네트워크와 관련이 있는지 확인하는 데 도움이 됩니다.

속도 문제는 일반적으로 로컬 ISP 연결 또는 로컬 인터넷 액세스 설정(예: 프록시 서버가 사용되는 경우)으로 인해 발생하며 [!DNL Workfront Proof]의 제어 범위를 벗어납니다.

즉, 연결 속도를 확인하는 몇 가지 단계를 수행할 수 있으므로 발생하는 문제의 근본 원인을 확인할 수 있습니다. 이러한 모든 단계는 문제 해결 프로세스에서도 동일하게 중요하며, 문제를 가장 정확하게 진단할 수 있도록 나열된 모든 단계에 대한 정보를 수집하는 시간을 가질 것을 권장합니다.

모든 세부 정보를 수집한 후에는 지역 문제를 파악하기 위해 지역 IT 부서에 문의하는 것이 좋습니다.

## 시스템의 어느 부분이 느리는지 확인합니다.

[!DNL Workfront Proof]을(를) 사용하는 경우, 폴더 컨텐츠 및 사용자 관리와 같은 대시보드 작업이나 [!DNL Workfront Proof] 뷰어를 사용하여 증명 검토 수행, 이미 작성된 댓글 확인 등의 작업을 수행할 수 있습니다.

시스템의 어느 부분이 느리는지 확인하는 것은 속도 문제 해결의 첫 번째 단계입니다. [!DNL Workfront Proof]이(가) 느려졌다고 보고할 때 다음을 설명하십시오.

* 다른 웹페이지에서 속도가 느려지고 있습니까?
* 대시보드 또는 [!DNL Workfront Proof] 뷰어에서 문제가 발생합니까?
* 시스템의 어떤 부분이 느립니까? (예: [!DNL Workfront Proof] 뷰어에서 새 증명 처리 또는 댓글 열기)

## traceroute 및 ping 테스트 실행

성능 문제가 발생하면 traceroute 명령을 실행하여 연결을 확인하는 것이 중요합니다. 이렇게 하려면 시스템(Mac/Linux의 터미널)에서 명령 프롬프트를 열고 다음 단계를 수행하십시오.

1. 다음 중 하나를 입력한 다음 추적기가 완료될 때까지 기다립니다.

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Windows만 해당) **app.proofhq.com**&#x200B;을(를) 입력합니다.
1. ping이 완료되면 명령 프롬프트에서 마우스 오른쪽 버튼을 클릭하고 모두 선택 을 클릭합니다.
1. 결과를 복사하여 이메일에 대한 회신에 붙여넣습니다.
결과를 지원 팀에 보내기 전에 traceroute 및 ping이 완료되도록 허용해야 합니다.

## Speedtest.net 을 사용하여 연결 속도 테스트

1. 브라우저를 열고 Speedtest.net으로 이동합니다.
1. Speedtest 기술 자료의 지침에 따라 인터넷 연결 속도를 테스트합니다.
1. 결과를 복사하여 지원 팀에 이메일로 붙여넣습니다.

## 브라우저 콘솔에서 네트워크 탭 확인

최신 브라우저에서 사용할 수 있는 웹 콘솔은 모든 네트워크 지연에 대한 유용한 정보를 수집하며, 이는 발생한 속도 문제의 근본 원인을 파악하는 데 도움이 됩니다.

웹 페이지의 로딩 시간을 확인하려면:

1. 브라우저의 콘솔과 네트워크 탭을 엽니다.
1. 페이지를 다시 로드합니다.
1. 스크린샷을 찍거나 결과를 스크린캐스트로 녹화하십시오.
1. 결과를 지원 팀과 공유합니다.

스크린샷에 모든 데이터가 표시되는지 확인하십시오. 스크린샷을 찍을 때 콘솔 창을 확장하거나 스크린캐스트에서 아래로 스크롤할 수 있습니다.

브라우저 설명서에서 자세한 지침을 확인할 수도 있습니다.

## 다른 네트워크 및 컴퓨터에서 연결 확인

다른 장치나 네트워크를 사용하여 연결 속도와 동일한 문제가 발생하는지 확인하는 것은 문제 해결 프로세스의 중요한 단계입니다. 다른 컴퓨터 또는 모바일 장치로 전환하고 대체 네트워크(예: 모바일 데이터)를 사용해 보십시오.

연결을 동일한 네트워크에서 다른 컴퓨터 사용, 다른 네트워크에서 동일한 컴퓨터 사용 및 대체 컴퓨터와 네트워크를 모두 사용하는 등 다양한 조합으로 비교한 후 결과를 지원 팀과 공유합니다.
