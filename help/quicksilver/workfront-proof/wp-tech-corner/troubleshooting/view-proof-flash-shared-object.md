---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 증명 보기 문제 - Flash 공유 개체 설명
description: '''참고: 이 문서의 정보는 현재 더 이상 사용되지 않으며 다음에서 제거될 기능을 참조합니다 [!DNL Workfront] 2018년에. Web Proofing Viewer에서 증명 검토에 설명된 대로 새 Web Proofing Viewer(Web Proofing Viewer에서 설명)나 데스크탑 교정 뷰어(Desktop Proofing Viewer에서 설명)를 사용하는 것이 좋습니다.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f1f3561e-8660-4c1e-b48f-446eb0eaac06
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 증명 보기 문제 - [!DNL Flash] 공유 개체 설명

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>이 문서의 정보는 현재 더 이상 사용되지 않으며 다음에서 제거될 기능을 참조합니다 [!DNL Workfront] 2018년에. 다음에 설명된 대로 새 Web Proofing Viewer를 사용하는 것이 좋습니다 [Web Proofing Viewer에서 증명 검토](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)) 또는 Desktop Proofing Viewer( [데스크탑 교정 뷰어에서 증명 검토](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)).

## [!DNL Flash] 공유 개체

로컬 공유 개체로서, 경우에 따라 &quot;[!DNL Flash] 쿠키&quot;는 사용자가 방문하는 사이트에서 컴퓨터에 만들 수 있는 데이터 파일입니다. 공유 객체는 웹 탐색 환경을 향상시키는 데 가장 많이 사용됩니다. A [!DNL Flash] 쿠키는 [!DNL Adobe Flash] 웹 서버에서 웹 브라우저로 전송되고 브라우저에 데이터 파일로 저장됩니다.

다음 이후 [!DNL Workfront Proof] 뷰어는 [!DNL Flash]에 대해 허용되는 스토리지를 확인하는 것이 좋습니다 [!DNL Flash] 컴퓨터에 있는 응용 프로그램

## [!DNL Flash] 공유 개체 - 알려진 문제

만약 [!DNL Flash] 저장소가 0KB로 설정되어 있거나 블록에 다른 설정이 있습니다 [!DNL Flash] 응용 프로그램에서 데이터를 로컬로 저장하지 않으므로, [!DNL Workfront Proof] 뷰어:

* 다시 표시하지 않는 옵션이 선택되었지만 &#39;시작하기&#39; 투어 팝업이 계속 나타납니다
* [!DNL Workfront Proof] 증명에 추가된 댓글 수가 증가하여 뷰어 성능이 느려집니다
* 증명을 로드할 수 없으며 실제 이미지 대신 &#39;회색 화면&#39;을 사용할 수 있습니다

## 허용 [!DNL Flash] 공유 개체

저장 [!DNL Flash] 공유 개체는 컴퓨터에서 허용되며 저장소 제한은 0이 아닙니다.

공유 객체가 허용되는지 확인하려면

1. 에서 마우스 오른쪽 단추를 클릭합니다. [!DNL Workfront Proof] 뷰어.
1. 선택 **[!UICONTROL 전역 설정]** 컨텍스트 메뉴에서 을 클릭합니다.
1. 로 이동합니다. **[!UICONTROL 스토리지]** 탭.
1. 확인 **[!UICONTROL 사이트에서 이 컴퓨터에 정보를 저장하도록 허용]** 이 선택됨 (1).
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## 증가 [!DNL Flash] 저장소

기본적으로 [!DNL Flash] 응용 프로그램은 사용자의 드라이브에 최대 100KB의 데이터를 저장할 수 있지만 사용자가 쉽게 수정할 수 있습니다. 많은 사용자를 위한 솔루션 [!DNL Flash] 관련 문제가 내부 [!DNL Flash] 저장. 이 작업은 [!DNL Workfront Proof] 뷰어:

1. 증명을 엽니다.
1. 증명의 마우스 오른쪽 단추 클릭 메뉴를 엽니다.
1. 클릭 **[!UICONTROL 설정]** 열다 [!DNL Flash] 설정 팝업.
1. 로 이동합니다. **[!UICONTROL 로컬]** 저장소 탭.
1. 스토리지를 최대 100KB(1)까지 늘립니다.
1. 설정 팝업을 닫고 증명 를 다시 엽니다.

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)
