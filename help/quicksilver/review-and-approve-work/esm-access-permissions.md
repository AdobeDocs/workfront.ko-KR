---
product-area: documents
navigation-topic: approvals
title: Adobe 엔터프라이즈 스토리지 모델에 대한 개체 권한 및 액세스 수준 개요
description: Adobe 엔터프라이즈 스토리지 권한 및 액세스 개요
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Adobe 엔터프라이즈 스토리지 모델에 대한 개체 권한 및 액세스 수준 개요

<!--linked in UI -->

Adobe 엔터프라이즈 스토리지는 Adobe 엔터프라이즈 제품 전반에 걸쳐 에셋의 중앙 저장소 역할을 하는 클라우드 기반 스토리지 솔루션입니다. Adobe 엔터프라이즈 스토리지를 사용하는 Workfront 환경에는 기존 Workfront 문서 스토리지를 사용하는 환경과는 개체 권한 및 액세스 수준 동작이 약간 다릅니다.

## 액세스 수준

Workfront 액세스 수준은 Workfront 내에서만 적용됩니다. Workfront 내의 프로젝트 및 문서 제한 사항이 다른 Adobe 애플리케이션에 항상 적용되는 것은 아닙니다.

### Adobe 엔터프라이즈 스토리지와 레거시 Workfront 스토리지를 모두 사용하는 환경

문서 액세스는 프로젝트가 Adobe 엔터프라이즈 스토리지에 있는지 또는 레거시 Workfront 스토리지에 있는지에 따라 다르게 동작합니다.

* **기존 Workfront 저장소**: 기존 Workfront 저장소를 사용하는 프로젝트, 프로그램, 포트폴리오 및 템플릿은 문서 액세스에 대한 표준 Workfront 액세스 수준 논리를 따릅니다. 액세스 수준에서 문서에 대해 **액세스 권한 없음**&#x200B;을 선택한 경우 Workfront 또는 Frame.io 또는 Creative Cloud과 같은 다른 Adobe 제품의 문서를 볼 수 없습니다.
* **Adobe 엔터프라이즈 스토리지**: Adobe 엔터프라이즈 스토리지를 사용하는 프로젝트, 프로그램, 포트폴리오 및 템플릿은 다른 Adobe 제품에 대한 Adobe 엔터프라이즈 스토리지 액세스 수준 논리를 따릅니다.


   * **프로젝트, 프로그램, 포트폴리오 및 템플릿 개체 권한**: 액세스 수준에 프로젝트, 프로그램, 포트폴리오 및 템플릿에 대해 **액세스 권한 없음**&#x200B;이 선택되었지만 개체가 공유되면 사용자는 Workfront에서 개체를 볼 수 없지만 Frame.io 및 Adobe Creative Cloud과 같은 다른 Adobe 도구에서 개체 이름 및 연결된 문서를 계속 볼 수 있습니다.
   * **문서 권한**: 액세스 수준에서 문서에 대해 **액세스 권한 없음**&#x200B;을 선택한 경우 사용자는 Workfront의 프로젝트에 대한 문서를 볼 수 없지만 Frame.io 및 Adobe Creative Cloud과 같은 다른 Adobe 도구에서 공유된 프로젝트에 대한 문서를 계속 보고 관리할 수 있습니다. 문서 액세스는 Workfront 액세스 수준만 결정하는 것이 아니라 Adobe 엔터프라이즈 스토리지의 프로젝트 수준 권한에 의해 결정되기 때문입니다.

Workfront 환경에서 Adobe 엔터프라이즈 스토리지를 활성화한 경우 Adobe 엔터프라이즈 스토리지 프로젝트와 레거시 Workfront 스토리지 프로젝트를 모두 생성할 수 있습니다. 기존 Workfront 스토리지 프로젝트는 Workfront에 표시되는 모든 프로젝트 이름 옆에 아이콘을 표시합니다. Adobe 엔터프라이즈 스토리지 프로젝트에 아이콘이 표시되지 않습니다.

![프로젝트 이름 옆에 있는 레거시 workfront 저장소 아이콘](assets/legacy-project-icon.png)


### Adobe 엔터프라이즈 스토리지만 사용하는 환경

Adobe 엔터프라이즈 스토리지를 사용하는 프로젝트, 프로그램 및 포트폴리오에 대한 액세스 수준에서 문서 권한을 수정할 수 없습니다.

모든 액세스 수준은 문서에 대한 편집 액세스 권한을 가집니다. 프로젝트 수준 권한은 다른 Adobe 도구의 문서 액세스를 결정합니다.

문서 상속 액세스를 제한할 수 없습니다.


### 기존 Workfront 스토리지만 사용하는 환경

문서 액세스 수준이나 동작이 변경되지 않습니다.


## 프로젝트

프로젝트 수준 권한이 있는 사용자는 Frame.io 및 Adobe Creative Cloud과 같은 다른 Adobe 제품의 프로젝트 문서를 보고 관리할 수 있습니다.

프로젝트 이름은 ESM 프로젝트용 Workfront 외부에도 표시됩니다.

재무 데이터는 ESM 프로젝트용 Workfront 외부에서 볼 수 없습니다.

## 작업 및 문제

문서는 프로젝트 수준에서 저장되지만 필요에 따라 개별 작업 및 문제에 공유할 수 있습니다. 작업 및 문제 액세스 권한이 있는 사용자는 프로젝트에서 문서 액세스 권한을 자동으로 상속합니다. 액세스 수준을 수정할 수 없습니다. 관리자 액세스 권한이 있거나 액세스 권한이 없습니다.