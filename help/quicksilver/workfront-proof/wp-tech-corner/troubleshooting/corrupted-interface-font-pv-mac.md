---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: 문제 해결 - Mac의 proofing viewer에서 인터페이스 글꼴이 손상되었습니다.
description: Mac의 증명 뷰어에서 Trobuelshot 손상된 인터페이스 글꼴
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 문제 해결 - Mac의 proofing viewer에서 인터페이스 글꼴이 손상되었습니다.

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

증명 뷰어에 인터페이스 글꼴이 제대로 표시되지 않는 경우 Mac 시스템의 글꼴에 문제가 있기 때문일 수 있습니다. 문제를 해결하려면 다음 해결 방법을 시도해 보십시오.

## 글꼴 중복 제거

시스템에 중복 글꼴이 있는지 확인합니다.

1. 사용 중인 브라우저를 닫습니다.
1. 응용 프로그램 폴더에서 글꼴 책 응용 프로그램을 엽니다.
1. **[!UICONTROL 모든 글꼴]**(1)을 클릭합니다.
1. **[!UICONTROL 편집]** > **[!UICONTROL 활성화된 중복 항목 찾기]**&#x200B;를 클릭합니다.

1. 중복을 해결하려면 **[!UICONTROL 예]**&#x200B;를 클릭하세요.
1. 손상된 글꼴에 대한 경고가 표시되면 **[!UICONTROL 예]**&#x200B;를 클릭합니다.
1. 컴퓨터를 다시 시작합니다.
1. 증명을 다시 시도하십시오.

## 글꼴 캐시 지우기

때때로 Mac OS X에서 글꼴 캐시가 손상됩니다. 예를 들어 글꼴이나 글꼴 모음을 여러 번 다시 설치하거나 응용 프로그램을 업데이트하거나 다시 설치한 경우 운영 체제의 글꼴 캐시 파일 외에도 일부 응용 프로그램에는 자체 글꼴 캐시가 있을 수 있습니다. 이러한 글꼴 캐시 파일을 삭제하면 잘못된 텍스트 문제가 해결될 수 있습니다.

먼저, Font Book을 실행하고 문제가 있는 글꼴이나 패밀리를 선택한 다음 키보드에서 삭제 단추를 눌러야 합니다. 마우스 오른쪽 단추를 클릭하고 [!UICONTROL 가족 제거]를 선택할 수도 있습니다. 어떤 글꼴 또는 제품군에서 문제가 발생하는지 확실하지 않은 경우 위에서 설명한 대로 중복 항목을 먼저 제거해 보십시오.

두 번째 단계는 글꼴 캐시를 지우는 것이며, 이를 위해 몇 가지 방법이 있습니다.

첫 번째는 시작할 때 부팅 소리를 들을 때 Shift 키를 바로 눌러 안전 모드로 재부팅하는 것입니다. 이 모드가 로드되면 진행률 표시줄이 나타나야 하며, 이 동안 시스템에서 다양한 확인 및 유지 관리 루틴이 실행되며, 그 중 하나는 글꼴 캐시를 지우는 것입니다.

두 번째 방법은 Terminal을 사용하는 것입니다. 관리 계정 내에서 다음 명령을 실행하여 수행할 수 있습니다. *sudo atsutil databases -remove*

>[!NOTE]
>
>이 명령을 사용하려면 암호를 입력해야 하며, 암호를 입력할 때 이 암호는 표시되지 않습니다. 이 경우 컴퓨터에 대한 관리자 권한이 필요할 수 있으므로 IT 부서에 문의하는 것이 좋습니다.

다른 접근 방식은 FontNuke와 같은 글꼴 캐시 유틸리티를 사용하고 그 도움을 받아 캐시를 지우는 것입니다.

많은 프리프레스 및 아트워크/디자인 스튜디오 또한 Universal Type Server 소프트웨어를 사용하여 글꼴의 라이선싱과 배포를 관리합니다. 경우에 따라 유니버설 형식 서버 글꼴 캐시에서 문제가 발생하여 [!DNL Workfront Proof] 주석이 사라질 수 있습니다.

이 문제를 해결하려면 유니버설 유형 서버 글꼴 캐시를 지우고 유니버설 유형 서버를 다시 시작합니다.

## [!DNL Flash] 글꼴 충돌 해결

이 기능은 대부분의 환경에서 더 이상 사용되지 않는 [!DNL Flash]에서 지원되므로 액세스할 수 없습니다.

레거시 증명 뷰어는 [!DNL Flash Player]을(를) 기반으로 하며, 증명 뷰어에 텍스트가 없는 경우 OS X와 [!DNL Flash Player] 간에 글꼴이 충돌할 수 있습니다. 다음을 시도해 보십시오.

1. Finder를 열고 **[!UICONTROL 이동]** 탭을 엽니다.
1. Option 키(⌥Alt)를 눌러 드롭다운 목록에서 [!UICONTROL Library] 폴더를 엽니다.
1. Option 키를 누른 상태에서 [!UICONTROL 라이브러리] 폴더를 클릭합니다.
1. [!UICONTROL Library] 폴더가 열린 후 내의 [!UICONTROL Fonts] 폴더로 이동하십시오.
1. [!UICONTROL Fonts] 폴더에 있는 모든 글꼴을 바탕 화면의 다른 폴더로 이동합니다(Fonts 폴더 내에 다른 폴더를 만들지 마십시오).
1. 이렇게 하면 사용자 정의 글꼴이 모두 숨겨집니다. 표준 시스템 글꼴은 별도의 위치에 저장되어야 합니다.
1. [!DNL Safari]을(를) 종료한 후 다시 시작합니다.
1. 증명을 다시 엽니다.

이제 글꼴이 표시됩니다. 홈 디렉터리에서 제거한 글꼴이 필요하지 않으면 안전하게 삭제할 수 있습니다. 그렇지 않으면 일괄로 이동하여 Library/Fonts 폴더에 다시 복사한 다음 문제의 원인이 무엇인지 확인합니다.
