---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 문제 해결 - Mac에서 언어 교정 뷰어의 인터페이스 글꼴이 손상되었습니다.
description: 언어 교정 뷰어에 인터페이스 글꼴이 제대로 표시되지 않는 경우 Mac 시스템의 글꼴에 문제가 있기 때문일 수 있습니다. 문제를 해결하려면 다음 해결 방법 - EDIT ME를 사용하십시오.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 문제 해결 - Mac에서 언어 교정 뷰어의 인터페이스 글꼴이 손상되었습니다.

>[!IMPORTANT]
>
>이 문서는 독립형 제품의 기능을 참조합니다 [!DNL Workfront Proof]. 내부 교정에 대한 자세한 정보 [!DNL Adobe Workfront]를 참조하십시오. [교정](../../../review-and-approve-work/proofing/proofing.md).

언어 교정 뷰어에 인터페이스 글꼴이 제대로 표시되지 않는 경우 Mac 시스템의 글꼴에 문제가 있기 때문일 수 있습니다. 문제를 해결하려면 다음 솔루션을 사용하십시오.

## 글꼴 중복 제거

시스템에 중복된 글꼴이 있는지 확인합니다.

1. 사용 중인 브라우저를 닫습니다.
1. 응용 프로그램 폴더에서 Font Book 응용 프로그램을 엽니다.
1. 클릭 **[!UICONTROL 모든 글꼴]** (1).
1. 클릭 **[!UICONTROL 편집]** > **[!UICONTROL 활성화된 중복 검색]**.

1. 클릭 **[!UICONTROL 예]** 중복 항목을 해결하기 위해
1. 손상된 글꼴에 대한 경고가 표시되면 **[!UICONTROL 예]**.
1. 컴퓨터를 다시 시작합니다.
1. 증명을 다시 시도하십시오.

## 글꼴 캐시 지우기

Mac OS X의 글꼴 캐시가 손상되는 경우가 있습니다. 예를 들어 글꼴이나 글꼴 모음을 여러 번 다시 설치하거나 응용 프로그램을 업데이트하거나 다시 설치한 경우 운영 체제의 글꼴 캐시 파일 외에도 일부 응용 프로그램에는 자체 글꼴 캐시가 있을 수 있습니다. 이러한 글꼴 캐시 파일을 삭제하면 잘못된 텍스트에서 문제가 해결됩니다.

먼저 Font Book을 실행하고 문제가 발생하는 글꼴이나 패밀리를 선택하고 키보드에서 Delete 단추를 누릅니다. 마우스 오른쪽 단추를 클릭하고 을 선택할 수도 있습니다 [!UICONTROL 패밀리 제거]. 어떤 글꼴이나 패밀리로 인해 문제가 발생하는지 확실하지 않은 경우 위에 설명된 대로 먼저 중복을 제거해 볼 수 있습니다.

두 번째 단계는 글꼴 캐시를 지우는 것이며 이를 실현하는 방법에는 여러 가지가 있습니다.

첫 번째 방법은 시작 시 부트 종소리가 들리면 즉시 Shift 키를 눌러 안전 모드로 재부팅하는 것입니다. 이 모드가 로드되면 진행률 표시줄이 나타나야 합니다. 이때 시스템은 글꼴 캐시를 지우는 다양한 검사 및 유지 관리 루틴을 실행합니다.

두 번째 방법은 관리 계정 내에서 다음 명령을 실행하여 수행할 수 있는 터미널을 사용하는 것입니다. *sutil databases -remove*

>[!NOTE]
>
>이 명령을 사용하려면 암호를 입력해야 합니다. 암호를 입력하면 표시되지 않습니다. 시스템에 대한 관리자 권한이 필요할 수 있으므로 IT 부서와 상담하는 것이 좋습니다.

또 다른 방법은 FontNuck과 같은 글꼴 캐시 유틸리티를 사용하여 캐시를 삭제하는 것입니다.

많은 사전 인쇄 및 기술 작업/디자인 스튜디오는 또한 Universal Type Server 소프트웨어를 사용하여 글꼴의 라이센스와 배포를 관리합니다. Universal Type Server Font Cache에서 문제가 발생할 수 있으며, 이로 인해 [!DNL Workfront Proof] 제거할 주석.

수정하려면 범용 유형 서버 글꼴 캐시를 지우고 범용 유형 서버를 다시 시작합니다.

## 수정 [!DNL Flash] 글꼴 충돌

이 기능은 [!DNL Flash]: 대부분의 환경에서 더 이상 사용되지 않습니다.

레거시 언어 교정 뷰어는 [!DNL Flash Player] 그리고 경우에 따라 교정 뷰어에서 텍스트가 누락된 경우 OS X와 글꼴 충돌이 있을 수 있습니다 [!DNL Flash Player]. 다음을 시도해 보십시오.

1. Finder를 열고 **[!UICONTROL 이동]** 탭.
1. Option 키(⌥ Alt)를 눌러 [!UICONTROL 라이브러리] 드롭다운 목록의 폴더.
1. Option 키를 누른 채 [!UICONTROL 라이브러리] 폴더를 입력합니다.
1. 다음 이후 [!UICONTROL 라이브러리] 폴더 열기 [!UICONTROL 글꼴] 폴더 내에 있습니다.
1. 에 있는 모든 글꼴을 [!UICONTROL 글꼴] 폴더를 다른 폴더로, 어쩌면 바탕 화면에 있을 수 있습니다(Fonts 폴더 내에 다른 폴더를 만들지 마십시오).
1. 이 작업은 모든 사용자 지정 글꼴을 숨깁니다. 표준 시스템 글꼴은 별도의 위치에 저장해야 합니다.
1. 종료 및 다시 시작 [!DNL Safari].
1. 증명을 다시 엽니다.

이제 글꼴이 표시됩니다. 홈 디렉터리에서 제거한 글꼴이 필요하지 않으면 안전하게 삭제할 수 있습니다. 그렇지 않으면 일괄적으로 살펴보고 Library/Fonts 폴더로 다시 복사하여 문제가 발생하는 항목을 확인합니다.
