---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 속도 문제 [!DNL Workfront Proof]
description: 이 도움말 페이지에서는 사용 시 발생할 수 있는 속도 문제를 확인할 수 있습니다 [!DNL Workfront Proof] ISP와 관련되었거나 [!DNL Workfront Proof]의 컨텐츠 전달 네트워크.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# 속도 문제 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

이 도움말 페이지에서는 사용 시 발생할 수 있는 속도 문제를 확인할 수 있습니다 [!DNL Workfront Proof] ISP와 관련되었거나 [!DNL Workfront Proof]의 컨텐츠 전달 네트워크.

속도 문제는 일반적으로 로컬 ISP 연결이나 로컬 인터넷 액세스 설정(예: 프록시 서버가 사용되는 경우)으로 인해 발생하므로 의 제어 범위를 벗어납니다 [!DNL Workfront Proof].

즉, 몇 가지 단계를 수행하여 발생하는 문제의 근본 원인을 확인할 수 있습니다. 이러한 모든 단계는 문제 해결 프로세스에 똑같이 중요하며, 나열된 모든 단계에 대한 정보를 수집하여 문제를 가장 정확하게 진단하도록 하는 것이 좋습니다.

모든 세부 사항을 수집하면 지역 IT 부서에 문의하여 모든 로컬 문제를 확인하는 것이 좋습니다. 이 문제에 대해 더 도움이 필요하면 [지원 팀](https://support.workfront.com/hc/en-us/requests/new).

## 시스템의 어느 부분이 느리지를 확인합니다

사용 시 [!DNL Workfront Proof]를 사용하여 작업하는 경우, 예를 들어, 폴더 컨텐츠와 사용자를 관리하거나 [!DNL Workfront Proof] 뷰어: 증명 검토, 이미 작성한 의견 확인 등을 수행합니다.

속도가 느린 시스템의 정확한 부분을 결정하는 것은 속도 문제를 해결하는 첫 번째 단계입니다. 보고할 때 [!DNL Workfront Proof] 속도가 느려지면 다음을 반드시 설명하십시오.

* 다른 웹 페이지에서 속도가 느려집니까?
* 대시보드에서 문제가 발생합니까? [!DNL Workfront Proof] 시청자?
* 시스템의 정확한 부분이 느리나요? (예: 새 증명 처리 또는 주석 열기) [!DNL Workfront Proof] 뷰어)

## 추적 및 ping 테스트 실행

성능 문제가 발생하는 경우 traceroute 명령을 실행하여 연결을 확인하는 것이 중요합니다. 이렇게 하려면 시스템(Mac/Linux의 터미널)에서 명령 프롬프트를 열고 다음 단계를 수행하십시오.

1. 다음 중 하나를 입력한 다음 추적기가 완료될 때까지 기다립니다.

   * Windows: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Windows 전용) 유형 **ping app.profhq.com**.
1. Ping이 완료되면 명령 프롬프트에서 마우스 오른쪽 버튼을 클릭하고 Select All(모두 선택)을 클릭합니다.
1. 결과를 복사하여 이메일에 회신합니다.
지원 팀에 결과를 보내기 전에 추적 및 ping이 완료되도록 허용했는지 확인하십시오.

## Speedtest.net을 사용하여 연결 속도 테스트

1. 클릭 [여기](http://www.speedtest.net/) speedtest.net에 액세스하려면
1. Speedtest 기술 자료의 지침에 따라 인터넷 연결 속도를 테스트합니다.
1. 결과를 복사하여 지원 팀에 붙여넣습니다.

## 브라우저 콘솔에서 네트워크 탭 확인

최신 브라우저에서 사용할 수 있는 웹 콘솔은 모든 네트워크 대기 시간에 대한 유용한 정보를 수집하므로 발생하는 속도 문제의 근본 원인을 파악하는 데 도움이 됩니다.

웹 페이지의 로드 시간을 확인하려면:

1. 브라우저의 콘솔 및 네트워크 탭을 엽니다.
1. 페이지를 다시 로드합니다.
1. 스크린샷을 촬영하거나 결과의 스크린샷을 기록합니다.
1. 지원 팀과 결과를 공유합니다.

스크린샷에 모든 데이터가 표시되는지 확인하십시오. 스크린샷을 작성하거나 스크린샷에서 아래로 스크롤할 때 콘솔 창을 확장할 수 있습니다.

브라우저에서 콘솔을 여는 방법을 모를 경우, 다음과 같이 기록된 단계를 참조하십시오.

* [Chrome](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Edge](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer](http://screencast.com/t/x5Q3eHczbc)

또한 브라우저의 설명서에서 자세한 지침을 확인할 수 있습니다.

## 다른 네트워크 및 시스템에서 연결 확인

다른 장치나 네트워크를 사용하는 연결 속도에 대해 동일한 문제가 발생하는지 확인하는 것은 문제 해결 프로세스의 중요한 단계입니다. 다른 컴퓨터 또는 모바일 장치로 전환하고 대체 네트워크(예: 모바일 데이터)를 사용해 보십시오.

다양한 조합으로 연결을 비교합니다. 같은 네트워크에서 다른 컴퓨터를 사용하고 다른 네트워크에서 같은 시스템을 사용하고 대체 시스템과 네트워크를 모두 사용한 다음 지원 팀과 결과를 공유하십시오.
