---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 조직의 Desktop Proofing Viewer 설치
description: 주로 대화형 콘텐츠의 증명을 위해 설계된 Desktop Proofing Viewer는 각 사용자의 로컬 컴퓨터에 설치해야 하는 애플리케이션입니다. Adobe Workfront 관리자 또는 Workfront Proof 관리자는 이 설치를 수행할 수 있습니다.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 5cc1acffff12d78e48228f3ae223514c0ff379ef
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 조직의 Desktop Proofing Viewer 설치

<!--Audited: 05/2024-->

주로 대화형 콘텐츠의 증명을 위해 설계된 Desktop Proofing Viewer는 각 사용자의 로컬 컴퓨터에 설치해야 하는 애플리케이션입니다. Adobe Workfront 관리자 또는 Workfront Proof 관리자는 이 설치를 수행할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td> <p>현재 플랜: Pro 이상</p> <p>또는</p> <p>기존 플랜: Premium 또는 선택</p> <p>다른 플랜의 증명 액세스에 대한 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront의 증명 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자에 대해 증명이 활성화되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>증명 권한 프로필에서 관리자를 선택해야 합니다. 자세한 내용은 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">사용자의 증명 액세스 구성</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 시스템 요구 사항

Desktop Proofing Viewer는 다음 운영 체제에서 지원됩니다.

* Windows 7 이상, 32비트 및 64비트
* Mac OS X 10.9 이상, 64비트

## 전제 조건

사용자가 Desktop Proofing Viewer를 사용할 수 있도록 하려면 설치하기 전에 대화형 증명에 대한 기본 보기로 Desktop Proofing Viewer를 시작하도록 시스템을 구성해야 합니다.

## 데스크탑 증명 뷰어를 대화형 증명의 기본값으로 구성

조직에 대한 데스크톱 증명 뷰어를 설치한 후 대화형 증명에 대한 기본 뷰어로 설정할 수 있습니다.

{{step1-to-proofing}}

1. 클릭 **계정 설정** Workfront Proof 오른쪽 위 모서리 근처에서 을(를) 클릭하고 **설정** 탭.

1. 아래 **증명 기본값**, 의 끝 **대화형 증명을 위한 데스크톱 증명 뷰어** 행, 클릭 **설정**.

   ![증명 기본값](assets/proof-defaults.png)

1. 클릭 **활성화됨 및 기본값**&#x200B;을 클릭한 다음 을 클릭합니다 **저장**.

## 사용자를 위한 Desktop Proof Viewer 설치

* [Mac에서 Desktop Proofing Viewer 설치](#installing-the-desktop-proofing-viewer-on-mac)
* [Windows에서 Desktop Proofing Viewer 설치](#installing-the-desktop-proofing-viewer-on-windows)

### Mac에서 Desktop Proofing Viewer 설치 {#installing-the-desktop-proofing-viewer-on-mac}

1. 사용자의 컴퓨터에서 다음 중 하나를 수행하여 앱을 다운로드합니다.

   * 프로덕션 환경을 사용하는 경우 [Desktop Proofing Viewer용 Mac 프로덕션 다운로드](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * 미리보기 환경을 사용하는 경우 [Desktop Proofing Viewer에 대한 Mac 미리 보기 다운로드](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. 방금 다운로드한 파일을 열어 설치를 시작합니다.
1. 표시되는 설치 상자에서 **계속**&#x200B;을 클릭한 다음 을 클릭합니다 **설치**.

   ![설치 상자](assets/install-wf-proof-box.png)

1. 각 사용자가 Workfront의 문서 영역에서 대화형 증명을 열어 설치를 완료해야 합니다.

### Windows에서 Desktop Proofing Viewer 설치 {#installing-the-desktop-proofing-viewer-on-windows}

1. 사용자의 컴퓨터에서 다음 중 하나를 수행하여 앱을 다운로드합니다.

   * 프로덕션 환경에서 [Desktop Proofing Viewer에 대한 Windows 프로덕션 다운로드](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * 미리보기 환경에서 [Desktop Proofing Viewer에 대한 Windows 미리 보기 다운로드](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. 방금 다운로드한 파일을 열어 설치를 시작합니다.
1. 표시되는 보안 경고 상자에서 **실행**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   Desktop Proofing Viewer 설치 및 실행

1. (조건부) Internet Explorer를 사용하여 응용 프로그램을 설치하는 경우 응용 프로그램이 설치된 후 브라우저에서 시작 페이지를 새로 고칩니다.
1. 각 사용자가 Workfront의 문서 영역에서 대화형 증명을 열어 설치를 완료해야 합니다.
