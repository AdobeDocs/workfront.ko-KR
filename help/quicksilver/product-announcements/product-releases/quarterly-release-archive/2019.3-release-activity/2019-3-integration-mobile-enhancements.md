---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 통합 및 모바일 개선 사항
description: 이 페이지에서는 2019.3 릴리스에 포함된 모든 변경 사항 통합 및 모바일 개선 사항에 대해 설명합니다. 2019년 8월 19일이 있는 주에 프로덕션 환경에서 사용할 수 있게 되었습니다.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 2019.3 통합 및 모바일 개선 사항

이 페이지에서는 2019.3 릴리스에 포함된 모든 변경 사항 통합 및 모바일 개선 사항에 대해 설명합니다. 2019년 8월 19일이 있는 주에 프로덕션 환경에서 사용할 수 있게 되었습니다.

2019.3의 모든 변경 사항 목록은 [2019.3 릴리스 활동 개요](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md)를 참조하십시오.

## MS OneDrive 통합에서 공유 항목 지원

이제 공유된 OneDrive 파일 및 폴더를 Workfront 개체에 연결할 수 있습니다. 반대로 Workfront의 파일을 OneDrive의 공유 폴더로 업로드할 수 있습니다.

자세한 내용은 문서 [외부 애플리케이션에서 문서 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)의 [Workfront에 외부 문서 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [하나 이상의 외부 폴더 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) 및 [Workfront에서 외부 클라우드 공급자에 문서 업데이트 및 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) 섹션을 참조하십시오.

자세한 내용은 문서 [외부 응용 프로그램에서 문서 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)의 [외부 문서를 Workfront에 연결](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) 섹션을 참조하십시오.

## 모든 Workfront 로그인에 필요한 도메인 사양

이제 Workfront URL에 도메인이 지정되지 않은 경우 모든 Workfront 로그인을 수행하려면 사용자가 도메인을 지정해야 합니다. 이 정보가 필요하므로 Workfront 인스턴스의 보안이 강화됩니다. 또한 Workfront 구현에 여러 인스턴스가 있는 경우 이 향상된 기능을 통해 구현 내에서 Workfront의 각 인스턴스에 동일한 사용자를 추가할 수 있습니다.

이 변경 사항은 사용자 로그인 및 API 통합 모두에 영향을 줄 수 있습니다.

* **사용자 로그인**

  회사 도메인이 Workfront URL에 포함되지 않은 경우 이제 로그인 화면에 사용자 이름 및 암호 필드 외에 새 도메인 필드가 표시됩니다.

  도메인 정보가 Workfront URL에 이미 포함되어 있으므로 대부분의 고객은 변경할 필요가 없습니다. 예: &quot;*도메인*.my.workfront.com&quot;

* **API 통합**

  도메인 이름을 포함하지 않는 주소로 이동하는 API 코드가 있는 경우 해당 API 코드는 더 이상 작동하지 않습니다.

자세한 내용은 [Adobe Workfront 로그인](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md)을 참조하세요.

## iOS에서 모바일 앱을 사용하여 작업 및 문제를 프로젝트로 전환

이제 iOS의 Workfront 모바일 앱에서 개별 작업 및 문제를 프로젝트로 변환할 수 있습니다.

## 지문 또는 얼굴 ID로 모바일 앱에 로그인

장치에 따라 지문 또는 얼굴 ID 기술을 사용하여 Workfront 모바일 앱에 로그인하도록 선택할 수 있습니다. 모바일 앱에 로그인하면 휴대폰에서 지원하는 인증 방법을 사용하여 로그인할지 묻는 메시지가 표시됩니다.

이 기능을 관리하는 방법에 대한 자세한 내용은 [iOS용 Adobe Workfront](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) 또는 [Android용 Adobe Workfront](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)을 참조하십시오.

## 모바일에서 사용자를 자동으로 로그아웃하는 새로운 설정

귀하와 귀사에서 Workfront 모바일 앱을 보다 안전하게 사용할 수 있도록 하기 위해 사용자는 15일 동안 활동이 없으면 자동으로 로그아웃됩니다. Workfront 관리자는 설정 > 시스템 > 환경 설정 아래의 웹 애플리케이션에서 이 시간 제한을 사용자 지정할 수 있습니다.

자세한 내용은 [시스템 보안 환경 설정 구성](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)을 참조하십시오.

## 로그인할 때 모바일 앱에 도메인 필요

SSO(Single Sign-On) 자격 증명으로 로그인하지 않은 경우 Workfront 모바일 앱에서 도메인을 제공하도록 요구합니다.

>[!NOTE]
>
>iOS 가용성: 2019년 6월 12일
>
>프로덕션 가용성: 2019년 6월 17일

## iOS에서 모바일 앱을 사용하여 오브젝트 삭제

>[!NOTE]
>
>이 기능은 2019년 8월 19일이 있는 주에 iOS의 앱 스토어에서 사용할 수 있습니다.

이제 iOS 모바일 앱에서 작업, 문제 및 타임시트와 같은 개체를 삭제할 수 있습니다. 개체를 삭제하려면 개체에 대한 올바른 권한이 있어야 합니다.

## 모바일 앱에서 중단 프로젝트로 필터링

>[!NOTE]
>
>이 기능은 2019년 8월 19일이 있는 주에 iOS 및 Android의 앱스토어에서 사용할 수 있습니다.

모바일 앱의 프로젝트 탭에 중단 프로젝트를 필터 옵션으로 추가했습니다.

## 모바일 앱을 사용하여 암호 재설정

암호를 잊은 경우 Workfront 모바일 앱을 사용하여 암호를 재설정할 수 있습니다. 암호를 잊으셨습니까? 화면의 지시를 따릅니다. 모바일 앱에서는 SSO 암호를 재설정할 수 없습니다.

## 모바일의 새로운 모양과 느낌

Workfront 모바일 앱에서의 경험을 개선하기 위해 다음과 같은 모양과 느낌 개선 사항이 추가되었습니다.

* 세부 정보 페이지의 상단 막대에서 다음을 화면의 더 눈에 띄는 영역으로 이동했습니다.

   * 이제 더하기 아이콘이 화면의 왼쪽 아래 모서리에 있습니다.
   * 항목 작업을 시작하기 위한 확인 표시가 이제 화면 상단 중간에 있는 처리 중 버튼입니다.

* 이제 세부 정보 페이지 하단의 자세히 표시 를 탭하여 첨부된 사용자 정의 양식을 볼 수 있습니다.
* 작업, 문제 및 요청을 제출하는 데 사용하는 페이지의 모양을 변경했습니다.

