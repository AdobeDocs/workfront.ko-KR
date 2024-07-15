---
title: 23.3 통합 개선 사항
description: 23.3 통합 개선 사항
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 23.3 통합 개선 사항

이 페이지에서는 23.3 릴리스의 모든 통합 개선 사항에 대해 설명합니다. 이러한 개선 사항은 2023년 7월 20일과 21일에 23.3 릴리스를 통해 프로덕션 환경에서 사용할 수 있습니다.

23.3 릴리스 주기 동안 현재 사용 가능한 모든 변경 사항 목록을 보려면 [23.3 릴리스 개요](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md)를 참조하십시오.

## 새로운 Google Workspace 통합 사용 가능

이제 Google Marketplace에서 새로운 Google Workspace 통합을 사용할 수 있습니다. 새 통합은 OAuth2를 사용하여 인증하고 이전 통합을 대체합니다.

이전 Google Workspace 통합은 이제 더 이상 사용되지 않으며 자동으로 제거됩니다.

새 통합을 설치하는 방법에 대한 지침은 [설치 [!DNL Adobe Workfront for Google Workspace]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)를 참조하십시오.

Google Workspace용 Workfront에 대한 자세한 내용은 Google Workspace용 [Workfront](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md)을(를) 참조하십시오.

## 이제 Adobe Creative Cloud 통합은 할당된 여러 사용자를 지원합니다

이제 Adobe Creative Cloud 통합은 작업 또는 문제에 여러 명의 사용자가 할당된 경우 &quot;내 부분 완료&quot;와 &quot;완료&quot;(또는 &quot;해결됨&quot;) 중에서 선택하는 기능을 지원합니다.

이전에는 통합을 통해 사용자가 &quot;내 부품으로 완료&quot; 또는 &quot;완료&quot;/&quot;해결됨&quot;을 지정하지 않고 작업을 완료됨으로 표시할 수 있었습니다.

이 기능을 활용하려면 Creative Cloud 플러그인용 최신 Workfront을 다운로드하여 설치하십시오.

기능에 대한 자세한 내용은 [Adobe Workfront 플러그인을 사용하여 작업 항목 완료 표시](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md)를 참조하십시오.

Creative Cloud 플러그인용 Workfront 설치에 대한 자세한 내용은 [Creative Cloud 애플리케이션용 Adobe Workfront 플러그인 설치](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md)를 참조하십시오.

## Creative Cloud 플러그인을 위해 Workfront에서 Workfront 알림 보기 및 관리

필요한 알림을 더 쉽게 받을 수 있도록 Adobe Creative Cloud을 종료하지 않고도 Workfront 알림을 보고 관리할 수 있도록 했습니다. 이제 Creative Cloud 애플리케이션 내의 Workfront 플러그인 창에서 직접 알림을 보고 해당 알림과 관련된 작업 항목 및 설명에 액세스할 수 있습니다.

이전에는 알림을 Workfront 내에서 이메일을 통해서만 사용할 수 있었습니다.

이 기능을 활용하려면 Creative Cloud 플러그인용 최신 Workfront을 다운로드하여 설치하십시오.

자세한 내용은 [Adobe Creative Cloud의 알림 보기 및 관리 [!DNL Adobe Workfront] 알림](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md)을 참조하세요.

Creative Cloud 플러그인용 Workfront 설치에 대한 자세한 내용은 [Creative Cloud 애플리케이션용 Adobe Workfront 플러그인 설치](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md)를 참조하십시오.

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## 프로젝트를 만들 때 Adobe Experience Manager Assets에 연결된 폴더를 자동으로 만듭니다.

Adobe Experience Manager 통합에 대한 새 연결된 폴더 만들기 워크플로를 사용하여 Adobe Experience Manager Assets 폴더의 경로로 통합을 구성할 수 있습니다. 통합이 프로젝트 템플릿에 추가되면 템플릿에서 만든 모든 프로젝트는 지정된 폴더의 Experience Manager Assets에 연결된 하위 폴더를 자동으로 만듭니다.

이전에는 연결된 폴더를 만들 때 사용자의 작업이 필요했습니다.

이 기능은 Workfront 내의 Adobe Experience Manager as a Cloud Service 통합에서만 사용할 수 있습니다. Adobe Experience Manager 강화 커넥터에서는 사용할 수 없습니다.

자세한 내용은 [Experience Manager Assets 통합에서 워크플로우 사용](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md)을 참조하십시오.

## Workfront 필드 값을 Experience Manager Assets의 태그에 매핑

이제 Workfront의 데이터를 기반으로 에셋을 분류하고 빠르게 찾을 수 있습니다. Workfront for Experience Manager Assets 통합에서 이 데이터를 메타데이터 구성의 일부로 매핑할 수 있습니다.

이전에는 Workfront 데이터를 Experience Manager Assets 태그에 매핑할 수 없었습니다.

Experience Manager Assetsas a Cloud Service 의 이 기능에 대한 자세한 내용은 [Experience Manager Assets as a Cloud Service 구성] 통합](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)을 참조하십시오.
[!UICONTROL 
Experience Manager Assets Essentials의 이 기능에 대한 자세한 내용은 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

## Workfront 필드를 사용자 지정 Experience Manager Assets 메타데이터 필드에 매핑

이제 기본 통합을 사용하여 Experience Manager Assetsas a Cloud Service 의 기본 메타데이터 스키마 필드와 기본 제공 Workfront 스키마 필드를 모두 매핑할 수 있습니다.

Experience Manager Assetsas a Cloud Service 의 이 기능에 대한 자세한 내용은 [Experience Manager Assets as a Cloud Service 구성] 통합](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)을 참조하십시오.
[!UICONTROL 
Experience Manager Assets Essentials의 이 기능에 대한 자세한 내용은 [Experience Manager Assets Essentials 통합 구성](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)을 참조하십시오.

## Adobe Workfront for Creative Cloud을 사용하여 자동 증명 워크플로 템플릿 설정 조정

이제 Creative Cloud에서 직접 기존의 자동화된 워크플로 템플릿 설정을 조정할 수 있습니다. 기존의 자동화된 워크플로 템플릿을 선택하면 다음과 같은 작업을 수행할 수 있습니다.

* 단계 비활성화
* 추가 수신자 추가
* 증명 역할 변경
* 기한 조정
* 이메일 알림 업데이트
* 기타!

자세한 내용은 [Plugin for [!DNL Creative Cloud] Applications](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md)을(를) 사용하여  [!DNL Adobe Workfront] 문서 및 증명 업로드 를 참조하십시오.

이러한 개선 사항은 다음 Creative Cloud 앱에서 사용할 수 있습니다.

* Photoshop
* XD
* InDesign
* Illustrator
