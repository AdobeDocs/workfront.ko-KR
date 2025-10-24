---
product-area: documents
navigation-topic: proofing-overview
title: 웹 증명 뷰어 확장에서 대화형 콘텐츠 검토
description: Adobe Workfront 검토 도구는 ZIP 파일 또는 URL로 인터랙티브한 콘텐츠를 증명 할 수 있는 브라우저 확장 기능입니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 78d9e8e47f8f6777f9211d8f85a3dfbc9405d798
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 1%

---

# Adobe Workfront 검토 도구를 사용하여 대화형 콘텐츠 검토


>[!IMPORTANT]
>
> SSO 인증이 필요하거나 Figma와 같이 iFrame에서 사이트를 열 수 없는 웹 사이트에서 호스팅되는 대화형 콘텐츠에는 데스크톱 증명 뷰어를 사용하는 것이 좋습니다.

Adobe Workfront 검토 도구는 ZIP 파일 또는 URL로 대화형 컨텐츠를 마크업할 수 있는 웹 기반 브라우저 확장 프로그램입니다. Adobe Workfront 검토 도구는 다음 브라우저에서 사용할 수 있습니다.

* Firefox
* Chrome
* Edge
* Safari

## 확장 설치

### 전제 조건

* Adobe Workfront 검토 도구를 사용하려면 기존 웹 뷰어 확장을 제거해야 합니다.

### 확장 설치

검토자와 승인자는 Adobe Workfront 검토 도구를 설치해야 합니다. 다음 브라우저 중 하나에서 다음을 수행합니다.

* [Firefox 확장 프로그램](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome 확장](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

* [Safari 확장](https://apps.apple.com/us/app/adobe-workfront-review-tool/id6741517062?mt=12)



Adobe Workfront 검토 도구에서 대화형 증명을 자동으로 열려면 Workfront 관리자가 아래 섹션에 설명된 대로 workfront에서 증명 설정을 업데이트해야 합니다.

## GenStudio for Performance Marketing 및 Creative Cloud Express에서 Adobe Workfront 검토 도구 사용

이 확장은 GenStudio for Performance Marketing 및 Creative Cloud Express에서 콘텐츠를 검토하는 데 필요합니다. Assets이 웹 뷰어에서 자동으로 열립니다. 계정 설정을 업데이트할 필요가 없습니다.


## Workfront 증명 기본값 업데이트

대화형 콘텐츠에 대한 기본 뷰어로 Workfront 검토 도구를 사용하려면 Workfront에서 증명 기본값을 업데이트해야 합니다.

>[!IMPORTANT]
>
>검토해야 하는 컨텐츠가 웹 사이트에 있는 경우 Desktop Proofing Viewer를 사용하는 것이 좋습니다.
>
>* SSO 인증 필요
>* Figma와 같은 iFrame에서 사이트 열기 방지

### Adobe Workfront 검토 도구를 URL 및 ZIP 증명에 대한 기본 뷰어로 설정

URL 및 ZIP 증명에 웹 검토 도구를 사용하려면 Workfront 관리자가 대화형 증명에 대한 기본 설정을 조정해야 합니다.

1. Workfront 주 메뉴에서 **증명**&#x200B;을 클릭합니다.
1. **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.
1. **증명 기본값** 섹션에서 대화형 증명을 위한 **데스크톱 증명 뷰어**&#x200B;를 찾은 다음 **설정**&#x200B;을 클릭합니다.
1. 드롭다운 메뉴에서 **사용 안 함**&#x200B;을 선택합니다. URL 또는 ZIP 파일에서 생성된 대화형 증명이 이제 웹 기반 브라우저인 Adobe Workfront 검토 도구에서 자동으로 열립니다.
1. **저장**&#x200B;을 클릭합니다.

>[!NOTE]
>
>이 변경 사항은 Workfront 인스턴스의 모든 대화형 증명에 적용됩니다. 프로덕션에서 활성화하기 전에 미리보기 환경에서 새 경험을 테스트하는 것이 좋습니다. **대화형 증명에 대한 데스크톱 증명 뷰어** 계정 설정을 **모든 대화형 증명에 대해 사용**(으)로 다시 변경하면 데스크톱 뷰어로 쉽게 다시 전환할 수 있습니다.

### Adobe Workfront 검토 도구를 ZIP 증명에 대한 기본 뷰어로 설정

ZIP 증명에만 웹 검토 도구를 사용하려면 Workfront 관리자가 대화형 증명에 대한 기본 설정을 조정해야 합니다.

1. Workfront 주 메뉴에서 **증명**&#x200B;을 클릭합니다.
1. **계정 설정**&#x200B;을 클릭한 다음 **설정** 탭을 클릭합니다.
1. **증명 기본값** 섹션에서 대화형 증명을 위한 **데스크톱 증명 뷰어**&#x200B;를 찾은 다음 **설정**&#x200B;을 클릭합니다.
1. 드롭다운 메뉴에서 **URL에서 만든 대화형 증명에 대해서만 활성화됨**&#x200B;을 선택합니다. ZIP 파일에서 생성된 대화형 증명이 이제 웹 기반 브라우저인 Adobe Workfront 검토 도구에서 자동으로 열립니다. URL에서 만든 대화형 증명은 여전히 데스크탑 증명 뷰어에서 열립니다.
1. **저장**&#x200B;을 클릭합니다.

>[!NOTE]
>
>이 변경 사항은 Workfront 인스턴스의 모든 ZIP 증명에 적용됩니다. 프로덕션에서 활성화하기 전에 미리보기 환경에서 새 경험을 테스트하는 것이 좋습니다. **대화형 증명에 대한 데스크톱 증명 뷰어** 계정 설정을 **모든 대화형 증명에 대해 사용**(으)로 다시 변경하면 데스크톱 뷰어로 쉽게 다시 전환할 수 있습니다.

