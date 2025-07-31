---
title: 2025년 3분기 교정 및 문서 관리 개선 사항
description: 2025년 3분기 교정 및 문서 관리 개선 사항
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4829d487-7041-447f-9a68-fb1acf467734
source-git-commit: 2ff08963018c83e8d4fe88446f26efc115111a5e
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 2025년 3분기 교정 및 문서 관리 개선 사항

이 페이지에서는 미리보기 환경에 대한 2025년 3분기 릴리스의 모든 문서 관리 개선 사항에 대해 설명합니다. 이러한 개선 사항은 언급된 대로 프로덕션 환경에서 사용할 수 있습니다.

2025년 3분기 릴리스 주기에 이 시점에서 사용할 수 있는 모든 변경 사항 목록은 [2025년 3분기 릴리스 개요](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)를 참조하십시오.


## 통합 승인 단계별 롤아웃

>[!NOTE]
>
>고객을 위한 프로덕션 릴리스: 2025년 7월 17일부터 단계적으로 롤아웃


단계별 롤아웃에서 이전에 새 문서 승인이라고 했던 통합 승인을 활성화합니다. 이 기능은 향후 6개월 동안 Workfront 인스턴스에서 자동으로 활성화됩니다.

통합 승인 은 기존 문서 승인을 대체하며 문서에서 직접 다음 기능을 제공합니다.

* 전체 Workfront 팀을 검토자 또는 승인자로 지정
* 검토 또는 승인 마감 설정
* 승인 템플릿 만들기 및 재사용
* 새 버전 사용
* Workfront 홈 위젯에서 승인에 대한 여러 주요 성능 지표 보기
* 캔버스 대시보드를 사용하여 통합 승인에 대한 보고 세부 사항을 봅니다

자세한 내용은 [통합 승인 개요](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)를 참조하세요.

## Desktop Proofing 뷰어 업데이트

>[!NOTE]
>
>* 모든 고객을 위한 프로덕션 릴리스: 2025년 6월 16일

Desktop Proofing Viewer가 버전 2.1.50으로 업데이트되었습니다.

이 업데이트에는 내부 도구 업데이트가 포함되어 있으며 최종 사용자 기능에는 영향을 주지 않습니다.

이 업데이트는 Mac 및 Windows 모두에 해당됩니다.

## 새로운 증명 및 GenStudio for Performance Marketing 통합

>[!NOTE]
>
>* 모든 고객을 위한 프로덕션 릴리스: 2025년 6월 12일

Proofing과 GenStudio for Performance Marketing 간의 새로운 통합을 소개하게 되어 기쁘게 생각합니다. 이 통합을 통해 다음과 같은 작업을 수행할 수 있습니다

* Workfront 승인 템플릿을 사용하여 승인 워크플로 정의

* Workfront 증명 뷰어에서 초안 콘텐츠 검토

* GenStudio for Performance Marketing에서의 최종 승인 및 게시를 위한 검토 결정 을 참조하십시오

### 통합 요구 사항

Workfront 및 GenStudio for Performance Marketing을 동일한 IMS 조직에 배포해야 합니다.

자세한 내용은 [GenStudio for Performance Marketing 및 Workfront Proof 통합 시작](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md)을 참조하십시오.

## Desktop Proofing 뷰어 업데이트

Desktop Proofing Viewer가 버전 2.1.48로 업데이트되었습니다.

이 업데이트는 Desktop Viewer를 Mac 운영 체제와 호환되도록 하는 문제 해결입니다. 전자는 34.4.0으로 다운그레이드되었고 크롬은 132로 다운그레이드되었다.

이 업데이트는 Mac 및 Windows 모두에 해당됩니다.


## 연결된 Google 폴더의 Assets을 Workfront에 표시하려면 개별적으로 추가해야 합니다.

>[!NOTE]
>
>* 미리보기 릴리스: 2025년 6월 2일, 모든 고객을 위한 프로덕션 릴리스: 2025년 6월 2일

Google은 Google Drive에 액세스하는 타사 응용 프로그램에 대해 [보안 제어를 강화](https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps)하므로 응용 프로그램에서 사용자별 동의 모델을 채택해야 합니다. 따라서 개별 에셋이 Workfront에서 표시되도록 한 번에 하나씩 연결되어야 합니다. 자세한 내용은 [문서 통합 구성](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md)을 참조하십시오.

변경되지 않는 주요 기능:

* Google 드라이브 모달 내에서 에셋 및 폴더를 검색하고 필터링합니다
* Google 드라이브에서 Workfront 개체에 자산 연결
* 문서 페이지의 &quot;전송 대상&quot; 드롭다운을 통해 Google 드라이브에 에셋 업로드
* 사용자의 내 드라이브 영역에서 폴더 구조 보기 및 액세스
* Google 드라이브의 새 자산 버전을 Workfront의 기존 문서에 연결합니다.
* Google 드라이브에서 Workfront 개체에 폴더 연결
* 연결된 폴더로 문서를 끌어다 놓아 Google 드라이브에 에셋 업로드
* Workfront 내에서 새 Google 드라이브 문서 만들기


## 증명 뷰어에서 사용할 수 있는 새 문서 승인 결정 버튼

>[!IMPORTANT]
>
>이 기능은 단계별 릴리스의 일부이며 특정 고객에게만 제공됩니다.

>[!NOTE]
>
>* 미리보기 릴리스: 2025년 4월 10일, 모든 고객을 위한 프로덕션 릴리스: 2025년 4월 17일

이제 증명 뷰어에 새 문서 승인 결정 버튼이 표시됩니다. 이제 간단한 증명을 만든 다음 문서 요약에서 승인자와 검토자를 추가하면 승인자가 증명 뷰어 내에서 직접 결정을 내릴 수 있습니다.

이전에는 결정을 내리기 위해 증명 뷰어를 종료해야 했습니다.

이 릴리스 전에 생성된 승인에는 증명 뷰어의 버튼이 표시되지 않습니다.

자세한 내용은 [새 문서 승인 및 증명 함께 사용](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)을 참조하십시오.
