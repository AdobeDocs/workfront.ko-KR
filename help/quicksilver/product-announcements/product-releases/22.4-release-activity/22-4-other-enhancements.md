---
title: 22.4 기타 개선 사항
description: 22.4 기타 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4e41eed3-1a3b-4247-8c0c-630efc9c1b69
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 0%

---

# 22.4 기타 개선 사항

이 페이지에서는 미리보기 환경에 대한 22.4 릴리스의 기타 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 10월 3일이 있는 주에 사용할 수 있습니다.

22.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록을 보려면 [22.4 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md)를 참조하십시오.

## InDesign용 Adobe Workfront

이 플러그인은 이제 InDesign에서 설치할 수 있습니다. XD을 종료하지 않고도 작업 항목 세부 정보에 액세스하고, 업데이트 영역에서 동료와 공동 작업하고, 검토를 위해 증명을 제출할 수 있습니다. 지금 Adobe Creative Cloud 마켓플레이스로 이동하여 플러그인을 다운로드하십시오.

플러그인에 대한 자세한 내용은 [[!DNL Adobe Workfront] 응용 프로그램 [!DNL Creative Cloud] 용 플러그인](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-cc.md)을 참조하십시오.

[현재 마켓플레이스에서 InDesign용 Adobe Workfront을 다운로드하세요](https://exchange.adobe.com/apps/cc/108938/adobe-workfront-for-indesign).

또한 관리자는 Admin Console에서 [플러그인을 사용하여 패키지를 만들고](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html) 관리 또는 자체 관리 방식으로 사용자에게 배포할 수 있습니다.

## 기본 Experience Manager Assets 통합으로 개체 메타데이터 동기화

이제 Workfront에서 필드를 변경하면 Workfront 포트폴리오, 프로그램, 프로젝트, 작업, 문제 및 문서 필드가 자동으로 업데이트됩니다.

오브젝트 메타데이터가 자동으로 동기화되도록 하려면 설정 > Experience Manager 통합에서 통합에 대해 오브젝트 메타데이터 동기화 토글을 활성화해야 합니다.

이전에는 프로젝트 필드만 자동으로 업데이트되었습니다.

자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)을 참조하십시오.

## 메타데이터가 프로그램 및 포트폴리오 상위 개체를 푸시합니다.

이제 에셋을 Experience Manager Assets 또는 Assets Essentials로 처음 전송하면 프로그램 및 포트폴리오 상위 오브젝트에 매핑되도록 구성된 메타데이터도 모두 전송됩니다.

이전에는 상위 프로젝트 데이터만 전송되었습니다.

자세한 내용은 [Experience Manager Assets 또는 Assets Essentials로 문서 보내기](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md)를 참조하십시오.

## 팀 설명 확장됨

이제 팀 영역에서 설명을 클릭하여 팝업에 표시하여 전체 팀 설명을 볼 수 있습니다. 설명의 모든 URL은 팝업에서 클릭할 수 있으며, 팀 설정을 편집할 수 있는 액세스 권한이 있는 경우 설명 텍스트를 클릭하여 편집할 수 있습니다.

이전에는 좁은 영역에서 설명을 스크롤하는 것이 모든 콘텐츠를 볼 수 있는 유일한 방법이었습니다.

설명에 대한 이 개선 사항은 애자일 팀과 애자일이 아닌 팀 모두에 적용됩니다.

자세한 내용은 [팀 만들기](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/create-a-team.md)를 참조하세요.

## Workfront 캠페인(Beta) - 작업을 관리하는 새로운 방법

>[!NOTE]
>
>이 기능은 원래 22.3 릴리스 주기 동안 미리보기에 도입되었습니다.

>[!NOTE]
>
>이 기능은 베타로만 사용할 수 있으며 현재 구성 중입니다. 향후 릴리스를 통해 Campaign 워크플로우에 대한 기능을 계속 추가할 예정입니다. Workfront Campaign의 Beta 프로그램 참여는 자발적입니다.

Adobe Workfront에 작업 관리 방식을 변경할 수 있는 가능성이 있는 새로운 개체를 도입합니다.

Workfront Campaign을 사용하면 새로운 작업 컨테이너에서 다양한 포트폴리오 및 프로그램의 프로젝트를 구성할 수 있습니다. 이 새 컨테이너는 향후 릴리스에서 발전하여 결국 별도의 사일로에서 현재 관리되는 모든 작업 개체를 포함하게 됩니다.

이 릴리스에는 다음과 같은 기능이 포함되어 있습니다.

* Campaign이라는 새 Workfront 개체

* 메인 메뉴의 새 캠페인(Beta) 영역

* 캠페인 영역의 캠페인 목록

* 캠페인에 대한 추가 정보를 표시하는 캠페인 세부 정보 페이지

* 캠페인에 프로젝트 추가 기능

* Campaign에 대한 정보 편집 기능

* 레이아웃 템플릿에서 Campaign 개체의 이름을 바꾸는 기능

  Workfront 시스템 및 그룹 관리자는 레이아웃 템플릿의 기본 메뉴에서 캠페인(Beta) 영역을 추가할 수 있습니다. 이렇게 하면 템플릿에 할당된 모든 사용자가 사용할 수 있습니다. 사용 가능한 상태가 되면 Workfront의 모든 사용자가 캠페인을 만들 수 있습니다.


