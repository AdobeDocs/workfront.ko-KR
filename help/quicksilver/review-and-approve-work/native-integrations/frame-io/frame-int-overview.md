---
product-area: documents
navigation-topic: approvals
title: Frame.io 통합 개요
description: Frame.io 통합 개요
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Frame.io 통합 개요

Workfront 및 Frame.io 통합을 통해 프로젝트 코디네이터는 Workfront에서 프로젝트를 관리하고 작업을 계획할 수 있으며 크리에이티브, 마케터 및 이해 당사자는 Frame.io에서 에셋을 검토하고 승인할 수 있습니다.

## Adobe 엔터프라이즈 스토리지 관리를 기반으로 구축

이 통합의 핵심은 Adobe ESM(Enterprise Storage Management)으로, Workfront 및 Frame.io를 포함하여 Adobe 엔터프라이즈 제품 전반에 걸쳐 자산의 중앙 저장소 역할을 하는 클라우드 기반 스토리지 솔루션입니다.

Adobe 엔터프라이즈 스토리지 관리의 주요 이점은 다음과 같습니다.

* 크리에이티브 및 작업 관리 자산을 위한 통합 스토리지 레이어
* 보안 액세스 제어를 위해 Adobe IMS를 통해 중앙 집중식 권한
* Workfront, Frame.io 및 Creative Cloud 앱 <!--coming soon?-->에서 전체 에셋 가시성
* 엔터프라이즈 요구 사항에 맞는 확장 가능한 스토리지 및 할당량 관리

자세한 내용은 [Adobe 엔터프라이즈 스토리지 관리 개요](help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

## 통합 검토 및 승인

Workfront 및 Frame.io 통합에서는 Workfront의 통합 승인 기능을 사용하여 검토 및 승인을 관리합니다. 통합 승인을 통해 다음과 같은 작업을 수행할 수 있습니다.

* Workfront에서 바로 검토 및 승인 만들기 및 관리
* 검토 및 승인 상태를 실시간으로 추적
* 한 곳에서 피드백 및 승인 중앙 집중화
* 모든 관련자가 최신 버전의 자산에 액세스할 수 있는지 확인합니다.
* AI 검토자를 활용하여 브랜드 준수 검토 자동화
* 외

자세한 내용은 [통합 문서 승인: 문서 색인](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md)을 참조하세요.


### Frame.io 뷰어 사용

또한 통합은 Frame.io 뷰어와 연결됩니다. Frame.io 뷰어에서는

* 마크업 및 주석 달기 도구
* 버전 기록 및 비교
* 비디오 검토에 대한 타임스탬프가 지정된 댓글
* 이동 중 검토 및 승인을 위한 모바일 액세스

자세한 내용은 [Frame.io 통합 시작](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md)을 참조하세요.

#### 비디오 검토 제한 사항

<!--need to confirm these-->

#### Frame.io 뷰어에서 지원되는 파일 형식

Frame.io 뷰어는 모든 일반적인 비디오, 이미지, 오디오, PDF 및 MS® Office 유형을 지원합니다. 지원되는 파일의 자세한 목록을 보려면 [Frame.io의 형식](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)을 참조하십시오.

#### Frame.io 뷰어에 대한 액세스 및 라이선스

Frame.io 뷰어는 유료 라이선스가 있는 모든 Workfront 사용자가 사용할 수 있습니다. 이 통합에서 검토 및 승인을 위해 Frame.io 뷰어를 사용하는 데 추가 Frame.io 라이선스가 필요하지 않습니다.

조직에서 Frame.io의 프로젝트에 직접 에셋을 업로드하는 것과 같이 추가 Frame.io 기능을 활용하려는 경우 Frame.io 엔터프라이즈 라이센스를 구입할 수 있습니다. <!--link to Frame.io enterprise license info or who to contacT?-->

이 통합에서는 Workfront 증명 기능을 사용할 수 없습니다.

## Workfront의 강력한 프로젝트 관리

Workfront 및 Frame.io 통합을 통해 프로젝트 코디네이터는 Workfront의 강력한 프로젝트 관리 기능을 활용하여 작업을 계획, 추적 및 관리할 수 있습니다.

Workfront에서 프로젝트를 관리하는 방법에 대한 자세한 내용은 [프로젝트: 문서 색인](/help/quicksilver/manage-work/projects/projects-toc.md)을 참조하세요.

### 적용된 구조 및 이름 지정 규칙

이 통합은 ESM을 사용하여 구축되기 때문에 프로젝트 및 문서 관리 시 알아야 하는 일부 강제 구조 및 이름 지정 규칙이 있습니다.

* 오브젝트 이름은 고유해야 하며 복제할 수 없습니다.
* ESM에는 계층 트리에서 상위가 동일한 피어 개체에 대한 고유한 이름이 필요합니다.
* 문서가 동일한 프로젝트에 속하는 경우 문서에 동일한 이름을 사용할 수 없습니다.

이러한 제한 사항을 고려하여 Workfront은 충돌을 방지하기 위해 필요에 따라 개체나 문서의 이름을 자동으로 변경합니다.

### Workfront의 문서 관리

문서는 이 통합을 통해 프로젝트 수준에서 관리되며 현재 작업 또는 문제로 업로드할 수 없습니다.

문서 액세스는 프로젝트 수준에서도 관리됩니다. 사용자에게 프로젝트에 대한 액세스 권한이 있는 경우 해당 프로젝트와 관련된 모든 문서에 액세스할 수 있습니다.

<!--Documents can't be dragged as full folders.-->

### 문서 경험 제한 사항

이 통합은 ESM을 사용하여 구축되었기 때문에 Workfront의 원본 문서 환경에 몇 가지 제한 사항이 있습니다.

#### 제한 사항

다음 기능은 이 통합에 포함되지 않습니다.

* 외부 문서 공급자
* 증명 액세스
* Workfront의 문서 뷰어


#### 임시 제한 사항

현재 다음 기능은 사용할 수 없습니다.

* 즐겨 찾는 문서
* 요청 문서
* Adobe Experience Manager Assets에 문서 보내기
* 다단계 승인
* Workfront의 댓글 또는 업데이트에 문서 업로드
* Workfront의 작업 또는 문제에 문서 업로드



