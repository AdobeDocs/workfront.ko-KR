---
title: 22.4 기타 개선 사항
description: 22.4 기타 개선 사항
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 4e41eed3-1a3b-4247-8c0c-630efc9c1b69
source-git-commit: 0fea13b0a1d8f14c2d601e0ed0a8d15684a3c4d7
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 0%

---

# 22.4 기타 개선 사항

이 페이지에서는 미리 보기 환경에 대한 22.4 릴리스로 수행된 다른 모든 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2022년 10월 3일이 있는 주에 제공될 예정입니다.

22.4 릴리스에서 사용할 수 있는 모든 변경 사항 목록에 대해서는 다음을 참조하십시오 [22.4 릴리스 개요](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Adobe Workfront for InDesign

이제 이 플러그인을 InDesign에 설치할 수 있습니다. 이 기능을 사용하면 XD를 종료하지 않고도 작업 항목 세부 사항에 액세스하고, 업데이트 영역에서 동료와 협업하며, 검토를 위해 증명을 제출할 수 있습니다. 지금 Adobe Creative Cloud 마켓플레이스로 이동하여 플러그인을 다운로드하십시오.

플러그인에 대한 자세한 내용은 [[!DNL Adobe Workfront] plugin for [!DNL Creative Cloud] 애플리케이션](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-cc.md).

[현재 마켓플레이스에서 InDesign용 Adobe Workfront 다운로드](https://exchange.adobe.com/apps/cc/108938/adobe-workfront-for-indesign).

또한 관리자는 [플러그인으로 패키지 만들기](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html) 관리 또는 자가 관리 방식으로 Admin Console 및 배포에서 사용자에게 할당합니다.

## 개체 메타데이터를 기본 Experience Manager Assets 통합과 동기화

이제 Workfront에서 필드가 변경되면 Workfront 포트폴리오, 프로그램, 프로젝트, 작업, 문제 및 문서 필드가 자동으로 업데이트됩니다.

개체 메타데이터를 자동으로 동기화하려면 설정 > Experience Manager 통합에서 통합을 위해 동기화 개체 메타데이터 전환을 활성화해야 합니다.

이전에는 프로젝트 필드만 자동으로 업데이트되었습니다.

자세한 내용은 [Experience Manager Assets as a Cloud Service 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## 메타데이터가 프로그램 및 포트폴리오 상위 개체를 푸시합니다.

이제, 자산이 Experience Manager Assets 또는 Assets Essentials으로 처음 전송되면 프로그램 및 포트폴리오 상위 개체에 대해 매핑하도록 구성된 모든 메타데이터도 전송됩니다.

이전에는 상위 프로젝트 데이터만 전송되었습니다.

자세한 내용은 [Experience Manager Assets 또는 Assets Essentials으로 문서 보내기](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md).

## 확장된 팀 설명

이제 팀 영역에서 설명을 클릭하여 전체 팀 설명을 클릭하여 팝업에 표시할 수 있습니다. 설명에 있는 모든 URL을 팝업에서 클릭할 수 있으며, 설명 텍스트를 클릭하여 편집할 수 있습니다(팀 설정을 편집할 수 있는 액세스 권한이 있는 경우).

이전에는 좁은 영역에서 설명을 스크롤하는 것이 모든 컨텐츠를 볼 수 있는 유일한 방법이었습니다.

설명에 대한 이러한 개선 사항은 민첩성 및 비애자일 팀 모두에 적용됩니다.

자세한 내용은 [팀 만들기](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/create-a-team.md).

## Workfront Campaigns(Beta) - 작업을 관리하는 새로운 방법

>[!NOTE]
>
>이 기능은 원래 22.3 릴리스 주기 동안 미리 보기에 도입되었습니다.

>[!NOTE]
>
>이 기능은 베타로만 사용할 수 있으며 현재 개발 중입니다. 향후 릴리스에서 Campaign 워크플로우에 대한 기능을 계속 추가할 예정입니다. Workfront 캠페인을 위한 베타 프로그램에 참여하는 것은 자발적입니다.

Adobe Workfront에 작업 방식을 변경할 수 있는 새로운 개체가 도입되었습니다.

Workfront Campaign을 사용하면 다양한 포트폴리오 및 프로그램에서 프로젝트를 새로운 작업 컨테이너에서 구성할 수 있습니다. 이 새 컨테이너는 이후 릴리스에서 발전하여 현재 별도의 사일로에서 관리되는 모든 작업 개체를 포함하게 됩니다.

이 릴리스에는 다음 기능이 포함됩니다.

* Campaign이라는 새로운 Workfront 개체

* 기본 메뉴의 새 캠페인(베타) 영역

* 캠페인 영역의 캠페인 목록

* 캠페인에 대한 추가 정보를 표시하는 캠페인 세부 사항 페이지

* 캠페인에 프로젝트 추가 기능

* 캠페인 정보 편집 기능

* 레이아웃 템플릿에서 Campaign 개체의 이름을 바꾸는 기능

   Workfront 시스템 및 그룹 관리자는 레이아웃 템플릿의 기본 메뉴에서 캠페인(베타) 영역을 추가할 수 있습니다. 이렇게 하면 템플릿에 할당된 모든 사용자가 사용할 수 있습니다. 사용 가능한 경우 Workfront의 모든 사용자가 캠페인을 만들 수 있습니다.


